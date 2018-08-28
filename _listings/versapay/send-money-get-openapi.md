---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 0
info:
  title: VersaPay Single Payment Hosted Checkout
  description: |-
    Clients, customers, or donors, for instance, can send your organization money directly from their bank account or credit card simply by clicking a link which displays a page with your account name allowing your customer to make a payment to you for the specified dollar amount:
    <br>
    `https://secure.versapay.com/send_money?api_token={your_api_token}&amount={dollar_amount_for_customer_to_pay}`
    <br>
    Funds will go to the fund destination passed in the to_fund parameter. By default, the funds will be deposited into your default bank account once the transaction clears from the other party.
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/exports/payment_amounts:
    get:
      summary: Payments made in ARC
      description: Payments made to your supplier account from your customers since
        watermark, limited to 100 payment amounts at a time.<br><br>A consumer should
        store the last `id` value of each response and include it as the watermark
        parameter for a subsequent calls.
      operationId: getARCPayments
      x-api-path-slug: apiexportspayment-amounts-get
      parameters:
      - in: query
        name: watermark
        description: The `id` value to base a subsequent extract of the next 100 payment
          amounts
      responses:
        200:
          description: OK
      tags:
      - Payments
      - made
      - in
      - ARC
  /send_money:
    get:
      summary: Single Payment Hosted Checkout
      description: |-
        Clients, customers, or donors, for instance, can send your organization money directly from their bank account or credit card simply by clicking a link which displays a page with your account name allowing your customer to make a payment to you for the specified dollar amount:
        <br>
        `https://secure.versapay.com/send_money?api_token={your_api_token}&amount={dollar_amount_for_customer_to_pay}`
        <br>
        Funds will go to the fund destination passed in the to_fund parameter. By default, the funds will be deposited into your default bank account once the transaction clears from the other party.
      operationId: hostedCheckout
      x-api-path-slug: send-money-get
      parameters:
      - in: query
        name: amount
        description: The amount in dollars that the transaction is for
      - in: query
        name: api_token
        description: A valid API token generated from your account
      - in: query
        name: link_url
        description: A url that gets stored and displayed on the transaction for an
          invoice
      - in: query
        name: locale
        description: Set the default language of the checkout, either `en` or `fr`
      - in: query
        name: message
        description: A message which will be stored with the transaction
      - in: query
        name: pref
        description: The preferred payment type either `ba` or `cc` for bank or credit
          card respectively
      - in: query
        name: reference
        description: Extra data (max 255 characters)
      - in: query
        name: return_to
        description: A url which will displayed to the user to return to your website
          after they finish the Signup and Confirmation
      - in: query
        name: to_fund
        description: The token of the bank account or balance where the funds should
          go to
      responses:
        200:
          description: OK
      tags:
      - Single
      - Payment
      - Hosted
      - Checkout
  /api/imports/payment:
    post:
      summary: Create a Payment
      description: |-
        Create and update external payment records in ARC.<br><br>The set of attributes to send in the request body may vary based on the account configuration. Please contact the implementation specialist for more information.<br><br>
        The request schema for posting a payment for a single invoice is slightly different than that for posting a payment for multiple invoices.

        For instance, sample request for posting payment for a single invoice looks like:
        ```
        {
          "identifier": "PMT0010-05",
          "invoice_number": "INV1234-01",
          "amount": 10000,
          "currency": "usd",
          "date": "2018-01-10",
          "customer_identifier": "C1234",
          "customer_name": "Acme Inc.",
          "notes": "Notes",
          "ref1": "1234",
          "ref2": "PO# 84767"
        }
        ```

        *Note: Customer will be created using the customer_&ast; attributes if it doesn???t already exist at the time of payment import.*
      operationId: createPayment
      x-api-path-slug: apiimportspayment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - CreatePayment
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