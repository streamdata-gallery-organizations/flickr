{
  "info": {
    "name": "Flickr Prefs Get Content Type",
    "_postman_id": "3ca91e79-9a57-4ce0-bf48-5424ca6ac22d",
    "description": "Returns the default content type preference for the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "77e7c68a-0652-4642-9fe6-fe8d9d73eca1",
          "name": "postRestMethodFlickr.photos.setcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setContentType?api_key=%7B%7D&content_type=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the content type of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdbe8eea-a755-4ee2-b306-15307c40e412"
            }
          ]
        }
      ]
    },
    {
      "name": "Prefs",
      "item": [
        {
          "id": "f3ddb92c-0a29-4668-9dd4-e0b5e0437bbc",
          "name": "getRestMethodFlickr.prefs.getcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getContentType?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default content type preference for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f7de214-54ac-4501-8b31-8ce43f24c12d"
            }
          ]
        }
      ]
    }
  ]
}