---
swagger: "2.0"
x-collection-name: Google Cloud Spanner
x-complete: 0
info:
  title: Google Cloud Spanner API Get Databases
  description: Lists Cloud Spanner databases.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: spanner.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{database}:
    delete:
      summary: Delete Database
      description: Drops (aka deletes) a Cloud Spanner database.
      operationId: spanner.projects.instances.databases.dropDatabase
      x-api-path-slug: v1database-delete
      parameters:
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
  /v1/{database}/ddl:
    get:
      summary: Get Database Schema
      description: |-
        Returns the schema of a Cloud Spanner database as a list of formatted
        DDL statements. This method does not show pending schema updates, those may
        be queried using the Operations API.
      operationId: spanner.projects.instances.databases.getDdl
      x-api-path-slug: v1databaseddl-get
      parameters:
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database Schema
    patch:
      summary: Update Database Schema
      description: |-
        Updates the schema of a Cloud Spanner database by
        creating/altering/dropping tables, columns, indexes, etc. The returned
        long-running operation will have a name of
        the format `<database_name>/operations/<operation_id>` and can be used to
        track execution of the schema change(s). The
        metadata field type is
        UpdateDatabaseDdlMetadata.  The operation has no response.
      operationId: spanner.projects.instances.databases.updateDdl
      x-api-path-slug: v1databaseddl-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database Schema
  /v1/{parent}/databases:
    get:
      summary: Get Databases
      description: Lists Cloud Spanner databases.
      operationId: spanner.projects.instances.databases.list
      x-api-path-slug: v1parentdatabases-get
      parameters:
      - in: query
        name: pageSize
        description: Number of databases to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_token from
          aprevious ListDatabasesResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
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