---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-40-release-api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v50-details-heretagapiv3deprecation-looking-for-the-api-v3-reference-it-has-moved-herehttpsapimattermostcomv3
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /database/recycle:
    post:
      summary: Recycle database connections
      description: |-
        Recycle database connections by closing and reconnecting all connections to master and read replica databases.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: recycle-database-connections-by-closing-and-reconnecting-all-connections-to-master-and-read-replica-
      x-api-path-slug: databaserecycle-post
      responses:
        200:
          description: OK
      tags:
      - Recycle
      - Database
      - Connections
---