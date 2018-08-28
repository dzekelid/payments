---
swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 0
info:
  title: Open Bank Project Get Scheduled Payments
  description: Get Scheduled Payments
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/scheduled-payments:
    get:
      summary: Get Account Scheduled Payments
      description: Get Scheduled Payments related to an account
      operationId: GetAccountScheduledPayments
      x-api-path-slug: accountsaccountidscheduledpayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Scheduled
      - Payments
  /scheduled-payments:
    get:
      summary: Get Scheduled Payments
      description: Get Scheduled Payments
      operationId: GetScheduledPayments
      x-api-path-slug: scheduledpayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Scheduled
      - Payments
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