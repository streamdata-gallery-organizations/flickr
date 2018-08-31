{
  "info": {
    "name": "Flickr Blogs Get List",
    "_postman_id": "ef54918d-92f1-4147-a31d-45fd98cb3c0d",
    "description": "Get a list of configured blogs for the calling user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "40259e4c-73ed-4037-a0be-43a6ed407d3d",
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
              "id": "db2a8cbd-7a53-4b15-8626-7c0b66aec846"
            }
          ]
        }
      ]
    }
  ]
}