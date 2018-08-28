swagger: "2.0"
x-collection-name: Venmo
x-complete: 1
info:
  title: Venmo API
  description: the-venmo-api-provides-developers-a-straightforward-way-to-integrate-venmo-into-their-applications--
  version: 1.0.0
host: api.venmo.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payments:
    get:
      summary: Get Payments
      description: Get payments.
      operationId: getPayments
      x-api-path-slug: payments-get
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
      responses:
        200:
          description: OK
      tags:
      - Payments
  /payments/{id}:
    get:
      summary: Get Payments
      description: Get payments.
      operationId: getPayments
      x-api-path-slug: paymentsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Id