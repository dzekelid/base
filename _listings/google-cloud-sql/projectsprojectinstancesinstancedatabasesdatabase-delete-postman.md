{
  "info": {
    "name": "Google Cloud SQL API Delete Projects Project Instances Instance Databases Database",
    "_postman_id": "6a22c0c1-9980-437e-ab06-792aec6aef02",
    "description": "Deletes a database from a Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "464661cc-393b-45e6-a12c-1539ce2c5fc5",
          "name": "sql.databases.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a database from a Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6247aa84-7f8f-406f-b242-b546942c5f4f"
            }
          ]
        }
      ]
    }
  ]
}