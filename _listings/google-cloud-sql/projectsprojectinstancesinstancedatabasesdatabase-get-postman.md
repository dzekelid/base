{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Databases Database",
    "_postman_id": "68f0bf79-4493-4db2-8781-04cf51678135",
    "description": "Retrieves a resource containing information about a database inside a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "d3c96b9a-b9b6-45d5-9e7b-8afc03d27c3c",
          "name": "sql.databases.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/databases/:database"
              ],
              "variable": [
                {
                  "id": "database",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "instance",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a resource containing information about a database inside a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03d1e2de-e98a-4a9a-8789-e4cf4674ce54"
            }
          ]
        }
      ]
    }
  ]
}