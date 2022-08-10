<template>

  <body
    bgcolor="#e1e1e1"
    leftmargin="0"
    marginwidth="0"
    topmargin="0"
    marginheight="0"
    offset="0"
  >
    <center style="background-color: #ededed">
      <table
        border="0"
        cellpadding="0"
        cellspacing="0"
        height="100%"
        width="100%"
        background-color="#FFFFFF"
        style="
          table-layout: fixed;
          max-width: 100% !important;
          width: 100% !important;
          min-width: 100% !important;
        "
      >
        <tbody
          background-color="#ededed"
          style="background-color: #ededed"
        >
          <tr>
            <td
              align="center"
              valign="top"
            >
              <table
                background-color="#FFFFFF"
                border="0"
                cellpadding="0"
                cellspacing="0"
                maxWidth="500"
                style="border: 0px solid #ffffff"
              >

                <tbody
                  background-color="#fff"
                  style="background-color: #fff"
                >
                  <tr style="display: flex; flex-direction: column">
                    <!-- //order name, email, phone .... -->
                    <td
                      align="center"
                      valign="top"
                    >
                      <table
                        border="0"
                        cellpadding="0"
                        cellspacing="0"
                        width="100%"
                        style="color: #ffffff"
                        bgcolor="#fffffff"
                      >

                        <tbody
                          background-color="#ffffff"
                          style="background-color: #ffffff"
                        >
                          <tr>
                            <td
                              align="center"
                              valign="top"
                            >
                              <table
                                border="0"
                                cellpadding="0"
                                cellspacing="0"
                                width="500"
                              >

                                <tbody
                                  background-color="#ffffff"
                                  style="background-color: #ffffff"
                                >
                                  <tr>
                                    <td
                                      align="center"
                                      valign="top"
                                      width="500"
                                    >
                                      <table
                                        border="0"
                                        cellspacing="0"
                                        width="100%"
                                      >

                                        <tbody
                                          background-color="#ffffff"
                                          style="background-color: #ffffff"
                                        >
                                          <tr>
                                            <td>
                                              <img
                                                src="https://api.coi.ua/media/shemax-logo.png"
                                                alt="shemax"
                                                width="500"
                                                height="200"
                                                title="Logo"
                                                style="display:block"
                                              />
                                            </td>
                                          </tr>
                                          <tr style="
                                    display: flex;
                                    flex-direction: column;
                                    padding: 0 10px;
                                  ">
                                            <td
                                              align="left"
                                              valign="top"
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 700;
                                        text-align: left;
                                        padding-bottom: 15px;
                                      ">
                                                Order details
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Id:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderId }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Date:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderDate }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Name:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderName }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Phone:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderPhone }}
                                              </h2>
                                            </td>
                                          </tr>

                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Email:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderEmail }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Country:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderCountry }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Comment:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderComment }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                City:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderCity }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                PostCode:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderPostCode }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Street:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderStreet }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                House:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderHouse }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Apartment:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderApartment }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      padding-bottom: 10px;
                                      padding-left: 10px;
                                      margin: 0;
                                      margin-bottom: 10px;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Payment:
                                              </h2>
                                              <h2 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                      ">
                                                {{ order.orderPayment }}
                                              </h2>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                            >
                                              <h1 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 700;
                                        text-align: left;
                                        padding: 0 10px;
                                      ">
                                                Items in order
                                              </h1>
                                            </td>
                                          </tr>

                                          <tr style="display: flex; flex-direction: column">
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      padding: 0;
                                      align-items: center;
                                      width: 100%;
                                    "
                                            >
                                              <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                        width: 70%;
                                        margin: 0;
                                      ">
                                                Product
                                              </h3>
                                              <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                        max-width: 70%;
                                        margin: 0;
                                      ">
                                                Count
                                              </h3>

                                              <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                        max-width: 70%;
                                        margin: 0;
                                      ">
                                                Price
                                              </h3>
                                            </td>
                                          </tr>

                                          <tr
                                            v-for="(item, index) in order.listItems"
                                            :key="index"
                                          >
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
    align-items: center;
                                      padding: 0;
                                      align-items: center;
                                      width: 100%;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <div style="
                                        flex-direction: column;
                                        text-align: left;
                                        padding: 15px;
                                        width: 70%;
                                        margin: 0;
                                      ">
                                                <a
                                                  style="
                                          color: blue;
                                          margin-bottom: 10px;
                                          line-height: 100%;
                                          font-family: Helvetica, Arial,
                                            sans-serif;
                                          font-size: 16px;
                                          font-weight: 400;
                                        "
                                                  :href="item.link"
                                                >
                                                  {{ item.link }}</a>
                                                <p style="
                                          color: #000;
                                          line-height: 100%;
                                          font-family: Helvetica, Arial,
                                            sans-serif;
                                          font-size: 14px;
                                          font-weight: 400;
                                          margin: 0;
                                        ">
                                                  Colors: {{ item.color }}
                                                </p>
                                              </div>
                                              <div style="
                                        width: 67px;
                                        margin: 0;
                                      ">
                                                <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: center;
                                        vertical-align: middle;">
                                                  {{ item.count }}</h3>
                                              </div>

                                              <div style="
                                        width: 67px;
                                        margin: 0;
                                      ">
                                                <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: center;
                                        vertical-align: middle;">
                                                  {{ item.price }}$</h3>
                                              </div>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      padding: 0;
                                      align-items: center;
                                      width: 100%;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <div style="
                                        text-align: left;
                                        padding: 15px;
                                        width: 70%;
                                        margin: 0;
                                        border-right: 1px solid #ededed;
                                      ">
                                                <p style="
                                          color: #000;
                                          text-align: right;
                                          line-height: 100%;
                                          font-family: Helvetica, Arial,
                                            sans-serif;
                                          font-size: 14px;
                                          font-weight: 400;
                                          margin: 0;
                                        ">
                                                  Count:
                                                </p>
                                              </div>

                                              <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: center;
                                        padding: 15px;
                                        width: 100px;
                                        margin: 0;
                                      ">
                                                {{count}}
                                              </h3>
                                            </td>
                                          </tr>
                                          <tr>
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      padding: 0;
                                      align-items: center;
                                      width: 100%;
                                      border-bottom: 1px solid #ededed;
                                    "
                                            >
                                              <div style="
                                        text-align: left;
                                        padding: 15px;
                                        width: 70%;
                                        margin: 0;
                                        border-right: 1px solid #ededed;
                                      ">
                                                <p style="
                                          color: #000;
                                          text-align: right;
                                          line-height: 100%;
                                          font-family: Helvetica, Arial,
                                            sans-serif;
                                          font-size: 14px;
                                          font-weight: 400;
                                          margin: 0;
                                        ">
                                                  Price:
                                                </p>
                                              </div>

                                              <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: center;
                                        padding: 15px;
                                        width: 100px;
                                        margin: 0;
                                      ">
                                                {{price}}$
                                              </h3>
                                            </td>
                                          </tr>
                                        </tbody>
                                      </table>
                                    </td>
                                  </tr>
                                </tbody>
                              </table>
                            </td>
                          </tr>

                        </tbody>
                      </table>
                    </td>
                  </tr>
                </tbody>
              </table>
            </td>
          </tr>
        </tbody>
      </table>
    </center>
  </body>
</template>
<script>
export default {
  data() {
    return {
      count: 0,
      price: 0,
    };
  },

  props: {
    order: {
      orderId: String,
      orderDate: String,
      orderName: String,
      orderPhone: String,
      orderEmail: String,
      orderComment: String,
      orderCountry: String,
      orderCity: String,
      orderPostCode: String,
      orderStreet: String,
      orderHouse: String,
      orderApartment: String,
      orderPayment: String,
      listItems: Array,
    },
  },

  mounted() {
    this.order.listItems.forEach((el) => {
      this.price += el.price * el.count;
      this.count += el.count;
    });
  },
};
</script>
