---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Capture Payment
  description: Capture payment.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/transactions/{key}/payments:
    get:
      summary: List Payments
      description: List payments.
      operationId: listPayments
      x-api-path-slug: apiv1transactionskeypayments-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      - in: query
        name: limit
        description: Max record count (no more than 100, defaults to 10)
      - in: query
        name: offset
        description: How many records need to be skipped, defaults to 0
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
    post:
      summary: Register A Payment
      description: Register a payment.
      operationId: createPayment
      x-api-path-slug: apiv1transactionskeypayments-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Register
      - Payment
  /api/v1/transactions/{key}/payments/capture:
    post:
      summary: Capture Payment
      description: Capture payment.
      operationId: capturePayment
      x-api-path-slug: apiv1transactionskeypaymentscapture-post
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Capture
      - Payment
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