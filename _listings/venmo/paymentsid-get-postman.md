{
  "info": {
    "name": "Venmo API Get Payments",
    "_postman_id": "fde7704f-8150-4513-bdd8-525b12e03399",
    "description": "Get payments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "c498357a-f440-4ca1-873d-717996420986",
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
              "id": "1150ca56-3ba7-48ac-8c6a-a573498f0499"
            }
          ]
        }
      ]
    },
    {
      "name": "Payments",
      "item": [
        {
          "id": "28929a1a-ab26-4204-bd6f-57e8a12423a1",
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
              "id": "1872e6eb-2d43-4811-98e9-7c60b723a306"
            }
          ]
        },
        {
          "id": "930fe6ac-4bf6-4270-9f46-59ac9763ebad",
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
              "id": "34e08ce5-1598-4163-9b93-82555479ec34"
            }
          ]
        },
        {
          "id": "40c56e62-085f-4e57-a8ab-79af921d1432",
          "name": "getPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.venmo.com",
              "path": [
                "v1",
                "payments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
              "id": "14f195c5-37df-4db6-9a89-3a144228aaec"
            }
          ]
        }
      ]
    }
  ]
}