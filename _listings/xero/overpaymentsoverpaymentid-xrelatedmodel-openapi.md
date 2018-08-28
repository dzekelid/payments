---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting X-related-model Overpayments Overpayment
  description: X-related-model overpayments overpayment.
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