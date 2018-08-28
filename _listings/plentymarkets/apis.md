---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Payments
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List payments
  x-api-slug: restpayments-get
  description: List payments.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-get-openapi.md
- name: plentymarkets REST-API - List payments by entry date
  x-api-slug: restpaymentsentrydate-get
  description: Lists all payments by entry date within a certain date range. The start
    and the end of the date range must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsentrydate-get-openapi.md
- name: plentymarkets REST-API - List payments by import date
  x-api-slug: restpaymentsimportdate-get
  description: Lists all payments by import date within a certain date range. The
    start and the end of the date range must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsimportdate-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment method
  x-api-slug: restpaymentsmethodsmethodid-get
  description: Lists all payments of the a payment method. The ID of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodsmethodid-get-openapi.md
- name: plentymarkets REST-API - List payments of an order
  x-api-slug: restpaymentsordersorderid-get
  description: Lists all payments of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsordersorderid-get-openapi.md
- name: plentymarkets REST-API - List payments by property type ID and value
  x-api-slug: restpaymentspropertypropertytypeidpropertyvalue-get
  description: Lists all payments by the given property type ID and the value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspropertypropertytypeidpropertyvalue-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - List payments of a transaction type
  x-api-slug: restpaymentstransactionstransactiontypeid-get
  description: Lists all payments of a transaction type. The ID of the transaction
    type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentstransactionstransactiontypeid-get-openapi.md
- name: plentymarkets REST-API - Get payment policy
  x-api-slug: restmarketsebaypayment-policiesid-get
  description: Get payment policy for given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restmarketsebaypayment-policiesid-get-openapi.md
- name: plentymarkets REST-API - Create a payment
  x-api-slug: restpayments-post
  description: Create a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-post-openapi.md
- name: plentymarkets REST-API - Update a payment
  x-api-slug: restpayments-put
  description: Update a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-put-openapi.md
- name: plentymarkets REST-API - List payment methods names
  x-api-slug: restpaymentsmethodnames-get
  description: Lists all payment method names.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-openapi.md
- name: plentymarkets REST-API - List all payment method names for a payment method
    id
  x-api-slug: restpaymentsmethodnamespaymentmethodid-get
  description: List all payment method names for a payment method id. The payment
    method id must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-openapi.md
- name: plentymarkets REST-API - Gets a payment method name by id and lang
  x-api-slug: restpaymentsmethodnamespaymentmethodidlang-get
  description: Gets a payment method name by id and lang. The ID and the requested
    lang of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-openapi.md
- name: plentymarkets REST-API - List payment methods
  x-api-slug: restpaymentsmethods-get
  description: Lists all payment method plugins.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-get-openapi.md
- name: plentymarkets REST-API - Create a payment method
  x-api-slug: restpaymentsmethods-post
  description: Creates a payment method. The plugin key, the payment key and the name
    of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-post-openapi.md
- name: plentymarkets REST-API - Update a payment method
  x-api-slug: restpaymentsmethods-put
  description: Updates the name of the payment method. The name of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-put-openapi.md
- name: plentymarkets REST-API - Get a payment method
  x-api-slug: restpaymentsmethodspluginspluginkey-get
  description: Gets a payment method plugin. The plugin key must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodspluginspluginkey-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment method
  x-api-slug: restpaymentsmethodsmethodid-get
  description: Lists all payments of the a payment method. The ID of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodsmethodid-get-openapi.md
- name: plentymarkets REST-API - Create a payment property
  x-api-slug: restpaymentsproperties-post
  description: Create a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-post-openapi.md
- name: plentymarkets REST-API - Update a payment property
  x-api-slug: restpaymentsproperties-put
  description: Update a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-put-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Get a payment
  x-api-slug: restpaymentspaymentid-get
  description: Gets a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentid-get-openapi.md
- name: plentymarkets REST-API - List properties for a payment
  x-api-slug: restpaymentspaymentidproperties-get
  description: Lists all properties for a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontact-delete
  description: Delete payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontact-delete-openapi.md
- name: plentymarkets REST-API - Create Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontactcontactid-post
  description: Create payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontactcontactid-post-openapi.md
- name: plentymarkets REST-API - Delete Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorder-delete
  description: Delete payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorder-delete-openapi.md
- name: plentymarkets REST-API - Create Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorderorderid-post
  description: Create payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorderorderid-post-openapi.md
- name: plentymarkets REST-API - Get payment policy
  x-api-slug: restmarketsebaypayment-policiesid-get
  description: Get payment policy for given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restmarketsebaypayment-policiesid-get-openapi.md
- name: plentymarkets REST-API - Create a payment
  x-api-slug: restpayments-post
  description: Create a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-post-openapi.md
- name: plentymarkets REST-API - Update a payment
  x-api-slug: restpayments-put
  description: Update a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-put-openapi.md
- name: plentymarkets REST-API - List payment methods names
  x-api-slug: restpaymentsmethodnames-get
  description: Lists all payment method names.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-openapi.md
- name: plentymarkets REST-API - List all payment method names for a payment method
    id
  x-api-slug: restpaymentsmethodnamespaymentmethodid-get
  description: List all payment method names for a payment method id. The payment
    method id must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-openapi.md
- name: plentymarkets REST-API - Gets a payment method name by id and lang
  x-api-slug: restpaymentsmethodnamespaymentmethodidlang-get
  description: Gets a payment method name by id and lang. The ID and the requested
    lang of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-openapi.md
