{
  "info": {
    "name": "Attom Data Solutions API Returns POIs based on zip code.",
    "_postman_id": "4305d6b2-875c-49f0-9473-ae1b6674b0e7",
    "description": "This search returns a list of Points of Interest in proximity to the centroid of a zip code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "a5317d3f-c969-48bc-87a6-e46fe0c1e88e",
          "name": "getPropertyIdList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/id?geoid=%7B%7D&maxBeds=%7B%7D&minBeds=%7B%7D&orderby=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50cf1356-ad69-4fcf-90e4-57ca57f26d51"
            }
          ]
        },
        {
          "id": "f3b42507-3faa-451f-9330-c78c39f4fb7e",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detail?address=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42374e50-9f66-45f7-930f-6e0d1b35207a"
            }
          ]
        },
        {
          "id": "aec713ca-1fe3-426a-b072-d4986721b93b",
          "name": "adressList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/address?address1=%7B%7D&address2=%7B%7D&orderby=%7B%7D&page=%7B%7D&pagesize=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of properties within a zip code. Use propertytype and order by to narrow down your results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf59e06e-b084-4af8-8399-b3203d9f1b4f"
            }
          ]
        },
        {
          "id": "fe25d55a-c2f9-4492-b5bd-025a39d8fbf4",
          "name": "propertySnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/snapshot?cityname=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&maxavmvalue=%7B%7D&maxLotSize1=%7B%7D&maxtaxamt=%7B%7D&minavmvalue=%7B%7D&minLotSize1=%7B%7D&mintaxamt=%7B%7D&orderby=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of property snapshots within a specific city that are within a desired size range and a specific property type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0b71f95-4fd1-42ae-8195-7198b463f15c"
            }
          ]
        },
        {
          "id": "742c9317-6539-4593-a170-d677bcadb823",
          "name": "propertyBasicProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/basicprofile?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get basic property information and most recent transaction and taxes for a specific attom id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "517aefd1-7120-47ea-9f8c-ad590b33cf19"
            }
          ]
        },
        {
          "id": "cf5a6345-4550-41fd-a0eb-ac5f3fca7d37",
          "name": "propertyExpandedProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/expandedprofile?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a detailed property information and most recent transaction and taxes for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa0fea61-8fa5-453f-b3d4-4428d163b898"
            }
          ]
        },
        {
          "id": "1f7e638e-6a59-4074-bf4c-417b27ff89bc",
          "name": "getAllEventsDetailAddress",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/allevents/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "API Security Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a detail of all the events on a specific property based on its address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b07b9cc3-3a88-46db-bad2-154324b5e194"
            }
          ]
        },
        {
          "id": "bdb92f15-1236-4c87-b7e7-6d197bdedb89",
          "name": "propertyDetailsMortage",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgage?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details mortgage based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ad5b4f1-3028-4a25-8260-d9327297af8d"
            }
          ]
        },
        {
          "id": "ac1c01d3-92b6-4c28-bf76-6b45624ab920",
          "name": "propertyDetailsOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details owner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a938f730-05cb-47e6-9a99-6eea6e9f54a7"
            }
          ]
        },
        {
          "id": "a21dbf4f-0b5f-4cc3-9b8c-8e14346e09ba",
          "name": "propertyDetailsMortgageOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgageowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details mortgageowner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4abbde5a-1629-4738-a07c-212dc15a2f18"
            }
          ]
        },
        {
          "id": "7eb827c9-4dbc-46d1-a357-6cef2a9b632a",
          "name": "getAssessmentSnapshotTotal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/snapshot?address1=%7B%7D&address2=%7B%7D&maxmktttlvalue=%7B%7D&minmktttlvalue=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get snapshots of the properties within a radius of a property that have a total market value within a specified range."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cabf1b88-5201-4873-8586-287e83357066"
            }
          ]
        },
        {
          "id": "f9045d0c-0490-4bbf-bed4-23ebb72a2955",
          "name": "assessmenDetailPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/detail?postalcode=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get assessment details for properties within a zip code. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "424db192-2067-403c-91df-2c382ee04e30"
            }
          ]
        },
        {
          "id": "8c1b7314-b768-4a3d-996d-3857e40d0225",
          "name": "assessmentHistoryDetailID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessmenthistory/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a full detail of property characteristics and assessment history information for a specific property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24bef958-3e8e-4a70-adcd-e629f5af7eb0"
            }
          ]
        },
        {
          "id": "047057a8-5af8-44a6-ac82-3a20b4dff352",
          "name": "avmSnapshotGeoID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/snapshot?geoid=%7B%7D&maxavmvalue=%7B%7D&minavmvalue=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of AVM snapshot records that fall within an Onboard GeoID with a specific value range. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c0f8cf7-119b-441e-902a-23951a35da70"
            }
          ]
        },
        {
          "id": "cfe40182-1ecb-49e6-a28b-7453e12c635e",
          "name": "avmDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get AVM details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2c32466-0f91-4118-89a3-be3f5a7dee76"
            }
          ]
        },
        {
          "id": "cf7b05bf-e6d8-4b13-bc2c-6d1b18757597",
          "name": "attomAvmDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/attomavm/detail?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Attomized AVM and other property details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c1819e4-3310-4d8c-90be-9e0224e5ef5a"
            }
          ]
        },
        {
          "id": "f24f7cdc-8864-4585-b651-4d920960af1f",
          "name": "getHomeSaleSnapshotsGeoId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/snapshot?address1=%7B%7D&address2=%7B%7D&endsalesearchdate=%7B%7D&geoid=%7B%7D&maxsaleamt=%7B%7D&minsaleamt=%7B%7D&propertytype=%7B%7D&radius=%7B%7D&startsalesearchdate=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of home sale snapshots within a Onboard GeoID that sold within a date range and specified sale amount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59b18837-c1ee-4759-96d4-dab961166f8e"
            }
          ]
        },
        {
          "id": "5fe45f0d-ad90-4854-a0ed-17ef3c3ec871",
          "name": "getSaleDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get sales information for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "311f2e3c-539d-4b68-9daf-3b47d0488a2b"
            }
          ]
        },
        {
          "id": "57c11cea-69f0-4a80-9e91-5f4e94ed1bbc",
          "name": "getSaleHistorySnapshotPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/snapshot?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a sales history snapshot of a property based on an Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36f85cb4-1cc1-4bae-9587-d39be8b34972"
            }
          ]
        },
        {
          "id": "995ef465-b63b-428d-b0e2-61b5719eb0a4",
          "name": "saleHistoryBasicHistory",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/basichistory?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the basic transaction and loan history on a property for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e16189b2-cc91-4914-8ebe-fabb1d5a4499"
            }
          ]
        },
        {
          "id": "3dbdd294-9de5-4545-a257-8f56666c81d5",
          "name": "saleHistoryExpandedHistory",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/expandedhistory?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the detailed transaction, pre-foreclosure and loan history on a property for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44f9f1a9-59bf-4719-9ccd-ea406ac9f3c1"
            }
          ]
        },
        {
          "id": "e5883993-6bb6-4d17-8dea-dfd6af9ed094",
          "name": "getSaleHistoryDetailAddress",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a sales history snapshot of a property based on an address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2def3560-345d-4e0d-9056-28fc8ef748e1"
            }
          ]
        },
        {
          "id": "e41b2aab-f0cf-4128-81a0-e32f24000eb7",
          "name": "getSalesTrendByYear",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/salestrend/snapshot?endmonth=%7B%7D&endyear=%7B%7D&geoid=%7B%7D&interval=%7B%7D&startmonth=%7B%7D&startyear=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the average sale price, median sale price, and count of sales for the past 2 years in yearly intervals."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9292c77b-96f3-48d9-a410-3e1e9a31a9d5"
            }
          ]
        },
        {
          "id": "1c5cb1f1-ac63-4c70-8ebd-7ea83ebd8c44",
          "name": "getAreaHierarchyLookup",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/hierarchy/lookup?geoType=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&WKTString=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This method allows you to pass a latitude and longitude point and geo type to retrieve a list of geographies that point falls within. Required input is a valid WKT (Well Known Text) point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78c23186-cd7d-429d-89b2-b72091ce88d6"
            }
          ]
        },
        {
          "id": "3ec3cc32-a96a-4890-8b42-8a2f443bda4e",
          "name": "getPOISearchGeography",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/poi/geography?PostalCodeKey=%7B%7D&RecordLimit=%7B%7D&SearchDistance=%7B%7D&Sort=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This search returns a list of Points of Interest in proximity to the centroid of a zip code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a6f2ceb-6f9f-4ca5-9d0d-f5bae18e87a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "9337577b-cf60-4da0-8cb9-dab0abd82d3c",
          "name": "propertyDetailsWithSchools",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailwithschools?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for a property to have the property details returned, along with the schools in the associated attendance zones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "577447e5-e9db-43ef-aa6f-eef49c91587f"
            }
          ]
        },
        {
          "id": "36f4b2b2-f96f-4155-ae93-a4ee96217c92",
          "name": "propertySchoolSnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/snapshot?filetypetext=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for all schools that are located within a given radius around a given latitude and longitude."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62b3e79d-7874-4a67-83fd-e1d82d751373"
            }
          ]
        },
        {
          "id": "f3175e1d-18d8-48e0-b291-467f4d37b84b",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search by school ID to return all of the available details about a school"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8af3ab3a-7d3b-4187-be63-47c3de88fc5a"
            }
          ]
        },
        {
          "id": "01690d2b-7ba5-4fd7-9604-856176130756",
          "name": "propertySchoolDistrictDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/districtdetail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search by district number to return all of the available details about a school district"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdb6ee90-917e-4cc5-8b81-782cf7a09e6f"
            }
          ]
        }
      ]
    }
  ]
}