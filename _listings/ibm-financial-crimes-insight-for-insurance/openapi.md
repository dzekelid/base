swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/physical_object/{id}:
    get:
      summary: Retrieve a specific physical object data from the database, based on
        its internal id
      description: This method is used to retrieve specific physical object data from
        the database, based on its internal id
      operationId: getPhysicalObject
      x-api-path-slug: ibmfciplatformfactphysical-objectid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Specific
      - Physical
      - Object
      - Data
      - From
      - Database
      - ""
      - Based
      - "On"
      - Its
      - Internal
      - Id
  /ibm/fci/platform/fact/watchlist/{id}:
    get:
      summary: Retrieve the contents of a watchlist, based on its id
      description: This method is used to retrieve the contents of a watchlist from
        the database
      operationId: getWatchlistById
      x-api-path-slug: ibmfciplatformfactwatchlistid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      - in: query
        name: summary
        description: If set to true, this flag will cause inclusion any Watchlist_Item_Properties
          associated with the item
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Contents
      - Of
      - Watchlist
      - ""
      - Based
      - "On"
      - Its
      - Id