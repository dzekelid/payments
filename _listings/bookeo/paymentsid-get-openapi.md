---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Retrieve a specific payment
  version: 1.0.0
  description: Retrieve a specific payment.
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bookings/{bookingNumber}/payments:
    get:
      summary: Get the payments received for a booking
      description: Get a list of all payments received for a booking. Only payments
        for which the apiKey has at least read permission will be included
      operationId: getBookingsBookingnumberPayments
      x-api-path-slug: bookingsbookingnumberpayments-get
      parameters:
      - in: path
        name: bookingNumber
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Payments
    post:
      summary: Add a payment to a booking
      description: Create a payment record associated with a booking
      operationId: postBookingsBookingnumberPayments
      x-api-path-slug: bookingsbookingnumberpayments-post
      parameters:
      - in: body
        name: apiPayment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bookingNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Payments
  /payments:
    get:
      summary: Get a list of payments received
      description: Get a list of payments received.
      operationId: getPayments
      x-api-path-slug: payments-get
      parameters:
      - in: query
        name: endTime
      - in: query
        name: itemsPerPage
        description: 'maximum: 300'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: paymentMethod
      - in: query
        name: paymentMethodOther
      - in: query
        name: startTime
      responses:
        200:
          description: OK
      tags:
      - Payments
  /payments/{id}:
    get:
      summary: Retrieve a specific payment
      description: Retrieve a specific payment.
      operationId: getPayments
      x-api-path-slug: paymentsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
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