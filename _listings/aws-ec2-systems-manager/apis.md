---
name: AWS EC2 Systems Manager
x-slug: aws-ec2-systems-manager
description: Amazon EC2 Systems Manager is a management service that helps you automatically
  collect software inventory, apply OS patches, create system images, and configure
  Windows and Linux operating systems. These capabilities help you define and track
  system configurations, prevent drift, and maintain software compliance of your EC2
  and on-premises configurations. By providing a management approach that is designed
  for the scale and agility of the cloud but extends into your on-premises data center,
  EC2 Systems Manager makes it easier for you to seamlessly bridge your existing infrastructure
  with AWS.EC2 Systems Manager is easy to use. Simply access EC2 Systems Manager from
  the EC2 Management Console, select the instances you want to manage, and define
  the management tasks you want to perform. EC2 Systems Manager is available now at
  no cost to manage both your EC2 and on-premises resources.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Base
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon EC2 Systems Manager API Create Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Creates a patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=CreatePatchBaseline
  tags: Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actioncreatepatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actioncreatepatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Delete Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Deletes a patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DeletePatchBaseline
  tags: Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiondeletepatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiondeletepatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Deregister Patch Baseline For Patch Group
  x-api-slug: amazon-ec2-systems-manager-api
  description: Removes a patch group from a patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DeregisterPatchBaselineForPatchGroup
  tags: Deregister, BaselineGroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionderegisterpatchbaselineforpatchgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionderegisterpatchbaselineforpatchgroup-get-openapi.md
- name: Amazon EC2 Systems Manager API Describe Effective Patches For Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves the current effective patches (the patch and the approval
    state) for the specified patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DescribeEffectivePatchesForPatchBaseline
  tags: Effective, PatchesBaseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiondescribeeffectivepatchesforpatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiondescribeeffectivepatchesforpatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Describe Patch Baselines
  x-api-slug: amazon-ec2-systems-manager-api
  description: Lists the patch baselines in your AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DescribePatchBaselines
  tags: Baselines
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiondescribepatchbaselines-get-openapi.md
- name: Amazon EC2 Systems Manager API Get Default Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves the default patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=GetDefaultPatchBaseline
  tags: Default, Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetdefaultpatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetdefaultpatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Get Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves information about a patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=GetPatchBaseline
  tags: Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetpatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetpatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Get Patch Baseline For Patch Group
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves the patch baseline that should be used for the specified
    patch group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=GetPatchBaselineForPatchGroup
  tags: BaselineGroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetpatchbaselineforpatchgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actiongetpatchbaselineforpatchgroup-get-openapi.md
- name: Amazon EC2 Systems Manager API Register Default Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Defines the default patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=RegisterDefaultPatchBaseline
  tags: Register, Default, Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionregisterdefaultpatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionregisterdefaultpatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API Register Patch Baseline For Patch Group
  x-api-slug: amazon-ec2-systems-manager-api
  description: Registers a patch baseline for a patch group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=RegisterPatchBaselineForPatchGroup
  tags: Register, BaselineGroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionregisterpatchbaselineforpatchgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionregisterpatchbaselineforpatchgroup-get-openapi.md
- name: Amazon EC2 Systems Manager API Update Patch Baseline
  x-api-slug: amazon-ec2-systems-manager-api
  description: Modifies an existing patch baseline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=UpdatePatchBaseline
  tags: Baseline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionupdatepatchbaseline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/actionupdatepatchbaseline-get-openapi.md
- name: Amazon EC2 Systems Manager API
  x-api-slug: amazon-ec2-systems-manager-api
  description: Amazon EC2 Systems Manager is a management service that helps you automatically
    collect software inventory, apply OS patches, create system images, and configure
    Windows and Linux operating systems. These capabilities help you define and track
    system configurations, prevent drift, and maintain software compliance of your
    EC2 and on-premises configurations. By providing a management approach that is
    designed for the scale and agility of the cloud but extends into your on-premises
    data center, EC2 Systems Manager makes it easier for you to seamlessly bridge
    your existing infrastructure with AWS.EC2 Systems Manager is easy to use. Simply
    access EC2 Systems Manager from the EC2 Management Console, select the instances
    you want to manage, and define the management tasks you want to perform. EC2 Systems
    Manager is available now at no cost to manage both your EC2 and on-premises resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: :///
  tags: Base
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/base/master/_listings/aws-ec2-systems-manager/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/ssm/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/ec2/systems-manager/faqs/
- type: x-getting-started
  url: http://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/systems-manager.html
- type: x-website
  url: https://aws.amazon.com/ec2/systems-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---