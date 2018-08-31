{
  "info": {
    "name": "Flickr Reflection Get Method Info",
    "_postman_id": "1d3fb272-2823-4ecf-963e-86acb72faefa",
    "description": "Returns information for a given Flickr API method.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "9fef0fd2-9f75-4dcf-aab1-6c2f6ccceec0",
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
              "id": "9e2b497f-6d82-4380-8cbc-493180c7d7c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "f3288c4f-d86e-421c-b465-b5e2bdb595c9",
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
              "id": "89baeed8-36f2-4414-9ce0-dc4e64f5df6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "d4db4f8c-92b9-4bcc-bda9-bdd6b98ad216",
          "name": "getRestMethodFlickr.groups.members.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.members.getList?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&membertypes=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the members of a group. The call must be signed on behalf of a Flickr member, and the ability to see the group membership will be determined by the Flickr member's group privileges."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d01565c-7214-43f2-8dcb-221ed2b1882a"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "751c7e76-abe7-4b74-bcd5-3a576ddd5f2a",
          "name": "getRestMethodFlickr.machinetags.getnamespaces",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getNamespaces?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique namespaces, optionally limited by a given predicate, in alphabetical order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e70095e-c942-48db-9f47-c105383d19be"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "bdb13bc6-ea17-40ec-aee7-f9ef3062fd6b",
          "name": "getRestMethodFlickr.people.findbyusername",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.findByUsername?api_key=%7B%7D&format=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a user's NSID, given their username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79939376-a3fb-46e3-a27b-f8762edd562b"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "3af2120b-b7e8-4083-9640-dd3824fda50f",
          "name": "postRestMethodFlickr.photos.setmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setMeta?api_key=%7B%7D&description=%7B%7D&photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the meta information for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8bd13a4-9b1f-485f-b1e8-b3e464d3a185"
            }
          ]
        },
        {
          "id": "6d63b772-7977-4e1c-b895-2df5b66be82d",
          "name": "postRestMethodFlickr.photos.comments.addcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.addComment?api_key=%7B%7D&comment_text=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add comment to a photo as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55c8f528-797d-42c5-8f8a-bcbdb99f05e3"
            }
          ]
        },
        {
          "id": "7bb23697-db08-4b1b-89da-7391cf4f8ce6",
          "name": "postRestMethodFlickr.photos.comments.deletecomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.deleteComment?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64fbc8ef-9e99-46db-adab-72641e7dc398"
            }
          ]
        },
        {
          "id": "56c7508b-6599-4ea4-85d7-d6f85c6671cf",
          "name": "postRestMethodFlickr.photos.comments.editcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.editComment?api_key=%7B%7D&comment_id=%7B%7D&comment_text=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the text of a comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12dc8643-da2c-4db2-bc81-d3aeff46fc37"
            }
          ]
        },
        {
          "id": "45326a21-0204-4c1a-9afd-ecd6b6ec4559",
          "name": "getRestMethodFlickr.photos.comments.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getList?api_key=%7B%7D&format=%7B%7D&max_comment_date=%7B%7D&min_comment_date=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the comments for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "caba0bec-6a31-40fc-9f68-f127ac6bc8a3"
            }
          ]
        },
        {
          "id": "5e1b1bd3-2b1d-4384-a8eb-335d32e5d298",
          "name": "getRestMethodFlickr.photos.comments.getrecentforcontacts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.comments.getRecentForContacts?api_key=%7B%7D&contacts_filter=%7B%7D&date_lastcomment=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos belonging to your contacts that have been commented on recently."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4618236-79d9-4f39-9ffb-1bacd14dbe9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "895b0f32-e616-41ba-a6e1-4f6cffdcde56",
          "name": "postRestMethodFlickr.photosets.editmeta",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.editMeta?api_key=%7B%7D&description=%7B%7D&photoset_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the meta-data for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79af5e86-a247-46d5-99a2-9270ba2d5650"
            }
          ]
        },
        {
          "id": "7475e896-84f1-4a8b-befc-2ed3a6429cff",
          "name": "postRestMethodFlickr.photosets.comments.addcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.addComment?api_key=%7B%7D&comment_text=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a comment to a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79ec4e40-6fde-464d-876c-b937b523a648"
            }
          ]
        },
        {
          "id": "247f8057-3659-44c6-853e-2323a9090e84",
          "name": "postRestMethodFlickr.photosets.comments.deletecomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.deleteComment?api_key=%7B%7D&comment_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a photoset comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feb910a9-78a4-4082-9d3f-897bcb1d1eb1"
            }
          ]
        },
        {
          "id": "266fe77f-376a-4aac-9a30-2eb7503c5b21",
          "name": "postRestMethodFlickr.photosets.comments.editcomment",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.editComment?api_key=%7B%7D&comment_id=%7B%7D&comment_text=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the text of a comment as the currently authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "deea790a-dfee-40af-98df-a0bc026435e7"
            }
          ]
        },
        {
          "id": "68063e69-02ca-41c7-954a-edaa90f03c83",
          "name": "getRestMethodFlickr.photosets.comments.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.comments.getList?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the comments for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9f23d0b-5b21-4480-8c1d-309a453e8ad6"
            }
          ]
        }
      ]
    },
    {
      "name": "Reflection",
      "item": [
        {
          "id": "73c39a07-a0fe-4b9b-886d-a8c7a5b4836c",
          "name": "getRestMethodFlickr.reflection.getmethodinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.reflection.getMethodInfo?api_key=%7B%7D&format=%7B%7D&method_name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information for a given Flickr API method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f37f9c4-f980-49b3-9158-03ef5db803f5"
            }
          ]
        }
      ]
    }
  ]
}