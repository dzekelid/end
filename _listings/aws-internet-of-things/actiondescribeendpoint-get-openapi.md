---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Describe Endpoint
  version: 1.0.0
  description: Returns a unique endpoint specific to the AWS account making the call.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEndpoint:
    get:
      summary: Describe Endpoint
      description: Returns a unique endpoint specific to the AWS account making the
        call.
      operationId: describeEndpoint
      x-api-path-slug: actiondescribeendpoint-get
      parameters:
      - in: query
        name: endpointAddress
        description: The endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
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