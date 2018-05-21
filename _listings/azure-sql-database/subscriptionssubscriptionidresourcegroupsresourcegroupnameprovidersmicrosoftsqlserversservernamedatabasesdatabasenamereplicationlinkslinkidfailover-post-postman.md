{
  "info": {
    "name": "Azure SQL Database API Databases Failover Replication Link",
    "_postman_id": "25591f30-6b76-466d-83bd-f54a4b8ff2bc",
    "description": "Sets which replica database is primary by failing over from the current primary replica database.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases failover replication link",
      "item": [
        {
          "id": "fd74d343-3a4b-4383-9207-fe25f00e2dfc",
          "name": "Databases_FailoverReplicationLink",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/replicationLinks/:linkId/failover"
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
              "id": "6046956c-6f5d-4d9c-be4b-c749248a7f29"
            }
          ]
        }
      ]
    }
  ]
}