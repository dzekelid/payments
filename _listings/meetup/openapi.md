---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  description: the-meetup-api-provides-simple-restful-http-and-streaming-interfaces-for-exploring-and-interacting-meetup-platform-from-your-own-apps--the-api-is-a-set-of-core-methods-and-a-common-request-format--these-are-combined-to-form-a-url-that-returns-the-information-you-want--
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
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Events
      - Payments
---