---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create a payment method
  description: Creates a payment method. The plugin key, the payment key and the name
    of the payment method must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/payments:
    get:
      summary: List payments
      description: List payments.
      operationId: getRestPayments
      x-api-path-slug: restpayments-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
    post:
      summary: Create a payment
      description: Create a payment.
      operationId: postRestPayments
      x-api-path-slug: restpayments-post
      parameters:
      - in: body
        name: /rest/payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
    put:
      summary: Update a payment
      description: Update a payment.
      operationId: putRestPayments
      x-api-path-slug: restpayments-put
      parameters:
      - in: body
        name: /rest/payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
  /rest/payments/entrydate:
    get:
      summary: List payments by entry date
      description: Lists all payments by entry date within a certain date range. The
        start and the end of the date range must be specified.
      operationId: getRestPaymentsEntrydate
      x-api-path-slug: restpaymentsentrydate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the entry date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the entry date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Entry
      - Date
  /rest/payments/importdate:
    get:
      summary: List payments by import date
      description: Lists all payments by import date within a certain date range.
        The start and the end of the date range must be specified.
      operationId: getRestPaymentsImportdate
      x-api-path-slug: restpaymentsimportdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the import date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the import date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Import
      - Date
  /rest/payments/methods/{methodId}:
    get:
      summary: List payments of a payment method
      description: Lists all payments of the a payment method. The ID of the payment
        method must be specified.
      operationId: getRestPaymentsMethodsMethod
      x-api-path-slug: restpaymentsmethodsmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: methodId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Method
  /rest/payments/orders/{orderId}:
    get:
      summary: List payments of an order
      description: Lists all payments of an order. The ID of the order must be specified.
      operationId: getRestPaymentsOrdersOrder
      x-api-path-slug: restpaymentsordersorderid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Order
  /rest/payments/property/{propertyTypeId}/{propertyValue}:
    get:
      summary: List payments by property type ID and value
      description: Lists all payments by the given property type ID and the value.
      operationId: getRestPaymentsPropertyPropertytypePropertyvalue
      x-api-path-slug: restpaymentspropertypropertytypeidpropertyvalue-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: propertyTypeId
      - in: path
        name: propertyValue
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Property
      - Type
      - ID
      - Value
  /rest/payments/status/{statusId}:
    get:
      summary: List payments of a payment status
      description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
        status</a> must be specified.
      operationId: getRestPaymentsStatusStatus
      x-api-path-slug: restpaymentsstatusstatusid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Status
  /rest/payments/transactions/{transactionTypeId}:
    get:
      summary: List payments of a transaction type
      description: Lists all payments of a transaction type. The ID of the transaction
        type must be specified.
      operationId: getRestPaymentsTransactionsTransactiontype
      x-api-path-slug: restpaymentstransactionstransactiontypeid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: transactionTypeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Transaction
      - Type
  /rest/markets/ebay/payment_policies/{id}:
    get:
      summary: Get payment policy
      description: Get payment policy for given ID.
      operationId: getRestMarketsEbayPaymentPolicies
      x-api-path-slug: restmarketsebaypayment-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Policy
  /rest/payments/methodNames:
    get:
      summary: List payment methods names
      description: Lists all payment method names.
      operationId: getRestPaymentsMethodnames
      x-api-path-slug: restpaymentsmethodnames-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
      - Names
  /rest/payments/methodNames/{paymentMethodId}:
    get:
      summary: List all payment method names for a payment method id
      description: List all payment method names for a payment method id. The payment
        method id must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethod
      x-api-path-slug: restpaymentsmethodnamespaymentmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Payment
      - Method
      - Namesa
      - Payment
      - Method
      - Id
  /rest/payments/methodNames/{paymentMethodId}/{lang}:
    get:
      summary: Gets a payment method name by id and lang
      description: Gets a payment method name by id and lang. The ID and the requested
        lang of the payment method must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethodLang
      x-api-path-slug: restpaymentsmethodnamespaymentmethodidlang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - S
      - Payment
      - Method
      - Name
      - By
      - Id
      - Lang
  /rest/payments/methods:
    get:
      summary: List payment methods
      description: Lists all payment method plugins.
      operationId: getRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
    post:
      summary: Create a payment method
      description: Creates a payment method. The plugin key, the payment key and the
        name of the payment method must be specified.
      operationId: postRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-post
      parameters:
      - in: body
        name: /rest/payments/methods
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
    put:
      summary: Update a payment method
      description: Updates the name of the payment method. The name of the payment
        method must be specified.
      operationId: putRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-put
      parameters:
      - in: body
        name: /rest/payments/methods
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
  /rest/payments/methods/plugins/{pluginKey}:
    get:
      summary: Get a payment method
      description: Gets a payment method plugin. The plugin key must be specified.
      operationId: getRestPaymentsMethodsPluginsPluginkey
      x-api-path-slug: restpaymentsmethodspluginspluginkey-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: pluginKey
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
  /rest/payments/properties:
    post:
      summary: Create a payment property
      description: Create a payment property.
      operationId: postRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-post
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
    put:
      summary: Update a payment property
      description: Update a payment property.
      operationId: putRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-put
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
  /rest/payments/{paymentId}:
    get:
      summary: Get a payment
      description: Gets a payment. The ID of the payment must be specified.
      operationId: getRestPaymentsPayment
      x-api-path-slug: restpaymentspaymentid-get
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment
  /rest/payments/{paymentId}/properties:
    get:
      summary: List properties for a payment
      description: Lists all properties for a payment. The ID of the payment must
        be specified.
      operationId: getRestPaymentsPaymentProperties
      x-api-path-slug: restpaymentspaymentidproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - List
      - Propertiesa
      - Payment
  /rest/payment/{paymentId}/contact:
    delete:
      summary: Delete Payment-Contact-Relation
      description: Delete payment-contact-relation.
      operationId: deleteRestPaymentPaymentContact
      x-api-path-slug: restpaymentpaymentidcontact-delete
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Contact-Relation
  /rest/payment/{paymentId}/contact/{contactId}:
    post:
      summary: Create Payment-Contact-Relation
      description: Create payment-contact-relation.
      operationId: postRestPaymentPaymentContactContact
      x-api-path-slug: restpaymentpaymentidcontactcontactid-post
      parameters:
      - in: path
        name: contactId
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Contact-Relation
  /rest/payment/{paymentId}/order:
    delete:
      summary: Delete Payment-Order-Relation
      description: Delete payment-order-relation.
      operationId: deleteRestPaymentPaymentOrder
      x-api-path-slug: restpaymentpaymentidorder-delete
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Order-Relation
  /rest/payment/{paymentId}/order/{orderId}:
    post:
      summary: Create Payment-Order-Relation
      description: Create payment-order-relation.
      operationId: postRestPaymentPaymentOrderOrder
      x-api-path-slug: restpaymentpaymentidorderorderid-post
      parameters:
      - in: path
        name: orderId
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Order-Relation
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