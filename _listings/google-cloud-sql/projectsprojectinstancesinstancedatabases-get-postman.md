{
  "info": {
    "name": "Google Cloud SQL API Get Projects Project Instances Instance Databases",
    "_postman_id": "aeea7591-67b0-4ea9-b900-6b998961bac4",
    "description": "Lists databases in the specified Cloud SQL instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "projects",
      "item": [
        {
          "id": "a85d4ffb-6875-45f5-a85d-18967dd49db3",
          "name": "sql.databases.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "sql",
                "v1beta4",
                "projects/:project/instances/:instance/databases"
              ],
              "variable": [
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
            "description": "Lists databases in the specified Cloud SQL instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fc89343-03cc-4286-84fa-5cb32a69e2a1"
            }
          ]
        }
      ]
    }
  ]
}