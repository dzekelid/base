{
  "info": {
    "name": "Azure SQL Database API Elastic Pools List Databases",
    "_postman_id": "8f6e0f57-0153-4ee8-81df-7ed5e663ced8",
    "description": "Returns a list of databases in an elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools databases",
      "item": [
        {
          "id": "18f0cb4c-1305-4c97-93d9-6a2267152c2f",
          "name": "ElasticPools_ListDatabases",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools/:elasticPoolName/databases"
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
            "description": "Returns a list of databases in an elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "080bb570-d376-46b8-9eb8-396ff416545b"
            }
          ]
        }
      ]
    }
  ]
}