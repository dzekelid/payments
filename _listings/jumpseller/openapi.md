swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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