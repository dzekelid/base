---
name: Azure Data Lake Analytics
x-slug: azure-data-lake-analytics
description: The Data Lake analytics service is a new distributed analytics service
  built on Apache YARN that dynamically scales so you can focus on your business goals,
  not on distributed infrastructure. Instead of deploying, configuring and tuning
  hardware, you write queries to transform your data and extract valuable insights.
  The analytics service can handle jobs of any scale instantly by simply setting the
  dial for how much power you need. You only pay for your job when it is running making
  it cost-effective. The analytics service supports Azure Active Directory letting
  you simply manage access and roles, integrated with your on-premises identity system.
  It also includes U-SQL, a language that unifies the benefits of SQL with the expressive
  power of user code. U-SQL&rsquo;s scalable distributed runtime enables you to efficiently
  analyze data in the store and across SQL Servers in Azure, Azure SQL Database and
  Azure SQL Data Warehouse.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
x-kinRank: "10"
x-alexaRank: ""
tags: Base
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Data Lake Analytics API Catalog List Table Statistics By Database And
    Schema
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all table statistics within the specified schema
    from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/schemas/{schemaName}/statistics
  tags: Catalog Table Statistic Database Schema
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamestatistics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameschemasschemanamestatistics-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Statistics By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all statistics in a database from the Data Lake
    Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/statistics
  tags: Catalog Table Statistic Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamestatistics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenamestatistics-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Tables By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all tables in a database from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/tables
  tags: Catalog Table Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametables-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Table Valued Functions By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all table valued functions in a database from
    the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/tablevaluedfunctions
  tags: Catalog Table Valued Function Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametablevaluedfunctions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenametablevaluedfunctions-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Views By Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of all views in a database from the Data Lake Analytics
    catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}/views
  tags: Catalog View Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasenameviews-get-openapi.md
- name: Azure Data Lake Analytics API Catalog Get Database
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the specified database from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases/{databaseName}
  tags: Catalog Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabasesdatabasename-get-openapi.md
- name: Azure Data Lake Analytics API Catalog List Databases
  x-api-slug: azure-data-lake-analytics-api
  description: Retrieves the list of databases from the Data Lake Analytics catalog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: ://////catalog/usql/databases
  tags: Catalog Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/catalogusqldatabases-get-openapi.md
- name: Azure Data Lake Analytics API
  x-api-slug: azure-data-lake-analytics-api
  description: The Data Lake analytics service is a new distributed analytics service
    built on Apache YARN that dynamically scales so you can focus on your business
    goals, not on distributed infrastructure. Instead of deploying, configuring and
    tuning hardware, you write queries to transform your data and extract valuable
    insights. The analytics service can handle jobs of any scale instantly by simply
    setting the dial for how much power you need. You only pay for your job when it
    is running making it cost-effective. The analytics service supports Azure Active
    Directory letting you simply manage access and roles, integrated with your on-premises
    identity system. It also includes U-SQL, a language that unifies the benefits
    of SQL with the expressive power of user code. U-SQL&rsquo;s scalable distributed
    runtime enables you to efficiently analyze data in the store and across SQL Servers
    in Azure, Azure SQL Database and Azure SQL Data Warehouse.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-lake-analytics-05.png
  humanURL: https://azure.microsoft.com/en-us/services/data-lake-analytics/
  baseURL: :////
  tags: Base
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-data-lake-analytics/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/data-lake-analytics/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/data-lake-analytics/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/data-lake-analytics/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/data-lake-analytics/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---