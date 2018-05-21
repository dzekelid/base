{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Patch Baseline For Patch Group",
    "_postman_id": "45af727f-ff2d-4d49-8bbc-f4e5de5b600e",
    "description": "Retrieves the patch baseline that should be used for the specified patch group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "bf354d24-b518-4567-b9fb-7b228cc16dc9",
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
              "id": "d68e3baa-b5d6-4657-a823-adcf668122f0"
            }
          ]
        },
        {
          "id": "e3bd1fe5-4fc2-458a-8e94-af72447811ef",
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
              "id": "c60a2bca-9e69-4cf9-b3e5-fa78ee8a9e3a"
            }
          ]
        },
        {
          "id": "259a2377-5fa7-4457-8da7-b664297e6aa0",
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
              "id": "29f31ef8-7bb3-4378-9536-de7cd1216c53"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "b32ac42a-d26f-48d4-a2f8-f2fc5bcc1069",
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
              "id": "e5f5b8e2-a7a7-4075-abbb-5da40757a0ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "4c1c2e26-b4c4-48cb-af23-fba53af428f9",
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
              "id": "3907e784-d717-4940-bb55-bb88b2481ad9"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "fca988fa-9b47-4b2a-98b9-90eda3773187",
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
              "id": "8781e76a-8318-448b-bf15-611194f7ef76"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "f21c22c7-7706-4192-9271-b50f6e235446",
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
              "id": "73805823-c773-49c5-9b3f-144adb441899"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "ecfdd1e1-3af8-4886-bcb3-6de3108fd42a",
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
              "id": "98ae5cbd-4210-4677-88df-42f8c5ebe1d4"
            }
          ]
        }
      ]
    }
  ]
}