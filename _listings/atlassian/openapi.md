swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/settings/baseUrl:
    put:
      summary: Set base url
      description: Sets the base URL that is configured for this Jira instance.
      operationId: com.atlassian.jira.rest.v2.admin.SettingsResource.setBaseURL_put
      x-api-path-slug: api2settingsbaseurl-put
      responses:
        200:
          description: OK
      tags:
      - Set
      - Base
      - Url