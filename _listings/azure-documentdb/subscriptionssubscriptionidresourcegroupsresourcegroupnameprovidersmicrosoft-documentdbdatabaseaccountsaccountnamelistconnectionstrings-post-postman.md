{
  "info": {
    "name": "Azure DocumentDB API Database Accounts List Connection Strings",
    "_postman_id": "a8340d72-3f11-4e22-b9be-ede4a3a23cb0",
    "description": "Lists the connection strings for the specified Azure DocumentDB database account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "e476914e-9bb9-4153-ad42-a7413eda5380",
          "name": "DatabaseAccounts_ListConnectionStrings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DocumentDB/databaseAccounts/:accountName/listConnectionStrings"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the connection strings for the specified Azure DocumentDB database account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4693941-2ecd-443b-b200-a810e159ec35"
            }
          ]
        }
      ]
    }
  ]
}