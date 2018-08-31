{
  "info": {
    "name": "Flickr Tags Get Clusters",
    "_postman_id": "98612168-b4c9-41c4-9cd2-bc39d41d9eac",
    "description": "Returns a list of tag clusters for the given tag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "fd632e2f-0595-4c65-b4a1-9f4607c7a5c2",
          "name": "getRestMethodFlickr.tags.getclusters",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getClusters?api_key=%7B%7D&format=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tag clusters for the given tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a681ff88-3375-4ce8-bcb1-05fdb7be01a8"
            }
          ]
        }
      ]
    }
  ]
}