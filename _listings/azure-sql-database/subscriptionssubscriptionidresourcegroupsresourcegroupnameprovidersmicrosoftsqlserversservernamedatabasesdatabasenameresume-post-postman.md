{
  "info": {
    "name": "Azure SQL Database API Databases Resume",
    "_postman_id": "81a18d32-e8d4-4e03-991a-5afea7a1dbd2",
    "description": "Resumes a data warehouse.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "databases resume",
      "item": [
        {
          "id": "9c238181-0d2e-41a2-ae5e-38b8dfb7a5ee",
          "name": "Databases_Resume",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/resume"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Resumes a data warehouse"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c711abc9-d077-4c55-b30b-0b6a909e1ee7"
            }
          ]
        }
      ]
    }
  ]
}