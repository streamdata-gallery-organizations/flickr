{
  "info": {
    "name": "Flickr Contacts Get List Recently Uploaded",
    "_postman_id": "da4ce9db-9f88-4632-bc39-105e232f063b",
    "description": "Return a list of contacts for a user who have recently uploaded photos along with the total count of photos uploaded. This method is still considered experimental. We don't plan for it to change or to go away but so long as this notice is present you should write your code accordingly.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "434d4e92-9ac8-449d-833e-45b04e3461fc",
          "name": "getRestMethodFlickr.contacts.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getList?api_key=%7B%7D&filter=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of contacts for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3274db1-6c02-4ab2-94d4-c7b74d350816"
            }
          ]
        },
        {
          "id": "52425d61-e041-4b74-ba97-99080dd57de3",
          "name": "getRestMethodFlickr.contacts.getlistrecentlyuploaded",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getListRecentlyUploaded?api_key=%7B%7D&date_lastupload=%7B%7D&filter=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of contacts for a user who have recently uploaded photos along with the total count of photos uploaded. This method is still considered experimental. We don't plan for it to change or to go away but so long as this notice is present you should write your code accordingly."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc0344df-12c9-46e9-855c-dad600989871"
            }
          ]
        }
      ]
    }
  ]
}