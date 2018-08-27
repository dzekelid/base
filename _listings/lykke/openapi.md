swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/BaseAsset:
    get:
      summary: Get API Baseasset
      description: Get api baseasset.
      operationId: ApiBaseAssetGet
      x-api-path-slug: apibaseasset-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Baseasset
    post:
      summary: Add API Baseasset
      description: Add api baseasset.
      operationId: ApiBaseAssetPost
      x-api-path-slug: apibaseasset-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Baseasset
  /api/BaseAssets:
    get:
      summary: Get API Baseassets
      description: Get api baseassets.
      operationId: ApiBaseAssetsGet
      x-api-path-slug: apibaseassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Baseassets
  /api/Client/balances/{baseAsset}:
    get:
      summary: Get API Client Balances Baseasset
      description: Get api client balances baseasset.
      operationId: ApiClientBalancesByBaseAssetGet
      x-api-path-slug: apiclientbalancesbaseasset-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: baseAsset
      responses:
        200:
          description: OK
      tags:
      - Client
      - Balances
      - Baseasset
  /api/LastBaseAssets:
    get:
      summary: Get API Lastbaseassets
      description: Get api lastbaseassets.
      operationId: ApiLastBaseAssetsGet
      x-api-path-slug: apilastbaseassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: "n"
      responses:
        200:
          description: OK
      tags:
      - Lastbaseassets