{
  "info": {
    "name": "Azure SQL Database API Databases Get Service Tier Advisor",
    "_postman_id": "b659d57f-8f5e-499d-9d80-374749a315d6",
    "description": "Gets a service tier advisor.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases service tier advisor",
      "item": [
        {
          "id": "7ea5c8a2-98b9-4413-9d88-58f47e51d72e",
          "name": "Databases_GetServiceTierAdvisor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/serviceTierAdvisors/:serviceTierAdvisorName"
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
                  "id": "serviceTierAdvisorName",
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
            "description": "Gets a service tier advisor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d77ead9e-8954-42c6-bfc3-3ab284bc54c5"
            }
          ]
        }
      ]
    }
  ]
}