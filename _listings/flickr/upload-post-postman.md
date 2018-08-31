{
  "info": {
    "name": "Flickr Upload",
    "_postman_id": "b2e05348-56e2-43ff-8fa1-bf3d4970f8e6",
    "description": "Uploads a photo. Uploading apps can call the flickr.people.getUploadStatus method in the regular API to obtain file and bandwidth limits for the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "e04cb048-9143-4134-a72b-87b80adbd095",
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
              "id": "8fb8fd79-01b1-423a-9dec-568e9b5e5389"
            }
          ]
        }
      ]
    }
  ]
}