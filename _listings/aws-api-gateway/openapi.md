---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 1
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domainnames/a.b.c.com/basepathmappings:
    get:
      summary: Get Domain Base Path
      description: Gets the BasePathMappings resource representing the collection
        of base path mappings for the specified custom domain name.
      operationId: domainnameBasepathmappings
      x-api-path-slug: domainnamesa-b-c-combasepathmappings-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domain
      - Base
      - Path
---