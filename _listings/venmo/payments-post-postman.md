{
  "info": {
    "name": "Venmo API Post Payments",
    "_postman_id": "df80b8a7-f4bd-4268-ad8f-eaea033e9617",
    "description": "Post payments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "d431be3f-929c-4da0-820d-c6546ff64c93",
          "name": "getMe",
          "request": {
            "url": "http://api.venmo.com/v1/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get me."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "340b7f19-0fbf-4a50-b556-94958a3fa576"
            }
          ]
        }
      ]
    },
    {
      "name": "Payments",
      "item": [
        {
          "id": "d2bb873c-be78-4ef8-8aaf-60a98d697303",
          "name": "getPayments",
          "request": {
            "url": "http://api.venmo.com/v1/payments",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get payments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9255e94a-90d9-4502-bbda-3710e6efd6de"
            }
          ]
        },
        {
          "id": "a55aa2cf-04b1-461f-b5fa-5ecfd1e76656",
          "name": "postPayments",
          "request": {
            "url": "http://api.venmo.com/v1/payments",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post payments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81f4d9c7-0905-4105-a042-6d291f210944"
            }
          ]
        }
      ]
    }
  ]
}