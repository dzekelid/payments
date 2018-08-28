swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/payment-options:
    get:
      summary: Get Shoppers Me Payment Options
      description: Get shoppers me payment options.
      operationId: getV1ShoppersMePaymentOptions
      x-api-path-slug: v1shoppersmepaymentoptions-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Payment
      - Options
  /v1/shoppers/me/payment-options/{id}:
    get:
      summary: Get Shoppers Me Payment Options
      description: Get shoppers me payment options.
      operationId: getV1ShoppersMePaymentOptions
      x-api-path-slug: v1shoppersmepaymentoptionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Payment
      - Options