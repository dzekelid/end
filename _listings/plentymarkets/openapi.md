swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/listings/markets/histories/end/{id?}:
    delete:
      summary: End the listing
      description: Ends the listing on the designated market.
      operationId: deleteRestListingsMarketsHistoriesEnd
      x-api-path-slug: restlistingsmarketshistoriesendid-delete
      parameters:
      - in: query
        name: deleteOnSuccess
        description: Tells if the listing market history should also be deleted from
          the database
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - End
      - Listing