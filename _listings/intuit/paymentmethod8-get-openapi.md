---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Payment Method
  description: |-
    Read a payment method
    Method : GET
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment:
    post:
      summary: Post Payment
      description: |-
        Create an payment object
        Method : POST
      operationId: postPayment
      x-api-path-slug: payment-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
  /paymentmethod:
    post:
      summary: Post Payment Method
      description: |-
        Update a payment method
        Method : POST
      operationId: postPaymentmethod
      x-api-path-slug: paymentmethod-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
      - Method
  /paymentmethod/8:
    get:
      summary: Get Payment Method
      description: |-
        Read a payment method
        Method : GET
      operationId: getPaymentmethod8
      x-api-path-slug: paymentmethod8-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
      - Method
  /billpayment:
    post:
      summary: Post BilL Payment
      description: |-
        Update a BillPayment
        Content-Type:application/json
        Method - POST
      operationId: postBillpayment
      x-api-path-slug: billpayment-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - BilL
      - Payment
  /payment/174:
    get:
      summary: Get Payment
      description: |-
        Read a payment object by Id
        Method : GET
      operationId: getPayment174
      x-api-path-slug: payment174-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
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