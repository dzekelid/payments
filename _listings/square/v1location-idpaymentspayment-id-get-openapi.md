---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Provides comprehensive information for a single payment.
  description: Provides comprehensive information for a single payment.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/payments:
    get:
      summary: Provides summary information for all payments taken by a merchant or
        any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      description: Provides summary information for all payments taken by a merchant
        or any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      operationId: ListPayments
      x-api-path-slug: v1location-idpayments-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list payments for
      - in: query
        name: order
        description: The order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Payments
      - Taken
      - By
      - Merchant
      - Any
      - Of
      - Merchants
      - Mobile
      - Staff
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
      - ""
      - See
      - Date
      - Rangesdetails
      - Of
      - Inclusive
      - Exclusive
      - Dates
  /v1/{location_id}/payments/{payment_id}:
    get:
      summary: Provides comprehensive information for a single payment.
      description: Provides comprehensive information for a single payment.
      operationId: RetrievePayment
      x-api-path-slug: v1location-idpaymentspayment-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the payments associated location
      - in: path
        name: payment_id
        description: The payments Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Payment
  /v1/{location_id}/refunds:
    post:
      summary: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      description: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      operationId: v1.location_id.refunds.post
      x-api-path-slug: v1location-idrefunds-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the original payments associated location
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Refunda
      - Previously
      - Processed
      - Payment
      - ""
      - You
      - Must
      - Issue
      - Refund
      - Within
      - "60"
      - Days
      - Of
      - Associated
      - Payment
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