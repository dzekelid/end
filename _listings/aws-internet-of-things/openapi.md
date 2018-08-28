swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
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