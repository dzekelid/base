{
  "info": {
    "name": "Amazon EC2 Systems Manager API Delete Patch Baseline",
    "_postman_id": "33995b1b-f1a3-45b2-960e-220a9cd64fd6",
    "description": "Deletes a patch baseline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "b93ba3a8-c94f-4970-82bf-d38684f1ff39",
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
              "id": "561f9987-91a1-42c2-83cb-40135de91786"
            }
          ]
        },
        {
          "id": "1adaa595-f501-4f81-826b-abc6128dec06",
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
              "id": "48885668-d368-40df-a0c6-c3635e0527cd"
            }
          ]
        }
      ]
    }
  ]
}