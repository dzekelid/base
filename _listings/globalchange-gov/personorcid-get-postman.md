{
  "info": {
    "name": "Global Change Information System API Redirect to a person based on an ORCID.",
    "_postman_id": "458700c6-08ef-4fb5-bd61-a53052c9cf6c",
    "description": "Given an ORCID, if there is a match, redirect to the persons URI.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Redirect",
      "item": [
        {
          "id": "36ae32e5-f024-4644-bc86-d28c4b2ff2cc",
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
              "id": "26beda78-da16-404b-b0ff-2f2e93271414"
            }
          ]
        },
        {
          "id": "59ca30e3-cda1-490a-8b79-9a92a61bf777",
          "name": "given-an-orcid-if-there-is-a-match-redirect-to-the-persons-uri",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:orcid"
              ],
              "variable": [
                {
                  "id": "orcid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an ORCID, if there is a match, redirect to the persons URI."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c04e27e-52dd-4c63-80f9-9943f6074ad8"
            }
          ]
        }
      ]
    }
  ]
}