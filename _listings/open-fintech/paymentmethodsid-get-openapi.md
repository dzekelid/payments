---
swagger: "2.0"
x-collection-name: Open FinTech
x-complete: 0
info:
  title: Open FinTech Payment method by ID
  description: Returns payment method with specific ID.
  version: "2017-08-24"
host: api.openfintech.io
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payment-providers:
    get:
      summary: List of payment providers
      description: 'A payment service provider (PSP) offers shops online services
        for accepting electronic payments by a variety of payment methods.<br> Endpoint
        returns list of PSPs. Each object contains: name, type, supported features
        and sales channels, also related link to available payment methods and main
        organization.'
      operationId: payment_providers.get
      x-api-path-slug: paymentproviders-get
      parameters:
      - in: query
        name: filter[features]
        description: Filtering by features
      - in: query
        name: filter[sales_channels]
        description: Filtering by sales channels
      - in: query
        name: filter[search]
        description: Full text search with id, code, name
      - in: query
        name: filter[types]
        description: Filtering by types
      - in: query
        name: No Name
      - in: query
        name: sort
        description: Sort params:| ASC | DESC ||-----|------|| name | -name || code
          | -code |
      responses:
        200:
          description: OK
      tags:
      - Payment-providers
  /payment-providers/{id}:
    get:
      summary: Payment provider by ID
      description: Returns payment provider with specific ID.
      operationId: payment_providers.id.get
      x-api-path-slug: paymentprovidersid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Payment-providers
  /payment-methods:
    get:
      summary: List of payment methods
      description: Returns list of payment methods. Each object contains information
        about payment method such as name and category, also related link to payment
        method issuer (which processing it).
      operationId: payment_methods.get
      x-api-path-slug: paymentmethods-get
      parameters:
      - in: query
        name: filter[category]
        description: Filtering by category
      - in: query
        name: filter[processor_name]
        description: Filtering by processor_name
      - in: query
        name: filter[search]
        description: Full text search with id, name, code, category
      - in: query
        name: No Name
      - in: query
        name: sort
        description: Sort params:| ASC | DESC ||-----|------|| name | -name || code
          | -code || processor_name | -processor_name || category | -category |
      responses:
        200:
          description: OK
      tags:
      - Payment-methods
  /payment-methods/{id}:
    get:
      summary: Payment method by ID
      description: Returns payment method with specific ID.
      operationId: payment_methods.id.get
      x-api-path-slug: paymentmethodsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Payment-methods
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