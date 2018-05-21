{
  "info": {
    "name": "Azure SQL Database API Recommended Elastic Pools Get Databases",
    "_postman_id": "12aa7165-9087-4788-a0c4-86d54eb08988",
    "description": "Gets a database inside of a recommented elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommended elastic pools databases",
      "item": [
        {
          "id": "14c5e109-95d8-41a3-af6c-d11172fcb4fc",
          "name": "RecommendedElasticPools_GetDatabases",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/recommendedElasticPools/:recommendedElasticPoolName/databases/:databaseName"
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
                  "id": "recommendedElasticPoolName",
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
            "description": "Gets a database inside of a recommented elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c72737d8-5c93-4824-9bc3-9d7f1480c528"
            }
          ]
        }
      ]
    }
  ]
}