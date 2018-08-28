---
swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 0
info:
  title: NetLicensing Update payment method
  description: Sets the provided properties to a payment method. Return an updated
    payment method
  termsOfService: https://www.labs64.com/legal/terms-of-service/netlicensing
  version: 2.x
host: go.netlicensing.io
basePath: /core/v2/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /paymentmethod:
    get:
      summary: Payment Methods list
      description: Return a list of all payment methods for the current vendor
      operationId: listPaymentMethods
      x-api-path-slug: paymentmethod-get
      responses:
        200:
          description: OK
      tags:
      - Paymentmethod
  /paymentmethod/{paymentMethodNumber}:
    get:
      summary: Get payment method
      description: Return a payment method info by paymentMethodNumber
      operationId: getPaymentMethod
      x-api-path-slug: paymentmethodpaymentmethodnumber-get
      parameters:
      - in: path
        name: paymentMethodNumber
        description: Payment method number
      responses:
        200:
          description: OK
      tags:
      - Paymentmethod
      - PaymentMethodNumber
    post:
      summary: Update payment method
      description: Sets the provided properties to a payment method. Return an updated
        payment method
      operationId: updatePaymentMethod
      x-api-path-slug: paymentmethodpaymentmethodnumber-post
      parameters:
      - in: formData
        name: active
        description: If set to false, the payment method is disabled
      - in: path
        name: paymentMethodNumber
        description: Payment method number
      - in: formData
        name: paypal.subject
        description: The e-mail address of the PayPal account for which you are making
          the API calls
      responses:
        200:
          description: OK
      tags:
      - Paymentmethod
      - PaymentMethodNumber
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