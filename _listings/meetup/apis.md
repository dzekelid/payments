---
name: Meetup
x-slug: meetup
description: Find Meetups so you can do more of what matters to you. Or create your
  own group and meet people near you who share your interests.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
x-kinRank: "9"
x-alexaRank: "917"
tags: Payments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup Event Payments
  x-api-slug: meetup
  description: Allows organizers of a group to note payments made by members for an
    event. This is the 'Mark Paid' feature seen in the RSVP listings on event details
    pages and affects the 'pay_status' response fields in [2/rsvps](/meetup_api/docs/2/rsvps/#response)
    for paid events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:id/payments
  tags: Events,Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/meetup/urlnameeventsidpayments-post-openapi.md
- name: Meetup
  x-api-slug: meetup
  description: Find Meetups so you can do more of what matters to you. Or create your
    own group and meet people near you who share your interests.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/meetup/openapi.md
x-common:
- type: x-base
  url: http://api.meetup.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/meetup
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-email
  url: privacy@meetup.com
- type: x-email
  url: abuse@meetup.com
- type: x-email
  url: api_license@meetup.com
- type: x-email
  url: arbitration-opt-out@meetup.com
- type: x-email
  url: legal@meetup.com
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-twitter
  url: https://twitter.com/Meetup
- type: x-website
  url: http://meetup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---