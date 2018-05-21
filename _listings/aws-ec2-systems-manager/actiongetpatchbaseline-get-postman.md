{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Patch Baseline",
    "_postman_id": "7bcaff6b-89e3-4a98-bce6-cb1b6c240cc9",
    "description": "Retrieves information about a patch baseline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "e6b793bb-38e7-4cc8-97c1-de68a36d81c5",
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
              "id": "5c8d5a68-a336-484a-9cd5-241784cec1bf"
            }
          ]
        },
        {
          "id": "d62f99dd-6949-4d0e-a63c-4b7651453321",
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
              "id": "a92430c0-b42f-4531-b91d-b763331cebd5"
            }
          ]
        },
        {
          "id": "5dece38e-3a43-4d71-a0df-bc4815c1a503",
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
              "id": "46b369d7-eb84-403f-bd41-cf562e9debae"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "c2677654-5985-4d40-a005-f88d83d4c02a",
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
              "id": "5283b562-952f-4994-b85a-bbbdbf645469"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "ce45fe6e-6e84-46a1-9ad8-c57bbeb94f44",
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
              "id": "cdf23003-b669-45d0-970f-deacff20ff0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "52f78578-aa76-4597-94bb-9fb4408f0103",
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
              "id": "3ac7d79d-4096-4f73-a6f0-deffa1561043"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "6d43f77a-2d88-470f-a8b6-cb2ee731351e",
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
              "id": "5dceda42-45c1-4be5-a21a-8af483f8c4e3"
            }
          ]
        }
      ]
    }
  ]
}