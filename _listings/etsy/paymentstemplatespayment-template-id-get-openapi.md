---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Payments Templates Payment Template
  description: Retrieves a PaymentTemplate by id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listings/{listing_id}/payments:
    get:
      summary: Get Listings Listing Payments
      description: Retrieves a set of ListingPayment objects associated to a Listing.
      operationId: getListingsListingPayments
      x-api-path-slug: listingslisting-idpayments-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Payments
  /users/{user_id}/payments:
    get:
      summary: Get Users User Payments
      description: Retrieves a set of BillPayment objects associated to a User.
      operationId: getUsersUserPayments
      x-api-path-slug: usersuser-idpayments-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
  /users/{user_id}/payments/templates:
    get:
      summary: Get Users User Payments Templates
      description: Retrieves a set of PaymentTemplate objects associated to a User.
      operationId: getUsersUserPaymentsTemplates
      x-api-path-slug: usersuser-idpaymentstemplates-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Payments
      - Templates
  /payments/templates/{payment_template_id}:
    get:
      summary: Get Payments Templates Payment Template
      description: Retrieves a PaymentTemplate by id.
      operationId: getPaymentsTemplatesPaymentTemplate
      x-api-path-slug: paymentstemplatespayment-template-id-get
      parameters:
      - in: path
        name: payment_template_id
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Templates
      - Payment
      - Template
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