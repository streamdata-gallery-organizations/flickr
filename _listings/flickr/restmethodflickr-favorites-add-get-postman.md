{
  "info": {
    "name": "Flickr Favorites Add",
    "_postman_id": "9e4ab2cf-5fbe-4630-8199-e05e10fa84be",
    "description": "Adds a photo to a user's favorites list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Favorites",
      "item": [
        {
          "id": "935c2b72-2048-4b77-9a29-7e7f2e210b19",
          "name": "getRestMethodFlickr.favorites.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.add?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to a user's favorites list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27e10691-f639-4486-b1d6-59d467f051fd"
            }
          ]
        }
      ]
    }
  ]
}