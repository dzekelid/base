{
  "info": {
    "name": "Azure DocumentDB API Database Accounts List Keys",
    "_postman_id": "ab0dac67-65eb-44cf-9a30-81a3145ca1df",
    "description": "Lists the access keys for the specified Azure DocumentDB database account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "7c2386e5-7c1d-4851-85e7-d79e85629857",
          "name": "DatabaseAccounts_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DocumentDB/databaseAccounts/:accountName/listKeys"
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
            "description": "Lists the access keys for the specified Azure DocumentDB database account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cb61f2f-4834-4b54-a7c2-d109584a22fb"
            }
          ]
        }
      ]
    }
  ]
}