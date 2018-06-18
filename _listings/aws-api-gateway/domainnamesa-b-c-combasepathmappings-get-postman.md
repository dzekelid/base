{
  "info": {
    "name": "AWS API Gateway API Get Domain Base Path",
    "_postman_id": "a9c5a9cc-43c7-45e0-bc53-d37794241f3a",
    "description": "Gets the BasePathMappings resource representing the collection of base path mappings for the specified custom domain name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Domain",
      "item": [
        {
          "id": "82da102a-b4d3-46a1-9e4f-9d2e62531ff6",
          "name": "domainnameBasepathmappings",
          "request": {
            "url": "http://example.com/api/domainnames/a.b.c.com/basepathmappings",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "Host",
                "description": "",
                "disabled": false
              },
              {
                "key": "X-Amz-Date",
                "value": "X-Amz-Date",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the BasePathMappings resource representing the collection of base path mappings for the specified custom domain name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b50abb04-4132-42a6-9a18-e521b9ff6dde"
            }
          ]
        }
      ]
    }
  ]
}