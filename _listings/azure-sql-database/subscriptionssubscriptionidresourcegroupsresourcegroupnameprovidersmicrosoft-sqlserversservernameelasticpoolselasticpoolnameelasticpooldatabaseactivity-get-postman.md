{
  "info": {
    "name": "Azure SQL Database API Elastic Pools List Database Activity",
    "_postman_id": "1544ac38-bd74-4d01-8764-7ee8f73f7cc7",
    "description": "Returns activity on databases inside of an elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools database activity",
      "item": [
        {
          "id": "632d87e4-3174-4534-8e0c-9bee72341703",
          "name": "ElasticPools_ListDatabaseActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools/:elasticPoolName/elasticPoolDatabaseActivity"
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
            "description": "Returns activity on databases inside of an elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "983efa97-2b98-4430-8a7e-4d9736a1deaf"
            }
          ]
        }
      ]
    }
  ]
}