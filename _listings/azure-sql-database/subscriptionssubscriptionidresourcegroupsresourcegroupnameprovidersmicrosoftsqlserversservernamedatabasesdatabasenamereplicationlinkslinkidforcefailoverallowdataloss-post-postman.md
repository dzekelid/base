{
  "info": {
    "name": "Azure SQL Database API Databases Failover Replication Link Allow Data Loss",
    "_postman_id": "c2bd9bb9-e64e-473c-b0f3-991b66e4836b",
    "description": "Sets which replica database is primary by failing over from the current primary replica database. This operation might result in data loss.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases failover replication link allow data loss",
      "item": [
        {
          "id": "4192c079-2d89-4197-927e-5a6d0db49abc",
          "name": "Databases_FailoverReplicationLinkAllowDataLoss",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/replicationLinks/:linkId/forceFailoverAllowDataLoss"
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
                  "id": "linkId",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets which replica database is primary by failing over from the current primary replica database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e4f304c-75bc-400d-a524-284688ea1c7a"
            }
          ]
        }
      ]
    }
  ]
}