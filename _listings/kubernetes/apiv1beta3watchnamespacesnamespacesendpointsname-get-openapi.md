---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Watch Namespaces Endpoints Name
  version: 1.0.0
  description: Watch a particular endpoints.
host: /api/v1beta3
basePath: 127.0.0.1:6443
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1beta3/endpoints:
    get:
      summary: Get Endpoints
      description: List objects of kind endpoints.
      operationId: listEndpoints
      x-api-path-slug: apiv1beta3endpoints-get
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /api/v1beta3/namespaces/{namespaces}/endpoints:
    get:
      summary: Get Namespaces Endpoints
      description: List objects of kind endpoints.
      operationId: listEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpoints-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
    post:
      summary: Post Namespaces Endpoints
      description: Create a endpoints.
      operationId: createEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpoints-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
  /api/v1beta3/namespaces/{namespaces}/endpoints/{name}:
    get:
      summary: Get Namespaces Endpoints Name
      description: Read the specified endpoints.
      operationId: readEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpointsname-get
      parameters:
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
      - Name
    put:
      summary: Put Namespaces Endpoints Name
      description: Update the specified endpoints.
      operationId: updateEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpointsname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
      - Name
  /api/v1beta3/watch/endpoints:
    get:
      summary: Get Watch Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchendpoints-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Endpoints
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints:
    get:
      summary: Get Watch Namespaces Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpoints-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints/{name}:
    get:
      summary: Get Watch Namespaces Endpoints Name
      description: Watch a particular endpoints.
      operationId: watchEndpoints
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpointsname-get
      parameters:
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
      - Name
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