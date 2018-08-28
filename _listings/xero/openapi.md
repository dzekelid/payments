swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Xero oAuth 1a
  description: a-collection-to-authenticate-to-the-xero-api-using-oauth1-0a
  version: 1.0.0
host: api.xero.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Payments:
    get:
      summary: Get Payments
      description: Get payments.
      operationId: getPayments
      x-api-path-slug: payments-get
      parameters:
      - in: query
        name: No Name
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
      - Payments
    post:
      summary: Post Payments
      description: Post payments.
      operationId: postPayments
      x-api-path-slug: payments-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
    put:
      summary: Put Payments
      description: Put payments.
      operationId: putPayments
      x-api-path-slug: payments-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
    x-related-model:
      summary: X-related-model Payments
      description: X-related-model payments.
      operationId: x-related-modelPayments
      x-api-path-slug: payments-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Payments
  /Payments/{PaymentID}:
    get:
      summary: Get Payments Payment
      description: Get payments payment.
      operationId: getPaymentsPayment
      x-api-path-slug: paymentspaymentid-get
      parameters:
      - in: path
        name: PaymentID
      responses:
        200:
          description: OK
      tags:
      - Payments
      - PaymentID
    post:
      summary: Post Payments Payment
      description: Post payments payment.
      operationId: postPaymentsPayment
      x-api-path-slug: paymentspaymentid-post
      parameters:
      - in: path
        name: PaymentID
      - in: body
        name: Payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
      - PaymentID
    x-related-model:
      summary: X-related-model Payments Payment
      description: X-related-model payments payment.
      operationId: x-related-modelPaymentsPayment
      x-api-path-slug: paymentspaymentid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Payments
      - PaymentID