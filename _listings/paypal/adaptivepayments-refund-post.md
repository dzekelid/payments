---
swagger: "2.0"
info:
  title: Paypal Refund
  description: Use the Refund API operation to refund all or part of a payment. You
    can specify the amount of the refund and identify the accounts to receive the
    refund by the payment key or tracking ID, and optionally, by transaction ID or
    the receivers of the original payment.
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
  /AdaptivePayments/Refund:
    post:
      summary: Refund
      description: Use the Refund API operation to refund all or part of a payment
      operationId: AdaptivePayments.Refund.post
      responses:
        200:
          description: OK
      tags:
      - payments
      - refunds
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