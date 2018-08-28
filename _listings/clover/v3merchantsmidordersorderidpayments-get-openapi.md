---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all payments for an order
  version: 1.0.0
  description: Get all payments for an order.
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
    get:
      summary: Get all payments for an order
      description: Get all payments for an order.
      operationId: GetOrderPayments
      x-api-path-slug: v3merchantsmidordersorderidpayments-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
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
  /v3/merchants/{mId}/payments/{payId}:
    get:
      summary: Get a single payment
      description: Get a single payment.
      operationId: GetPayment
      x-api-path-slug: v3merchantsmidpaymentspayid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: payId
        description: Payment Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
      - PayId
    post:
      summary: ""
      description: .
      operationId: UpdatePayment
      x-api-path-slug: v3merchantsmidpaymentspayid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: payId
        description: Payment Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
      - PayId
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