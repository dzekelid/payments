---
swagger: "2.0"
info:
  title: Paypal Pay
  description: "Use the Pay API operation to transfer funds from a sender\u2019s PayPal
    account to one or more receivers\u2019 PayPal accounts. You can use the Pay API
    operation to make simple payments, chained payments, or parallel payments; these
    payments can be explicitly approved, preapproved, or implicitly approved."
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/Pay:
    post:
      summary: Pay
      description: "Use the Pay API operation to transfer funds from a sender\u2019s
        PayPal account to one or more receivers\u2019 PayPal accounts"
      operationId: AdaptivePayments.Pay.post
      responses:
        200:
          description: OK
      tags:
      - payments
definitions: []
x-collection-name: PayPal
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