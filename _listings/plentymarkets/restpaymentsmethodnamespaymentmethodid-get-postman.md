{
  "info": {
    "name": "Plentymarkets List all payment method names for a payment method id",
    "_postman_id": "1e9d2ae1-c620-45c9-9a84-505e60674f66",
    "description": "List all payment method names for a payment method id. The payment method id must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "22cfefee-d1ca-4f06-b215-e12878a60114",
          "name": "getRestPaymentsMethodnamesPaymentmethod",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/payments/methodNames/:paymentMethodId"
              ],
              "query": [
                {
                  "key": "itemsPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "paymentMethodId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List all payment method names for a payment method id. The payment method id must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d4e141b-b97b-4610-a5aa-bb7619672370"
            }
          ]
        }
      ]
    }
  ]
}