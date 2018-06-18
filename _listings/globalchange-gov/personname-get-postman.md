{
  "info": {
    "name": "Global Change Information System API Redirect to a person based on a name",
    "_postman_id": "e2256a2e-68db-4092-afbe-5ef101ad4492",
    "description": "Given a name (case sensitive, concatenated by dashes), redirect if there is a single match.  The first and last names can be in either order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Redirect",
      "item": [
        {
          "id": "2b469b58-858e-41f6-b28c-2ea492e2f933",
          "name": "given-a-name-case-sensitive-concatenated-by-dashes-redirect-if-there-is-a-single-match--the-first-an",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a name (case sensitive, concatenated by dashes), redirect if there is a single match.  The first and last names can be in either order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eecb65b6-1bb5-475c-bdd4-a658dd2a9587"
            }
          ]
        }
      ]
    }
  ]
}