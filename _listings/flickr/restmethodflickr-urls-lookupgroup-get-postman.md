{
  "info": {
    "name": "Flickr Urls Lookup Group",
    "_postman_id": "068d2003-8a01-41b3-9947-277508ed711a",
    "description": "Returns a group NSID, given the url to a group's page or photo pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "587489d7-5d61-453f-a0ab-6b3461a4ff5a",
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
              "id": "92b34e6c-1b3b-4128-adf1-0d6cb04d1322"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "a43efbf9-32e4-4b69-9958-265b30358e90",
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
              "id": "d2bdcaab-ac50-4389-857d-e1f5a9584ac8"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "d7db5000-ea90-49f9-8e98-4304253cf6b9",
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
              "id": "c349dabe-9aa5-43d3-85e0-897e3d65fb54"
            }
          ]
        },
        {
          "id": "d1a35b67-22ef-4d01-8580-eb7cd62f1812",
          "name": "getRestMethodFlickr.activity.userphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userPhotos?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&timeframe=%7B%7D",
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
              "id": "1a3698f3-e014-446b-9b8a-144104de9fdb"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "0b6d9d65-bf31-4b67-8653-7c5cb21df787",
          "name": "getRestMethodFlickr.auth.checktoken",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.auth.checkToken?api_key=%7B%7D&auth_token=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the credentials attached to an authentication token. This call must be signed as specified in the authentication API spec."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f549b262-2f78-40af-8d38-3f80ac75aad2"
            }
          ]
        },
        {
          "id": "0d62a6c4-bbfa-4f95-b9b1-df87cb622142",
          "name": "getRestMethodFlickr.auth.getfrob",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.auth.getFrob?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a frob to be used during authentication. This method call must be signed, and is deprecated in favour of OAuth."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5146933-4aec-48d9-840c-9ab2858a64aa"
            }
          ]
        },
        {
          "id": "079a8423-73bd-4e6f-b3f3-51eeed470a54",
          "name": "getRestMethodFlickr.auth.getfulltoken",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.auth.getFullToken?api_key=%7B%7D&format=%7B%7D&mini_token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the full authentication token for a mini-token. This method call must be signed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47cb642b-feb5-47b8-888f-c35fbb81e4d2"
            }
          ]
        },
        {
          "id": "895003a1-71a9-454a-8b65-0358b9a96f74",
          "name": "getRestMethodFlickr.auth.gettoken",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.auth.getToken?api_key=%7B%7D&format=%7B%7D&frob=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the auth token for the given frob, if one has been attached. This method call must be signed, and is deprecated in favour of OAuth."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b7a500a-29f8-4c1d-9d9d-d761d8d14eff"
            }
          ]
        },
        {
          "id": "04e3e446-7c92-4e59-bcf2-9b7445f19ad2",
          "name": "getRestMethodFlickr.auth.oauth.getaccesstoken",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.auth.oauth.getAccessToken?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Exchange an auth token from the old Authentication API, to an OAuth access token. Calling this method will delete the auth token used to make the request. The request must be signed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7eeaf995-53a7-493f-b39a-cc0c72ad4fe5"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "a1cada9e-de91-4e24-b031-3d0f4acfaccb",
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
              "id": "bc96ecfc-c7be-4ef5-a59f-7ac84eeafa30"
            }
          ]
        },
        {
          "id": "ab6e1bd8-4c0e-41f2-a903-25d64f2cd3e0",
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
              "id": "014a95d7-46a6-4d2b-9640-acd53347a9e8"
            }
          ]
        },
        {
          "id": "019a7c25-494c-4b3d-9efd-5243b07dcd04",
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
              "id": "749ec33a-d577-49ca-9b5b-1ebae6586275"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "7b175ad7-f0f2-42a0-8a06-142fa20a6fbf",
          "name": "getRestMethodFlickr.collections.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.collections.getInfo?api_key=%7B%7D&collection_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information for a single collection. Currently can only be called by the collection owner, this may change."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "309516bb-97d6-4c31-a943-60efb1feef3b"
            }
          ]
        },
        {
          "id": "213bad56-34d7-482a-be3f-d66f95890a2e",
          "name": "getRestMethodFlickr.collections.gettree",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.collections.getTree?api_key=%7B%7D&collection_id=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a tree (or sub tree) of collections belonging to a given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78ae91c2-eaa6-4034-a8ff-8052591f170c"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "0125471d-6dab-4c5d-80b0-469e392e2558",
          "name": "getRestMethodFlickr.commons.getinstitutions",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.commons.getInstitutions?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of the current Commons institutions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1146f4c-0169-4a9d-9909-f51b3e2681b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "6f1de407-dc5b-4fae-a151-c9ba50778e0a",
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
              "id": "6860cba1-00ca-499d-8e9a-00c082ebde61"
            }
          ]
        },
        {
          "id": "ed7f4114-4ffa-49a6-993f-dc2b457bb8b0",
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
              "id": "8840bf0a-14f2-4ca5-b387-07eaed36932f"
            }
          ]
        },
        {
          "id": "8e180c29-23e9-4fd1-b87e-5098d33572ae",
          "name": "getRestMethodFlickr.contacts.getpubliclist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.contacts.getPublicList?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the contact list for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "908e4e70-1023-40f0-8a0b-64885d7293ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "e7dca2a1-9c40-462d-b1d2-153621e45144",
          "name": "getRestMethodFlickr.favorites.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.add?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to a user's favorites list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a74bda7-7be2-4538-84cf-f73e9d45245c"
            }
          ]
        },
        {
          "id": "c7388df7-b66e-4556-94d5-8a20e37e5671",
          "name": "getRestMethodFlickr.favorites.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's favorite photos. Only photos which the calling user has permission to see are returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96ac36e1-71f8-406b-bef2-b5bdd3ffaa95"
            }
          ]
        },
        {
          "id": "5e10e232-e6c4-43a0-8bce-bc553f437a7f",
          "name": "getRestMethodFlickr.favorites.getpubliclist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.getPublicList?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of favorite public photos for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee1b2304-599e-40a2-af42-23a4325e9a14"
            }
          ]
        },
        {
          "id": "69840621-396d-4408-b4ef-e261b45b8fb3",
          "name": "getRestMethodFlickr.favorites.remove",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.favorites.remove?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to a user's favorites list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beff99b0-50e0-4d59-bf64-676e7f20fdb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "5970b874-d459-4141-9023-431507904fee",
          "name": "postRestMethodFlickr.galleries.addphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.addPhoto?api_key=%7B%7D&comment=%7B%7D&gallery_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a photo to a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9469ab3e-2516-4b06-90d1-43105d2c1ee2"
            }
          ]
        },
        {
          "id": "9b83c0d1-63f7-4a12-9f92-0a877fbcd79b",
          "name": "postRestMethodFlickr.galleries.create",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.create?api_key=%7B%7D&description=%7B%7D&format=%7B%7D&primary_photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new gallery for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "099ede7e-9891-4714-837a-5cc957f51b65"
            }
          ]
        },
        {
          "id": "a930c555-c72e-4f80-b5a7-af181953ac91",
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
              "id": "6709bc46-411d-4b6e-afa3-20f6c93de5e2"
            }
          ]
        },
        {
          "id": "1939f7cb-0a4f-4338-8e0f-020fde41096a",
          "name": "postRestMethodFlickr.galleries.editphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editPhoto?api_key=%7B%7D&comment=%7B%7D&gallery_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the comment for a gallery photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09f5b921-80ee-485f-b3c2-7f536adebdc1"
            }
          ]
        },
        {
          "id": "119105e9-2dc6-4d82-94f9-3645be30475b",
          "name": "postRestMethodFlickr.galleries.editphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.editPhotos?api_key=%7B%7D&gallery_id=%7B%7D&photo_ids=%7B%7D&primary_photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the photos in a gallery. Use this method to add, remove and re-order photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "116c1b9a-a547-437a-9734-ee5ef090254b"
            }
          ]
        },
        {
          "id": "f2947be1-f33f-4f17-b1e7-3afa0a06c609",
          "name": "getRestMethodFlickr.galleries.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getInfo?api_key=%7B%7D&format=%7B%7D&gallery_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55046de2-e2bb-494c-a9e2-26db6b1b1117"
            }
          ]
        },
        {
          "id": "2e90a1d2-0b37-49b8-aa30-17c59d827631",
          "name": "getRestMethodFlickr.galleries.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getList?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of galleries created by a user. Sorted from newest to oldest."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a35b4656-2c39-4f54-9b8f-d855bfa2d605"
            }
          ]
        },
        {
          "id": "73188f4d-30fa-4934-b784-8f3c9aa70356",
          "name": "getRestMethodFlickr.galleries.getlistforphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getListForPhoto?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of galleries to which a photo has been added. Galleries are returned sorted by date which the photo was added to the gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a5a6442-368a-4f17-95a8-b723ce7e7485"
            }
          ]
        },
        {
          "id": "4a5a0cd0-5210-4682-8045-99ca4a7a1ad7",
          "name": "getRestMethodFlickr.galleries.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.galleries.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&gallery_id=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of photos for a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "252f9667-cc8f-4102-86dd-1d9e4d7d1447"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "b1b1928d-60c1-4e8e-8098-1aea747f9515",
          "name": "getRestMethodFlickr.groups.browse",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.browse?api_key=%7B%7D&cat_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse the group category tree, finding groups and sub-categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d299de2a-fe87-4b02-8889-dec3efaacd84"
            }
          ]
        },
        {
          "id": "8081e3cb-5698-4cd7-a926-cd4c1dba5b67",
          "name": "getRestMethodFlickr.groups.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.getInfo?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c820d42-725f-43f6-b9e2-8da62001f3c7"
            }
          ]
        },
        {
          "id": "b1209bc0-f1bb-45cf-aaa7-429e06756253",
          "name": "getRestMethodFlickr.groups.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.search?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&text=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baba71f2-8ee9-4b81-8440-a884af9e49a4"
            }
          ]
        },
        {
          "id": "f507ea0c-3aac-4665-9987-b31a65369831",
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
              "id": "75ea1f23-d625-4cba-9a2d-c663bfded452"
            }
          ]
        },
        {
          "id": "d90635c7-79da-4756-9328-6dc777270de7",
          "name": "postRestMethodFlickr.groups.pools.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.add?api_key=%7B%7D&group_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a photo to a group's pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79919278-eb14-4dff-8235-92ad5bc1a567"
            }
          ]
        },
        {
          "id": "1f8979dd-a4ea-461c-a370-d8239bcb898a",
          "name": "getRestMethodFlickr.groups.pools.getcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.getContext?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a group pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7639da6a-9bce-48e9-bcd5-60ca59901355"
            }
          ]
        },
        {
          "id": "e7d78912-8b5f-4627-b1a4-09035a64784a",
          "name": "getRestMethodFlickr.groups.pools.getgroups",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.getGroups?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of groups to which you can add photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78a57924-0d08-4733-8527-2748d4760e6e"
            }
          ]
        },
        {
          "id": "f6977b42-045f-42b1-8edb-f3aefabb03fc",
          "name": "getRestMethodFlickr.groups.pools.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&tags=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of pool photos for a given group, based on the permissions of the group and the user logged in (if any)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11f3ecd3-49df-4674-a4da-8a5fae69ff92"
            }
          ]
        },
        {
          "id": "fb8d0067-17ec-4355-baa1-6ef36b236d63",
          "name": "postRestMethodFlickr.groups.pools.remove",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.pools.remove?api_key=%7B%7D&group_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a photo from a group pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15af0397-457c-48b5-93e4-84350e99ae2d"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "30a849ad-3982-4c14-bddf-4ad906f6734f",
          "name": "getRestMethodFlickr.interestingness.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.interestingness.getList?api_key=%7B%7D&date=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of interesting photos for the most recent day or a user-specified date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dffac251-917b-4d08-ac49-92cd54efc34d"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "c060b578-7d47-431c-8016-27adebd17b3c",
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
              "id": "8bff13dc-4ed3-464a-b98c-4cf63f04eb33"
            }
          ]
        },
        {
          "id": "624ec16d-94bb-43fa-a2c4-9b1ed50ee151",
          "name": "getRestMethodFlickr.machinetags.getpairs",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getPairs?api_key=%7B%7D&format=%7B%7D&namespace=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique namespace and predicate pairs, optionally limited by predicate or namespace, in alphabetical order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "360ccd6a-f7eb-466d-8795-1b28b25b82fb"
            }
          ]
        },
        {
          "id": "9e300d3f-cfa4-4945-b3c2-286ce331e183",
          "name": "getRestMethodFlickr.machinetags.getpredicates",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getPredicates?api_key=%7B%7D&format=%7B%7D&namespace=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique predicates, optionally limited by a given namespace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d02a72ba-425c-40f3-bc1a-399d645cfac6"
            }
          ]
        },
        {
          "id": "f1809eea-82fc-423a-b00c-48357695b604",
          "name": "getRestMethodFlickr.machinetags.getrecentvalues",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getRecentValues?api_key=%7B%7D&format=%7B%7D&namespace=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch recently used (or created) machine tags values."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e10b2b8-7e82-49b8-86f1-cc5b8c930057"
            }
          ]
        },
        {
          "id": "7b022cb4-a48a-41e9-af8d-fe7e63270e3f",
          "name": "getRestMethodFlickr.machinetags.getvalues",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.machinetags.getValues?api_key=%7B%7D&format=%7B%7D&namespace=%7B%7D&page=%7B%7D&per_page=%7B%7D&predicate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of unique values for a namespace and predicate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24db5ef5-12e2-4bc3-bb34-892da392cb90"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "4675e23b-9f45-4e0a-b423-18b7c28b4016",
          "name": "getRestMethodFlickr.panda.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.panda.getList?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of Flickr pandas, from whom you can request photos using the flickr.panda.getPhotos API method. More information about the pandas can be found on the dev blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "192ed6df-4ab4-4d09-9d1d-3e8f484384c5"
            }
          ]
        },
        {
          "id": "9862e5cf-086e-4326-be6a-06384cd62fde",
          "name": "getRestMethodFlickr.panda.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.panda.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&panda_name=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Ask the Flickr Pandas for a list of recent public (and \"safe\") photos. More information about the pandas can be found on the dev blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5615cf46-94fe-4cce-95dc-b78a70f5e6e8"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "aebabe97-c950-44ce-86bb-6361f6a86402",
          "name": "getRestMethodFlickr.people.findbyemail",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.findByEmail?api_key=%7B%7D&find_email=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a user's NSID, given their email address"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf9bccb0-6c2c-4f09-a5f1-3c5891894aa1"
            }
          ]
        },
        {
          "id": "babee61c-6535-445e-a2cc-e8bda87dbfa5",
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
              "id": "b6a42cd7-b8bb-43a2-96f9-d7c98419e070"
            }
          ]
        },
        {
          "id": "addb8b80-857c-4b69-99bb-5eabf21509e4",
          "name": "getRestMethodFlickr.people.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getInfo?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03006e8f-6428-48ec-8d89-1a2411effc17"
            }
          ]
        },
        {
          "id": "f62928bb-9533-4fb6-9747-14769c7358fa",
          "name": "getRestMethodFlickr.people.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPhotos?api_key=%7B%7D&content_type=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D&safe_search=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return photos from the given user's photostream. Only photos visible to the calling user will be returned. This method must be authenticated; to return public photos for a user, use flickr.people.getPublicPhotos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70514e6f-3892-436a-af8f-a52de4b48d8c"
            }
          ]
        },
        {
          "id": "d0951bd0-201c-41cc-b7ff-4e7341a44672",
          "name": "getRestMethodFlickr.people.getphotosof",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPhotosOf?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&owner_id=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos containing a particular Flickr member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db3356b6-0be2-4689-87e1-69c630321907"
            }
          ]
        },
        {
          "id": "8d435edf-1469-4c58-9215-4a0c87469c82",
          "name": "getRestMethodFlickr.people.getpublicgroups",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPublicGroups?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of public groups a user is a member of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c478cef0-69dc-4385-99b8-89c635577e3c"
            }
          ]
        },
        {
          "id": "de95ab3b-80de-44fd-be40-9cd23c2a4422",
          "name": "getRestMethodFlickr.people.getpublicphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getPublicPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&safe_search=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of public photos for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dff48050-9420-4294-849f-678f8e4f08ab"
            }
          ]
        },
        {
          "id": "7d00ab51-af21-44d3-b644-09e9d9f4004e",
          "name": "getRestMethodFlickr.people.getuploadstatus",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.people.getUploadStatus?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information for the calling user related to photo uploads."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bb41e76-70d9-42bc-8b84-1c8a0263b26f"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "8fe54aec-5ede-494a-a313-809110b49ebf",
          "name": "postRestMethodFlickr.photos.addtags",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.addTags?api_key=%7B%7D&photo_id=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add tags to a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "987ea8a5-79db-4858-b204-22638e129c28"
            }
          ]
        },
        {
          "id": "e5b7fbc4-a14a-467a-9392-c99da1d70b35",
          "name": "postRestMethodFlickr.photos.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.delete?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a photo from Flickr."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea5700d0-b918-443e-9620-79b0e54e8821"
            }
          ]
        },
        {
          "id": "35f8e63f-2fd1-4f3e-af1d-8e8610cdd13d",
          "name": "getRestMethodFlickr.photos.getallcontexts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getAllContexts?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all visible sets and pools the photo belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e0f89cf-1775-468a-ae51-658c782bec3b"
            }
          ]
        },
        {
          "id": "36c1fe95-ea7f-4047-b5a1-5ac2c08b2062",
          "name": "getRestMethodFlickr.photos.getcontactsphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContactsPhotos?api_key=%7B%7D&count=%7B%7D&extras=%7B%7D&format=%7B%7D&include_self=%7B%7D&just_friends=%7B%7D&single_photo=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a list of recent photos from the calling users' contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58982a49-bb66-4096-829e-4729d365d76d"
            }
          ]
        },
        {
          "id": "ecbff92a-20fd-4b4e-aea1-3ea2a33cfd87",
          "name": "getRestMethodFlickr.photos.getcontactspublicphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContactsPublicPhotos?api_key=%7B%7D&count=%7B%7D&extras=%7B%7D&format=%7B%7D&include_self=%7B%7D&just_friends=%7B%7D&single_photo=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch a list of recent public photos from a users' contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82c82ff1-d2f1-4265-9b3a-9ff25b93bd6e"
            }
          ]
        },
        {
          "id": "b94d1753-85de-40c5-9ae3-467f411a9ac8",
          "name": "getRestMethodFlickr.photos.getcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getContext?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40d4fa88-c434-47f9-a67f-56726c3d22d8"
            }
          ]
        },
        {
          "id": "53cbc64a-ccf5-484d-9c2b-122062e30129",
          "name": "getRestMethodFlickr.photos.getcounts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getCounts?api_key=%7B%7D&dates=%7B%7D&format=%7B%7D&taken_dates=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "482c4c58-9554-4e33-b8fd-0f3ab1cb11c5"
            }
          ]
        },
        {
          "id": "ccc5133b-f815-4cf7-9c8a-ed11a396e282",
          "name": "getRestMethodFlickr.photos.getexif",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getExif?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7c05ea0-9f16-4704-886f-9ff761b4f0f2"
            }
          ]
        },
        {
          "id": "6fe3ba7a-7909-4cce-9f83-5fb17fb23593",
          "name": "getRestMethodFlickr.photos.getfavorites",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getFavorites?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of people who have favorited a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adaba1c1-9e0b-470e-9377-0c3de587c7cf"
            }
          ]
        },
        {
          "id": "07a51caa-a142-4170-8fac-505b2e805a57",
          "name": "getRestMethodFlickr.photos.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getInfo?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e59d5b0b-a6bd-43fc-b23a-1232e1a928bf"
            }
          ]
        },
        {
          "id": "5b93d468-cf13-4280-b236-b3477894b891",
          "name": "getRestMethodFlickr.photos.getnotinset",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getNotInSet?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos that are not part of any sets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d06315c7-df1e-43e8-99a2-9a240d76cf7b"
            }
          ]
        },
        {
          "id": "ec53b458-19c0-48eb-a0bc-ac78f5bb9b4c",
          "name": "getRestMethodFlickr.photos.getperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getPerms?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get permissions for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beafb4bb-8caa-4df1-bf9a-80faa55f2a74"
            }
          ]
        },
        {
          "id": "97ab3efe-d366-4ef7-bb24-3ce1180ce08d",
          "name": "getRestMethodFlickr.photos.getrecent",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getRecent?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of people who have favorited a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c365db27-af49-4ca2-9c46-657edc9524c7"
            }
          ]
        },
        {
          "id": "8d62b677-322b-4179-8970-5de83707d22e",
          "name": "getRestMethodFlickr.photos.getsizes",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getSizes?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the available sizes for a photo. The calling user must have permission to view the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84dd8414-393a-46d7-9b37-969c4113d72b"
            }
          ]
        },
        {
          "id": "53bb119c-1861-494e-8688-f573203c0938",
          "name": "getRestMethodFlickr.photos.getuntagged",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getUntagged?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos that are not tagged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c40de18f-37b4-4ddd-9873-9d3cb1bfc65d"
            }
          ]
        },
        {
          "id": "55ecabed-98fb-48d7-919e-bf49c03aa94c",
          "name": "getRestMethodFlickr.photos.getwithgeodata",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getWithGeoData?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your geo-tagged photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bef6195-ab6b-4c68-a89b-3a2c416dd1f6"
            }
          ]
        },
        {
          "id": "e15dca41-9294-4564-a72d-b74e203ff898",
          "name": "getRestMethodFlickr.photos.getwithoutgeodata",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getWithoutGeoData?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your photos which haven't been geo-tagged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "259e109d-6f66-4569-9635-c74d0d250557"
            }
          ]
        },
        {
          "id": "9a12f85d-5439-4b09-90f7-43766a9023c4",
          "name": "getRestMethodFlickr.photos.getrecentlyupdated",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.getRecentlyUpdated?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&min_date=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of your photos that have been recently created or which have been recently modified. Recently modified may mean that the photo's metadata (title, description, tags) may have been changed or a comment has been added (or just modified somehow :-)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb6abcd3-1440-4bf3-9a28-b7a328b5de3e"
            }
          ]
        },
        {
          "id": "a32e5f3c-a776-4cb7-b99b-e9fc2843ce6f",
          "name": "postRestMethodFlickr.photos.removetag",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.removeTag?api_key=%7B%7D&photo_id=%7B%7D&tag_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a tag from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65b37335-a9b8-4951-be2a-9f5aae5b3ea8"
            }
          ]
        },
        {
          "id": "0edcbc28-27f0-4af3-8be9-6ec98a67b169",
          "name": "getRestMethodFlickr.photos.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.search?accuracy=%7B%7D&api_key=%7B%7D&contacts=%7B%7D&content_type=%7B%7D&extras=%7B%7D&format=%7B%7D&geo_context=%7B%7D&group_id=%7B%7D&has_geo=%7B%7D&hbox=%7B%7D&is_commons=%7B%7D&is_gallery=%7B%7D&is_getty=%7B%7D&lat=%7B%7D&license=%7B%7D&lon=%7B%7D&machine_tags=%7B%7D&machine_tag_mode=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&place_id=%7B%7D&privacy_filter=%7B%7D&radius=%7B%7D&radius_units=%7B%7D&safe_search=%7B%7D&sort=%7B%7D&tags=%7B%7D&tag_mode=%7B%7D&text=%7B%7D&user_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos matching some criteria. Only photos visible to the calling user will be returned. To return private or semi-private photos, the caller must be authenticated with 'read' permissions, and have permission to view the photos. Unauthenticated calls will only return public photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "679df48c-30fc-4247-8138-c4da6b0e6876"
            }
          ]
        },
        {
          "id": "360d9048-af22-4c29-bc4e-178943ed07a0",
          "name": "postRestMethodFlickr.photos.setcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setContentType?api_key=%7B%7D&content_type=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the content type of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5f63bb5-a236-4c46-a3f7-75b3b4a8358b"
            }
          ]
        },
        {
          "id": "cc732239-26b0-4e8c-b3a4-27d391fd6e4f",
          "name": "postRestMethodFlickr.photos.setdates",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setDates?api_key=%7B%7D&date_posted=%7B%7D&date_taken=%7B%7D&date_taken_granularity=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set one or both of the dates for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbc2c476-b8c9-4e81-97b9-6311b3f0e231"
            }
          ]
        },
        {
          "id": "ca274d26-65ca-43bc-a457-b74dc168fa43",
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
              "id": "0c7e4b1e-627f-460d-9507-0b913fbbd2cd"
            }
          ]
        },
        {
          "id": "15a9585e-afa1-4fc3-b2bb-721c327d3702",
          "name": "postRestMethodFlickr.photos.setperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setPerms?api_key=%7B%7D&format=%7B%7D&is_family=%7B%7D&is_friend=%7B%7D&is_public=%7B%7D&perm_addmeta=%7B%7D&perm_comment=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set permissions for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "264be940-c92d-436d-ae17-20873d72a841"
            }
          ]
        },
        {
          "id": "f3d28fff-165d-4da0-9f7a-c0b311972e06",
          "name": "postRestMethodFlickr.photos.setsafetylevel",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setSafetyLevel?api_key=%7B%7D&format=%7B%7D&hidden=%7B%7D&photo_id=%7B%7D&safety_level=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the safety level of a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04a05d11-0262-4edc-82e0-f45737ac61f6"
            }
          ]
        },
        {
          "id": "36c1ac78-e49b-4a4b-8ef6-b21a41796169",
          "name": "postRestMethodFlickr.photos.settags",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.setTags?api_key=%7B%7D&photo_id=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the tags for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34418ff1-7f4f-40c7-b73e-1c80c17c9de8"
            }
          ]
        },
        {
          "id": "a10385d3-d04c-4a9a-a19a-6bf56e804d8c",
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
              "id": "7cd6944a-48e4-4730-a467-f59df26603e0"
            }
          ]
        },
        {
          "id": "4d85ceb2-0cb0-484b-9805-970a1726ec57",
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
              "id": "2a29940c-b172-4278-a80c-ad2b1a3519d6"
            }
          ]
        },
        {
          "id": "2820b749-8394-4a27-8fe8-2da9aaee49e4",
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
              "id": "534f4607-02fa-4d38-93e4-4607438bc714"
            }
          ]
        },
        {
          "id": "911946eb-e78c-4fd4-a6b1-21c53f4bc6c7",
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
              "id": "41ca1831-f826-487c-b463-0902a683521e"
            }
          ]
        },
        {
          "id": "96f2744e-e705-4666-b075-78095feddcff",
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
              "id": "d4416bef-e8dc-4d71-b506-0d3037bcfc2a"
            }
          ]
        },
        {
          "id": "c4103926-1891-441e-81a2-763193320fa5",
          "name": "postRestMethodFlickr.photos.geo.batchcorrectlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.batchCorrectLocation?accuracy=%7B%7D&api_key=%7B%7D&lat=%7B%7D&lon=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Correct the places hierarchy for all the photos for a user at a given latitude, longitude and accuracy. Batch corrections are processed in a delayed queue so it may take a few minutes before the changes are reflected in a user's photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c09dca6-ed02-4840-9096-78ad6783289c"
            }
          ]
        },
        {
          "id": "31630703-bfd7-487f-ba94-85cd057132c3",
          "name": "postRestMethodFlickr.photos.geo.correctlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.correctLocation?api_key=%7B%7D&photo_id=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Corrects a photo's location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06c4c9e8-3598-45ac-a9a6-695e9b6bcd1a"
            }
          ]
        },
        {
          "id": "48dd47bb-f253-41af-b831-9dafd07eda8b",
          "name": "getRestMethodFlickr.photos.geo.getlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.getLocation?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the geo data (latitude and longitude and the accuracy level) for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf81a736-8db5-4bae-9332-6d0ea42d3ba7"
            }
          ]
        },
        {
          "id": "364f206a-928d-410f-ab53-e5f7b283c69d",
          "name": "getRestMethodFlickr.photos.geo.getperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.getPerms?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get permissions for who may view geo data for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f2750ff-cf19-40c4-8fe8-3e945d4f3f69"
            }
          ]
        },
        {
          "id": "96c0392d-eb58-422d-b250-b8dcc9e18e1e",
          "name": "getRestMethodFlickr.photos.geo.photosforlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.photosForLocation?accuracy=%7B%7D&api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&lat=%7B%7D&lon=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos for the calling user at a specific latitude, longitude and accuracy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3d0d517-5a3c-4fdb-9fac-a33b320ddf83"
            }
          ]
        },
        {
          "id": "0ce69fcd-37a4-4a61-9147-b92e1041b303",
          "name": "postRestMethodFlickr.photos.geo.removelocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.removeLocation?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the geo data associated with a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96acb15a-ec87-47ed-a851-d7a8edb165eb"
            }
          ]
        },
        {
          "id": "4e98cc4b-6c10-4ff6-9acd-d457105eeaf2",
          "name": "postRestMethodFlickr.photos.geo.setcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setContext?api_key=%7B%7D&context=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Indicate the state of a photo's geotagginess beyond latitude and longitude. Note : photos passed to this method must already be geotagged (using the flickr.photos.geo.setLocation method)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "644d795f-0b96-4690-a378-bbba477be2bf"
            }
          ]
        },
        {
          "id": "a8051339-6226-489f-ae26-1e4e9a99bb81",
          "name": "postRestMethodFlickr.photos.geo.setlocation",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setLocation?accuracy=%7B%7D&api_key=%7B%7D&context=%7B%7D&format=%7B%7D&lat=%7B%7D&lon=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the geo data (latitude and longitude and, optionally, the accuracy level) for a photo. Before users may assign location data to a photo they must define who, by default, may view that information. Users can edit this preference at http://www.flickr.com/account/geo/privacy/. If a user has not set this preference, the API method will return an error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d4311e5-2048-42c3-98be-2c2370fe4ed1"
            }
          ]
        },
        {
          "id": "2d8a73b5-d74e-4d76-9b23-96ba439dafd9",
          "name": "getRestMethodFlickr.photos.geo.setperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.geo.setPerms?api_key=%7B%7D&is_contact=%7B%7D&is_family=%7B%7D&is_friend=%7B%7D&is_public=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Set the permission for who may view the geo data associated with a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03130065-c0d9-4747-b71e-2716c6c1d2b9"
            }
          ]
        },
        {
          "id": "47c326c4-feb3-4861-9d67-92d7b22f8c78",
          "name": "getRestMethodFlickr.photos.licenses.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.licenses.getInfo?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a list of available photo licenses for Flickr."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2392d644-917c-48ba-87c4-f6d70a8b9664"
            }
          ]
        },
        {
          "id": "bc2efdc1-1289-477b-9f73-590dbad5338f",
          "name": "postRestMethodFlickr.photos.licenses.setinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.licenses.setInfo?api_key=%7B%7D&license_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the license for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e4719d7-636a-4e96-b9b3-6cba7154f2fc"
            }
          ]
        },
        {
          "id": "86f9754c-d99c-4215-94a6-7f08eeaa71c1",
          "name": "postRestMethodFlickr.photos.notes.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.add?api_key=%7B%7D&format=%7B%7D&note_h=%7B%7D&note_text=%7B%7D&note_w=%7B%7D&note_x=%7B%7D&note_y=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a note to a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5afbc887-c0fe-48f9-8a17-fd2d4b1a002c"
            }
          ]
        },
        {
          "id": "aca3671b-9376-4eaf-a6e8-22793b467205",
          "name": "postRestMethodFlickr.photos.notes.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.delete?api_key=%7B%7D&note_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a note from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54d80374-a44b-4a32-9f39-e832c258751c"
            }
          ]
        },
        {
          "id": "3161fa9c-1689-4df9-87df-477f74ff8ece",
          "name": "postRestMethodFlickr.photos.notes.edit",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.notes.edit?api_key=%7B%7D&note_h=%7B%7D&note_id=%7B%7D&note_text=%7B%7D&note_w=%7B%7D&note_x=%7B%7D&note_y=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a note on a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40dea0ad-586d-46d2-a756-39ad70054434"
            }
          ]
        },
        {
          "id": "c7c512be-1f17-4b88-9b06-6352c214f94f",
          "name": "postRestMethodFlickr.photos.people.add",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.add?api_key=%7B%7D&person_h=%7B%7D&person_w=%7B%7D&person_x=%7B%7D&person_y=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a person to a photo. Coordinates and sizes are in pixels, based on the 500px image size shown on individual photo pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81da6553-f58b-46d4-8105-c85b1e1c976e"
            }
          ]
        },
        {
          "id": "d9601878-afce-4b2c-a5ad-ca47e83b58f8",
          "name": "postRestMethodFlickr.photos.people.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.delete?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a person from a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a20e062-a002-433f-b429-19c1a8dc83bb"
            }
          ]
        },
        {
          "id": "733d1461-d644-4021-916e-8513bd00299f",
          "name": "postRestMethodFlickr.photos.people.deletecoords",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.deleteCoords?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove the bounding box from a person in a photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90fb1288-6a83-4b65-b2af-01ac01ed4cfe"
            }
          ]
        },
        {
          "id": "c8d114da-4311-4991-acbf-81a7b0fa420b",
          "name": "postRestMethodFlickr.photos.people.editcoords",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.editCoords?api_key=%7B%7D&person_h=%7B%7D&person_w=%7B%7D&person_x=%7B%7D&person_y=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edit the bounding box of an existing person on a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b07011f-6bd1-4f52-839c-0a1e6b8b01bf"
            }
          ]
        },
        {
          "id": "50310c50-59fd-4fd2-8336-8d70f019c264",
          "name": "getRestMethodFlickr.photos.people.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.people.getList?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of people in a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4c34562-b735-44b9-99b4-01dbfd1e9374"
            }
          ]
        },
        {
          "id": "d8a6fecc-2486-42a7-8fe5-e9e75a8a424e",
          "name": "postRestMethodFlickr.photos.transform.rotate",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.transform.rotate?api_key=%7B%7D&degrees=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rotate a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec720f9b-6108-460f-a8bf-918eeb314131"
            }
          ]
        },
        {
          "id": "96699628-c69d-4a56-ace4-b743f934a7a1",
          "name": "getRestMethodFlickr.photos.upload.checktickets",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photos.upload.checkTickets?api_key=%7B%7D&format=%7B%7D&tickets=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the status of one or more asynchronous photo upload tickets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b4770f4-49d4-4248-bf69-f9ea7824a659"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "3109480d-f488-497e-af91-bf09dd70ac71",
          "name": "postRestMethodFlickr.photosets.addphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.addPhoto?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a photo to the end of an existing photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76a023c8-5658-46c3-90c8-6d6fdd869457"
            }
          ]
        },
        {
          "id": "9fddd4ce-893d-419f-b9a0-bb1bb2d4ebd4",
          "name": "postRestMethodFlickr.photosets.create",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.create?api_key=%7B%7D&description=%7B%7D&format=%7B%7D&primary_photo_id=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new photoset for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cde6fa9b-08ff-46c5-9673-eb94ea4768de"
            }
          ]
        },
        {
          "id": "6ec7a329-b97e-4a24-a922-c71360740a8b",
          "name": "postRestMethodFlickr.photosets.delete",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.delete?api_key=%7B%7D&photoset_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a new photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "908845fc-58fe-41d4-9ec9-deb2ed59274b"
            }
          ]
        },
        {
          "id": "37521689-0f88-4f91-aa27-d7714b2097df",
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
              "id": "510cd5b0-1c49-424b-a0a6-5d4f851be82b"
            }
          ]
        },
        {
          "id": "e8ef741a-7f36-46fd-9d63-e625b18e9fef",
          "name": "postRestMethodFlickr.photosets.editphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.editPhotos?api_key=%7B%7D&photoset_id=%7B%7D&photo_ids=%7B%7D&primary_photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Modify the photos in a photoset. Use this method to add, remove and re-order photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbcb485c-0755-4337-8ebf-abc32c407f5d"
            }
          ]
        },
        {
          "id": "c5ed6425-6d96-4e8d-b91f-ffc2372b23b3",
          "name": "getRestMethodFlickr.photosets.getcontext",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getContext?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49892d9a-6145-4b6c-8ee2-c6ff50e80752"
            }
          ]
        },
        {
          "id": "c401bd13-f319-4ecc-9b4e-de58ca1825b5",
          "name": "getRestMethodFlickr.photosets.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getInfo?api_key=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b5dd9e0-03c0-4dbd-9d11-d475f4911f7d"
            }
          ]
        },
        {
          "id": "15d1211d-6fd2-436d-a5bd-2522660ddcbd",
          "name": "getRestMethodFlickr.photosets.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getList?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the photosets belonging to the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a991ba3e-e3a7-49cd-aedf-357234c299bc"
            }
          ]
        },
        {
          "id": "857e4968-f2ec-4b01-9117-3b4780bd0868",
          "name": "getRestMethodFlickr.photosets.getphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.getPhotos?api_key=%7B%7D&extras=%7B%7D&format=%7B%7D&media=%7B%7D&page=%7B%7D&per_page=%7B%7D&photoset_id=%7B%7D&privacy_filter=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of photos in a set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1da3fbd8-cc29-4d50-a8cb-c5f3442a2641"
            }
          ]
        },
        {
          "id": "79b0f957-fbec-4ecb-9c1e-ec64fc037dbe",
          "name": "postRestMethodFlickr.photosets.ordersets",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.orderSets?api_key=%7B%7D&photoset_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set the order of photosets for the calling user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18aaa4f3-5201-456a-a37f-915a66f7d27e"
            }
          ]
        },
        {
          "id": "2cf511ce-d767-428c-8ab8-6837c4994746",
          "name": "postRestMethodFlickr.photosets.removephoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.removePhoto?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a photo from a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "967f4077-a8d8-460f-a4cc-c577ac800faa"
            }
          ]
        },
        {
          "id": "fa2ed1c7-26b4-4357-a166-57ce3e4abed6",
          "name": "postRestMethodFlickr.photosets.removephotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.removePhotos?api_key=%7B%7D&photoset_id=%7B%7D&photo_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove multiple photos from a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2990188f-5c03-41d8-b812-02a96058c636"
            }
          ]
        },
        {
          "id": "83cff149-0f8c-4995-9a0b-9e8b12e40ed2",
          "name": "postRestMethodFlickr.photosets.reorderphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.reorderPhotos?api_key=%7B%7D&photoset_id=%7B%7D&photo_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Update the order of photos in a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f174266-b4b8-406d-9f48-2a6cfc8e9075"
            }
          ]
        },
        {
          "id": "968cb036-e3d2-42db-bcaf-098ef2a574ae",
          "name": "postRestMethodFlickr.photosets.setprimaryphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.photosets.setPrimaryPhoto?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set photoset primary photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "623b782a-976d-4c1d-9623-8f9672bc75de"
            }
          ]
        },
        {
          "id": "ad006e59-d165-4bea-b75e-55b08099be88",
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
              "id": "0a8a81c0-4e39-4297-9c38-1ebc4e889dc4"
            }
          ]
        },
        {
          "id": "31befde4-fedb-4d35-9f18-1f1ebbaa5445",
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
              "id": "752d4830-1f18-4ba7-adf7-d7f86051a94d"
            }
          ]
        },
        {
          "id": "23c51063-90fc-4eab-b622-056aecaef813",
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
              "id": "7fd141f7-6cc2-4d5b-8f26-e4874ca596c4"
            }
          ]
        },
        {
          "id": "b4f8823b-b315-49b6-83ce-69614c5cb3af",
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
              "id": "361f0630-32fe-4980-8e99-ee329bf8cebb"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "ecbb4c5c-93dc-4506-8a06-1dcd16b399cc",
          "name": "getRestMethodFlickr.places.find",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.find?api_key=%7B%7D&format=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of place IDs for a query string."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "675832db-4ef1-4dff-9f22-b85724ebb5b3"
            }
          ]
        },
        {
          "id": "d7f2bb0f-3c44-4299-8562-09fc2564b438",
          "name": "getRestMethodFlickr.places.findbylatlon",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.findByLatLon?accuracy=%7B%7D&api_key=%7B%7D&format=%7B%7D&lat=%7B%7D&lon=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a place ID for a latitude, longitude and accuracy triple."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "892fbbce-906e-46d0-a8e2-aac208c7d9e5"
            }
          ]
        },
        {
          "id": "679997d6-e62a-49a9-9534-377f3c2ad23a",
          "name": "getRestMethodFlickr.places.getchildrenwithphotospublic",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getChildrenWithPhotosPublic?api_key=%7B%7D&format=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of locations with public photos that are parented by a Where on Earth (WOE) or Places ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f1c127b-cbeb-4b42-bb65-d044da214d84"
            }
          ]
        },
        {
          "id": "d1aab04b-d2f8-4250-82c3-b539a9b6dfcb",
          "name": "getRestMethodFlickr.places.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getInfo?api_key=%7B%7D&format=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a place."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4d77a3d-c214-442d-af0f-314efff553b7"
            }
          ]
        },
        {
          "id": "a3ddecff-cb53-426a-ae02-8bf8c5fd60cf",
          "name": "getRestMethodFlickr.places.getinfobyurl",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getInfoByUrl?api_key=%7B%7D&format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lookup information about a place, by its flickr.com/places URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c747c9cf-d94b-4d9e-a2d5-fcf7a151d622"
            }
          ]
        },
        {
          "id": "650c6bf7-f04c-4fdc-ba5f-9645685f270a",
          "name": "getRestMethodFlickr.places.getplacetypes",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getPlaceTypes?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a list of available place types for Flickr."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db7eba2e-83e3-4c65-a0e6-f02b025dcc3b"
            }
          ]
        },
        {
          "id": "b85ac167-da78-4f5d-a071-b0af7ad49982",
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
              "id": "aed6e161-e769-44c2-8367-0f83cb3286a2"
            }
          ]
        },
        {
          "id": "9dfbe0d0-b430-4a1c-b44f-c683b9a2155b",
          "name": "getRestMethodFlickr.places.gettopplaceslist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.getTopPlacesList?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&place_id=%7B%7D&place_type_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the top 100 most geotagged places for a day."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b26b0e3-91b3-48bc-9ddc-128871e42ad2"
            }
          ]
        },
        {
          "id": "948d0366-cf5d-4124-8121-1c81c90f2895",
          "name": "getRestMethodFlickr.places.placesforboundingbox",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.placesForBoundingBox?api_key=%7B%7D&bbox=%7B%7D&format=%7B%7D&place_type=%7B%7D&place_type_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return all the locations of a matching place type for a bounding box."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edd1e701-e508-498c-a3f2-ca81b8305142"
            }
          ]
        },
        {
          "id": "a7830132-955a-439d-b55a-e851ceb3ff0d",
          "name": "getRestMethodFlickr.places.placesforcontacts",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.placesForContacts?api_key=%7B%7D&contacts=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&place_id=%7B%7D&place_type=%7B%7D&place_type_id=%7B%7D&threshold=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of the top 100 unique places clustered by a given placetype for a user's contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d6e0848-8239-46b9-b2db-ab57ba8121e6"
            }
          ]
        },
        {
          "id": "421184e9-75c6-4b22-8bc4-6eef18390474",
          "name": "getRestMethodFlickr.places.placesfortags",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.placesForTags?api_key=%7B%7D&format=%7B%7D&machine_tags=%7B%7D&machine_tag_mode=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&place_id=%7B%7D&place_type_id=%7B%7D&tags=%7B%7D&tag_mode=%7B%7D&threshold=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of the top 100 unique places clustered by a given placetype for set of tags or machine tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2f11332-cf34-412d-80c8-f5403a72fb10"
            }
          ]
        },
        {
          "id": "07c836ae-4fad-4834-89d0-a8c34decd442",
          "name": "getRestMethodFlickr.places.placesforuser",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.placesForUser?api_key=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&place_id=%7B%7D&place_type=%7B%7D&place_type_id=%7B%7D&threshold=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of the top 100 unique places clustered by a given placetype for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5f74f33-8943-4c04-a8fa-a14615d0a075"
            }
          ]
        },
        {
          "id": "4db4101d-b810-435e-a721-d3a7e9ef5c23",
          "name": "getRestMethodFlickr.places.resolveplace",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.resolvePlaceId?api_key=%7B%7D&format=%7B%7D&place_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find Flickr Places information by Place ID. This method has been deprecated. It won't be removed but you should use flickr.places.getInfo instead."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d4cbdd8-01ca-4385-9d2b-5b3c880706d2"
            }
          ]
        },
        {
          "id": "ab63fbf2-c5b5-41ae-aac5-9c025a92a5d8",
          "name": "getRestMethodFlickr.places.resolveplaceurl",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.resolvePlaceURL?api_key=%7B%7D&format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find Flickr Places information by Place URL. This method has been deprecated. It won't be removed but you should use flickr.places.getInfo instead."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79926664-0db5-4063-8670-be0e1a8d4505"
            }
          ]
        },
        {
          "id": "3d1666c1-1069-4dd0-bd09-b785a1855bd6",
          "name": "getRestMethodFlickr.places.tagsforplace",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.places.tagsForPlace?api_key=%7B%7D&format=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&place_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of the top 100 unique tags for a Flickr Places or Where on Earth (WOE) ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4177b6c2-bb97-48cc-8dee-fd971e7454a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Prefs",
      "item": [
        {
          "id": "467f1534-94d2-429d-8c55-1cd1d15132dc",
          "name": "getRestMethodFlickr.prefs.getcontenttype",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getContentType?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default content type preference for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce4424a4-1af2-45e2-aff3-28597984a840"
            }
          ]
        },
        {
          "id": "84b3e27f-f6b8-4239-98b7-96502def1b45",
          "name": "getRestMethodFlickr.prefs.getgeoperms",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getGeoPerms?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default privacy level for geographic information attached to the user's photos and whether or not the user has chosen to use geo-related EXIF information to automatically geotag their photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ede72790-1928-46b3-901a-5f0674698947"
            }
          ]
        },
        {
          "id": "9a881d62-c430-401e-9300-cb556d20a850",
          "name": "getRestMethodFlickr.prefs.gethden",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getHidden?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default hidden preference for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a58d227f-1e28-4bc4-9ac5-4a9c9ee8fc3f"
            }
          ]
        },
        {
          "id": "f0d4cbd1-4a2b-4895-af19-0b6201c01cd9",
          "name": "getRestMethodFlickr.prefs.getprivacy",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getPrivacy?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default privacy level preference for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b621053-6973-4a14-bc7c-ec4f88de5b09"
            }
          ]
        },
        {
          "id": "6f362c97-de55-4601-9449-9c7c27ee729f",
          "name": "getRestMethodFlickr.prefs.getsafetylevel",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.prefs.getSafetyLevel?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default safety level preference for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2cdbb13-b789-4ccb-9571-d1e3a63564d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Reflection",
      "item": [
        {
          "id": "efc521c0-d486-4d34-ae8a-a7a4089f5fca",
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
              "id": "4fd4c2af-25a7-49ff-8ada-0eb29bcd9e4e"
            }
          ]
        },
        {
          "id": "3f32196e-3eeb-456c-8688-37007ea58ef4",
          "name": "getRestMethodFlickr.reflection.getmethods",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.reflection.getMethods?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of available Flickr API methods."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29dc74a0-29fa-4c25-bed1-5e77e30ecf57"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "5cab738e-ad64-41e6-804a-017a97fbaa0e",
          "name": "getRestMethodFlickr.stats.getcollectiondomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionDomains?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a collection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "396718b9-d9a5-4fc1-a7ac-cdc0cc95087e"
            }
          ]
        },
        {
          "id": "10ca9fa7-22be-458f-822d-f91e5a22af2d",
          "name": "getRestMethodFlickr.stats.getcollectionreferrers",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionReferrers?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&domain=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referrers from a given domain to a collection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34a75d52-08c7-4f4d-b672-a6a530bdeb22"
            }
          ]
        },
        {
          "id": "e0ed0a5d-0af0-40b4-845c-b2b004b3a31c",
          "name": "getRestMethodFlickr.stats.getcollectionstats",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionStats?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the number of views on a collection for a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bc3eda0-ac74-4603-81cb-83601cda594d"
            }
          ]
        },
        {
          "id": "0a809b2b-6e64-4ee3-bd69-00cf6489b971",
          "name": "getRestMethodFlickr.stats.getphotodomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotoDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dd3e5d0-e7c0-49d5-bdc2-d349f2d49d4d"
            }
          ]
        },
        {
          "id": "d283c716-dd06-45ea-9c04-93a16e7f97d1",
          "name": "getRestMethodFlickr.stats.getphotoreferrers",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotoReferrers?api_key=%7B%7D&domain=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bb9b3a4-b9be-4ec3-8eb9-dd3a85a7f0b7"
            }
          ]
        },
        {
          "id": "1bbf72e8-9336-47ef-a986-5616bbe21c9f",
          "name": "getRestMethodFlickr.stats.getphotostats",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotoStats?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the number of views, comments and favorites on a photo for a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fc04bef-05e5-45ab-b2ba-c11344d9eb1b"
            }
          ]
        },
        {
          "id": "2e7a79e4-57d4-49e7-9871-2287a7bc23d7",
          "name": "getRestMethodFlickr.stats.getphotosetdomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotosetDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f00fa9a8-9161-4a02-8af8-f049dbd46885"
            }
          ]
        },
        {
          "id": "0e4be576-c57d-4638-a0ac-d51ee486c0fe",
          "name": "getRestMethodFlickr.stats.getphotosetreferrers",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotosetReferrers?api_key=%7B%7D&domain=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photoset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f01c78e9-2509-4e6d-8eef-aa04ed492d71"
            }
          ]
        },
        {
          "id": "b82ad684-f54a-4cd6-b8be-80c5ce8346ae",
          "name": "getRestMethodFlickr.stats.getphotosetstats",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotosetStats?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the number of views on a photoset for a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c86a61bd-abc8-4eae-9b1b-6108bb8075d0"
            }
          ]
        },
        {
          "id": "2a82590f-d773-437c-94ab-5565facc795f",
          "name": "getRestMethodFlickr.stats.getphotostreamdomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotostreamDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photostream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68ea405d-05cf-4508-ad49-519e8feba5bf"
            }
          ]
        },
        {
          "id": "34ba32c3-a3d3-486d-8ce9-bc9cfb419b24",
          "name": "getRestMethodFlickr.stats.getphotostreamreferrers",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotostreamReferrers?api_key=%7B%7D&domain=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referrers from a given domain to a user's photostream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dbc25ba-d640-4dce-9d6c-e0dc637b1a8e"
            }
          ]
        },
        {
          "id": "5b5054c1-cbcb-49fd-a2d0-093bad4f05ac",
          "name": "getRestMethodFlickr.stats.getphotostreamstats",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotostreamStats?api_key=%7B%7D&date=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the number of views on a user's photostream for a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3da7e4d8-7847-4a92-832b-f92b152c9f0b"
            }
          ]
        },
        {
          "id": "f7b2dcc8-2c94-4a33-bc47-ad94aedfa930",
          "name": "getRestMethodFlickr.stats.getpopularphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPopularPhotos?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the photos with the most views, comments or favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "241677f8-88be-4e3b-9332-00227d5735e4"
            }
          ]
        },
        {
          "id": "304375dd-fef2-4c6b-b833-3597f89fa09c",
          "name": "getRestMethodFlickr.stats.gettotalviews",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getTotalViews?api_key=%7B%7D&date=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the overall view counts for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ab30de4-eaea-401c-a46f-42b41b037af8"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "6c172253-b995-47bd-8fd9-d41516f41db2",
          "name": "getRestMethodFlickr.tags.getclusterphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getClusterPhotos?api_key=%7B%7D&cluster_id=%7B%7D&format=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the first 24 photos for a given tag cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fd60d90-bc9f-4150-adeb-618a88b9a206"
            }
          ]
        },
        {
          "id": "8ba779bf-5c40-48d7-994e-1ac760630c90",
          "name": "getRestMethodFlickr.tags.getclusters",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getClusters?api_key=%7B%7D&format=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tag clusters for the given tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f441a9d9-a380-47fd-bfb5-383cba0d90f7"
            }
          ]
        },
        {
          "id": "28e0d697-ec2f-45e1-b127-f58d9798ca52",
          "name": "getRestMethodFlickr.tags.gethotlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getHotList?api_key=%7B%7D&count=%7B%7D&format=%7B%7D&period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of hot tags for the given period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c77f3e3-f134-480f-8a14-366a1ceb9d4a"
            }
          ]
        },
        {
          "id": "a7f46420-d509-4210-8a78-47d8cd9ad806",
          "name": "getRestMethodFlickr.tags.getlistphoto",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getListPhoto?api_key=%7B%7D&format=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the tag list for a given photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "040458b3-926a-4841-9dd9-f0c904cd9e16"
            }
          ]
        },
        {
          "id": "3ea2a84f-f2cc-43a9-b3d0-f4c0a12532f7",
          "name": "getRestMethodFlickr.tags.getlistuser",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getListUser?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the tag list for a given user (or the currently logged in user)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "638969f2-c217-4281-909a-c3bcdf48f589"
            }
          ]
        },
        {
          "id": "bba7f9ab-7ffd-4bfc-b4f2-8b3de89808e1",
          "name": "getRestMethodFlickr.tags.getlistuserpopular",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getListUserPopular?api_key=%7B%7D&count=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the popular tags for a given user (or the currently logged in user)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dc22497-0e48-4609-adc1-36bb16bec75c"
            }
          ]
        },
        {
          "id": "0bcf2c31-6dcf-455c-bd1e-69b83eec0d92",
          "name": "getRestMethodFlickr.tags.getlistuserraw",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getListUserRaw?api_key=%7B%7D&format=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the raw versions of a given tag (or all tags) for the currently logged-in user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23f63ea9-be8b-4214-ba8d-b13df61cf558"
            }
          ]
        },
        {
          "id": "0456476b-11d3-4a2d-82e6-f336bc8d23de",
          "name": "getRestMethodFlickr.tags.getrelated",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.tags.getRelated?api_key=%7B%7D&format=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tags 'related' to the given tag, based on clustered usage analysis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cc2df07-30bf-4a69-b532-cd43d7da2603"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "a04f6bc7-54a1-4e1e-92cb-e899fe1533f8",
          "name": "getRestMethodFlickr.test.echo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.test.echo?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A testing method which echoes all parameters back in the response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4ec3784-cf69-4cdd-808c-8e8194852fd3"
            }
          ]
        },
        {
          "id": "c6b7ca7b-cb55-4f41-8ac5-9628a53bbe39",
          "name": "getRestMethodFlickr.test.login",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.test.login?api_key=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A testing method which checks if the caller is logged in then returns their username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51b35245-544f-40e7-804f-2fb186b15820"
            }
          ]
        },
        {
          "id": "d4f17cd7-18fc-451b-bea8-a57e86ac5735",
          "name": "getRestMethodFlickr.test.null",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.test.null?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method doesn't do anything."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6eddd2c-ca64-45c4-981b-246a624b5f6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Urls",
      "item": [
        {
          "id": "3dd44596-f25e-4501-aa4f-e05805f4d9aa",
          "name": "getRestMethodFlickr.urls.getgroup",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.getGroup?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the url to a group's page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68a62959-e8ee-4b13-ba7c-a1994d41c1a3"
            }
          ]
        },
        {
          "id": "1a9bd2e4-9330-4c78-ad12-4e9ddb61558e",
          "name": "getRestMethodFlickr.urls.getuserphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.getUserPhotos?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the url to a user's photos."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59efeed1-2366-4a9c-add6-4e7704a73cc4"
            }
          ]
        },
        {
          "id": "115439ab-2058-4db9-b466-89bd145607a0",
          "name": "getRestMethodFlickr.urls.getuserprofile",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.getUserProfile?api_key=%7B%7D&format=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the url to a user's profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "401ea6e7-d4d6-4c34-a77e-3c9b60f1bba8"
            }
          ]
        },
        {
          "id": "7c632fd0-c617-4b36-a7a0-81fe69211d57",
          "name": "getRestMethodFlickr.urls.lookupgallery",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.lookupGallery?api_key=%7B%7D&format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns gallery info, by url."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43b68481-13bd-4f4f-bfe3-8bf392d5da47"
            }
          ]
        },
        {
          "id": "693240f6-a414-4b2b-9ed7-5907b146e468",
          "name": "getRestMethodFlickr.urls.lookupgroup",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.lookupGroup?api_key=%7B%7D&format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a group NSID, given the url to a group's page or photo pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc8d4335-e96f-4b31-8ce4-c563e1c87b86"
            }
          ]
        }
      ]
    }
  ]
}