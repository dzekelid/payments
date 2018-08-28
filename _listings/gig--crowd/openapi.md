swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/payment/add:
    post:
      summary: Post Payment Add
      description: Post payment add.
      operationId: postApiV1PaymentAdd
      x-api-path-slug: apiv1paymentadd-post
      parameters:
      - in: body
        name: payRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
  /api/v1/payment/promocode/price:
    post:
      summary: Post Payment Promocode Price
      description: Post payment promocode price.
      operationId: postApiV1PaymentPromocodePrice
      x-api-path-slug: apiv1paymentpromocodeprice-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Promocode
      - Price
  /api/v1/payment/promocode/{requestId}:
    post:
      summary: Post Payment Promocode Requestid
      description: Post payment promocode requestid.
      operationId: postApiV1PaymentPromocodeRequest
      x-api-path-slug: apiv1paymentpromocoderequestid-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Promocode
      - Requestid