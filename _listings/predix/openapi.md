swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{collection}/{id}:
    get:
      summary: Get entity based on  uri
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: getV1Collection
      x-api-path-slug: v1collectionid-get
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      - in: path
        name: id
        description: ID of the domain object to retrieve
      responses:
        200:
          description: Successful response
      tags:
      - Entity
      - Based
      - "On"
      - ""
      - Uri