swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/listings/{slug}/state/end:
    put:
      summary: Put My Listings Slug State End
      description: Put my listings slug state end.
      operationId: putMyListingsSlugStateEnd
      x-api-path-slug: mylistingsslugstateend-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
      - Slug
      - State
      - End