swagger: "2.0"
x-collection-name: Open FinTech
x-complete: 1
info:
  title: Open FinTech
  description: openfintech-io-is-an-open-database-that-comprises-of-standardized-primary-data-for-fintech-industry--it-contains-such-information-as-geolocation-data-countries-cities-regions-organizations-currencies-national-digital-virtual-crypto-banks-digital-exchangers-payment-providers-psp-payment-methods-etc-it-is-created-for-communication-of-crossintegrated-microservices-on-one-language--this-is-achieved-through-standardization-of-entity-identifiers-that-are-used-to-exchange-information-among-different-services-
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