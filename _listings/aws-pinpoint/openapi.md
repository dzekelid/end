swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 1
info:
  title: AWS Pinpoint API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/endpoints:
    put:
      summary: Endpoints List
      description: Use the PUT method to update your endpoints.
      operationId: updateEndpointsList
      x-api-path-slug: appsapplicationidendpoints-put
      parameters:
      - in: query
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Endpoint
  /apps/application-id/endpoints/endpoint-id:
    get:
      summary: Endpoint Instance
      description: Use the GET method to request information about an endpoint.
      operationId: getEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-get
      responses:
        200:
          description: OK
      tags:
      - Endpoint
    put:
      summary: Update Endpoint Instance
      description: Use the PUT method to update an endpoint.
      operationId: updateEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-put
      responses:
        200:
          description: OK
      tags:
      - Endpoint