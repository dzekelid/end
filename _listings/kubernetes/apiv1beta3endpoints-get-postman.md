{
  "info": {
    "name": "Kubernetes Get Endpoints",
    "_postman_id": "9883b19f-1ab0-4106-a801-e9f116d23b57",
    "description": "List objects of kind endpoints.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "b272507f-6d84-4ab0-90a2-f7e89e76f7e3",
          "name": "listEndpoints",
          "request": {
            "url": "http:///api/v1beta3/127.0.0.1:6443/api/v1beta3/endpoints",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List objects of kind endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a599b90-0c99-4c97-ba11-f6e889fb3cf7"
            }
          ]
        }
      ]
    }
  ]
}