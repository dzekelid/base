---
swagger: "2.0"
x-collection-name: Pay Run
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Templates/rtitransactionbase:
    get:
      summary: Gets the rti transaction base template
      description: Return the rti transaction base data object template
      operationId: GetRtiTransactionBaseTemplate
      x-api-path-slug: templatesrtitransactionbase-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Transaction
      - Base
      - Template
---