{
  "info": {
    "name": "Stripe Get Payments Payment",
    "_postman_id": "792cbddb-c73b-473d-819d-779fa134997e",
    "description": "Get Payments, Payment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "payments",
      "item": [
        {
          "id": "28467f3c-f421-43e3-80dc-dfd77d27f549",
          "name": "getPaymentsPayment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "payments/:payment"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "payment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Payments, Payment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "177db4cd-80ca-4682-8201-7c5216df3f57"
            }
          ]
        }
      ]
    }
  ]
}