{
  "info": {
    "name": "Amazon EC2 Systems Manager API Deregister Patch Baseline For Patch Group",
    "_postman_id": "afb7e7ea-f4b8-49b2-a0c5-16e813c3251e",
    "description": "Removes a patch group from a patch baseline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "b109192a-26a5-4adc-b6c0-0eccd9062d6d",
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
              "id": "7a6ded2f-7f17-4144-858a-f47ebf1364de"
            }
          ]
        },
        {
          "id": "fe15c3a8-4a1a-43a7-8ec4-d31574d5bb55",
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
              "id": "47d8a1aa-0556-46b0-ba59-2633ccbe22d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "c507a95b-da42-4b12-9b44-eec8e3860886",
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
              "id": "2204e24b-5c7c-4716-9381-674c66dce6ce"
            }
          ]
        }
      ]
    }
  ]
}