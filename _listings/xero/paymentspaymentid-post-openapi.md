---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Post Payments Payment
  description: Post payments payment.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Overpayments:
    get:
      summary: Get Overpayments
      description: Get overpayments.
      operationId: getOverpayments
      x-api-path-slug: overpayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Overpayments
    x-related-model:
      summary: X-related-model Overpayments
      description: X-related-model overpayments.
      operationId: x-related-modelOverpayments
      x-api-path-slug: overpayments-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Overpayments
  /Overpayments/{OverpaymentID}:
    get:
      summary: Get Overpayments Overpayment
      description: Get overpayments overpayment.
      operationId: getOverpaymentsOverpayment
      x-api-path-slug: overpaymentsoverpaymentid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: OverpaymentID
      responses:
        200:
          description: OK
      tags:
      - Overpayments
      - OverpaymentID
    x-related-model:
      summary: X-related-model Overpayments Overpayment
      description: X-related-model overpayments overpayment.
      operationId: x-related-modelOverpaymentsOverpayment
      x-api-path-slug: overpaymentsoverpaymentid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Overpayments
      - OverpaymentID
  /Overpayments/{OverpaymentID}/Allocations:
    put:
      summary: Put Overpayments Overpayment Allocations
      description: Put overpayments overpayment allocations.
      operationId: putOverpaymentsOverpaymentAllocations
      x-api-path-slug: overpaymentsoverpaymentidallocations-put
      parameters:
      - in: body
        name: Allocations
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: OverpaymentID
      responses:
        200:
          description: OK
      tags:
      - Overpayments
      - OverpaymentID
      - Ocations
    x-related-model:
      summary: X-related-model Overpayments Overpayment Allocations
      description: X-related-model overpayments overpayment allocations.
      operationId: x-related-modelOverpaymentsOverpaymentAllocations
      x-api-path-slug: overpaymentsoverpaymentidallocations-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Overpayments
      - OverpaymentID
      - Ocations
  /Payments:
    get:
      summary: Get Payments
      description: Get payments.
      operationId: getPayments
      x-api-path-slug: payments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Payments
    post:
      summary: Post Payments
      description: Post payments.
      operationId: postPayments
      x-api-path-slug: payments-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
    put:
      summary: Put Payments
      description: Put payments.
      operationId: putPayments
      x-api-path-slug: payments-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
    x-related-model:
      summary: X-related-model Payments
      description: X-related-model payments.
      operationId: x-related-modelPayments
      x-api-path-slug: payments-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Payments
  /Payments/{PaymentID}:
    get:
      summary: Get Payments Payment
      description: Get payments payment.
      operationId: getPaymentsPayment
      x-api-path-slug: paymentspaymentid-get
      parameters:
      - in: path
        name: PaymentID
      responses:
        200:
          description: OK
      tags:
      - Payments
      - PaymentID
    post:
      summary: Post Payments Payment
      description: Post payments payment.
      operationId: postPaymentsPayment
      x-api-path-slug: paymentspaymentid-post
      parameters:
      - in: path
        name: PaymentID
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
      - PaymentID
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