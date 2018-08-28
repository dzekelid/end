---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API Delete Endpoint
  version: 1.0.0
  description: Deletes the endpoint for a device and mobile app from Amazon SNS.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreatePlatformEndpoint:
    get:
      summary: Create Platform Endpoint
      description: |-
        Creates an endpoint for a device and mobile app on one of the supported push notification
              services, such as GCM and APNS.
      operationId: createPlatformEndpoint
      x-api-path-slug: actioncreateplatformendpoint-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: For a list of attributes, see SetEndpointAttributes
        type: string
      - in: query
        name: CustomUserData
        description: Arbitrary user data to associate with the endpoint
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn returned from CreatePlatformApplication
          is used to create a an endpoint
        type: string
      - in: query
        name: Token
        description: Unique identifier created by the notification service for an
          app on a device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Endpoints
  /?Action=DeleteEndpoint:
    get:
      summary: Delete Endpoint
      description: Deletes the endpoint for a device and mobile app from Amazon SNS.
      operationId: deleteEndpoint
      x-api-path-slug: actiondeleteendpoint-get
      parameters:
      - in: query
        name: EndpointArn
        description: EndpointArn of endpoint to delete
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