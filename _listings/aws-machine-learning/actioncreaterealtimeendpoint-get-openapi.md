---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 0
info:
  title: AWS Machine Learning API Create Realtime Endpoint
  version: 1.0.0
  description: Creates a real-time endpoint for the MLModel.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateRealtimeEndpoint:
    get:
      summary: Create Realtime Endpoint
      description: Creates a real-time endpoint for the MLModel.
      operationId: createRealtimeEndpoint
      x-api-path-slug: actioncreaterealtimeendpoint-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel during creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Real Time
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