- name: plentymarkets REST-API - List payment methods
  x-api-slug: restpaymentsmethods-get
  description: Lists all payment method plugins.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-get-openapi.md
- name: plentymarkets REST-API - Create a payment method
  x-api-slug: restpaymentsmethods-post
  description: Creates a payment method. The plugin key, the payment key and the name
    of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-post-openapi.md
- name: plentymarkets REST-API - Update a payment method
  x-api-slug: restpaymentsmethods-put
  description: Updates the name of the payment method. The name of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-put-openapi.md
- name: plentymarkets REST-API - Get a payment method
  x-api-slug: restpaymentsmethodspluginspluginkey-get
  description: Gets a payment method plugin. The plugin key must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodspluginspluginkey-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment method
  x-api-slug: restpaymentsmethodsmethodid-get
  description: Lists all payments of the a payment method. The ID of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodsmethodid-get-openapi.md
- name: plentymarkets REST-API - Create a payment property
  x-api-slug: restpaymentsproperties-post
  description: Create a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-post-openapi.md
- name: plentymarkets REST-API - Update a payment property
  x-api-slug: restpaymentsproperties-put
  description: Update a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-put-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Get a payment
  x-api-slug: restpaymentspaymentid-get
  description: Gets a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentid-get-openapi.md
- name: plentymarkets REST-API - List properties for a payment
  x-api-slug: restpaymentspaymentidproperties-get
  description: Lists all properties for a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontact-delete
  description: Delete payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontact-delete-openapi.md
- name: plentymarkets REST-API - Create Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontactcontactid-post
  description: Create payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontactcontactid-post-openapi.md
- name: plentymarkets REST-API - Delete Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorder-delete
  description: Delete payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorder-delete-openapi.md
- name: plentymarkets REST-API - Create Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorderorderid-post
  description: Create payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorderorderid-post-openapi.md
- name: plentymarkets REST-API - List properties for a payment
  x-api-slug: restpaymentspaymentidproperties-get
  description: Lists all properties for a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentidproperties-get-openapi.md
- name: plentymarkets REST-API - Get a payment
  x-api-slug: restpaymentspaymentid-get
  description: Gets a payment. The ID of the payment must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentspaymentid-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Update a payment property
  x-api-slug: restpaymentsproperties-put
  description: Update a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-put-openapi.md
- name: plentymarkets REST-API - Create a payment property
  x-api-slug: restpaymentsproperties-post
  description: Create a payment property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsproperties-post-openapi.md
- name: plentymarkets REST-API - List payments of a payment method
  x-api-slug: restpaymentsmethodsmethodid-get
  description: Lists all payments of the a payment method. The ID of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodsmethodid-get-openapi.md
- name: plentymarkets REST-API - Get a payment method
  x-api-slug: restpaymentsmethodspluginspluginkey-get
  description: Gets a payment method plugin. The plugin key must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodspluginspluginkey-get-openapi.md
- name: plentymarkets REST-API - Update a payment method
  x-api-slug: restpaymentsmethods-put
  description: Updates the name of the payment method. The name of the payment method
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-put-openapi.md
- name: plentymarkets REST-API - Create a payment method
  x-api-slug: restpaymentsmethods-post
  description: Creates a payment method. The plugin key, the payment key and the name
    of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-post-openapi.md
- name: plentymarkets REST-API - List payment methods
  x-api-slug: restpaymentsmethods-get
  description: Lists all payment method plugins.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethods-get-openapi.md
- name: plentymarkets REST-API - Gets a payment method name by id and lang
  x-api-slug: restpaymentsmethodnamespaymentmethodidlang-get
  description: Gets a payment method name by id and lang. The ID and the requested
    lang of the payment method must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodidlang-get-openapi.md
- name: plentymarkets REST-API - List all payment method names for a payment method
    id
  x-api-slug: restpaymentsmethodnamespaymentmethodid-get
  description: List all payment method names for a payment method id. The payment
    method id must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnamespaymentmethodid-get-openapi.md
- name: plentymarkets REST-API - List payment methods names
  x-api-slug: restpaymentsmethodnames-get
  description: Lists all payment method names.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentsmethodnames-get-openapi.md
- name: plentymarkets REST-API - Update a payment
  x-api-slug: restpayments-put
  description: Update a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-put-openapi.md
- name: plentymarkets REST-API - Create a payment
  x-api-slug: restpayments-post
  description: Create a payment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpayments-post-openapi.md
- name: plentymarkets REST-API - Get payment policy
  x-api-slug: restmarketsebaypayment-policiesid-get
  description: Get payment policy for given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restmarketsebaypayment-policiesid-get-openapi.md
- name: plentymarkets REST-API - Create Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontactcontactid-post
  description: Create payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontactcontactid-post-openapi.md
- name: plentymarkets REST-API - Delete Payment-Contact-Relation
  x-api-slug: restpaymentpaymentidcontact-delete
  description: Delete payment-contact-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidcontact-delete-openapi.md
- name: plentymarkets REST-API - Create Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorderorderid-post
  description: Create payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorderorderid-post-openapi.md
- name: plentymarkets REST-API - Delete Payment-Order-Relation
  x-api-slug: restpaymentpaymentidorder-delete
  description: Delete payment-order-relation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/plentymarkets/restpaymentpaymentidorder-delete-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---