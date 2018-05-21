---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Catalog List Databases
  description: Retrieves the list of databases from the Data Lake Analytics catalog.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/usql/databases/{databaseName}/schemas/{schemaName}/statistics:
    get:
      summary: Catalog List Table Statistics By Database And Schema
      description: Retrieves the list of all table statistics within the specified
        schema from the Data Lake Analytics catalog.
      operationId: Catalog_ListTableStatisticsByDatabaseAndSchema
      x-api-path-slug: catalogusqldatabasesdatabasenameschemasschemanamestatistics-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the statistics
      - in: query
        name: No Name
      - in: path
        name: schemaName
        description: The name of the schema containing the statistics
      responses:
        200:
          description: OK
      tags:
      - Catalog Table Statistic Database Schema
  /catalog/usql/databases/{databaseName}/statistics:
    get:
      summary: Catalog List Table Statistics By Database
      description: Retrieves the list of all statistics in a database from the Data
        Lake Analytics catalog.
      operationId: Catalog_ListTableStatisticsByDatabase
      x-api-path-slug: catalogusqldatabasesdatabasenamestatistics-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the table statistics
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Table Statistic Database
  /catalog/usql/databases/{databaseName}/tables:
    get:
      summary: Catalog List Tables By Database
      description: Retrieves the list of all tables in a database from the Data Lake
        Analytics catalog.
      operationId: Catalog_ListTablesByDatabase
      x-api-path-slug: catalogusqldatabasesdatabasenametables-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the tables
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Table Database
  /catalog/usql/databases/{databaseName}/tablevaluedfunctions:
    get:
      summary: Catalog List Table Valued Functions By Database
      description: Retrieves the list of all table valued functions in a database
        from the Data Lake Analytics catalog.
      operationId: Catalog_ListTableValuedFunctionsByDatabase
      x-api-path-slug: catalogusqldatabasesdatabasenametablevaluedfunctions-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the table valued functions
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Table Valued Function Database
  /catalog/usql/databases/{databaseName}/views:
    get:
      summary: Catalog List Views By Database
      description: Retrieves the list of all views in a database from the Data Lake
        Analytics catalog.
      operationId: Catalog_ListViewsByDatabase
      x-api-path-slug: catalogusqldatabasesdatabasenameviews-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the views
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog View Database
  /catalog/usql/databases/{databaseName}:
    get:
      summary: Catalog Get Database
      description: Retrieves the specified database from the Data Lake Analytics catalog.
      operationId: Catalog_GetDatabase
      x-api-path-slug: catalogusqldatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Database
  /catalog/usql/databases:
    get:
      summary: Catalog List Databases
      description: Retrieves the list of databases from the Data Lake Analytics catalog.
      operationId: Catalog_ListDatabases
      x-api-path-slug: catalogusqldatabases-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Catalog Databases
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