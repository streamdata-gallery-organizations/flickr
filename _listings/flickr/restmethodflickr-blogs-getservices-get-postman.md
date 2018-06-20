{
  "info": {
    "name": "Flickr Blogs Get Services",
    "_postman_id": "5b1efe96-2e03-4ee0-a4b8-5332863a718b",
    "description": "Returns a list of Flickr supported blogging services.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "87999693-4750-4519-b71c-0d6d7b7d552f",
          "name": "getRestMethodFlickr.blogs.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.blogs.getList?api_key=%7B%7D&format=%7B%7D&service=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of configured blogs for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0265c3f0-2d59-4ef3-a5ec-ee6a8fb4cd81"
            }
          ]
        },
        {
          "id": "557fcafc-7eee-4206-b7ae-137a0147ca6a",
          "name": "getRestMethodFlickr.blogs.getservices",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.blogs.getServices?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Flickr supported blogging services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a2b9172-ce2e-49f2-8088-af244207a307"
            }
          ]
        }
      ]
    }
  ]
}