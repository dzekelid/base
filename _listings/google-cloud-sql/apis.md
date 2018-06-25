---
name: Google Cloud SQL
x-slug: google-cloud-sql
description: Cloud SQL is a fully-managed database service that makes it easy to set
  up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL databases
  in the cloud. Cloud SQL offers high performance, scalability, and convenience. Hosted
  on Google Cloud Platform, Cloud SQL provides a database infrastructure for applications
  running anywhere.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Base
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud SQL API Get Projects Project Instances Instance Databases
  x-api-slug: google-cloud-sql-api
  description: Lists databases in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases
  tags: Projects, Project, Instances, Instance, Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Databases
  x-api-slug: google-cloud-sql-api
  description: Inserts a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases
  tags: Projects, Project, Instances, Instance, Databases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance Databases
    Database
  x-api-slug: google-cloud-sql-api
  description: Deletes a database from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-openapi.md
- name: Google Cloud SQL API Patch Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-patch-openapi.md
- name: Google Cloud SQL API Put Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Put, Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-put-openapi.md
- name: Google Cloud SQL API
  x-api-slug: google-cloud-sql-api
  description: Cloud SQL is a fully-managed database service that makes it easy to
    set up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL
    databases in the cloud. Cloud SQL offers high performance, scalability, and convenience.
    Hosted on Google Cloud Platform, Cloud SQL provides a database infrastructure
    for applications running anywhere.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Base
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/google-cloud-sql/openapi.md
x-common:
- type: x-change-log
  url: https://cloud.google.com/sql/docs/release-notes
- type: x-code
  url: https://cloud.google.com/sql/docs/admin-api/libraries
- type: x-concepts
  url: https://cloud.google.com/sql/docs/postgres/concepts
- type: x-documentation
  url: https://cloud.google.com/sql/docs/
- type: x-getting-started
  url: https://cloud.google.com/sql/docs/postgres/quickstart
- type: x-guides
  url: https://cloud.google.com/sql/docs/postgres/how-to
- type: x-pricing
  url: https://cloud.google.com/sql/pricing
- type: x-service-level-agreements
  url: https://cloud.google.com/sql/sla
- type: x-support
  url: https://cloud.google.com/sql/docs/support
- type: x-website
  url: https://cloud.google.com/sql/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---