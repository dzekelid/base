{
  "info": {
    "name": "Azure DocumentDB API Database Accounts List By Resource Group",
    "_postman_id": "00cf1778-1290-49ff-b7ee-71b517d5069d",
    "description": "Lists all the Azure DocumentDB database accounts available under the given resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "e28a65d8-94da-4a8f-ad59-39b2906af789",
          "name": "DatabaseAccounts_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DocumentDB/databaseAccounts"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the Azure DocumentDB database accounts available under the given resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34482c92-d6de-4cf8-ac78-9c07709c9935"
            }
          ]
        }
      ]
    }
  ]
}