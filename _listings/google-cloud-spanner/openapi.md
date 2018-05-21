---
swagger: "2.0"
x-collection-name: Google Cloud Spanner
x-complete: 1
info:
  title: Cloud Spanner
  description: cloud-spanner-is-a-managed-missioncritical-globally-consistent-and-scalable-relational-database-service
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
    post:
      summary: Create Database
      description: |-
        Creates a new Cloud Spanner database and starts to prepare it for serving.
        The returned long-running operation will
        have a name of the format `<database_name>/operations/<operation_id>` and
        can be used to track preparation of the database. The
        metadata field type is
        CreateDatabaseMetadata. The
        response field type is
        Database, if successful.
      operationId: spanner.projects.instances.databases.create
      x-api-path-slug: v1parentdatabases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
---