swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 1
info:
  title: NetLicensing
  description: the-labs64-netlicensing-restful-api-gives-you-access-to-netlicensings-core-features--you-authenticate-to-the-netlicensing-api-by-providing-your-account-credentials-or-simply-use-our-demo-account--find-out-more-about-labs64-netlicensing-at-netlicensing-io-
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