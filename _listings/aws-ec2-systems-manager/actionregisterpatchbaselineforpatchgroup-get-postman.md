{
  "info": {
    "name": "Amazon EC2 Systems Manager API Register Patch Baseline For Patch Group",
    "_postman_id": "3903d306-8533-4615-b0a6-7318045f49db",
    "description": "Registers a patch baseline for a patch group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "cce653cf-27b5-4f38-b307-47c7d5b70c83",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a9819bf-9039-4894-880a-73e3f828e352"
            }
          ]
        },
        {
          "id": "80504947-3a04-4890-9cbb-f0d71fd80416",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "709b8766-c0ee-42cf-83f7-cdb9794d3817"
            }
          ]
        },
        {
          "id": "fbe73dda-580a-441f-a13d-bb4947340691",
          "name": "getPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ef74a40-9887-40d5-888e-da863fe06f06"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "160011ad-4063-4e68-b6bb-357aa047fc63",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d287570-5c88-45fa-a507-3574f8a3b4c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "e444b632-d638-49b6-96c6-f6efc2fe451e",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca11e66c-6bf3-4929-a9e4-da15a108c947"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "a37392e4-e9b8-4f42-a499-928e0e2e01fa",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35743dd2-43b5-40a9-9e9e-1f7305b26632"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "35cf83d3-6a61-40b4-93d8-1a8a60e1aa39",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18970310-3e29-4045-8612-44d261ab8bd0"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "1ac696e9-a828-4d55-9e26-49cc375db253",
          "name": "getPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaselineForPatchGroup?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the patch baseline that should be used for the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b784750a-b7a9-4981-a0e1-be92ef7b23b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Register",
      "item": [
        {
          "id": "e0f94b54-b1f4-4daa-96e4-9da829a5e735",
          "name": "registerDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=RegisterDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Defines the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5195e7a4-0c79-4d93-b6cc-8991a8d96c38"
            }
          ]
        },
        {
          "id": "a305f013-a073-4c4b-a471-cdffff13c2da",
          "name": "registerPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=RegisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a patch baseline for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39af91cd-f353-4dfb-97b0-2c45411454d0"
            }
          ]
        }
      ]
    }
  ]
}