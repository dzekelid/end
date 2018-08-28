---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Api Keys
  description: |-
    **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api_keys:
    get:
      summary: Get Api Keys
      description: |-
        **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: GET_api_keys
      x-api-path-slug: api-keys-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---