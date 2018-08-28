swagger: "2.0"
x-collection-name: VersaPay
x-complete: 1
info:
  title: VersaPay API Reference
  description: -introductionthe-versapay-api-offers-operations-in-support-of-its-flagship-products-arc--accounts-receivable-platform-with-automated-invoicing-effective-collaboration-flexible-payments-and-cash-application-to-improve-efficiency-and-customer-relationships----importing--exporting-customers-invoices-and-payments----monitoring-file-based-importsbatches--payport--cloud-based-platform-to-electronically-push-and-pull-funds-across-the-eft--ach-network----moving-funds-using-transactions-and-preauthorized-debit-agreements----a-secure-hosted-checkout-for-accepting-payments-through-your-website-or-email-please-contact-us-at-supportversapay-com-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance--environmentsthe-demo-environment-is-a-useful-sandbox-for-integration-testing-where-transaction-settlements-are-simulated-using-test-account-numbers-and-test-dollar-amounts-httpsdemo-versapay-comonce-integration-testing-is-complete-via-the-demo-environment-start-sending-your-requests-to-the-production-url-to-start-moving-money-andor-integrating-with-versapay-httpssecure-versapay-com-rate-limitsthere-is-a-60-request-per-minute-api-limit--any-requests-above-this-limit-will-result-in-http-return-code-403-forbidden-rate-limit-exceeded--access-to-api-keysvisit-your-account-settings-in-demohttpsdemo-versapay-comaccount-or-productionhttpssecure-versapay-comaccount-to-setup-api-keys-needed-for-authentication-as-well-as-webhooks-to-receive-relevant-callbacks-from-versapay-transaction-processing--you-can-generatedisable-your-api-keys-as-often-as-necessary-for-security-reasons-if-you-do-not-have-an-account-please-contact-versapay-support-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance--authenticationapi-requests-are-authenticated-using-http-basic-access-authenticationhttpsen-wikipedia-orgwikibasic-access-authentication--simply-provide-the-tokenkey-values-as-the-user-and-password-parameters-using-curl-for-instancecurl-u-nvax---un0i----x-post-httpssecure-versapay-comapi----testing-transactions-eft-bank-account-numbersin-the-demo-environment-the-following-test-bank-accounts-can-be-setup-up-in-your-account-institutioninstitution-numberbranchaccount-numbertd00499960112-digitsrbc00316824112-digitsbmo00199520112-digitshsbc01610880112-digitswhen-versapay-prompts-you-to-verify-these-bank-accounts-enter-a-value-of-1-23-for-the-verification-amount-to-determine-the-outcome-of-a-transaction-funded-by-a-bank-account-set-the-amount-accordinglyamountresulting-statex-10nsfedx-11completed-but-nsfedx-30erroranything-elsecompleted-ach-bank-account-numbersplease-contact-supportversapay-com-for-support--setup-of-ach-acceptance-and-bank-account-numbers-that-can-be-used-for-testing--credit-card-numbersplease-contact-supportversapay-com-for-support--setup-of-credit-card-acceptance-and-card-brandsnumbers-that-can-be-used-for-testing--tools-postmantry-out-the-api-using-postman-apphttpswww-getpostman-com-a-powerful-rest-api-client--download-the-versapay-api-reference-as-a-postman-collection-by-clicking-on-the-button-belowrun-in-postmanhttpsrun-pstmn-iobutton-svghttpsapp-getpostman-comruncollection7e34e0700a2f8c3074c6after-downloading-the-collection-set-up-and-configure-the-environment-as-follows1--download-the-sample-environment-filehttpsdevelopers-versapay-comdemo-postman-environment-json-2--import-the-environment-file-in-postman---import-environmenthttpsdevelopers-versapay-comimagesimport-environment-png3--once-it-is-imported-edit-the-environment-to-add-api-token-and-keys-associated-to-your-test-account---edit-environmenthttpsdevelopers-versapay-comimagesedit-environment-png4--click-update-to-save-your-changes-5--before-placing-api-calls-make-sure-the-correct-environment-is-selected---select-environmenthttpsdevelopers-versapay-comimagesselect-environment-png
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