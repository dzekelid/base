{
  "info": {
    "name": "Pay Run.IO Gets the rti transaction base template",
    "_postman_id": "12b1cb2e-e222-49f1-bfa7-5da934e4abc7",
    "description": "Return the rti transaction base data object template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Rti",
      "item": [
        {
          "id": "64470e2d-927a-4037-9e5b-45c3186faddf",
          "name": "GetRtiTransactionBaseTemplate",
          "request": {
            "url": "http://api.test.payrun.io/Templates/rtitransactionbase",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Return the rti transaction base data object template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fbb5ef9-2045-427a-8129-b6e65451e739"
            }
          ]
        }
      ]
    }
  ]
}