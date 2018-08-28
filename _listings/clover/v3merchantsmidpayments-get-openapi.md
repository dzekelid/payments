---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all payments
  version: 1.0.0
  description: 'Retrieve payment information including total amount, tipAmount, taxAmount,
    and result status.To POST a payment see: https://docs.clover.com/build/developer-pay-api/'
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/orders/{orderId}/payments:
    post:
      summary: Create a payment record on an order
      description: Create a payment record on an order.
      operationId: CreatePaymentForOrder
      x-api-path-slug: v3merchantsmidordersorderidpayments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Payments
  /v3/merchants/{mId}/payments:
    get:
      summary: Get all payments
      description: 'Retrieve payment information including total amount, tipAmount,
        taxAmount, and result status.To POST a payment see: https://docs.clover.com/build/developer-pay-api/'
      operationId: GetPayments
      x-api-path-slug: v3merchantsmidpayments-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tender, taxRates, germanInfo, lineItemPayments,
          cardTransaction, dccInfo, appTracking, refunds, order, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
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