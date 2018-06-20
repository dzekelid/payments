---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 0
info:
  title: VersaPay Payments made in ARC
  description: Payments made to your supplier account from your customers since watermark,
    limited to 100 payment amounts at a time.<br><br>A consumer should store the last
    `id` value of each response and include it as the watermark parameter for a subsequent
    calls.
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