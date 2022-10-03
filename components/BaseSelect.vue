<template>
  <div
    :class="[
      select.error && 'base-select--error', 
    select.load && 'base-select--load',
    select.disabled && 'base-select--disabled'
    ]"
    :style="{ zIndex: 100 - index }"
    class="base-select__content"
  >
    <div
      :class="
    [isFocus && 'base-input--focus',
  className]"
      class="base-input base-select"
    >
      <input
        @input="updateInput"
        @blur="checkEmptyInput"
        @focus="isFocus = true, isContent = true, isTarget = true"
        :value="valueInput"
        :name="select.title"
        :id="select.title"
        autocomplete="off"
        class="base-input__input"
        type="text"
      />
      <label
        :for="select.title"
        class="base-input__label"
      > {{ select.title }}</label>
      <div
        v-if="isContent"
        v-scroll="onScroll"
        :style="{ zIndex: 100 - index + 5 }"
        class="base-select__wrapper"
        :id="`element-show-${index}`"
      >

        <button
          v-for="(item, index) in
             isSearch ? 
             select.listOptions.filter(el => el.toLowerCase().match(valueInput.toLowerCase())).slice(0, 15 * isCount) :
             select.listOptions.slice(0, 15 * isCount)"
          :style="{ zIndex: 100 + index }"
          :key="index"
          @focus="updateSelect"
          :class="modelValue === item && 'is-active'"
          :id="item"
          type="button"
          class="base-select__item"
        >{{ item }}</button>
      </div>
    </div>
    <p
      v-if="select.error"
      class="base-input__helper base-select__helper base-select__helper--top"
    >{{ select.errorText }}</p>
  </div>
</template>

<script>
export default {
  name: "base-select",
  props: {
    select: {
      title: String,
      listOptions: Array,
      disabled: {
        type: Boolean,
        default: false,
      },
      load: {
        type: Boolean,
        default: false,
      },
      error: {
        type: Boolean,
        default: false,
      },
      errorText: {
        type: String,
        default: "",
      },
    },
    className: {
      type: String,
      default: "",
    },
    modelValue: {
      type: String,
      default: "",
    },
    index: {
      type: Number,
      default: 1,
    },
  },
  data() {
    return {
      isCount: 1,
      valueInput: this.modelValue,
      isFocus: false,
      isTarget: false,
      isContent: false,
      isArrow: false,
      isSearch: false,
    };
  },
  watch: {
    modelValue(newValue) {
      this.valueInput = newValue;
      if (!this.isFocus || !this.isTarget) {
        newValue.length ? (this.isFocus = true) : (this.isFocus = false);
      }
    },
    isArrow() {
      setTimeout(() => {
        this.isArrow = false;
      }, 500);
    },
  },

  methods: {
    elementInViewport(el) {
      const scroll = el.scrollTop;
      const height = el.scrollHeight - el.clientHeight;
      console.log("elementInViewport", scroll, height);
      if (height - scroll <= 50) {
        console.log("elementInViewport: if is work");
        this.isCount++;
      }
    },
    arrowChange() {
      if (this.isArrow) {
        this.modelValue != ``
          ? (this.isFocus = true)
          : (this.isFocus = !this.isFocus);
      } else {
        this.modelValue != ``
          ? (this.isFocus = true)
          : (this.isFocus = !this.isFocus);
        this.isContent = !this.isContent;
        this.isTarget = !this.isTarget;
      }
    },
    onScroll(e) {
      this.elementInViewport(e.path[0]);
    },
    updateSelect(e) {
      console.log(e);
      const value = e.target.innerHTML;
      const id = e.target.id;
      this.valueInput = value;
      this.isContent = false;
      this.isCount = 1;
      this.$emit("update:modelValue", value);
      this.$emit("update:modelId", id);
    },

    updateInput(e) {
      const value = e.target.value;
      this.valueInput = value;
      this.isSearch = true;
      this.isCount = 1;
    },

    checkEmptyInput(e) {
      this.isContent = false;
      this.isTarget = false;
      this.isSearch = false;
      this.isArrow = true;
      this.isCount = 1;
      !e.target.value.length && this.$emit("update:modelId", "");

      const value = e.target.value;
      value.length ? (this.isFocus = true) : (this.isFocus = false);
      !value.length
        ? this.$emit("update:modelValue", value)
        : (this.valueInput = this.modelValue);
    },
  },

  mounted() {
    this.modelValue != "" ? (this.isFocus = true) : (this.isFocus = false);
  },
};
</script>