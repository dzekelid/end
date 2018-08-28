---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: End
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/end/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops - Create a new incident
  x-api-slug: apipublicv1incidents-post
  description: |-
    Create a new incident.

    This call replicates the function of our
    manual incident creation process.
    Monitoring tools and custom integrations
    should be configured using our
    REST Endpoint.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com//
  tags: Orchestration, Stack Network, Technology, SaaS, Enterprise, internet, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/end/master/_listings/victorops/apipublicv1incidents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/end/master/_listings/victorops/apipublicv1incidents-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://vestorly.api.gallery.streamdata.io
- type: x-api-stack
  url: http://victorops.stack.network
- type: x-blog
  url: https://victorops.com/blog/
- type: x-blog-rss
  url: https://victorops.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/victorops
- type: x-email
  url: support@victorops.com
- type: x-email
  url: info@victorops.com
- type: x-email
  url: press@victorops.com
- type: x-email
  url: sales@victorops.com
- type: x-github
  url: https://github.com/victorops
- type: x-openapi
  url: https://portal.victorops.com/api-docs/victorops-api-v1.yaml
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: http://victorops.com
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---