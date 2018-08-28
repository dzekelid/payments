---
name: Coord
x-slug: coord
description: Coord is a mobility company that creates seamless mobility and self-driving
  experiences today through deep integrations. The company offers bike-share API,
  Curbs API, Tolls API, Routing API and etc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
x-kinRank: "7"
x-alexaRank: "1035226"
tags: Payments
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Users API - Update the user's stripe payment info
  x-api-slug: usercurrentstripe-info-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/coord/usercurrentstripe-info-post-openapi.md
- name: Users API - Update the user's stripe payment info
  x-api-slug: usercurrentstripe-info-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/coord/usercurrentstripe-info-post-openapi.md
- name: Users API - Update the user's stripe payment info
  x-api-slug: usercurrentstripe-info-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/coord/usercurrentstripe-info-post-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/coord
- type: x-blog-rss
  url: https://medium.com/feed/coord
- type: x-openapi
  url: https://jsapi.apiary.io/apis/coordprodsearchtolls.source
- type: x-api-gallery
  url: http://convertapi.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coord.stack.network
- type: x-developer
  url: https://coord.co/docs/
- type: x-pricing
  url: https://coord.co/#pricing
- type: x-twitter
  url: https://twitter.com/coordcity
- type: x-website
  url: https://coord.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---