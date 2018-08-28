---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List payments of an order
  description: Lists all payments of an order. The ID of the order must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/payments:
    get:
      summary: List payments
      description: List payments.
      operationId: getRestPayments
      x-api-path-slug: restpayments-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
  /rest/payments/entrydate:
    get:
      summary: List payments by entry date
      description: Lists all payments by entry date within a certain date range. The
        start and the end of the date range must be specified.
      operationId: getRestPaymentsEntrydate
      x-api-path-slug: restpaymentsentrydate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the entry date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the entry date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Entry
      - Date
  /rest/payments/importdate:
    get:
      summary: List payments by import date
      description: Lists all payments by import date within a certain date range.
        The start and the end of the date range must be specified.
      operationId: getRestPaymentsImportdate
      x-api-path-slug: restpaymentsimportdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the import date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the import date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Import
      - Date
  /rest/payments/methods/{methodId}:
    get:
      summary: List payments of a payment method
      description: Lists all payments of the a payment method. The ID of the payment
        method must be specified.
      operationId: getRestPaymentsMethodsMethod
      x-api-path-slug: restpaymentsmethodsmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: methodId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Method
  /rest/payments/orders/{orderId}:
    get:
      summary: List payments of an order
      description: Lists all payments of an order. The ID of the order must be specified.
      operationId: getRestPaymentsOrdersOrder
      x-api-path-slug: restpaymentsordersorderid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Order
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---