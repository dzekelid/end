swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
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