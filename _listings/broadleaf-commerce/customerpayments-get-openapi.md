---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Customer Payments
  description: Get customer payments.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/checkout/payments:
    get:
      summary: Get Cart Checkout Payments
      description: Get cart checkout payments.
      operationId: getCartCheckoutPayments
      x-api-path-slug: cartcheckoutpayments-get
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payments
  /customer/payments:
    get:
      summary: Get Customer Payments
      description: Get customer payments.
      operationId: getCustomerPayments
      x-api-path-slug: customerpayments-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
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