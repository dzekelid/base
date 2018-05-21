{
  "info": {
    "name": "Azure SQL Database API Databases List Service Tier Advisors",
    "_postman_id": "ed4afaf9-590d-45ce-aa90-7d40a8bf0309",
    "description": "Returns service tier advisors for specified database.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases service tier advisors",
      "item": [
        {
          "id": "52a6650f-1b9a-48dc-9109-6308add24863",
          "name": "Databases_ListServiceTierAdvisors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/serviceTierAdvisors"
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
            "description": "Returns service tier advisors for specified database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c4f79d9-e1fd-43e9-be7b-4c4fbabab54a"
            }
          ]
        }
      ]
    }
  ]
}