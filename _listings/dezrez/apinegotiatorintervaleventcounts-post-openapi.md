---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Return interval based event counts for negotiators.
  version: 1.0.0
  description: Return interval based event counts for negotiators..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/{id}/invoiceoverview:
    post:
      summary: Get summary of an account based on invoice amounts allocated
      description: Get summary of an account based on invoice amounts allocated.
      operationId: Account_GetInvoiceOverviewByidBydataContract
      x-api-path-slug: apiaccountidinvoiceoverview-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Summary
      - Of
      - Account
      - Based
      - "On"
      - Invoice
      - Amounts
      - Ocated
  /api/inboundlead/checkformatchinggroups:
    get:
      summary: Check for Matching groups for the given leads based on contact item
        values i.e. Emails and Phones.
      description: Check for matching groups for the given leads based on contact
        item values i.e. emails and phones..
      operationId: InboundLead_CheckForMatchingGroupsByleadIdBypageSizeBypageNumber
      x-api-path-slug: apiinboundleadcheckformatchinggroups-get
      parameters:
      - in: query
        name: leadId
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - CheckMatching
      - Groupsthe
      - Given
      - Leads
      - Based
      - "On"
      - Contact
      - Item
      - Values
      - I
      - E
      - ""
      - Emails
      - Phones
  /api/locale/{culture}:
    get:
      summary: returns the json file containing localization for the app based on
        a culture string, and any custom values for the agent
      description: Returns the json file containing localization for the app based
        on a culture string, and any custom values for the agent.
      operationId: Locale_GetLocalisationFileByculture
      x-api-path-slug: apilocaleculture-get
      parameters:
      - in: path
        name: culture
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Json
      - File
      - Containing
      - Localizationthe
      - App
      - Based
      - "On"
      - Culture
      - String
      - ""
      - Any
      - Custom
      - Valuesthe
      - Agent
  /api/negotiator/intervaleventcounts:
    post:
      summary: Return interval based event counts for negotiators.
      description: Return interval based event counts for negotiators..
      operationId: Negotiator_IntervalEventCountsByintervalEventCountDataContract
      x-api-path-slug: apinegotiatorintervaleventcounts-post
      parameters:
      - in: body
        name: intervalEventCountDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Interval
      - Based
      - Event
      - Countsnegotiators
  /api/people/searchcontacts:
    post:
      summary: Search contacts based on the phone number provided
      description: Search contacts based on the phone number provided.
      operationId: People_SearchContactsBysearchCommandDataContract
      x-api-path-slug: apipeoplesearchcontacts-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchCommandDataContract
        description: Search data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Contacts
      - Based
      - "On"
      - Phone
      - Number
      - Provided
  /api/tenantreferncing/case/{tenancyRoleId}:
    get:
      summary: Gets a tenancy referencing case based on the role id supplied
      description: Gets a tenancy referencing case based on the role id supplied.
      operationId: TenantReferencing_GetCaseBytenancyRoleId
      x-api-path-slug: apitenantreferncingcasetenancyroleid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The id of the tenancy role the case linked to
      responses:
        200:
          description: OK
      tags:
      - S
      - Tenancy
      - Referencing
      - Case
      - Based
      - "On"
      - Role
      - Id
      - Supplied
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