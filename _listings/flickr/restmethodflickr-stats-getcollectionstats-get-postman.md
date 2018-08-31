{
  "info": {
    "name": "Flickr Stats Get Collection Stats",
    "_postman_id": "df60feba-e55d-4e1d-80f1-c5c3402b3bc4",
    "description": "Get the number of views on a collection for a given date.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "910fde35-6b51-4fc5-abb9-cfed70b8f3e4",
          "name": "getRestMethodFlickr.collections.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.collections.getInfo?api_key=%7B%7D&collection_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information for a single collection. Currently can only be called by the collection owner, this may change."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f27c20de-130a-424d-b2d2-41b00b39f5a2"
            }
          ]
        },
        {
          "id": "65485b5b-1941-4436-be68-74e7bd93b7bf",
          "name": "getRestMethodFlickr.collections.gettree",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.collections.getTree?api_key=%7B%7D&collection_id=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a tree (or sub tree) of collections belonging to a given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "534b92dc-684d-4e07-98e1-806d148e1651"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "70ff7fbf-890a-4af4-88fc-6acfc3ee456d",
          "name": "getRestMethodFlickr.stats.getcollectionstats",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionStats?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the number of views on a collection for a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d093cd3-a0a6-4867-b8ae-cbe7fd40eead"
            }
          ]
        }
      ]
    }
  ]
}