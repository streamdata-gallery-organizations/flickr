{
  "info": {
    "name": "Flickr Favorites Get List",
    "_postman_id": "37ad2e8f-5dcd-4b98-88e7-f4774e6aafae",
    "description": "Returns a list of the user's favorite photos. Only photos which the calling user has permission to see are returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Favorites",
      "item": [
        {
          "id": "11fd93a7-101c-401b-8e8f-d22434fbed0a",
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
              "id": "a44e78af-27d2-4d72-9f23-dd7fb4c1d0ac"
            }
          ]
        },
        {
          "id": "dc0e0c05-c1ca-4bab-9a51-931e3c7b7e48",
          "name": "getRestMethodFlickr.favorites.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's favorite photos. Only photos which the calling user has permission to see are returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4f004a5-ab7c-49ca-9526-b0cf4d7fe738"
            }
          ]
        }
      ]
    }
  ]
}