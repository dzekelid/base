---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global Real Time Futures
  description: this-web-service-provides-global-realtime-future-and-option-quotes-for-us-and-international-future-contracts
  version: 1.0.0
host: globalrealtimefutures.xignite.com
basePath: xGlobalRealTimeFutures.json/XigniteGlobalRealTimeFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListBaseFutures:
    post:
      summary: List Base Futures
      description: Returns a list of base future symbols
      operationId: ListBaseFutures
      x-api-path-slug: listbasefutures-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Base
      - Futures
---