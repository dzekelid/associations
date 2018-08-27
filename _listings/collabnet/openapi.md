swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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
    put:
      summary: Creates association
      description: Creates association.
      operationId: createAssociation
      x-api-path-slug: objectsobjectidassociationstargetid-put
      parameters:
      - in: body
        name: body
        description: Association parameters
        schema:
          $ref: '#/definitions/holder'
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
      - Creates
      - Association
  /objects/{objectid}/associations:
    get:
      summary: Gets the association information for the given object id
      description: Gets the association information for the given object id.
      operationId: getObjectAssociations
      x-api-path-slug: objectsobjectidassociations-get
      parameters:
      - in: query
        name: depth
        description: Number of levels
      - in: query
        name: includeDependencies
        description: Include dependency associations (parent and child)
      - in: query
        name: includeEvents
        description: Include events
      - in: query
        name: includePhantoms
        description: Include phantom events
      - in: query
        name: limit
        description: Maximum number of generic associations for an object
      - in: path
        name: objectid
        description: Object/Activity id
      responses:
        200:
          description: OK
      tags:
      - Association
      - Informationthe
      - Given
      - Object
  /associations:
    get:
      summary: Gets the association information for the given object/activity ids
      description: Gets the association information for the given object/activity
        ids.
      operationId: getAssociations
      x-api-path-slug: associations-get
      parameters:
      - in: query
        name: depth
        description: Number of levels
      - in: query
        name: ids
        description: Comma separated object ids
      - in: query
        name: includeDependencies
        description: Include dependency associations (parent and child)
      - in: query
        name: includeEvents
        description: Include events
      - in: query
        name: includePhantoms
        description: Include phantom events
      - in: query
        name: limit
        description: Maximum number of generic associations for an object
      responses:
        200:
          description: OK
      tags:
      - Association
      - Informationthe
      - Given
      - Object
      - Activitys