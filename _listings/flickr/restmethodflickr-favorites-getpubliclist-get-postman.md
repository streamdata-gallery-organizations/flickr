{
  "info": {
    "name": "Flickr Favorites Get Public List",
    "_postman_id": "094778eb-4f1e-4e8f-8a35-c67396928b42",
    "description": "Returns a list of favorite public photos for the given user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Favorites",
      "item": [
        {
          "id": "969a6770-1518-45bd-8ce8-d9a504728041",
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
              "id": "8e7db145-2dd4-4c03-afb5-d602a21b24a3"
            }
          ]
        },
        {
          "id": "769ec4f3-a6ee-426c-8b32-c5c53b182be9",
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
              "id": "c517a83f-c339-49d8-91bb-b2861d7daf8b"
            }
          ]
        },
        {
          "id": "e0ce0f7d-1fb6-4894-ae12-e99f3eab7387",
          "name": "getRestMethodFlickr.favorites.getpubliclist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getPublicList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of favorite public photos for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f6df2f6-8c4b-481f-9d2b-ac866d69a1e2"
            }
          ]
        }
      ]
    }
  ]
}