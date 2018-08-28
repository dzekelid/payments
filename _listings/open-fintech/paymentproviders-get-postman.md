{
  "info": {
    "name": "Open FinTech List of payment providers",
    "_postman_id": "51737d3a-eef8-466d-bf4f-9561fef96d2a",
    "description": "A payment service provider (PSP) offers shops online services for accepting electronic payments by a variety of payment methods.<br> Endpoint returns list of PSPs. Each object contains: name, type, supported features and sales channels, also related link to available payment methods and main organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Merchant-industries",
      "item": [
        {
          "id": "6dbeba7a-8b57-4203-a237-34c52b18c1d6",
          "name": "merchant_industries.get",
          "request": {
            "url": "http://api.openfintech.io/v1/merchant-industries?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all available merchant fields of activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65d96d3a-5964-4ca6-9f7c-8bab8aad849d"
            }
          ]
        },
        {
          "id": "482d972c-0f80-4b05-83b0-80725340cd3e",
          "name": "merchant_industries.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.openfintech.io",
              "path": [
                "v1",
                "merchant-industries/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns merchant industry with specific ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da760ecb-7e8a-43e3-a3dc-4487e1802b99"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment-methods",
      "item": [
        {
          "id": "10f91f7f-d059-43a8-8b22-ed921e600787",
          "name": "payment_methods.get",
          "request": {
            "url": "http://api.openfintech.io/v1/payment-methods?filter[category]=%7B%7D&filter[processor_name]=%7B%7D&filter[search]=%7B%7D&No Name=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of payment methods. Each object contains information about payment method such as name and category, also related link to payment method issuer (which processing it)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b2cae49-9681-4d75-95cb-27eebe105698"
            }
          ]
        },
        {
          "id": "152667e2-dd36-415e-a8f6-ca82f85aff4d",
          "name": "payment_methods.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.openfintech.io",
              "path": [
                "v1",
                "payment-methods/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns payment method with specific ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59b66fe4-012a-442b-8383-d28f531653a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment-providers",
      "item": [
        {
          "id": "752bbb71-323c-4ec2-9de0-0add57633860",
          "name": "payment_providers.get",
          "request": {
            "url": "http://api.openfintech.io/v1/payment-providers?filter[features]=%7B%7D&filter[sales_channels]=%7B%7D&filter[search]=%7B%7D&filter[types]=%7B%7D&No Name=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A payment service provider (PSP) offers shops online services for accepting electronic payments by a variety of payment methods.<br> Endpoint returns list of PSPs. Each object contains: name, type, supported features and sales channels, also related link to available payment methods and main organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "270e2205-7e0e-4cba-b2f2-acc789593c3e"
            }
          ]
        }
      ]
    }
  ]
}