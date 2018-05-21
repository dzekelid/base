{
  "info": {
    "name": "Azure SQL Database API Databases Get Transparent Data Encryption Configuration",
    "_postman_id": "a3da1653-7d32-4853-a239-6664a5b89bb5",
    "description": "Gets a database's transparent data encryption configuration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases transparent data encryption configuration",
      "item": [
        {
          "id": "7d7c3d67-0e75-4b7f-b68e-60c30e487ed0",
          "name": "Databases_GetTransparentDataEncryptionConfiguration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/transparentDataEncryption/current"
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
            "description": "Gets a database's transparent data encryption configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "144db5ee-8cd3-46d6-a78e-97b22a837d3a"
            }
          ]
        }
      ]
    }
  ]
}