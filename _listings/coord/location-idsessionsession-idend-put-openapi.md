---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Parking Access API End a previously started session
  description: |-
    End a previously started session. Note that it is invalid to call this method for sessions
    where checkout is controlled physically (those returned with a `redemption_info` field).

    On success, the response will be the existing session with billing info:
    ```
      {
        "billing_info": {
          "cost": {
            "amount": 100,
            "currency": "USD"
          }
        },
        "end_time": "2018-04-12T00:17:50.161Z",
        "id":1,
        "start_time":"2018-04-12T00:14:20.292Z",
        "user_id":"00000000-0000-0000-0000-000000000000"
      }
    ```
  version: 1.0.0
host: api.coord.co
basePath: /v1/access/parking
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{location_id}/session/{session_id}/end:
    put:
      summary: End a previously started session
      description: |-
        End a previously started session. Note that it is invalid to call this method for sessions
        where checkout is controlled physically (those returned with a `redemption_info` field).

        On success, the response will be the existing session with billing info:
        ```
          {
            "billing_info": {
              "cost": {
                "amount": 100,
                "currency": "USD"
              }
            },
            "end_time": "2018-04-12T00:17:50.161Z",
            "id":1,
            "start_time":"2018-04-12T00:14:20.292Z",
            "user_id":"00000000-0000-0000-0000-000000000000"
          }
        ```
      operationId: end_session
      x-api-path-slug: location-idsessionsession-idend-put
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - End
      - Previously
      - Started
      - Session
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