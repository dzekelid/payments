swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
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
    delete:
      summary: Delete Customer Payments
      description: Delete customer payments.
      operationId: deleteCustomerPayments
      x-api-path-slug: customerpayments-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
  /cart/checkout/payment/{paymentId}:
    delete:
      summary: Delete Cart Checkout Payment Paymentid
      description: Delete cart checkout payment paymentid.
      operationId: deleteCartCheckoutPaymentPayment
      x-api-path-slug: cartcheckoutpaymentpaymentid-delete
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
  /cart/checkout/payment/{paymentId}/transaction:
    put:
      summary: Put Cart Checkout Payment Paymentid Transaction
      description: Put cart checkout payment paymentid transaction.
      operationId: putCartCheckoutPaymentPaymentTransaction
      x-api-path-slug: cartcheckoutpaymentpaymentidtransaction-put
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
      - Transaction
  /customer/payment/{paymentId}:
    put:
      summary: Put Customer Payment Paymentid
      description: Put customer payment paymentid.
      operationId: putCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-put
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
    delete:
      summary: Delete Customer Payment Paymentid
      description: Delete customer payment paymentid.
      operationId: deleteCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-delete
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
  /cart/checkout/payment:
    post:
      summary: Post Cart Checkout Payment
      description: Post cart checkout payment.
      operationId: postCartCheckoutPayment
      x-api-path-slug: cartcheckoutpayment-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
  /cart/checkout/payment/{customerPaymentId}:
    post:
      summary: Post Cart Checkout Payment Customerpaymentid
      description: Post cart checkout payment customerpaymentid.
      operationId: postCartCheckoutPaymentCustomerpayment
      x-api-path-slug: cartcheckoutpaymentcustomerpaymentid-post
      parameters:
      - in: query
        name: amount
        description: amount
      - in: query
        name: cartId
        description: cartId
      - in: query
        name: currency
        description: currency
      - in: path
        name: customerPaymentId
        description: customerPaymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Customerpaymentid
  /customer/payment:
    get:
      summary: Get Customer Payment
      description: Get customer payment.
      operationId: getCustomerPayment
      x-api-path-slug: customerpayment-get
      parameters:
      - in: query
        name: customerId
      - in: query
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
    post:
      summary: Post Customer Payment
      description: Post customer payment.
      operationId: postCustomerPayment
      x-api-path-slug: customerpayment-post
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment