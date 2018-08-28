{
  "info": {
    "name": "Open FinTech List of payment methods",
    "_postman_id": "9d71efbd-0a6b-4a08-9915-fd3a4ddb2af4",
    "description": "Returns list of payment methods. Each object contains information about payment method such as name and category, also related link to payment method issuer (which processing it).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Merchant-industries",
      "item": [
        {
          "id": "04f72b21-ab46-4fcf-b239-1396b1f56c88",
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
              "id": "28bc8044-7d43-42eb-b694-f9da8b9424b0"
            }
          ]
        },
        {
          "id": "d28b651f-9a69-476f-9d6d-d2d111ec0698",
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
              "id": "af71b63f-6d29-4666-ab63-de7455148e44"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment-methods",
      "item": [
        {
          "id": "cf16d936-ea1a-42a8-9f75-03dd3b68e0e2",
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
              "id": "9bdbc4d8-ba54-4e03-8a08-cba118c80c90"
            }
          ]
        }
      ]
    }
  ]
}