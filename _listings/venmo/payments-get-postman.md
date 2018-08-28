{
  "info": {
    "name": "Venmo API Get Payments",
    "_postman_id": "22ad525d-64d8-43ab-a228-a9b257ef1f9e",
    "description": "Get payments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "8b1c8e1e-cf87-48be-b766-d51addf72df0",
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
              "id": "b87d3221-0848-494f-aa3f-58aa295e7b28"
            }
          ]
        }
      ]
    },
    {
      "name": "Payments",
      "item": [
        {
          "id": "9b9f4c5a-8a6f-4ad6-b32c-ff740841b3c5",
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
              "id": "1a4bb1bc-eedc-4faf-b9a3-3bd336256797"
            }
          ]
        }
      ]
    }
  ]
}