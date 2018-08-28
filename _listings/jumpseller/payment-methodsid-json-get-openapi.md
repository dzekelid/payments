---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Payment Methods
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment_methods.json:
    get:
      summary: Get Payment Methods
      description: ""
      operationId: getPaymentMethods.json
      x-api-path-slug: payment-methods-json-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Methods
      - Json
  /payment_methods/{id}.json:
    get:
      summary: Get Payment Methods
      description: ""
      operationId: getPaymentMethods.json
      x-api-path-slug: payment-methodsid-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Payment Method
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Methods
      - Id
      - Json
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