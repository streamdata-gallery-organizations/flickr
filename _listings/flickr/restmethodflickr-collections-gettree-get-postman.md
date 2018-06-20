{
  "info": {
    "name": "Flickr Collections Get Tree",
    "_postman_id": "a88e50df-c6b9-44cd-a94b-c2e739542f03",
    "description": "Returns a tree (or sub tree) of collections belonging to a given user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "efab48df-2d97-4bd3-9abd-5714beccb8e9",
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
              "id": "a58dd578-2572-4152-858e-c61a880c2a3b"
            }
          ]
        },
        {
          "id": "eadd4fdc-521e-4ad4-9d01-6ca2adaa2788",
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
              "id": "c49b366d-c531-497e-abf5-e48da8c7af22"
            }
          ]
        }
      ]
    }
  ]
}