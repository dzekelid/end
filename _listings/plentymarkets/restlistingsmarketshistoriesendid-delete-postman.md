{
  "info": {
    "name": "Plentymarkets End the listing",
    "_postman_id": "8cd0d970-acd2-4237-b6a1-6ba72aaab29b",
    "description": "Ends the listing on the designated market.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "End",
      "item": [
        {
          "id": "beb1dd7e-6e0c-4f3a-919d-304170bfbeda",
          "name": "deleteRestListingsMarketsHistoriesEnd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/listings/markets/histories/end/:id?"
              ],
              "query": [
                {
                  "key": "deleteOnSuccess",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id?",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Ends the listing on the designated market."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a98aa1cf-fa25-4954-80b1-c98cc6863047"
            }
          ]
        }
      ]
    }
  ]
}