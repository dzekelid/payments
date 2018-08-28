---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a payment card with predefined ID
  description: ""
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment-cards:
    get:
      summary: Retrieve a list of Payment Cards
      description: Retrieve a list of Payments Cards
      operationId: payment_cards.get
      x-api-path-slug: paymentcards-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
    post:
      summary: Create a Payment Card
      description: Create a Payment Card
      operationId: payment_cards.post
      x-api-path-slug: paymentcards-post
      parameters:
      - in: body
        name: body
        description: PaymentCard resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Card
  /payment-cards/{id}:
    get:
      summary: Retrieve a Payment Card
      description: Retrieve a Payment Card with specified identifier string
      operationId: payment_cards.id.get
      x-api-path-slug: paymentcardsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Payment
      - Card
    patch:
      summary: Update a payment card's cvv value with predefined ID
      description: Update a payment card's cvv value with predefined identifier string
      operationId: payment_cards.id.patch
      x-api-path-slug: paymentcardsid-patch
      parameters:
      - in: body
        name: body
        description: Payment card
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Cards
      - Cvv
      - Value
      - Predefined
      - ID
    put:
      summary: Create a payment card with predefined ID
      description: ""
      operationId: payment_cards.id.put
      x-api-path-slug: paymentcardsid-put
      parameters:
      - in: body
        name: body
        description: Payment card
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Card
      - Predefined
      - ID
  /payment-cards/{id}/authorization:
    post:
      summary: Authorize a Payment Card
      description: Authorize a Payment Card
      operationId: payment_cards.id.authorization.post
      x-api-path-slug: paymentcardsidauthorization-post
      parameters:
      - in: body
        name: body
        description: Payment Card resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Authorize
      - Payment
      - Card
  /payment-cards/{id}/deactivation:
    post:
      summary: Deactivate a Payment Card
      description: Deactivate a Payment Card
      operationId: payment_cards.id.deactivation.post
      x-api-path-slug: paymentcardsiddeactivation-post
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Payment
      - Card
  /payment-cards/{id}/matched-rules:
    get:
      summary: Get matched rules for the payment card
      description: Get matched rules for the payment card
      operationId: payment_cards.id.matched_rules.get
      x-api-path-slug: paymentcardsidmatchedrules-get
      responses:
        200:
          description: OK
      tags:
      - Matched
      - Rulesthe
      - Payment
      - Card
  /payments:
    get:
      summary: Retrieve a payment list
      description: Retrieve a payment list
      operationId: payments.get
      x-api-path-slug: payments-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Payment
      - List
    post:
      summary: Create a payment
      description: Create a payment
      operationId: payments.post
      x-api-path-slug: payments-post
      parameters:
      - in: body
        name: body
        description: Payment resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
  /payments/{id}:
    get:
      summary: Retrieve a payment
      description: Retrieve a payment with specified identifier string
      operationId: payments.id.get
      x-api-path-slug: paymentsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Payment
    put:
      summary: Create a payment with predefined ID
      description: Make a payment with predefined identifier string
      operationId: payments.id.put
      x-api-path-slug: paymentsid-put
      parameters:
      - in: body
        name: body
        description: Payment resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Predefined
      - ID
  /queue/payments:
    get:
      summary: Retrieve a scheduled payment list
      description: Retrieve a scheduled payment list
      operationId: queue.payments.get
      x-api-path-slug: queuepayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Payment
      - List
  /queue/payments/{id}:
    get:
      summary: Retrieve a scheduled payment
      description: Retrieve a payment with specified identifier string
      operationId: queue.payments.id.get
      x-api-path-slug: queuepaymentsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Payment
    put:
      summary: Update pending payment
      description: ""
      operationId: queue.payments.id.put
      x-api-path-slug: queuepaymentsid-put
      parameters:
      - in: body
        name: body
        description: Payment resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pending
      - Payment
  /tokens:
    post:
      summary: Create a payment token
      description: Create a token
      operationId: tokens.post
      x-api-path-slug: tokens-post
      parameters:
      - in: body
        name: body
        description: PaymentToken resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Token
  /payment-cards-migrations:
    get:
      summary: Retrieve a list of payment cards ready for migration
      description: Retrieve a list of payment cards ready for migration
      operationId: retrieve-a-list-of-payment-cards-ready-for-migration
      x-api-path-slug: paymentcardsmigrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
      - Readymigration
  /payment-cards-migrations/migrate:
    post:
      summary: Migrate payment cards to another gateway account
      description: Migrate payment cards to another gateway account
      operationId: migrate-payment-cards-to-another-gateway-account
      x-api-path-slug: paymentcardsmigrationsmigrate-post
      parameters:
      - in: body
        name: body
        description: Payment card migration attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Migrate
      - Payment
      - Cards
      - To
      - Another
      - Gateway
      - Account
  /queue/payments/{id}/cancel:
    post:
      summary: Cancel a scheduled payment
      description: Cancel a scheduled payment with specified identifier string
      operationId: cancel-a-scheduled-payment-with-specified-identifier-string
      x-api-path-slug: queuepaymentsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Scheduled
      - Payment
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