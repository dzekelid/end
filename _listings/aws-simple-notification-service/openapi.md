swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 1
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
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
  /?Action=GetEndpointAttributes:
    get:
      summary: Get Endpoint Attributes
      description: |-
        Retrieves the endpoint attributes for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: getEndpointAttributes
      x-api-path-slug: actiongetendpointattributes-get
      parameters:
      - in: query
        name: EndpointArn
        description: EndpointArn for GetEndpointAttributes input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=ListEndpointsByPlatformApplication:
    get:
      summary: List Endpoints By Platform Application
      description: |-
        Lists the endpoints and endpoint attributes for devices in a supported push notification
              service, such as GCM and APNS.
      operationId: listEndpointsByPlatformApplication
      x-api-path-slug: actionlistendpointsbyplatformapplication-get
      parameters:
      - in: query
        name: NextToken
        description: NextToken string is used when calling ListEndpointsByPlatformApplication
          action to retrieve additional records that are available after the first
          page results
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for ListEndpointsByPlatformApplicationInput
          action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=SetEndpointAttributes:
    get:
      summary: Set Endpoint Attributes
      description: |-
        Sets the attributes for an endpoint for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: setEndpointAttributes
      x-api-path-slug: actionsetendpointattributes-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the endpoint attributes
        type: string
      - in: query
        name: EndpointArn
        description: EndpointArn used for SetEndpointAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints