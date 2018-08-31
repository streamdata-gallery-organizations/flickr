{
  "info": {
    "name": "Flickr Groups Get Info",
    "_postman_id": "f026da30-22f2-4d2b-b4f4-12cee045b5db",
    "description": "Get information about a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "19e9ac6a-265d-4e5f-8231-acafe703a352",
          "name": "getRestMethodFlickr.groups.browse",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.browse?api_key=%7B%7D&cat_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse the group category tree, finding groups and sub-categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94807fd9-13e3-4e33-bb9d-0111f30c27cf"
            }
          ]
        },
        {
          "id": "a6994d0a-8ffd-4990-98e9-c1292e18ebde",
          "name": "getRestMethodFlickr.groups.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.getInfo?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20346bff-3a08-4d0d-9e3d-722cbf8cebf4"
            }
          ]
        }
      ]
    }
  ]
}