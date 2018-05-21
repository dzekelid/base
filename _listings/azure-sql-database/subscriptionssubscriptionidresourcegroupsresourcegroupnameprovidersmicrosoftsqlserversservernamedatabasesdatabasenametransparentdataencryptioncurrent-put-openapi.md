---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 0
info:
  title: Azure SQL Database API Databases Create Or Update Transparent Data Encryption
    Configuration
  description: Creates or updates a database's transparent data encryption configuration.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/restorePoints
  : get:
      summary: Databases List Restore Points
      description: Returns a list of database restore points.
      operationId: Databases_ListRestorePoints
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamerestorepoints-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database from which to retrieve available restore
          points
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Restore Points
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/securityAlertPolicies/default
  : get:
      summary: Databases Get Threat Detection Policy
      description: Gets a database's threat detection policy.
      operationId: Databases_GetThreatDetectionPolicy
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which database Threat Detection
          policy is defined
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Threat Detection Policy
    put:
      summary: Databases Create Or Update Threat Detection Policy
      description: Creates or updates a database's threat detection policy.
      operationId: Databases_CreateOrUpdateThreatDetectionPolicy
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which database Threat Detection
          policy is defined
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The database Threat Detection policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Threat Detection Policy
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/import:
    post:
      summary: Databases Import
      description: Imports a bacpac into a new database.
      operationId: Databases_Import
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernameimport-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for importing a Bacpac into a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Import
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/extensions/import
  : put:
      summary: Databases Create Import Operation
      description: Creates an import operation that imports a bacpac into an existing
        database. The existing database must be empty.
      operationId: Databases_CreateImportOperation
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameextensionsimport-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to import into
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for importing a Bacpac into a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Import Operation
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/export
  : post:
      summary: Databases Export
      description: Exports a database to a bacpac.
      operationId: Databases_Export
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameexport-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be exported
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for exporting a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Export
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}
  : delete:
      summary: Databases Delete Replication Link
      description: Deletes a database replication link. Cannot be done during failover.
      operationId: Databases_DeleteReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          dropped
      - in: path
        name: linkId
        description: The ID of the replication link to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Link
    get:
      summary: Databases Get Replication Link
      description: Gets a database replication link.
      operationId: Databases_GetReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to get the link for
      - in: path
        name: linkId
        description: The replication link ID to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Link
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/failover
  : post:
      summary: Databases Failover Replication Link
      description: Sets which replica database is primary by failing over from the
        current primary replica database.
      operationId: Databases_FailoverReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkidfailover-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          failed over
      - in: path
        name: linkId
        description: The ID of the replication link to be failed over
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Failover Replication Link
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/forceFailoverAllowDataLoss
  : post:
      summary: Databases Failover Replication Link Allow Data Loss
      description: Sets which replica database is primary by failing over from the
        current primary replica database. This operation might result in data loss.
      operationId: Databases_FailoverReplicationLinkAllowDataLoss
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkidforcefailoverallowdataloss-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          failed over
      - in: path
        name: linkId
        description: The ID of the replication link to be failed over
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Failover Replication Link Allow Data Loss
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks
  : get:
      summary: Databases List Replication Links
      description: Lists a database's replication links.
      operationId: Databases_ListReplicationLinks
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinks-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to retrieve links for
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Links
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/pause
  : post:
      summary: Databases Pause
      description: Pauses a data warehouse.
      operationId: Databases_Pause
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamepause-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the data warehouse to pause
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Pause
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/resume
  : post:
      summary: Databases Resume
      description: Resumes a data warehouse.
      operationId: Databases_Resume
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameresume-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the data warehouse to resume
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Resume
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}
  : put:
      summary: Databases Create Or Update
      description: Creates a new database or updates an existing database. Location
        is a required property in the request body, and it must be the same as the
        location of the SQL server.
      operationId: Databases_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasename-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be operated on (updated or created)
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases
    delete:
      summary: Databases Delete
      description: Deletes a database.
      operationId: Databases_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasename-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases
    get:
      summary: Databases Get
      description: Gets a database.
      operationId: Databases_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases:
    get:
      summary: Databases List By Server
      description: Returns a list of databases in a server.
      operationId: Databases_ListByServer
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabases-get
      parameters:
      - in: query
        name: $filter
        description: An OData filter expression that describes a subset of databases
          to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Server
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/usages
  : get:
      summary: Databases List Usages
      description: Returns database usages.
      operationId: Databases_ListUsages
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameusages-get
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
      - Databases Usages
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/elasticPoolDatabaseActivity
  : get:
      summary: Elastic Pools List Database Activity
      description: Returns activity on databases inside of an elastic pool.
      operationId: ElasticPools_ListDatabaseActivity
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernameelasticpoolselasticpoolnameelasticpooldatabaseactivity-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Database Activity
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases/{databaseName}
  : get:
      summary: Elastic Pools Get Database
      description: Gets a database inside of an elastic pool.
      operationId: ElasticPools_GetDatabase
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernameelasticpoolselasticpoolnamedatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be retrieved
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Database
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases
  : get:
      summary: Elastic Pools List Databases
      description: Returns a list of databases in an elastic pool.
      operationId: ElasticPools_ListDatabases
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernameelasticpoolselasticpoolnamedatabases-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Databases
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/databases/{databaseName}
  : get:
      summary: Recommended Elastic Pools Get Databases
      description: Gets a database inside of a recommented elastic pool.
      operationId: RecommendedElasticPools_GetDatabases
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be retrieved
      - in: query
        name: No Name
      - in: path
        name: recommendedElasticPoolName
        description: The name of the elastic pool to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Recommended Elastic Pools Databases
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/databases
  : get:
      summary: Recommended Elastic Pools List Databases
      description: Returns a list of databases inside a recommented elastic pool.
      operationId: RecommendedElasticPools_ListDatabases
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabases-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: recommendedElasticPoolName
        description: The name of the recommended elastic pool to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Recommended Elastic Pools Databases
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/serviceTierAdvisors/{serviceTierAdvisorName}
  : get:
      summary: Databases Get Service Tier Advisor
      description: Gets a service tier advisor.
      operationId: Databases_GetServiceTierAdvisor
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameservicetieradvisorsservicetieradvisorname-get
      parameters:
      - in: path
        name: databaseName
        description: The name of database
      - in: query
        name: No Name
      - in: path
        name: serviceTierAdvisorName
        description: The name of service tier advisor
      responses:
        200:
          description: OK
      tags:
      - Databases Service Tier Advisor
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/serviceTierAdvisors
  : get:
      summary: Databases List Service Tier Advisors
      description: Returns service tier advisors for specified database.
      operationId: Databases_ListServiceTierAdvisors
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameservicetieradvisors-get
      parameters:
      - in: path
        name: databaseName
        description: The name of database
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Service Tier Advisors
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/transparentDataEncryption/current
  : put:
      summary: Databases Create Or Update Transparent Data Encryption Configuration
      description: Creates or updates a database's transparent data encryption configuration.
      operationId: Databases_CreateOrUpdateTransparentDataEncryptionConfiguration
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrent-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which setting the transparent data
          encryption applies
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating transparent
          data encryption
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Transparent Data Encryption Configuration
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