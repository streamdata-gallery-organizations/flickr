{
  "info": {
    "name": "Flickr Groups Browse",
    "_postman_id": "80d498a8-4821-4378-b40f-3e0e3b967408",
    "description": "Browse the group category tree, finding groups and sub-categories.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "52b0dbc6-6289-4af8-b934-f4cac0c64660",
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
              "id": "1f8b8ea2-b256-4659-b21b-2d943f922f53"
            }
          ]
        }
      ]
    }
  ]
}