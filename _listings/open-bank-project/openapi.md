swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
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