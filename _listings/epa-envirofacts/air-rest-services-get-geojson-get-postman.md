{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Air Act Clean Air Act GeoJSON Service",
    "_postman_id": "24861126-c601-4ffa-831c-feb0b7048067",
    "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return GeoJSON of the facilities found.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "01c99feb-52b7-443c-bf7f-14b758d48e88",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "222b7f42-77b2-44ab-a0b8-9f4e26b2dacf"
        }
      ]
    },
    {
      "id": "37b94209-eadf-41ff-bf50-1cc494f8f268",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d6b7d9f8-10d3-40e5-ace8-aa4e14a2c9f0"
        }
      ]
    },
    {
      "id": "3b2ad50f-c84f-463d-8f66-c6365a651354",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "0f0eea63-e218-4861-ad5d-ac1db96e8ab0"
        }
      ]
    },
    {
      "id": "d7452959-bf00-406b-8c0b-cf0395e980ba",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_geojson?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return GeoJSON of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8e04b2bd-7551-4b8b-9197-ad1f619f14f0"
        }
      ]
    }
  ]
}