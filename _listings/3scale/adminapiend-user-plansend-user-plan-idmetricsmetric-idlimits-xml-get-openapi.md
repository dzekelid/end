---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Limit List for End User Plans
  description: Limit list for end user plans .
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  //{hostname}/games/2:
    patch:
      summary: End Game
      description: ""
      operationId: Games2ByHostnamePatch2
      x-api-path-slug: hostnamegames2-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  /admin/api/end_user_plans.xml:
    get:
      summary: End User Plan List (all services)
      description: End user plan list (all services).
      operationId: end_user_plan
      x-api-path-slug: adminapiend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
      - (all
      - Services)
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml:
    delete:
      summary: Limit Delete for End User Plans
      description: Limit delete for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
    put:
      summary: Limit Update for End User Plans
      description: Limit update for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
  /admin/api/services/{service_id}/end_users.xml:
    post:
      summary: End User Create
      description: End user create.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-users-xml-post
      parameters:
      - in: query
        name: plan_id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Create
  /admin/api/services/{service_id}/end_users/{username}.xml:
    delete:
      summary: End User Delete
      description: End user delete.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-usersusername-xml-delete
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: path
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
    get:
      summary: End User Read
      description: End user read.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-usersusername-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: path
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Read
  /admin/api/services/{service_id}/end_users/{username}/change_plan.xml:
    put:
      summary: End User Change Plan
      description: End user change plan.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-usersusernamechange-plan-xml-put
      parameters:
      - in: query
        name: plan_id
        description: id of the new end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: path
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Change
      - Plan
  /admin/api/services/{service_id}/end_user_plans.xml:
    get:
      summary: End User Plan List
      description: End user plan list.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
    post:
      summary: End User Plan Create
      description: End user plan create.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plans-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Create
  /admin/api/services/{service_id}/end_user_plans/{id}.xml:
    get:
      summary: End User Plan Read
      description: End user plan read.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Read
    put:
      summary: End User Plan Update
      description: End user plan update.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: name
        description: Name of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
  /admin/api/services/{service_id}/end_user_plans/{id}/default.xml:
    put:
      summary: End User Plan set to Default
      description: End user plan set to default.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Set
      - To
      - Default
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits.xml:
    get:
      summary: Limit List for End User Plans
      description: Limit list for end user plans .
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - ListEnd
      - User
      - Plans
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