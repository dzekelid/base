{
  "info": {
    "name": "Azure DocumentDB API Database Accounts Delete",
    "_postman_id": "1a7a0bf7-1f39-46df-b5c1-a79468f783d0",
    "description": "Deletes an existing Azure DocumentDB database account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "2f9fdaa5-2300-4150-a722-1240bd8530db",
          "name": "DatabaseAccounts_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing Azure DocumentDB database account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31cc330c-58ab-4879-a777-41c78d460647"
            }
          ]
        }
      ]
    }
  ]
}