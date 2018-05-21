---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Get Patch Baseline
  version: 1.0.0
  description: Retrieves information about a patch baseline.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreatePatchBaseline:
    get:
      summary: Create Patch Baseline
      description: Creates a patch baseline.
      operationId: createPatchBaseline
      x-api-path-slug: actioncreatepatchbaseline-get
      parameters:
      - in: query
        name: ApprovalRules
        description: A set of rules used to include patches in the baseline
        type: string
      - in: query
        name: ApprovedPatches
        description: A list of explicitly approved patches for the baseline
        type: string
      - in: query
        name: ClientToken
        description: Caller-provided idempotency token
        type: string
      - in: query
        name: Description
        description: A description of the patch baseline
        type: string
      - in: query
        name: GlobalFilters
        description: A set of global filters used to exclude patches from the baseline
        type: string
      - in: query
        name: Name
        description: The name of the patch baseline
        type: string
      - in: query
        name: RejectedPatches
        description: A list of explicitly rejected patches for the baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
  /?Action=DeletePatchBaseline:
    get:
      summary: Delete Patch Baseline
      description: Deletes a patch baseline.
      operationId: deletePatchBaseline
      x-api-path-slug: actiondeletepatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
  /?Action=DeregisterPatchBaselineForPatchGroup:
    get:
      summary: Deregister Patch Baseline For Patch Group
      description: Removes a patch group from a patch baseline.
      operationId: deregisterPatchBaselineForPatchGroup
      x-api-path-slug: actionderegisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to deregister the patch group from
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be deregistered from
          the patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - BaselineGroup
  /?Action=DescribeEffectivePatchesForPatchBaseline:
    get:
      summary: Describe Effective Patches For Patch Baseline
      description: Retrieves the current effective patches (the patch and the approval
        state) for the specified patch baseline.
      operationId: describeEffectivePatchesForPatchBaseline
      x-api-path-slug: actiondescribeeffectivepatchesforpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to retrieve the effective patches
          for
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Effective
      - PatchesBaseline
  /?Action=DescribePatchBaselines:
    get:
      summary: Describe Patch Baselines
      description: Lists the patch baselines in your AWS account.
      operationId: describePatchBaselines
      x-api-path-slug: actiondescribepatchbaselines-get
      parameters:
      - in: query
        name: Filters
        description: 'Each element in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patch baselines to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baselines
  /?Action=GetDefaultPatchBaseline:
    get:
      summary: Get Default Patch Baseline
      description: Retrieves the default patch baseline.
      operationId: getDefaultPatchBaseline
      x-api-path-slug: actiongetdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the default patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default
      - Baseline
  /?Action=GetPatchBaseline:
    get:
      summary: Get Patch Baseline
      description: Retrieves information about a patch baseline.
      operationId: getPatchBaseline
      x-api-path-slug: actiongetpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
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