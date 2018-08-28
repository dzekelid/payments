---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Users API Update the user's stripe payment info
  description: |-
    Update the Stripe information associated with this user. You must call this endpoint in
    order for the current user to transact with a system that requires Stripe information. If
    this is the case, the system's transaction_info will contain
    `stripe_info.stripe_customer_id` in the `users_api_fields` array.

    Note that it's not possible to call this endpoint for test users (using a test JWT) and as
    such we do not support test transactions for any system with the
    stripe_info.stripe_customer_id requirement. If you are interested in transacting, please
    contact sales@coord.co.

    The request body must contain a Stripe token for this user that's targeted to Coord. You
    can do this either by tokenizing a new credit card on Stripe, or by generating a token from
    an existing Stripe customer in your system. In order to target the token to Coord, you must
    have already registered your Stripe account as a "platform" via Stripe Connect, and we must
    have accepted an invitation to connect to your platform. Assuming that has happened,
    you'll be able to generate coord-targeted tokens via an API call like the folllwing:

    Assuming your already have a customer with id `cus_abc` on your side:

    ```
    curl https://api.stripe.com/v1/tokens \
      -u sk_your_stripe_secret_key: \
      -d customer=cus_abc \
      -H "Stripe-Account: acct_coord_connected_account_id"
    ```

    Note the Stripe-Account header, which tells Stripe to create a token targeted to a specific
    connected account. You must always include that header and set its value to the ID of
    Coord's connected account, which you can find here: https://dashboard.stripe.com/applications/users.

    See https://stripe.com/docs/api#tokens for more info on Stripe tokens.

    ```
      {
        "coord_targeted_token": "tok_123"
      }
    ```

    On success, the response will be the identical object with a customer_id field set. This ID
    is the ID of the customer that Coord creates on Stripe.
    ```
      {
        "coord_targeted_token": "tok_123"
        "customer_id": "cus_xyz"
      }
    ```
  version: 1.0.0
host: api.coord.co
basePath: /v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/current/stripe_info:
    post:
      summary: Update the user's stripe payment info
      description: |-
        Update the Stripe information associated with this user. You must call this endpoint in
        order for the current user to transact with a system that requires Stripe information. If
        this is the case, the system's transaction_info will contain
        `stripe_info.stripe_customer_id` in the `users_api_fields` array.

        Note that it's not possible to call this endpoint for test users (using a test JWT) and as
        such we do not support test transactions for any system with the
        stripe_info.stripe_customer_id requirement. If you are interested in transacting, please
        contact sales@coord.co.

        The request body must contain a Stripe token for this user that's targeted to Coord. You
        can do this either by tokenizing a new credit card on Stripe, or by generating a token from
        an existing Stripe customer in your system. In order to target the token to Coord, you must
        have already registered your Stripe account as a "platform" via Stripe Connect, and we must
        have accepted an invitation to connect to your platform. Assuming that has happened,
        you'll be able to generate coord-targeted tokens via an API call like the folllwing:

        Assuming your already have a customer with id `cus_abc` on your side:

        ```
        curl https://api.stripe.com/v1/tokens \
          -u sk_your_stripe_secret_key: \
          -d customer=cus_abc \
          -H "Stripe-Account: acct_coord_connected_account_id"
        ```

        Note the Stripe-Account header, which tells Stripe to create a token targeted to a specific
        connected account. You must always include that header and set its value to the ID of
        Coord's connected account, which you can find here: https://dashboard.stripe.com/applications/users.

        See https://stripe.com/docs/api#tokens for more info on Stripe tokens.

        ```
          {
            "coord_targeted_token": "tok_123"
          }
        ```

        On success, the response will be the identical object with a customer_id field set. This ID
        is the ID of the customer that Coord creates on Stripe.
        ```
          {
            "coord_targeted_token": "tok_123"
            "customer_id": "cus_xyz"
          }
        ```
      operationId: post_stripe_info
      x-api-path-slug: usercurrentstripe-info-post
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: body
        name: stripe_info
        description: A `StripeInfo` object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Stripe
      - Payment
      - Info
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