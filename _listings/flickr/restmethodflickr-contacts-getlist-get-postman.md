{
  "info": {
    "name": "Flickr Contacts Get List",
    "_postman_id": "cd2743ca-743b-45b4-9896-f94b1362c25d",
    "description": "Get a list of contacts for the calling user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "5682e5f4-7ce1-44bd-9ddd-d715a51cbaef",
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
              "id": "66caa0a5-3101-4061-9377-f840ec32a14b"
            }
          ]
        }
      ]
    }
  ]
}