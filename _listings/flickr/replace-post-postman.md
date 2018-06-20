{
  "info": {
    "name": "Flickr Replace",
    "_postman_id": "f1dc186f-8b8c-400e-aa23-57dbde6a18ca",
    "description": "Replaces a photo that has already been uploaded to Flickr. Uploading apps can call the flickr.people.getUploadStatus method in the regular API to obtain file and bandwidth limits for the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "29247ef4-c790-40c3-aa44-7488cdd1bc6f",
          "name": "postUpload",
          "request": {
            "url": "http://api.flickr.com/services/upload?async=%7B%7D&content_type=%7B%7D&description=%7B%7D&hidden=%7B%7D&is_family=%7B%7D&is_friend=%7B%7D&is_public=%7B%7D&safety_level=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads a photo. Uploading apps can call the flickr.people.getUploadStatus method in the regular API to obtain file and bandwidth limits for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5a31943-f4ac-4c57-bb95-00ecc1ebcbeb"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "1d8de9cb-4a1a-4324-9116-403f04971d9f",
          "name": "postReplace",
          "request": {
            "url": "http://api.flickr.com/services/replace?async=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Replaces a photo that has already been uploaded to Flickr. Uploading apps can call the flickr.people.getUploadStatus method in the regular API to obtain file and bandwidth limits for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "599daa01-7f4c-45c3-8a9f-b88987c7c113"
            }
          ]
        }
      ]
    }
  ]
}