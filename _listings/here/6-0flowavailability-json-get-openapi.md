---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Traffic API Traffic Flow Availability Data
  description: |-
    *Flow availability requests allow you to see what traffic flow coverage exists in the current Traffic API.*

    T<i></i>he Server also supports an XML response.



    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  version: 1.0.0
host: tiles.traffic.cit.api.here.com
basePath: /traffic/6.0/tiles/8/133/86/256
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /6.0/flowavailability.json:
    get:
      summary: Traffic Flow Availability Data
      description: |-
        *Flow availability requests allow you to see what traffic flow coverage exists in the current Traffic API.*

        T<i></i>he Server also supports an XML response.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 60FlowavailabilityJsonGet
      x-api-path-slug: 6-0flowavailability-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      responses:
        200:
          description: OK
      tags:
      - Traffic
      - Flow
      - Availability
      - Data
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