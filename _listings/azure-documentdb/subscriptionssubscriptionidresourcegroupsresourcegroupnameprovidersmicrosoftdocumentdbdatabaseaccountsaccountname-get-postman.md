{
  "info": {
    "name": "Azure DocumentDB API Database Accounts Get",
    "_postman_id": "4d235f72-4e7f-4235-a2ac-0b078b042a55",
    "description": "Retrieves the properties of an existing Azure DocumentDB database account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "eaa5975b-182d-4316-92c5-0d3c6aca785b",
          "name": "DatabaseAccounts_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DocumentDB/databaseAccounts/:accountName"
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
                  "id": "accountName",
                  "value": "accountName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the properties of an existing Azure DocumentDB database account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4562cb0-75ae-4dad-8d00-2173cbb9bb2d"
            }
          ]
        }
      ]
    }
  ]
}