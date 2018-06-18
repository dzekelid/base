{
  "info": {
    "name": "Azure SQL Database API Databases Get Threat Detection Policy",
    "_postman_id": "5c0e1e85-e808-4419-bad1-d26608097bde",
    "description": "Gets a database's threat detection policy.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases threat detection policy",
      "item": [
        {
          "id": "f90e1728-efcf-40fd-ae30-a17ad1fc8a91",
          "name": "Databases_GetThreatDetectionPolicy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/securityAlertPolicies/default"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "databaseName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serverName",
                  "value": "serverName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a database's threat detection policy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "684e02e4-30fa-415c-bb30-fc3c48649f1e"
            }
          ]
        }
      ]
    }
  ]
}