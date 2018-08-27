{
  "info": {
    "name": "Amazon EC2 Systems Manager API Create Patch Baseline",
    "_postman_id": "e431938d-2c1f-487a-821c-ce2185265f82",
    "description": "Creates a patch baseline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baseline",
      "item": [
        {
          "id": "d0a2107a-719b-4bd6-baa9-d66721f4466e",
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
              "id": "8bf3dde2-18d5-4d41-a169-dbf2646f7c0d"
            }
          ]
        }
      ]
    }
  ]
}