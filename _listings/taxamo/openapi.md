swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
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