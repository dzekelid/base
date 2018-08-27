---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Returns property details mortgageowner based on
    an ID.
  description: Get property details mortgageowner based on its Onboard property ID.
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /property/detail:
    get:
      summary: Returns property details based on an ID.
      description: Get property details based on its Onboard property ID.
      operationId: propertyDetails
      x-api-path-slug: propertydetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address
        description: The mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Based
      - "On"
      - ID
  /property/detailmortgage:
    get:
      summary: Returns property details mortgage based on ID.
      description: Get property details mortgage based on its Onboard property ID.
      operationId: propertyDetailsMortage
      x-api-path-slug: propertydetailmortgage-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Mortgage
      - Based
      - "On"
      - ID
  /property/detailowner:
    get:
      summary: Returns property details owner based on an ID.
      description: Get property details owner based on its Onboard property ID.
      operationId: propertyDetailsOwner
      x-api-path-slug: propertydetailowner-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Owner
      - Based
      - "On"
      - ID
  /property/detailmortgageowner:
    get:
      summary: Returns property details mortgageowner based on an ID.
      description: Get property details mortgageowner based on its Onboard property
        ID.
      operationId: propertyDetailsMortgageOwner
      x-api-path-slug: propertydetailmortgageowner-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Mortgageowner
      - Based
      - "On"
      - ID
  /poi/geography:
    get:
      summary: Returns POIs based on zip code.
      description: This search returns a list of Points of Interest in proximity to
        the centroid of a zip code.
      operationId: getPOISearchGeography
      x-api-path-slug: poigeography-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: ApiKey
        description: Application Key
      - in: query
        name: PostalCodeKey
        description: This is the Postal Code
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Zip
      - Code
  /poi/point:
    get:
      summary: Returns POIs based on point.
      description: This search returns a list of POI in proximity to a latitude/longitude.
      operationId: getPOISearchPoint
      x-api-path-slug: poipoint-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: BusinessCategory
        description: This is Business Category as per Lookup separated by pipe |
      - in: query
        name: Point
        description: This is the Point value
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Point
  /poi/street+address:
    get:
      summary: Returns POIs based on an address.
      description: This search returns a list of POI in proximity to an address.
      operationId: getPOISearchPoint
      x-api-path-slug: poistreetaddress-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      - in: query
        name: StreetAddress
        description: This is the Point value
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Address
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