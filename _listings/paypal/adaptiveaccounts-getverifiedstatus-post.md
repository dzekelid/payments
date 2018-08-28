---
swagger: "2.0"
info:
  title: Paypal Get Verified Status
  description: The GetVerifiedStatus API operation lets you check if a PayPal account
    status is verified. A PayPal account gains verified status under a variety of
    circumstances, such as when an account is linked to a verified funding source.
    Verified status serves to indicate a trust relationship. For more information
    about account verified status, refer to PayPal.com.
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
  /AdaptiveAccounts/GetVerifiedStatus:
    post:
      summary: Get Verified Status
      description: The GetVerifiedStatus API operation lets you check if a PayPal
        account status is verified
      operationId: AdaptiveAccounts.GetVerifiedStatus.post
      responses:
        200:
          description: OK
      tags:
      - payments
      - verified
      - status
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