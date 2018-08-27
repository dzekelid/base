---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Get Domain Base Path
  version: 1.0.0
  description: Gets the BasePathMappings resource representing the collection of base
    path mappings for the specified custom domain name.
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