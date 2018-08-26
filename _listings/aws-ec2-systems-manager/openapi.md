---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
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
  /?Action=RegisterDefaultPatchBaseline:
    get:
      summary: Register Default Patch Baseline
      description: Defines the default patch baseline.
      operationId: registerDefaultPatchBaseline
      x-api-path-slug: actionregisterdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline that should be the default patch
          baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Default
      - Baseline
  /?Action=UpdatePatchBaseline:
    get:
      summary: Update Patch Baseline
      description: Modifies an existing patch baseline.
      operationId: updatePatchBaseline
      x-api-path-slug: actionupdatepatchbaseline-get
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
        name: BaselineId
        description: The ID of the patch baseline to update
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
  /?Action=GetPatchBaselineForPatchGroup:
    get:
      summary: Get Patch Baseline For Patch Group
      description: Retrieves the patch baseline that should be used for the specified
        patch group.
      operationId: getPatchBaselineForPatchGroup
      x-api-path-slug: actiongetpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: PatchGroup
        description: The name of the patch group whose patch baseline should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - BaselineGroup
  /?Action=RegisterPatchBaselineForPatchGroup:
    get:
      summary: Register Patch Baseline For Patch Group
      description: Registers a patch baseline for a patch group.
      operationId: registerPatchBaselineForPatchGroup
      x-api-path-slug: actionregisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to register the patch group with
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be registered with the
          patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - BaselineGroup
---