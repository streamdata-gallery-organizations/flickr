{
  "info": {
    "name": "Flickr Blogs Add Photo",
    "_postman_id": "33f84166-c1bc-48c0-99a9-c748477706fe",
    "description": "Posts a photo to a blog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "6e541a52-98e3-4739-9bbe-16abe14c7673",
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
              "id": "4ea5dce4-5313-42f1-8037-eb297fc9fa31"
            }
          ]
        },
        {
          "id": "a8f8e93a-058a-4bbf-9def-ce39388449e5",
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
              "id": "521bbff8-6620-4460-8ff0-4f1a210e15d9"
            }
          ]
        },
        {
          "id": "52c42d93-238f-4f9d-af69-06105e5a8a6e",
          "name": "getRestMethodFlickr.blogs.addphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.blogs.postPhoto?api_key=%7B%7D&blog_id=%7B%7D&blog_password=%7B%7D&description=%7B%7D&format=%7B%7D&photo_id=%7B%7D&service=%7B%7D&title=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a photo to a blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a3de4a0-5e1f-4b5e-9791-0fc1c9ab0609"
            }
          ]
        }
      ]
    }
  ]
}