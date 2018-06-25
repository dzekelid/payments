---
name: Allied Irish Bank
x-slug: allied-irish-bank
description: Allied Irish Banks (AIB) is one of the so-called Big Four commercial
  banks in Ireland. AIB offers a full range of personal and corporate banking services.
  AIB Capital Markets is the division of the company that offers international banking
  and treasury operations. The bank also offers a range of general insurance products
  such as home, travel, and health insurance. It offers life assurance and pensions
  through its tied agency with Irish Life Assurance plc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
x-kinRank: "8"
x-alexaRank: "0"
tags: Payments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/apis.md
specificationVersion: "0.14"
apis:
- name: Allied Irish Bank Payment APIs Create a single immediate payment
  x-api-slug: allied-irish-bank-payment-apis
  description: Create a single immediate payment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
  humanURL: https://aibgb.co.uk/
  baseURL: https:////open-banking/v1.1//payments
  tags: Banking, Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/payments-post-openapi.md
- name: Allied Irish Bank Payment APIs Get a single immediate payment
  x-api-slug: allied-irish-bank-payment-apis
  description: Get a single immediate payment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
  humanURL: https://aibgb.co.uk/
  baseURL: https:////open-banking/v1.1//payments/{PaymentId}
  tags: Banking, Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/paymentspaymentid-get-openapi.md
- name: Allied Irish Bank Payment APIs Create a payment submission
  x-api-slug: allied-irish-bank-payment-apis
  description: Submit a previously setup payment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
  humanURL: https://aibgb.co.uk/
  baseURL: https:////open-banking/v1.1//payment-submissions
  tags: Banking, Payments, Submissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/paymentsubmissions-post-openapi.md
- name: Allied Irish Bank Payment APIs Get a payment submission
  x-api-slug: allied-irish-bank-payment-apis
  description: Get payment submission
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
  humanURL: https://aibgb.co.uk/
  baseURL: https:////open-banking/v1.1//payment-submissions/{PaymentSubmissionId}
  tags: Banking, Payments, Submissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/paymentsubmissionspaymentsubmissionid-get-openapi.md
- name: Allied Irish Bank Payment APIs
  x-api-slug: allied-irish-bank-payment-apis
  description: Allied Irish Banks (AIB) is one of the so-called Big Four commercial
    banks in Ireland. AIB offers a full range of personal and corporate banking services.
    AIB Capital Markets is the division of the company that offers international banking
    and treasury operations. The bank also offers a range of general insurance products
    such as home, travel, and health insurance. It offers life assurance and pensions
    through its tied agency with Irish Life Assurance plc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/allied-irish-bank.jpeg
  humanURL: https://aibgb.co.uk/
  baseURL: https:////open-banking/v1.1
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/allied-irish-bank/openapi.md
x-common:
- type: x-developer
  url: http://openbankingapis.io/Allied-Irish-Bank
- type: x-documentation
  url: https://openbanking.atlassian.net/wiki/spaces/DZ/pages/54919225/Open+Data+API+Dashboard#
- type: x-twitter
  url: https://twitter.com/AIBGB
- type: x-website
  url: https://aibgb.co.uk/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---