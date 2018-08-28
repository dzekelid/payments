swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment_update:
    get:
      summary: Get Payment Update
      description: This method creates or updates the payment options for this event.
        Only the fields passed as arguments will be modified.
      operationId: Get_payment_update_
      x-api-path-slug: payment-update-get
      parameters:
      - in: query
        name: accept_cash
        description: Accept ???Pay by Cash??? payments (1 or 0)
      - in: query
        name: accept_check
        description: Accept ???Pay by Check??? payments (1 or 0)
      - in: query
        name: accept_google
        description: Accept Google Checkout payments (1 or 0)
      - in: query
        name: accept_invoice
        description: Accept ???Send an Invoice??? payments (1 or 0)
      - in: query
        name: accept_paypal
        description: Accept PayPal payments (1 or 0)
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: google_merchant_id
        description: Google Checkout Merchant ID
      - in: query
        name: google_merchant_key
        description: Google Checkout Merchant Key
      - in: query
        name: instructions_cash
        description: Instructions to attendees who want to pay by cash
      - in: query
        name: instructions_check
        description: Instructions to attendees who want to pay by check
      - in: query
        name: instructions_invoice
        description: Instructions to attendees who need to be sent an invoice
      - in: query
        name: paypal_email
        description: Your PayPal email
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Update