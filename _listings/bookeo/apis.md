---
name: Bookeo
x-slug: bookeo
description: Bookeo provides a leading online booking and scheduling system for tours,
  classes, and appointments, to help you save money and time. Click to learn more!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
x-kinRank: "7"
x-alexaRank: "23042"
tags: Payments
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/bookeo/apis.md
specificationVersion: "0.14"
apis:
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Get a list of payments received
  x-api-slug: payments-get
  description: Get a list of payments received.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/bookeo/payments-get-openapi.md
- name: Bookeo - Retrieve a specific payment
  x-api-slug: paymentsid-get
  description: Retrieve a specific payment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/bookeo/paymentsid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bmc.software.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bookeo.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bookeo
- type: x-developer
  url: https://www.bookeo.com/api/
- type: x-documentation
  url: https://www.bookeo.com/apiref/index.html
- type: x-partners
  url: https://www.bookeo.com/affiliate/
- type: x-privacy-policy
  url: https://www.bookeo.com/privacy/
- type: x-terms-of-service
  url: https://www.bookeo.com/termsofservice/
- type: x-twitter
  url: https://twitter.com/bookeo
- type: x-webhook
  url: https://www.bookeo.com/api/webhooks/
- type: x-website
  url: https://www.bookeo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---