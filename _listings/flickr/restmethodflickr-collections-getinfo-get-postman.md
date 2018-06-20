{
  "info": {
    "name": "Flickr Collections Get Info",
    "_postman_id": "749a2ac9-1c8a-4a53-bd4a-ac6ab24d0897",
    "description": "Returns information for a single collection. Currently can only be called by the collection owner, this may change.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "f37416d9-3241-4f5a-aec5-00cfadbb34c3",
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
              "id": "8dab0b7d-3754-4a14-b79f-0ab557149733"
            }
          ]
        }
      ]
    }
  ]
}