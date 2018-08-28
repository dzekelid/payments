---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Get a Payment Token
  version: 1.0.0
  description: Get a payment token.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/PaymentTokens:
    post:
      summary: Adds a new paymenttoken to the system
      description: Adds a new paymenttoken to the system.
      operationId: PaymentToken_Post
      x-api-path-slug: 3dcartwebapiv1paymenttokens-post
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Paymenttoken
      - To
      - System
    put:
      summary: This method is used to update multiple paymenttokens in the database.
        No URL parameters should be included.
      description: This method is used to update multiple paymenttokens in the database.
        no url parameters should be included..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokens-put
      parameters:
      - in: body
        name: paymenttokens
        description: A Json or XML object containing the new PaymentTokens
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Paymenttokens
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    get:
      summary: Get all Payment Tokens
      description: Get all payment tokens.
      operationId: PaymentToken_GetAllPaymentTokens
      x-api-path-slug: 3dcartwebapiv1paymenttokens-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Tokens
  /3dCartWebAPI/v1/PaymentTokens/{paymenttokenid}:
    put:
      summary: This method is used to update a single paymenttoken record in the database.
        The {paymenttokenid} parameter specifies which paymenttoken record to update.
      description: This method is used to update a single paymenttoken record in the
        database. the {paymenttokenid} parameter specifies which paymenttoken record
        to update..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokenspaymenttokenid-put
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new paymenttoken
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: paymenttokenid
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Paymenttoken
      - Record
      - In
      - Database
      - ""
      - Paymenttokenid
      - Parameter
      - Specifies
      - Which
      - Paymenttoken
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/PaymentTokens/{id}:
    get:
      summary: Get a Payment Token
      description: Get a payment token.
      operationId: PaymentToken_GetPaymentToken
      x-api-path-slug: 3dcartwebapiv1paymenttokensid-get
      parameters:
      - in: path
        name: id
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Token
    delete:
      summary: Deletes a Payment Token in the system
      description: Deletes a payment token in the system.
      operationId: PaymentToken_Delete
      x-api-path-slug: 3dcartwebapiv1paymenttokensid-delete
      parameters:
      - in: path
        name: id
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Payment
      - Token
      - In
      - System
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