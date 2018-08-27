---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Deletes association
  version: 1.0.0
  description: Deletes association.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /objects/{objectid}/associations/{targetid}:
    delete:
      summary: Deletes association
      description: Deletes association.
      operationId: deleteAssociation
      x-api-path-slug: objectsobjectidassociationstargetid-delete
      parameters:
      - in: path
        name: objectid
        description: Origin object id
      - in: path
        name: targetid
        description: Target object id
      responses:
        200:
          description: OK
      tags:
      - Association
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