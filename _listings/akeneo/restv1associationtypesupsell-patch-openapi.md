---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API association type (2.x only)
  description: Association type (2.x only).
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/association-types/upsell:
    get:
      summary: association type (2.x only)
      description: Assuming that the given code is the code of an existing association
        type
      operationId: RestV1AssociationTypesUpsellGet
      x-api-path-slug: restv1associationtypesupsell-get
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
    patch:
      summary: association type (2.x only)
      description: Association type (2.x only).
      operationId: RestV1AssociationTypesUpsellPatch
      x-api-path-slug: restv1associationtypesupsell-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
  /rest/v1/association-types:
    get:
      summary: association types (2.x only)
      description: Association types (2.x only).
      operationId: RestV1AssociationTypesGet
      x-api-path-slug: restv1associationtypes-get
      responses:
        200:
          description: OK
      tags:
      - Association
      - Types
      - (2
      - X
      - Only)
    post:
      summary: association type (2.x only)
      description: Assuming that there is no "new_association_type" already existing
      operationId: RestV1AssociationTypesPost
      x-api-path-slug: restv1associationtypes-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
    patch:
      summary: association types (2.x only)
      description: Association types (2.x only).
      operationId: RestV1AssociationTypesPatch
      x-api-path-slug: restv1associationtypes-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Types
      - (2
      - X
      - Only)
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