{
  "info": {
    "name": "Azure SQL Database API Recommended Elastic Pools List Databases",
    "_postman_id": "0876d6ca-c1b5-4d84-bf5b-6040bdbc22ec",
    "description": "Returns a list of databases inside a recommented elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommended elastic pools databases",
      "item": [
        {
          "id": "c587c1ba-02ff-460d-bc48-be5986ae3145",
          "name": "RecommendedElasticPools_ListDatabases",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/recommendedElasticPools/:recommendedElasticPoolName/databases"
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
            "description": "Returns a list of databases inside a recommented elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2e4cf0a-5546-4189-a8ff-0afea457630e"
            }
          ]
        }
      ]
    }
  ]
}