{
  "info": {
    "name": "Azure DocumentDB API Database Accounts List Read Only Keys",
    "_postman_id": "e76b31b2-11dd-46fb-a5d6-de60235da499",
    "description": "Lists the read-only access keys for the specified Azure DocumentDB database account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "e16d18d0-57a9-4452-b077-dc04f68cc1d9",
          "name": "DatabaseAccounts_ListReadOnlyKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DocumentDB/databaseAccounts/:accountName/readonlykeys"
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
            "description": "Lists the read-only access keys for the specified Azure DocumentDB database account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c28bda0-1d6a-45db-b79b-3755f6012b43"
            }
          ]
        }
      ]
    }
  ]
}