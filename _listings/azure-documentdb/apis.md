---
name: Azure DocumentDB
x-slug: azure-documentdb
description: Azure DocumentDB is a fully-managed NoSQL document database service that
  offers querying and transaction-processing over schema-free data, predictable and
  reliable performance, and rapid development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
x-kinRank: "10"
x-alexaRank: ""
tags: Base
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/apis.md
specificationVersion: "0.14"
apis:
- name: Azure DocumentDB API Database Accounts Get
  x-api-slug: azure-documentdb-api
  description: Retrieves the properties of an existing Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}
  tags: Database, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-get-openapi.md
- name: Azure DocumentDB API Database Accounts Patch
  x-api-slug: azure-documentdb-api
  description: Patches the properties of an existing Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}
  tags: Database, Accounts, Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-patch-openapi.md
- name: Azure DocumentDB API Database Accounts Create Or Update
  x-api-slug: azure-documentdb-api
  description: Creates or updates an Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}
  tags: Database, Accounts, Or
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-put-openapi.md
- name: Azure DocumentDB API Database Accounts Delete
  x-api-slug: azure-documentdb-api
  description: Deletes an existing Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}
  tags: Database, Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountname-delete-openapi.md
- name: Azure DocumentDB API Database Accounts Failover Priority Change
  x-api-slug: azure-documentdb-api
  description: Changes the failover priority for the Azure DocumentDB database account.
    A failover priority of 0 indicates a write region. The maximum value for a failover
    priority = (total number of regions - 1). Failover priority values must be unique
    for each of the regions in which the database account exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/failoverPriorityChange
  tags: Database, Accounts, Failover, Priority, Change
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamefailoverprioritychange-post-openapi.md
- name: Azure DocumentDB API Database Accounts List
  x-api-slug: azure-documentdb-api
  description: Lists all the Azure DocumentDB database accounts available under the
    subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.DocumentDB/databaseAccounts
  tags: Database, Accounts, List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidprovidersmicrosoftdocumentdbdatabaseaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidprovidersmicrosoftdocumentdbdatabaseaccounts-get-openapi.md
- name: Azure DocumentDB API Database Accounts List By Resource Group
  x-api-slug: azure-documentdb-api
  description: Lists all the Azure DocumentDB database accounts available under the
    given resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts
  tags: Database, Accounts, ListResource, Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccounts-get-openapi.md
- name: Azure DocumentDB API Database Accounts List Keys
  x-api-slug: azure-documentdb-api
  description: Lists the access keys for the specified Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listKeys
  tags: Database, Accounts, List, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamelistkeys-post-openapi.md
- name: Azure DocumentDB API Database Accounts List Connection Strings
  x-api-slug: azure-documentdb-api
  description: Lists the connection strings for the specified Azure DocumentDB database
    account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listConnectionStrings
  tags: Database, Accounts, List, Connection, Strings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamelistconnectionstrings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamelistconnectionstrings-post-openapi.md
- name: Azure DocumentDB API Database Accounts List Read Only Keys
  x-api-slug: azure-documentdb-api
  description: Lists the read-only access keys for the specified Azure DocumentDB
    database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/readonlykeys
  tags: Database, Accounts, List, Read, Only, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamereadonlykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnamereadonlykeys-get-openapi.md
- name: Azure DocumentDB API Database Accounts Regenerate Key
  x-api-slug: azure-documentdb-api
  description: Regenerates an access key for the specified Azure DocumentDB database
    account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/regenerateKey
  tags: Database, Accounts, Regenerate, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftdocumentdbdatabaseaccountsaccountnameregeneratekey-post-openapi.md
- name: Azure DocumentDB API Database Accounts Check Name Exists
  x-api-slug: azure-documentdb-api
  description: Checks that the Azure DocumentDB account name already exists. A valid
    account name may contain only lowercase letters, numbers, and the '-' character,
    and must be between 3 and 50 characters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////providers/Microsoft.DocumentDB/databaseAccountNames/{accountName}
  tags: Database, Accounts, Checks, Name, Exists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/providersmicrosoftdocumentdbdatabaseaccountnamesaccountname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/providersmicrosoftdocumentdbdatabaseaccountnamesaccountname-head-openapi.md
- name: Azure DocumentDB API
  x-api-slug: azure-documentdb-api
  description: Azure DocumentDB is a fully-managed NoSQL document database service
    that offers querying and transaction-processing over schema-free data, predictable
    and reliable performance, and rapid development.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com//
  tags: Base
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/azure-documentdb/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/documentdb/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/documentdb/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/documentdb/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/documentdb/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---