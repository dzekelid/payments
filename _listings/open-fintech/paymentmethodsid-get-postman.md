{
  "info": {
    "name": "Open FinTech Payment method by ID",
    "_postman_id": "8779abf9-c586-4ae0-8ad3-7f94ae54ca50",
    "description": "Returns payment method with specific ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Merchant-industries",
      "item": [
        {
          "id": "c03448c4-9853-4001-910e-a0cf54648ef6",
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
              "id": "fb404dd2-fc63-4332-a21b-96e6392f14e7"
            }
          ]
        },
        {
          "id": "4cb2fdf3-c2fc-4d01-bba0-024fe7b6f140",
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
              "id": "4753e4c9-b7d5-4ec7-916e-09a02be4273d"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment-methods",
      "item": [
        {
          "id": "ca3c93fe-08b5-4e7f-924b-455178b19bda",
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
              "id": "a11121c3-e6b7-47b9-ab0f-61332091940b"
            }
          ]
        },
        {
          "id": "cd5ce964-4cae-4d54-afe1-0b77992fadf3",
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
              "id": "b9f7f7a5-5ad7-48ad-a7b6-d92b2cf6e415"
            }
          ]
        }
      ]
    }
  ]
}