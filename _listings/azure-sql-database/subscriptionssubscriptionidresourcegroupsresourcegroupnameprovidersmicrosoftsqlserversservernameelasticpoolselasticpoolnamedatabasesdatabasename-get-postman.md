{
  "info": {
    "name": "Azure SQL Database API Elastic Pools Get Database",
    "_postman_id": "8e4b6868-e255-4f19-a264-0df77f0d67c1",
    "description": "Gets a database inside of an elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools database",
      "item": [
        {
          "id": "100cea4a-7622-4b62-bb60-dd2b8b111d03",
          "name": "ElasticPools_GetDatabase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools/:elasticPoolName/databases/:databaseName"
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
                  "id": "elasticPoolName",
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
            "description": "Gets a database inside of an elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb6d864c-cc6c-41fe-a891-fc63053652fa"
            }
          ]
        }
      ]
    }
  ]
}