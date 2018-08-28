---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Event Payments
  description: Allows organizers of a group to note payments made by members for an
    event. This is the 'Mark Paid' feature seen in the RSVP listings on event details
    pages and affects the 'pay_status' response fields in [2/rsvps](/meetup_api/docs/2/rsvps/#response)
    for paid events
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/events/:id/payments:
    post:
      summary: Event Payments
      description: Allows organizers of a group to note payments made by members for
        an event. This is the 'Mark Paid' feature seen in the RSVP listings on event
        details pages and affects the 'pay_status' response fields in [2/rsvps](/meetup_api/docs/2/rsvps/#response)
        for paid events
      operationId: events
      x-api-path-slug: urlnameeventsidpayments-post
      parameters:
      - in: query
        name: amount
        description: The monetary amount of money the member submitted
        type: string
      - in: query
        name: member
        description: Member Id of member who made a payment
        type: string
      - in: query
        name: paid_on
        description: The time the payment was made in milliseconds from the epoc
        type: string
      - in: query
        name: quantity
        description: The number of payments made
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
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