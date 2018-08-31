{
  "info": {
    "name": "Flickr Favorites Remove",
    "_postman_id": "45ce4516-f980-4bc5-966a-386778d9e145",
    "description": "Adds a photo to a user's favorites list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Favorites",
      "item": [
        {
          "id": "18bc7c7a-4c27-4122-b5dd-59cf4c61f425",
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
              "id": "bc58cb40-2d4f-470f-ba1c-519b40ff1d31"
            }
          ]
        },
        {
          "id": "daa996e6-f804-4433-92df-ce2d76e89a47",
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
              "id": "10bdd758-b9cf-48c2-81da-01a30c30f0a4"
            }
          ]
        },
        {
          "id": "4d6ceddc-88df-4d81-b557-025e5e3d385b",
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
              "id": "126f3b55-5b62-4c52-a1f7-e775c5ffcf4b"
            }
          ]
        },
        {
          "id": "6441bd1a-0e73-466d-8194-5ecb0057d460",
          "name": "getRestMethodFlickr.favorites.remove",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.remove?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
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
              "id": "027c4360-23dd-4252-a57d-c7d083447620"
            }
          ]
        }
      ]
    }
  ]
}