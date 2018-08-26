{
  "info": {
    "name": "SendGrid Get Api Keys",
    "_postman_id": "f827489e-06e8-4f8a-ba04-b2b2455e703f",
    "description": "**This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**\n\nThe API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "b6a8e269-dd84-4692-aa65-86ee4969e77e",
          "name": "GET_api_keys",
          "request": {
            "url": "http://api.sendgrid.com/v3/api_keys?limit=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve all API Keys that belong to the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d05acbe6-96d3-424d-b6bc-7b196a128dd4"
            }
          ]
        }
      ]
    }
  ]
}