{
  "info": {
    "name": "Flickr Galleries Edit Meta",
    "_postman_id": "cdb5f200-bfd1-4125-80b6-d67de414a31a",
    "description": "Modify the metadata for a gallery.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "59a5f31f-aa36-4a87-9ddc-8faba868f555",
          "name": "getRestMethodFlickr.activity.usercomments",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userComments?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31abbdcd-dcc0-453f-803d-46ff08592c1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "8af6c211-06f1-4189-8c49-8f7d4e7625f5",
          "name": "postRestMethodFlickr.galleries.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editMeta?api_key=%7B%7D&description=%7B%7D&gallery_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the metadata for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4453fff2-3b83-446d-9510-ac1c783c0afa"
            }
          ]
        }
      ]
    }
  ]
}