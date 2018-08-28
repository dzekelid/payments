---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Update Payment Status
  description: Update Payment Status
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/events/{event-id}/registrants/{registrant-id}/paymentstatus:
    get:
      summary: Get Payment Status
      description: Get Payment Status
      operationId: get-payment-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidpaymentstatus-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Status
    put:
      summary: Update Payment Status
      description: Update Payment Status
      operationId: update-payment-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidpaymentstatus-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Status
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