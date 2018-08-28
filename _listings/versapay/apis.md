---
name: VersaPay
x-slug: versapay
description: VersaPay handles elements of both credit and debit card merchant payment
  processing in Canada. In offering a host of merchant account services and credit
  card POS terminals it allows for an efficient merchant payment service in all aspects-
  in person, on the go, online, and at the office. Founded in 2005 by Michael Gokturk,
  VersaPay is a Canadian owned and operated national financial transaction services
  provider partnered with Chase Paymentech. Versapay also offers electronic funds
  transfer through a system called Versapay EMT.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
x-kinRank: "9"
x-alexaRank: "410909"
tags: Payments
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apis.md
specificationVersion: "0.14"
apis:
- name: VersaPay API Reference - Payments made in ARC
  x-api-slug: apiexportspayment-amounts-get
  description: Payments made to your supplier account from your customers since watermark,
    limited to 100 payment amounts at a time.<br><br>A consumer should store the last
    `id` value of each response and include it as the watermark parameter for a subsequent
    calls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-openapi.md
- name: VersaPay API Reference - Single Payment Hosted Checkout
  x-api-slug: send-money-get
  description: |-
    Clients, customers, or donors, for instance, can send your organization money directly from their bank account or credit card simply by clicking a link which displays a page with your account name allowing your customer to make a payment to you for the specified dollar amount:
    <br>
    `https://secure.versapay.com/send_money?api_token={your_api_token}&amount={dollar_amount_for_customer_to_pay}`
    <br>
    Funds will go to the fund destination passed in the to_fund parameter. By default, the funds will be deposited into your default bank account once the transaction clears from the other party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/send-money-get-openapi.md
- name: VersaPay API Reference - Single Payment Hosted Checkout
  x-api-slug: send-money-get
  description: |-
    Clients, customers, or donors, for instance, can send your organization money directly from their bank account or credit card simply by clicking a link which displays a page with your account name allowing your customer to make a payment to you for the specified dollar amount:
    <br>
    `https://secure.versapay.com/send_money?api_token={your_api_token}&amount={dollar_amount_for_customer_to_pay}`
    <br>
    Funds will go to the fund destination passed in the to_fund parameter. By default, the funds will be deposited into your default bank account once the transaction clears from the other party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/send-money-get-openapi.md
- name: VersaPay API Reference - Payments made in ARC
  x-api-slug: apiexportspayment-amounts-get
  description: Payments made to your supplier account from your customers since watermark,
    limited to 100 payment amounts at a time.<br><br>A consumer should store the last
    `id` value of each response and include it as the watermark parameter for a subsequent
    calls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-openapi.md
- name: VersaPay API Reference - Create a Payment
  x-api-slug: apiimportspayment-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiimportspayment-post-openapi.md
- name: VersaPay API Reference - Payments made in ARC
  x-api-slug: apiexportspayment-amounts-get
  description: Payments made to your supplier account from your customers since watermark,
    limited to 100 payment amounts at a time.<br><br>A consumer should store the last
    `id` value of each response and include it as the watermark parameter for a subsequent
    calls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiexportspayment-amounts-get-openapi.md
- name: VersaPay API Reference - Create a Payment
  x-api-slug: apiimportspayment-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/apiimportspayment-post-openapi.md
- name: VersaPay API Reference - Single Payment Hosted Checkout
  x-api-slug: send-money-get
  description: |-
    Clients, customers, or donors, for instance, can send your organization money directly from their bank account or credit card simply by clicking a link which displays a page with your account name allowing your customer to make a payment to you for the specified dollar amount:
    <br>
    `https://secure.versapay.com/send_money?api_token={your_api_token}&amount={dollar_amount_for_customer_to_pay}`
    <br>
    Funds will go to the fund destination passed in the to_fund parameter. By default, the funds will be deposited into your default bank account once the transaction clears from the other party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/versapay/send-money-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://venmo.api.gallery.streamdata.io
- type: x-api-stack
  url: http://versapay.stack.network
- type: x-base
  url: https://secure.versapay.com/api/
- type: x-blog
  url: https://www.versapay.com/blog/
- type: x-blog-rss
  url: http://www.versapay.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/versapay
- type: x-crunchbase
  url: https://crunchbase.com/organization/versapay
- type: x-github
  url: https://github.com/versapay
- type: x-partners
  url: https://www.versapay.com/partners/
- type: x-support
  url: https://www.versapay.com/support/
- type: x-twitter
  url: https://twitter.com/VersaPay
- type: x-website
  url: http://developers.versapay.com/index.html
- type: x-website
  url: https://www.versapay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---