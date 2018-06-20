---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: reverb Get My Payments Selling
  description: Get my payments selling.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/payments/selling:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentsselling-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: order_id
        description: Look up payments by order id
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
  /my/payments/selling/{id}:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
      - Id
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