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
          style="background-color: #ffffff; 
                                          width: 100%;
                                          max-width: 100%;"
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
                  style="background-color: #ffffff; 
                                          width: 100%;
                                          max-width: 100%;"
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
                          style="background-color: #ffffff; 
                                          width: 100%;
                                          max-width: 100%;"
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
                                  style="background-color: #ffffff; 
                                          width: 100%;
                                          max-width: 100%;"
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
                                          style="background-color: #ffffff; 
                                          width: 100%;
                                          max-width: 100%;"
                                        >
                                          <tr>
                                            <td>
                                              <img
                                                src="https://api.coi.ua/media/123456.png"
                                                alt="shemax"
                                                width="500"
                                                height="150"
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
                                      align-items: center;
                                      text-align: left;
                                      margin: 0;
                                      margin-right: 5px;
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
                                        width: 75px;
                                      ">
                                                Id:
                                              </h2>
                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Date:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
                                            <td>
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
                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Phone:
                                              </h2>

                                            </td>
                                            <td>
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

                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Email:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Country:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Comment:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                City:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                PostCode:
                                              </h2>
                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Street:
                                              </h2>

                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                House:
                                              </h2>
                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Apartment:
                                              </h2>
                                            </td>
                                            <td>
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
                                          <tr style="
                                              padding-bottom: 10px;
                                              display: flex;
                                              padding-left: 10px;
                                              margin-bottom: 10px;
                                              border-bottom: 1px solid rgb(237,237,237);">
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
                                        font-weight: 400;
                                        text-align: left;
                                        padding: 0;
                                        margin: 0;
                                        margin-right: 5px;
                                        width: 75px;
                                      ">
                                                Payment:
                                              </h2>
                                            </td>
                                            <td>
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

                                          <tr style="display: flex;">
                                            <td style="
                                              
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                              width: 77%;
                                        margin: 0;">
                                              Product

                                            </td>
                                            <td style="
                                            
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                        max-width: 100%;
                                        width: 15%;
                                        margin: 0;">
                                              Count
                                            </td>
                                            <td style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: left;
                                        background-color: #ededed;
                                        padding: 15px;
                                        max-width: 100%;
                                        width: 15%;
                                        margin: 0;">
                                              Price
                                            </td>
                                          </tr>

                                          <tr
                                            v-for="(item, index) in order.listItems"
                                            :key="index"
                                            style="display: flex; 
                                      border-bottom: 1px solid #ededed;"
                                          >
                                            <td
                                              align="left"
                                              valign="top"
                                              style="
                                      display: flex;
                                      flex-direction: row;
    align-items: center;
                                      padding: 0;
                                      align-items: right;
                                      max-width: 100%;
                                      width: 296px;
                                        padding: 15px;
                                    "
                                            >
                                              <div style="
                                        flex-direction: column;
                                        text-align: left;
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
                                                  {{ item.title }}</a>
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
                                            </td>
                                            <td style="
                                            max-width: 100%;
                                            width: 86px;
                                        margin: 0;
                                        display: flex;
                                      ">
                                              <div style="
    margin: auto 0 auto auto;
                                      ">
                                                <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: right;
                                        vertical-align: middle;">
                                                  {{ item.count }}</h3>
                                              </div>

                                            </td>
                                            <td style="
                                            max-width: 100%;
                                        width: 86px;
                                        display: flex;
                                        margin: 0;
                                      ">
                                              <div style="
    margin: auto 0 auto auto;
                                      ">
                                                <h3 style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: right;
                                        vertical-align: middle;">
                                                  {{ item.price }}$</h3>
                                              </div>
                                            </td>
                                          </tr>
                                          <tr style="display: flex; 
                                      border-bottom: 1px solid #ededed; 
                                      width: 100%;
                                      max-width: 100%;">
                                            <td style="
                                            max-width: 100%;
                                          color: #000;
                                          text-align: right;
                                          line-height: 100%;
                                          font-family: Helvetica, Arial,
                                            sans-serif;
                                          font-size: 14px;
                                          font-weight: 400;
                                        padding: 15px;
                                        border-right: 1px solid #ededed;
                                        width: 296px;
                                          margin: 0;
                                    ">
                                              Count:
                                            </td>
                                            <td style="width: 86px"></td>
                                            <td style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: right;
                                        margin: 0;
                                        max-width: 100%;
                                        padding: 15px 0;
                                        width: 86px;
                                      ">

                                              {{count}}
                                            </td>
                                          </tr>
                                          <tr style="display: flex; 
                                      max-width: 100%">
                                            <td style="
                                      max-width: 100%;
                                        padding: 15px;
                                        width:296px;
                                        border-right: 1px solid #ededed;
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
                                            </td>
                                            <td style="width: 86px"></td>
                                            <td style="
                                        color: #000;
                                        line-height: 100%;
                                        font-family: Helvetica, Arial,
                                          sans-serif;
                                        font-size: 14px;
                                        font-weight: 400;
                                        text-align: right;
                                        max-width: 30%;
                                        width: 86px;
                                        margin: 0;
                                        padding: 15px 0;
                                      ">
                                              {{price}}$
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
