{
  "info": {
    "name": "Azure DocumentDB API Database Accounts List",
    "_postman_id": "62081381-6595-4abe-9a12-62f0c53ebd10",
    "description": "Lists all the Azure DocumentDB database accounts available under the subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "database",
      "item": [
        {
          "id": "a082c91a-2e9d-462f-a803-1b8bcbec67ab",
          "name": "DatabaseAccounts_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.DocumentDB/databaseAccounts"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the Azure DocumentDB database accounts available under the subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67b5bb5e-01ad-434c-8b13-5285a36b9c1c"
            }
          ]
        }
      ]
    }
  ]
}