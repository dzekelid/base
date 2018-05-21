---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 0
info:
  title: Azure DocumentDB API Database Accounts Delete
  description: Deletes an existing Azure DocumentDB database account.
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}:
    get:
      summary: Database Accounts Get
      description: Retrieves the properties of an existing Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
    patch:
      summary: Database Accounts Patch
      description: Patches the properties of an existing Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_Patch
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: updateParameters
        description: The tags parameter to patch for the current database account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Patch
    put:
      summary: Database Accounts Create Or Update
      description: Creates or updates an Azure DocumentDB database account.
      operationId: DatabaseAccounts_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-put
      parameters:
      - in: body
        name: createUpdateParameters
        description: The parameters to provide for the current database account
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Or
    delete:
      summary: Database Accounts Delete
      description: Deletes an existing Azure DocumentDB database account.
      operationId: DatabaseAccounts_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
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