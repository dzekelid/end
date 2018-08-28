swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaigns/{CAMPAIGN_ID}/end:
    post:
      summary: Post Campaigns End
      description: /campaigns/{CAMPAIGN_ID}/delete
      operationId: campaignscampaign-iddelete
      x-api-path-slug: campaignscampaign-idend-post
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The ID of the campaign to end
      - in: path
        name: CAMPAIGN_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - End