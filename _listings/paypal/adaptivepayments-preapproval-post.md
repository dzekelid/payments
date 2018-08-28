---
swagger: "2.0"
info:
  title: Paypal Preapproval
  description: "Use the Preapproval API operation to set up an agreement between yourself
    and a sender for making payments on the sender\u2019s behalf. You set up a preapprovals
    for a specific maximum amount over a specific period of time and, optionally,
    by any of the following constraints: the number of payments, a maximum per-payment
    amount, a specific day of the week or the month, and whether or not a PIN is required
    for each payment request."
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
  /AdaptivePayments/Preapproval:
    post:
      summary: Preapproval
      description: "Use the Preapproval API operation to set up an agreement between
        yourself and a sender for making payments on the sender\u2019s behalf"
      operationId: AdaptivePayments.Preapproval.post
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