{
  "info": {
    "name": "Flickr Places Get Shape History",
    "_postman_id": "ff56b3bd-cc0a-41e3-ad2f-f12325a49eee",
    "description": "Return an historical list of all the shape data generated for a Places or Where on Earth (WOE) ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Places",
      "item": [
        {
          "id": "d6c853e8-1b86-4b56-bc15-019d00bd5a84",
          "name": "getRestMethodFlickr.places.getshapehistory",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getShapeHistory?api_key=%7B%7D&format=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return an historical list of all the shape data generated for a Places or Where on Earth (WOE) ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fde87bde-0a31-430b-ae11-28d2de0b3c23"
            }
          ]
        }
      ]
    }
  ]
}