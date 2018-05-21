---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 1
info:
  title: Cloud SQL Administration
  description: creates-and-configures-cloud-sql-instances-which-provide-fullymanaged-mysql-databases
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances/{instance}/databases:
    get:
      summary: Get Projects Project Instances Instance Databases
      description: Lists databases in the specified Cloud SQL instance.
      operationId: sql.databases.list
      x-api-path-slug: projectsprojectinstancesinstancedatabases-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project for which to list Cloud SQL instances
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
    post:
      summary: Add Projects Project Instances Instance Databases
      description: Inserts a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.insert
      x-api-path-slug: projectsprojectinstancesinstancedatabases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
  /projects/{project}/instances/{instance}/databases/{database}:
    delete:
      summary: Delete Projects Project Instances Instance Databases Database
      description: Deletes a database from a Cloud SQL instance.
      operationId: sql.databases.delete
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
      parameters:
      - in: path
        name: database
        description: Name of the database to be deleted in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    get:
      summary: Get Projects Project Instances Instance Databases Database
      description: Retrieves a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.get
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-get
      parameters:
      - in: path
        name: database
        description: Name of the database in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    patch:
      summary: Patch Projects Project Instances Instance Databases Database
      description: Updates a resource containing information about a database inside
        a Cloud SQL instance. This method supports patch semantics.
      operationId: sql.databases.patch
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Name of the database to be updated in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    put:
      summary: Put Projects Project Instances Instance Databases Database
      description: Updates a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.update
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Name of the database to be updated in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
---