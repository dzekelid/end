---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Line s  Status  Start Date to  End Date
  description: Gets the line status for given line ids during the provided dates e.g
    minor delays.
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Line/{ids}/Status/{StartDate}/to/{EndDate}:
    get:
      summary: Line s  Status  Start Date to  End Date
      description: Gets the line status for given line ids during the provided dates
        e.g minor delays.
      operationId: Line_Status
      x-api-path-slug: lineidsstatusstartdatetoenddate-get
      parameters:
      - in: query
        name: dateRange.endDate
      - in: query
        name: dateRange.startDate
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: query
        name: endDate
      - in: path
        name: EndDate
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: query
        name: startDate
      - in: path
        name: StartDate
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Status
      - ""
      - Start
      - Date
      - To
      - ""
      - End
      - Date
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