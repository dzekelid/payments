{
  "info": {
    "name": "Digital River Shopper API Get Shoppers Me Payment Options",
    "_postman_id": "42705e36-7067-41cc-9df8-d3fc679719a7",
    "description": "Get shoppers me payment options.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth20",
      "item": [
        {
          "id": "2f020f95-f880-4c7e-aeef-6c76af19f0fb",
          "name": "getOauth20Authorize",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../oauth20/authorize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get oauth20 authorize."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42332520-e342-4c28-aa1a-60d95bba59f0"
            }
          ]
        },
        {
          "id": "fd069e84-fb3a-43a2-822c-d5ed091ce263",
          "name": "postOauth20Token",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../oauth20/token",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post oauth20 token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaca48c9-8c38-4db6-8d6e-f222344f4962"
            }
          ]
        }
      ]
    },
    {
      "name": "Shoppers",
      "item": [
        {
          "id": "79ce5096-46d4-4a27-a2af-971c17f7599c",
          "name": "postV1Shoppers",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f8dc6a1-3488-4404-aa65-9d589e36afa3"
            }
          ]
        },
        {
          "id": "3a97d0d1-c639-41e6-a36b-3cdf2ff74959",
          "name": "getV1ShoppersApi",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers-api",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed36f4b-557f-4aac-b359-635be07191c7"
            }
          ]
        },
        {
          "id": "7558fad8-7f3d-42db-8b72-0df8bea37070",
          "name": "getV1ShoppersMe",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2966d07f-0c1f-49cf-88a3-3b310a75d62c"
            }
          ]
        },
        {
          "id": "ef186e69-58ea-45a6-af0b-a09e0367a649",
          "name": "postV1ShoppersMe",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34297693-208f-44fe-95e3-c42755e68876"
            }
          ]
        },
        {
          "id": "faa54211-5e98-41e6-a4ba-91f569d037df",
          "name": "getV1ShoppersMeAccount",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eee23d7-f3bc-4f6c-8d9b-bf1fd6bb99cc"
            }
          ]
        },
        {
          "id": "89233e0c-e057-4d94-818f-d13ff2dd8b9e",
          "name": "getV1ShoppersMeAddresses",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/addresses",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af552c4e-e09c-43c3-9bf3-56fb0ff13549"
            }
          ]
        },
        {
          "id": "ba5493bc-f8aa-4e3c-94b3-42887c6d2845",
          "name": "getV1ShoppersMeAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/addresses/:id"
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
            "description": "Get shoppers me addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d1e8672-6ec0-4138-8892-f83d865e7ace"
            }
          ]
        },
        {
          "id": "dbfa4a28-1861-4ce6-81c7-d99c5f3c8f41",
          "name": "getV1ShoppersMeCartsActive",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed150f96-dc40-4996-b918-0dc1d69e3478"
            }
          ]
        },
        {
          "id": "5204e653-57b2-4ccb-99fd-4a83305d1dd6",
          "name": "postV1ShoppersMeCartsActive",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cd780b9-94a9-41d8-8acf-4a127c1446dc"
            }
          ]
        },
        {
          "id": "ce09f5e5-127d-41ba-aaa7-f9961492d8d2",
          "name": "postV1ShoppersMeCartsActiveApplyShippingOption",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/apply-shipping-option",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active apply shipping option."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33b476fc-a4de-44ca-96c5-7093d6209f57"
            }
          ]
        },
        {
          "id": "49c686bf-0cfa-4122-9ae8-d2ee267a6385",
          "name": "postV1ShoppersMeCartsActiveApplyShopper",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/apply-shopper",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active apply shopper."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b8a849e-051d-4840-8147-d31aed2ddd51"
            }
          ]
        },
        {
          "id": "6fe4c38a-4079-4e6f-99fe-c761ec9307a9",
          "name": "getV1ShoppersMeCartsActiveBillingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/billing-address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0732194d-51a7-4233-a49c-04892c6b0b8d"
            }
          ]
        },
        {
          "id": "a2ce60d0-ec29-4ee9-ac23-110df9b0b1b8",
          "name": "putV1ShoppersMeCartsActiveBillingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/billing-address",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put shoppers me carts active billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "567e2ed6-62ec-45e5-9d20-493e5d0f0cb9"
            }
          ]
        },
        {
          "id": "89eed34e-ee57-4561-9d0c-d475e6b97989",
          "name": "getV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/line-items",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "126e013b-fd60-4af1-814d-a911495edfb8"
            }
          ]
        },
        {
          "id": "ca8ae098-b13a-4be4-be6c-bc74db27c003",
          "name": "postV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/line-items",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c9cb1c7-3b6f-4f2b-b939-5d542dc195de"
            }
          ]
        },
        {
          "id": "d01ff892-a5b6-4925-88fa-692f4ae12893",
          "name": "deleteV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/line-items",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de8c1803-46b6-4fbc-94e5-bf6285291856"
            }
          ]
        },
        {
          "id": "afc339fa-cac1-4a1a-8c73-545a15c4a22c",
          "name": "getV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/carts/active/line-items/:id"
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
            "description": "Get shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f38cf0e-fb6d-409b-af77-b6927d35bd05"
            }
          ]
        },
        {
          "id": "d6aee712-5798-4d82-af13-e406601a025e",
          "name": "postV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/carts/active/line-items/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b84df889-d54c-4ef3-82b6-e290632a8382"
            }
          ]
        },
        {
          "id": "73eb0363-8c9c-4c1a-a579-3179744dbbf6",
          "name": "deleteV1ShoppersMeCartsActiveLineItems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/carts/active/line-items/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete shoppers me carts active line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79134da2-a0d6-41bd-bb5e-8d41809a3b39"
            }
          ]
        },
        {
          "id": "87b033f6-73ec-47d1-a621-ac7ef27f3029",
          "name": "getV1ShoppersMeCartsActivePointOfPromotionsOffers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/carts/active/point-of-promotions/:id/offers"
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
            "description": "Get shoppers me carts active point of promotions offers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "976c6c44-755e-44a9-80f4-27c9396a94a9"
            }
          ]
        },
        {
          "id": "68eed313-c223-4de1-9526-dafadafd3450",
          "name": "getV1ShoppersMeCartsActiveShippingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/shipping-address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active shipping address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edd78ea3-237b-4cdb-a9af-0df8c57fe15f"
            }
          ]
        },
        {
          "id": "d9408b8c-a18c-4162-8142-9cc28820fc3c",
          "name": "putV1ShoppersMeCartsActiveShippingAddress",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/shipping-address",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put shoppers me carts active shipping address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20e34e43-d575-4f1d-8ed1-1d9c22dcb1d8"
            }
          ]
        },
        {
          "id": "4fb54f91-1a2f-4a75-8f41-59c20f041297",
          "name": "getV1ShoppersMeCartsActiveShippingOptions",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/shipping-options",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active shipping options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0abc581a-0276-4003-8cdf-4c40cbb005f0"
            }
          ]
        },
        {
          "id": "a3fa8fc7-6f61-4574-930c-06fd14bc0135",
          "name": "getV1ShoppersMeCartsActiveShippingOptions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/carts/active/shipping-options/:id"
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
            "description": "Get shoppers me carts active shipping options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b2df5fd-61e5-4ba3-9489-73c437bbfac8"
            }
          ]
        },
        {
          "id": "94d82d6e-d8e4-496e-a027-3193f4dab04d",
          "name": "postV1ShoppersMeCartsActiveSubmitCart",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/submit-cart",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active submit cart."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dd8ab07-ed9a-4245-9c92-82390e0a0af9"
            }
          ]
        },
        {
          "id": "a1d484d0-a000-4c76-a19e-cb2533c14e80",
          "name": "getV1ShoppersMeCartsActiveWebCheckout",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/web-checkout",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me carts active web checkout."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5e9781a-a83c-4ca1-ac92-0ae5a9b9ea9f"
            }
          ]
        },
        {
          "id": "c302abed-2009-4a40-bbfe-6cf10caec230",
          "name": "postV1ShoppersMeCartsActiveWebCheckout",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/carts/active/web-checkout",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me carts active web checkout."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2978ca7-4143-45a4-8877-9e3b82e15f87"
            }
          ]
        },
        {
          "id": "30c4e03b-cee2-4f4b-a391-3269b3971afe",
          "name": "getV1ShoppersMeCategories",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c30f14c8-3451-4c1d-8552-bb8812d5d688"
            }
          ]
        },
        {
          "id": "d9e46f37-a9e6-4402-98fd-52e07cf2f31e",
          "name": "getV1ShoppersMeCategories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/categories/:id"
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
            "description": "Get shoppers me categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cabb45d5-bcc8-40e2-99ec-10946eff4aa8"
            }
          ]
        },
        {
          "id": "ad1cd028-3c3f-44b5-a1d7-da2718064d6f",
          "name": "getV1ShoppersMeCategoriesProducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/categories/:id/products"
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
            "description": "Get shoppers me categories products."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d16a6da3-50e5-4e98-bc41-db585c69cf10"
            }
          ]
        },
        {
          "id": "8cad46bf-44df-456c-8e8e-fd28f0b7e5d1",
          "name": "getV1ShoppersMeOrders",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/orders",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f74bfc2-9942-451e-8e7a-cdbc4faba829"
            }
          ]
        },
        {
          "id": "29344c78-875c-40f7-8814-6b3014b328ee",
          "name": "postV1ShoppersMeOrders",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/orders",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post shoppers me orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "518a36b4-c941-4879-81e0-5eac2ce59c93"
            }
          ]
        },
        {
          "id": "1287f3a6-b33e-4a4a-8696-10184db73d11",
          "name": "getV1ShoppersMeOrders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id"
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
            "description": "Get shoppers me orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ec2da8f-a676-410b-b708-baabc3e46634"
            }
          ]
        },
        {
          "id": "b2c7638a-795f-4460-bfd4-b74c25850b25",
          "name": "getV1ShoppersMeOrdersBillingAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id/billing-address"
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
            "description": "Get shoppers me orders billing address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1a939c3-10fa-4f70-a1aa-a75efee676c9"
            }
          ]
        },
        {
          "id": "0ed5f66f-9ac7-4f59-85c7-59dca32aa952",
          "name": "getV1ShoppersMeOrdersLineItems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id/line-items"
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
            "description": "Get shoppers me orders line items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0246757c-a11e-408e-a9a1-560f97e41529"
            }
          ]
        },
        {
          "id": "988564f1-6304-4ac9-a96f-386c1f1c6c54",
          "name": "getV1ShoppersMeOrdersLineItemsLineitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id/line-items/:lineItemId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lineItemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me orders line items lineitemid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2c0ed6e-e55c-42e1-bfda-eed21ae832af"
            }
          ]
        },
        {
          "id": "5be9d199-e77a-4187-8576-220241b74929",
          "name": "getV1ShoppersMeOrdersShippingAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/orders/:id/shipping-address"
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
            "description": "Get shoppers me orders shipping address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a068c287-94cf-4379-a13b-6916106ffc76"
            }
          ]
        },
        {
          "id": "d166f8eb-e8a1-4057-8c53-ce436982d943",
          "name": "getV1ShoppersMePaymentOptions",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/payment-options",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me payment options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5bfc626-73bd-4706-a6ed-eee215232148"
            }
          ]
        }
      ]
    }
  ]
}