---
swagger: "2.0"
info:
  title: Etsy Post Payments Templates
  description: Creates a new PaymentTemplate
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payments/templates:
    post:
      summary: Post Payments Templates
      description: Creates a new PaymentTemplate
      operationId: postPaymentsTemplates
      parameters:
      - in: query
        name: allow_check
      - in: query
        name: allow_mo
      - in: query
        name: allow_other
      - in: query
        name: allow_paypal
      - in: query
        name: city
      - in: query
        name: country_id
      - in: query
        name: first_line
      - in: query
        name: name
      - in: query
        name: paypal_email
      - in: query
        name: second_line
      - in: query
        name: state
      - in: query
        name: zip
      responses:
        200:
          description: OK
      tags:
      - payments
      - templates
definitions: []
x-collection-name: Etsy
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