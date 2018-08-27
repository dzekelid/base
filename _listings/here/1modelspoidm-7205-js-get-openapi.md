---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Venue Maps Places within a Venue
  description: |-
    *Request a list of the places within a venue*

    Details of the individual places to be found within a venue can be obtained by passing `models-poi` in the path of the request URL and appending the `id` of the venue in question along with associated authentication credentials.



    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

    * **Signature**  `text`
     \- Signature

    * **Policy**  `text`
     \- Policy

    * **Key-Pair-Id**  `text`
     \- Key-Pair-Id
  version: 1.0.0
host: signature.venue.maps.cit.api.here.com
basePath: /venues/signature
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
  /6.0/incidents.json:
    get:
      summary: Traffic Incidents via Proximity
      description: |-
        *Request traffic incident information within specified area*

        Traffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.



        * **prox**  `prox`
         \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

        * **criticality**  `multi-enum`
         \- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact

         Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 60IncidentsJsonGet3
      x-api-path-slug: 6-0incidents-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: criticality
      - in: query
        name: prox
      responses:
        200:
          description: OK
      tags:
      - Traffic
      - Incidents
      - Via
      - Proximity
  /6.1/flow.json:
    get:
      summary: Flow using Proximity returning Additional Attributes
      description: |-
        *Request traffic flow information using proximity, returning shape and functional class*

        The request is made through combining the `prox` parameter and the `responseattributes` in the request URL. The server also supports an XML response.



        * **prox**  `prox`
         \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

        * **responseattributes**  `multi-enum`
         \- A list indicating optional information to be included in the traffic flow data response

         Valid values are : `fc` - functionalClass, `sh` - shape

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 61FlowJsonGet7
      x-api-path-slug: 6-1flow-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: prox
      - in: query
        name: responseattributes
      responses:
        200:
          description: OK
      tags:
      - Flow
      - Using
      - Proximity
      - Returning
      - Itional
      - Attributes
  /0/tiles-ia-b64/L1/12022001101210030210.js:
    get:
      summary: Base64 Encoded Map Tiles
      description: |-
        *Request a base64 encoded map tile and associated room definitions with a single request*

        A base64 encoded map tile together with the room definitions, is requested by passing `tiles-ia-b64` in the path of the request URL, along with a known `floor` and `quadkey` and associated authentication credentials.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Signature**  `text`
         \- Signature

        * **Policy**  `text`
         \- Policy

        * **Key-Pair-Id**  `text`
         \- Key-Pair-Id
      operationId: 0TilesIaB64L112022001101210030210JsGet
      x-api-path-slug: 0tilesiab64l112022001101210030210-js-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: Key-Pair-Id
      - in: query
        name: Policy
      - in: query
        name: Signature
      responses:
        200:
          description: OK
      tags:
      - Base64
      - Encoded
      - Map
      - Tiles
  /0/tiles-ia/L1/12022001101210030210.js:
    get:
      summary: Room Definitions
      description: |-
        *Request a list of the name and shape of rooms found within a single venue map tile*

        Room data associated with a map tile is requested by passing `tiles-ia` in the path of the request URL, along with a known `floor` and `quadkey` and associated authentication credentials.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Signature**  `text`
         \- Signature

        * **Policy**  `text`
         \- Policy

        * **Key-Pair-Id**  `text`
         \- Key-Pair-Id
      operationId: 0TilesIaL112022001101210030210JsGet
      x-api-path-slug: 0tilesial112022001101210030210-js-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: Key-Pair-Id
      - in: query
        name: Policy
      - in: query
        name: Signature
      responses:
        200:
          description: OK
      tags:
      - Room
      - Definitions
  /0/tiles-png/L1/12022001101210030210.png:
    get:
      summary: Venue Map Tile
      description: |-
        *Request an individual venue map tile*

        In addition to the usual `app_id` and `app_code`, three additional parameters are required for authentication purposes. The `Signature`, `Policy` and `Key-Pair-Id` parameters have been obtained from a prior request to the `Signature` endpoint.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Signature**  `text`
         \- Signature

        * **Policy**  `text`
         \- Policy

        * **Key-Pair-Id**  `text`
         \- Key-Pair-Id
      operationId: 0TilesPngL112022001101210030210PngGet
      x-api-path-slug: 0tilespngl112022001101210030210-png-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: Key-Pair-Id
      - in: query
        name: Policy
      - in: query
        name: Signature
      responses:
        200:
          description: OK
      tags:
      - Venue
      - Map
      - Tile
  /1/models-full/DM_12321.js:
    get:
      summary: Full Venue Model
      description: "*Request extended details of places found within a venue*\n\nA
        full model of a venue can be obtained by passing `models-full` in the path
        of the request URL and appending the `id` of the venue in question along with
        associated authentication credentials. \n  \n  Note that the client-side process
        formatting the JSON response may take some time in older browsers.\n\n\n\n*
        **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an `app_id`
        with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an `app_code` with every request.\n\n* **Signature**  `text`\n
        \\- Signature\n\n* **Policy**  `text`\n \\- Policy\n\n* **Key-Pair-Id**  `text`\n
        \\- Key-Pair-Id"
      operationId: 1ModelsFullDM12321JsGet
      x-api-path-slug: 1modelsfulldm-12321-js-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: Key-Pair-Id
      - in: query
        name: Policy
      - in: query
        name: Signature
      responses:
        200:
          description: OK
      tags:
      - Full
      - Venue
      - Model
  /1/models-poi/DM_7205.js:
    get:
      summary: Places within a Venue
      description: |-
        *Request a list of the places within a venue*

        Details of the individual places to be found within a venue can be obtained by passing `models-poi` in the path of the request URL and appending the `id` of the venue in question along with associated authentication credentials.



        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Signature**  `text`
         \- Signature

        * **Policy**  `text`
         \- Policy

        * **Key-Pair-Id**  `text`
         \- Key-Pair-Id
      operationId: 1ModelsPoiDM7205JsGet
      x-api-path-slug: 1modelspoidm-7205-js-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: Key-Pair-Id
      - in: query
        name: Policy
      - in: query
        name: Signature
      responses:
        200:
          description: OK
      tags:
      - Places
      - Within
      - Venue
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