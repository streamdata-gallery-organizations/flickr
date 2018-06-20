{
  "info": {
    "name": "Flickr Places Get Top Places List",
    "_postman_id": "c8b70fb5-8ce3-41a1-827b-93bd2fdf575a",
    "description": "Return the top 100 most geotagged places for a day.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "7181d272-cae1-4e24-8128-e57274a079d0",
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
              "id": "94941873-b629-473e-9e3b-c358c4868c40"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "b0d2a4bc-5503-49dc-a33f-af4710f9990b",
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
              "id": "d466c92c-febe-49d1-96ae-e3158ad2a133"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "ffd521a1-08fa-487e-b65f-aadb494508bf",
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
              "id": "f30822c8-9e5f-48d5-a088-7b03781fa4f7"
            }
          ]
        },
        {
          "id": "975ae772-654a-49ab-ac4a-b3260fa4d069",
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
              "id": "cb7a5c4e-4c5c-4ecb-9800-e6b133fbbdab"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "addbde27-aaa0-468b-9a61-db46c32ed9a4",
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
              "id": "3bc0d417-989c-419e-87a2-4ebaf1c2d5cb"
            }
          ]
        },
        {
          "id": "8edded7e-07d9-43eb-bb89-9a4bf62b1cfc",
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
              "id": "17ce2255-ce3f-4121-857a-7739db201f36"
            }
          ]
        },
        {
          "id": "ba3b8831-6da3-42e8-846b-df84e3d0fe70",
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
              "id": "811d576d-4745-4e95-a2ee-f3b6331cd063"
            }
          ]
        },
        {
          "id": "25565ae7-9827-4009-9745-c628a9511039",
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
              "id": "0279e50e-fc87-4b17-bc9a-f55abac231e9"
            }
          ]
        },
        {
          "id": "5e9e0b8d-eba7-4c77-a97e-cd3254f86013",
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
              "id": "c09cb8d9-7b91-480a-b0a5-7f9caedf7e5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "a0e8c3e4-8848-459e-8b0b-3691cdf25060",
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
              "id": "1d83028f-ea96-4694-94bb-cd626eae1f48"
            }
          ]
        },
        {
          "id": "810bd084-8c00-4dc9-a8b2-c66ca8f95fe8",
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
              "id": "d942dba3-c522-4b1b-b348-8de916f8259e"
            }
          ]
        },
        {
          "id": "10116ba7-77ce-48c7-8236-ad75a6f689bf",
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
              "id": "d5cf5650-1553-4317-888a-d71e5ed1c999"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "a4d9ff9d-5019-4d50-b8e6-ae180b2f90be",
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
              "id": "03451c4d-cad8-4c1e-80e4-c60aebbf6b3b"
            }
          ]
        },
        {
          "id": "07f2a371-2656-47da-acb7-1e86e6f88be5",
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
              "id": "c6dd25d1-543d-4c6e-813e-f71713b8a5ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "eddd4fee-f9c0-473f-a569-7ae367d2130b",
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
              "id": "ef49e4f8-b0d6-4bfd-b37c-c1036f10d360"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "dfe5697d-5f30-45b0-a76c-7b7c972b4437",
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
              "id": "d1788501-a031-4d13-a149-e792aaf74332"
            }
          ]
        },
        {
          "id": "ff0d097f-1d1b-42ac-a622-678610a0b001",
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
              "id": "841feca0-f731-4740-87da-f23a4570e35f"
            }
          ]
        },
        {
          "id": "98632407-c986-4633-82ba-cb4e770a9a2f",
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
              "id": "5a63d147-f625-4439-a118-d368781e182b"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "88f4eaab-e507-4cd1-95c3-9fc1288a6bff",
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
              "id": "cff18397-2eec-48bd-83b2-5eb723c329f3"
            }
          ]
        },
        {
          "id": "20b52603-115a-4b23-b94f-10566cd87994",
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
              "id": "105be9be-af54-4883-b492-b6a86f563faf"
            }
          ]
        },
        {
          "id": "c42bf339-af62-446b-b29a-15e50beb4385",
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
              "id": "4b0ff7c4-a295-42d5-8fb9-650a7bbb0e74"
            }
          ]
        },
        {
          "id": "a77dd222-87dc-4c72-ad1d-600edc404ae0",
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
              "id": "e85decfe-68dd-4c66-bdbe-d155b79b2a3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "4e4590b8-00c2-4455-b40f-e467f0d667df",
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
              "id": "b38735c2-7d56-4fc7-bcc7-436e3a9e084e"
            }
          ]
        },
        {
          "id": "f1314d80-1aaf-4939-a787-1c4850937125",
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
              "id": "77a0fe68-b784-46c5-9bd7-d25c73ffcbc5"
            }
          ]
        },
        {
          "id": "e2848b26-a17a-40a9-9be0-1c235bba2a24",
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
              "id": "1fd4e447-74a7-4d76-955d-a7211554eeff"
            }
          ]
        },
        {
          "id": "37305e1e-425e-4c98-842a-afab49d120d2",
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
              "id": "e70abc76-39a3-4e78-9c19-d25da780be59"
            }
          ]
        },
        {
          "id": "189df6d4-8788-44f2-8ac6-7b17ea8571ed",
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
              "id": "c7035894-1ca7-48c8-a284-a0239d6914bd"
            }
          ]
        },
        {
          "id": "4998744a-5fa0-42d2-8a07-2c679c7dc6f3",
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
              "id": "ea496d9c-5f3e-4578-b32d-362e0e87f1a1"
            }
          ]
        },
        {
          "id": "39eafc76-1483-41cf-9f83-5fbee04dfe1a",
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
              "id": "906d1490-e915-4696-832e-bc86db073b42"
            }
          ]
        },
        {
          "id": "d0829247-140e-4793-a9d5-918290d11747",
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
              "id": "04a2ccc6-1577-40a5-a098-a50018179f31"
            }
          ]
        },
        {
          "id": "e7a0b4b7-391e-45f0-965f-b10b00e15a09",
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
              "id": "20e11699-09d6-4990-87e8-c61269c15d48"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "5e231e87-5b36-4168-8d29-2befeeeb74de",
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
              "id": "bd102ca9-56c1-4b31-b4e9-b2e096af6da9"
            }
          ]
        },
        {
          "id": "95dc273b-93a2-4786-9b7b-bf9d576d43fa",
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
              "id": "e9f98087-2d46-42d6-8214-6aa510553025"
            }
          ]
        },
        {
          "id": "2506a38e-c930-4322-bb4f-eb3c3ee4784f",
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
              "id": "3a9912a7-4c96-4b72-8098-cd84350170a8"
            }
          ]
        },
        {
          "id": "0c28ac4b-f048-4fc9-a895-a367e5f7177f",
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
              "id": "78fe6fb8-1a4c-4044-b54c-43c53b638fb1"
            }
          ]
        },
        {
          "id": "93d61d4b-8a13-4ead-aef7-5be550eb6402",
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
              "id": "cc709618-766a-4de7-a827-0ab0ebe8085c"
            }
          ]
        },
        {
          "id": "c948d54a-93e9-4c11-82bc-3601853ac888",
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
              "id": "d8ad3530-9635-4cc0-a5c1-8a6c85a9cfc7"
            }
          ]
        },
        {
          "id": "199126eb-a45d-4080-8f25-3c0b38c121dd",
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
              "id": "0d88a235-eb58-4260-b75b-bdfcb84f226f"
            }
          ]
        },
        {
          "id": "6863b666-0352-4c7e-8d5a-2c9e4acc668a",
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
              "id": "9637a52d-3f18-44f0-a40a-8f0c050079f8"
            }
          ]
        },
        {
          "id": "bdbcef53-9abd-4afa-8102-e3e4429aeefc",
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
              "id": "0546b9e2-b0f8-4d1f-912a-2302f9128f47"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "e270197b-0ce7-433b-acd7-38ca61f9a891",
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
              "id": "82c466c7-86f5-4266-a905-db3702041d32"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "0658ef90-e504-42ff-a808-c439cb7d8e89",
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
              "id": "56f9daae-a986-4f4b-bdc0-99bd5ae1ca0b"
            }
          ]
        },
        {
          "id": "1c303b91-860e-4c67-b2ce-955ad21c25e4",
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
              "id": "80630157-2fa0-41b8-b44e-b1feaa5ee752"
            }
          ]
        },
        {
          "id": "a4c0ac79-2959-42d6-94a0-0f41711fcde4",
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
              "id": "2f208163-6adb-4674-9d6a-3d356a0d7596"
            }
          ]
        },
        {
          "id": "67fa4823-5028-426c-9e27-a1ae5724b0b5",
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
              "id": "420245ba-1e30-4985-986f-fe5c72d88f6d"
            }
          ]
        },
        {
          "id": "c5cfab47-1bbb-4403-8ce3-dedf6a8e03d2",
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
              "id": "a7f773de-8111-426b-b872-7c569befa468"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "4a9ebd45-f2fd-45c8-b711-a89d596447ca",
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
              "id": "ae87f851-aa29-44d0-9fa0-93175972b64c"
            }
          ]
        },
        {
          "id": "906215e7-828c-4149-8e6d-0ba5e10b05fd",
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
              "id": "ee3dc51c-48e7-45fa-9e96-973d7b67d94f"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "31878dce-f85f-4908-9723-23e7bdbb690e",
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
              "id": "d6284af9-1604-42d1-87b3-9ee85062c3b6"
            }
          ]
        },
        {
          "id": "77255d7d-5b21-46b1-99a5-53697296f03d",
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
              "id": "dfb51996-b81b-49ec-a6fd-10a071844ef7"
            }
          ]
        },
        {
          "id": "7d8a57a9-3b21-4215-ab51-ffa8ff67d413",
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
              "id": "62a1baa2-9193-4222-8fba-b438d9b8cacf"
            }
          ]
        },
        {
          "id": "75bbcf40-815e-4f7a-bdc3-5a05d697653d",
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
              "id": "41d403b8-3641-4909-98ac-53fa39ed118f"
            }
          ]
        },
        {
          "id": "28b739e0-a122-485b-92ab-9ed82db4a178",
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
              "id": "284c10db-0fd7-4f5c-8183-839294a37922"
            }
          ]
        },
        {
          "id": "53917444-d8be-4419-9883-3041a518df03",
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
              "id": "512dfcc8-ed41-47dd-8ae7-28d3fe90e8d3"
            }
          ]
        },
        {
          "id": "18b30d46-e664-4627-8cf5-97b07483f933",
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
              "id": "493eda6b-98f7-41c3-bb53-58f328322046"
            }
          ]
        },
        {
          "id": "a367c749-c208-4f13-aff0-0b4bc24218e7",
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
              "id": "9a6014cb-ed93-46a9-867e-a727bb6d2d5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "ae862462-2479-419d-a2a0-31b43aa074ed",
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
              "id": "5235c9b5-1948-42fc-b8d5-839a0eeb11d0"
            }
          ]
        },
        {
          "id": "9ccd4d8d-0e2a-4b7e-b1a1-49b7a4c8f6f8",
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
              "id": "8c1f8eba-1676-47b0-a224-a0af8de26f11"
            }
          ]
        },
        {
          "id": "04025a90-b3b6-42f4-92e2-d735d0cb01ff",
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
              "id": "fc801696-6254-46e4-b7de-09e2bf39a81c"
            }
          ]
        },
        {
          "id": "22b41994-ddad-46e7-9b03-bba72979e143",
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
              "id": "cf332797-dadf-47ca-aa04-62588e7192e3"
            }
          ]
        },
        {
          "id": "4d596e11-7331-4a62-a1bd-73237dd15f12",
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
              "id": "28222989-0835-4bfb-883a-c8210fd1342a"
            }
          ]
        },
        {
          "id": "9a659c9d-7d4e-4ba9-af3b-3c84152f4101",
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
              "id": "cbddf094-bf48-4356-b4ff-33e1b5ddea20"
            }
          ]
        },
        {
          "id": "a4c73150-33c1-44ae-9d0b-5bc79e61f72b",
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
              "id": "57de762e-91e9-4445-8ebe-72fc16c8e55f"
            }
          ]
        },
        {
          "id": "dc854887-f32f-406e-aefa-ffa436661892",
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
              "id": "6d1b73bd-be75-44bb-874d-4e91a0a8408a"
            }
          ]
        },
        {
          "id": "7b8a95ad-fd21-47df-b3dd-0ff0d844d80f",
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
              "id": "8b05040b-e875-4f27-a323-76bd533eb34e"
            }
          ]
        },
        {
          "id": "978afae3-a04f-4149-925d-53d769521ab0",
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
              "id": "42f4c331-e88c-4338-b797-0859a49bce4c"
            }
          ]
        },
        {
          "id": "528ea174-5b73-4c79-87d1-efce4331d0e8",
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
              "id": "6c8066bc-e2a5-4a68-8b91-aa1f85eced48"
            }
          ]
        },
        {
          "id": "2d77c283-e429-4550-b332-72f813f445f9",
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
              "id": "6524fc3f-7cb1-4cff-bddc-8696eeb1df7a"
            }
          ]
        },
        {
          "id": "d7030777-4207-43a6-9781-16e3c14e9d11",
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
              "id": "f69fa8fe-c4f8-4260-9e40-af2f0154b571"
            }
          ]
        },
        {
          "id": "4ed11670-78dd-4c83-8a3b-3fbd3ebaee5a",
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
              "id": "745c17b4-d8ce-4ee6-b00d-35f2ff822421"
            }
          ]
        },
        {
          "id": "0646ddb8-5af8-4b34-a952-0a9a7c044a93",
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
              "id": "f6e704ea-ef41-44cc-80bc-560fefcf78dd"
            }
          ]
        },
        {
          "id": "b9501499-86fa-48fc-9742-5f7668e372b0",
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
              "id": "5ba7f41d-e2f0-4d35-b9d5-0eb2688be36e"
            }
          ]
        },
        {
          "id": "5a3a9510-ef5f-4d6a-9b71-c5fce5f254b0",
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
              "id": "c640d4a3-5975-403c-bcc3-9acb7f597de5"
            }
          ]
        },
        {
          "id": "3a2ae61c-0769-4844-865f-29d3d8d8a504",
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
              "id": "38719c72-b6ec-4be6-9861-400e0af8fa0e"
            }
          ]
        },
        {
          "id": "d810b424-dd94-4a66-8b99-4dce8b7ef6cc",
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
              "id": "f9de55c0-2fcb-4444-9800-45392fc6cc50"
            }
          ]
        },
        {
          "id": "fc3ff1e0-4e9e-4747-b745-dc9e625b17be",
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
              "id": "7ee5f47e-f925-43d3-959b-0e2363fcdf5e"
            }
          ]
        },
        {
          "id": "91b14caa-7368-4402-867a-bb66cc187357",
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
              "id": "c5904bd1-c6fd-4263-9c5e-93fec9bf7ac2"
            }
          ]
        },
        {
          "id": "5825dfab-21ab-4798-b1e5-735126c2f86e",
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
              "id": "fdfd0eec-aedb-4b5b-9370-a292b4ba3e92"
            }
          ]
        },
        {
          "id": "9d2009ee-f5a3-4dea-b43a-3d7ca247910f",
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
              "id": "6431b5d6-a6d7-4a05-bace-43b3af08e2c7"
            }
          ]
        },
        {
          "id": "a76a785a-af62-4d8d-a5aa-599d81d7faec",
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
              "id": "e3b7055f-f595-4579-a2a4-4e10ffe6c733"
            }
          ]
        },
        {
          "id": "aec812a6-8973-413a-9253-d250c9eeeb37",
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
              "id": "9c79e060-c9fd-459b-9dee-a07da5fb382a"
            }
          ]
        },
        {
          "id": "c6c5ecf2-ee61-4dd6-8868-91cec1869e4f",
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
              "id": "087717b5-e98e-4fe1-9e93-3e6b8d3c99f6"
            }
          ]
        },
        {
          "id": "1f797461-c5aa-4fea-9193-27fd9ea000ce",
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
              "id": "2587aeb4-2366-4a04-a27a-4a5df3472f7b"
            }
          ]
        },
        {
          "id": "1521c9e9-0140-4d0e-8016-348b497d6590",
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
              "id": "d4b9dfd6-ec61-4e3a-9c4b-fed80009abf1"
            }
          ]
        },
        {
          "id": "299903f5-fa4c-4606-a581-9408f95fa647",
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
              "id": "28301bbf-739d-4cb6-8591-0805dd43f144"
            }
          ]
        },
        {
          "id": "346fc41d-3ae3-4bc6-9f1d-7dc733f6ddf9",
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
              "id": "ffeb11ac-ebe0-4cf3-9ba4-338e7b111117"
            }
          ]
        },
        {
          "id": "9c90925b-a33d-4df6-98cd-e72b76ead80f",
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
              "id": "f520f575-77c0-4ec0-a285-c6d93c920174"
            }
          ]
        },
        {
          "id": "fbe6f789-bf67-4362-af94-ae2fd470e570",
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
              "id": "57166518-0e11-428f-9856-ea00bb2db094"
            }
          ]
        },
        {
          "id": "6e9698d0-2685-41ea-bd07-08299b945184",
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
              "id": "d37ddcb2-422c-407d-b7b4-60598da8e399"
            }
          ]
        },
        {
          "id": "31d3088b-50ac-41a6-a918-bb724bbc1d9e",
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
              "id": "c751a177-c41d-4184-9eff-ada2cb113dce"
            }
          ]
        },
        {
          "id": "8c537a1b-1a7b-4a82-bf6d-7f0465aa26c4",
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
              "id": "0bd0f4d8-19a8-4f10-ad7e-320c029d5c88"
            }
          ]
        },
        {
          "id": "4a2da536-cc97-4b55-b70e-dd4df6e98f0f",
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
              "id": "e5aa930b-8375-422d-bb44-94f0bcecfe58"
            }
          ]
        },
        {
          "id": "83fb03c4-fb10-4568-aee2-fe86082670af",
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
              "id": "be09bd95-83db-4b3d-9673-b245497a4e38"
            }
          ]
        },
        {
          "id": "cbfebfe3-6012-4805-8961-101d6d26c1be",
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
              "id": "077c02e8-03cb-4152-b323-18be643919e1"
            }
          ]
        },
        {
          "id": "73e0c493-47c7-4f7a-88a6-239a1d688a20",
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
              "id": "1288e134-59ab-4676-b112-34dbd14942d8"
            }
          ]
        },
        {
          "id": "28587cfa-f3c6-4e48-b44c-5443662b28c1",
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
              "id": "2e85457a-f016-4e12-8155-01f8ae385751"
            }
          ]
        },
        {
          "id": "e89d2150-61a2-4f44-804d-3b41b6da66f6",
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
              "id": "2a0f715b-7251-4109-956a-68ab70afc244"
            }
          ]
        },
        {
          "id": "3560f55b-5bc3-48bc-b53f-ec3267e7ca03",
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
              "id": "a0d9f7fc-5167-439c-a2e5-06cdd48f52ed"
            }
          ]
        },
        {
          "id": "4d5f7a08-b21d-4635-96d7-9677d6fc8bd2",
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
              "id": "c5356a74-39ea-4e3d-964f-fbba07b0dbd0"
            }
          ]
        },
        {
          "id": "3b419939-a925-4eef-92f1-5df9429947c4",
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
              "id": "091f9d82-b41b-4643-847e-5170a8ebddda"
            }
          ]
        },
        {
          "id": "746f6f3e-993c-40e7-ac3b-2fe3e6645158",
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
              "id": "bb5f0ba8-b23d-4935-bf90-48d959cda752"
            }
          ]
        },
        {
          "id": "d1a85ff0-7560-44b0-a175-3b6f12ab322a",
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
              "id": "1481b25d-3134-4eff-95cc-f6cf31f983dc"
            }
          ]
        },
        {
          "id": "2220ce39-c03b-45b2-8229-a0cf5bec6539",
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
              "id": "3e4cab44-00d1-4974-9573-4a83a867a100"
            }
          ]
        },
        {
          "id": "d957a50d-b669-4db6-a878-912496c814cb",
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
              "id": "408e81b9-e004-4391-ac33-80f736c0c704"
            }
          ]
        },
        {
          "id": "41ba295d-5437-4a9a-98b1-4990d70decc9",
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
              "id": "f5c41d9c-7f36-481c-8746-ecfa9e9e3f8d"
            }
          ]
        },
        {
          "id": "e18989f7-2608-44e8-8d02-e0a0f03e0b8f",
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
              "id": "0be43250-dc3e-4bb2-ad9c-731cbdb460ce"
            }
          ]
        },
        {
          "id": "c5bcd9e2-b480-48b7-bb0c-732718dcd266",
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
              "id": "02753ddc-88d9-403c-9a23-19fa52d05f37"
            }
          ]
        },
        {
          "id": "4214bf56-17c5-44a1-8c3c-c04e4ebc2171",
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
              "id": "0869e3c0-4517-4f07-be05-48f4bb671ea8"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "726cb8af-22e3-47f4-8988-37aaa1f1aad6",
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
              "id": "b14dc98f-4c2e-40f1-8d19-4bf1ed06d2de"
            }
          ]
        },
        {
          "id": "10b93006-dac6-4bc8-a42b-0d9cad5d9f21",
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
              "id": "1fad869a-99c7-447e-b028-d19d2714f257"
            }
          ]
        },
        {
          "id": "dc71a576-ce30-436f-a8f1-804c686b2cec",
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
              "id": "d416d491-3c3f-4b5b-8229-af9872ad0b4c"
            }
          ]
        },
        {
          "id": "53a53c60-bb61-4572-ac5a-dc201d91f61c",
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
              "id": "a368764e-afaa-4e36-8dc1-c285f867d6cf"
            }
          ]
        },
        {
          "id": "d0dfff40-86bb-42c4-93c7-17cff1f01ca7",
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
              "id": "664decc9-0297-48ca-a841-558bf0ebbdd7"
            }
          ]
        },
        {
          "id": "24113861-450b-4b11-afde-f68097a1661f",
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
              "id": "ac01104c-a1f0-4e04-91cb-b9c2b7d15c0f"
            }
          ]
        },
        {
          "id": "de6a62e9-df55-43c1-b8ab-cd281ff3c540",
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
              "id": "cc31918b-db3e-41c4-8793-ce2ecf8a2bcd"
            }
          ]
        },
        {
          "id": "c8c20ca8-3361-457f-b7ec-67ffb6ac8f8b",
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
              "id": "4a969575-cb7f-43da-b466-bab926f30a3a"
            }
          ]
        },
        {
          "id": "6adca887-7483-46c1-bb64-3c58aff9b24a",
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
              "id": "a3118465-7928-4ff8-b530-c2445b2df7f6"
            }
          ]
        },
        {
          "id": "9fed0f08-4356-41b9-a644-e4d799cc5529",
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
              "id": "ce179a04-6f67-41f3-b22a-2521d86cade8"
            }
          ]
        },
        {
          "id": "9ea87525-3200-4b50-b03f-75c028546894",
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
              "id": "93eadbb2-69d4-4ced-8618-7e563c360edf"
            }
          ]
        },
        {
          "id": "adef609e-bb31-4aac-ae04-5506066babf1",
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
              "id": "4253ca7f-e9d3-45c0-aa51-727ff25303f3"
            }
          ]
        },
        {
          "id": "89c60c27-b2e2-4382-bf5d-d74e68aa31c3",
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
              "id": "3801b9c9-be8d-4bec-8404-5d6a3e210b73"
            }
          ]
        },
        {
          "id": "025190d1-858d-4955-b9f8-b7e71ef5c64d",
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
              "id": "20618d97-d5ca-4c77-8a88-809c17309900"
            }
          ]
        },
        {
          "id": "b147d3ec-5879-41f4-bd2e-cc58ab337188",
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
              "id": "043d0114-fe10-4759-81d1-283c04269e7f"
            }
          ]
        },
        {
          "id": "779b84fe-8ae7-4caf-a1fc-eb74b344b77c",
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
              "id": "9b22ca6b-48be-4687-a278-33826f7fdf4a"
            }
          ]
        },
        {
          "id": "a3d31e57-398a-474d-a6cf-b7feea71db05",
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
              "id": "8ebe7c9f-51f9-479a-8739-839ba493af63"
            }
          ]
        },
        {
          "id": "54ff7fa8-0844-4d71-813e-25448f03192e",
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
              "id": "d2a1d730-e61f-4d1b-acdb-2687282617e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "27213cb0-fb76-43e4-a62a-b3ee643af281",
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
              "id": "e7722d15-c1fd-4d15-94df-4ea80a4a93c6"
            }
          ]
        },
        {
          "id": "8c734bbf-517b-4774-8284-3ea4a939ad68",
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
              "id": "9035ea5a-4bf1-4ffe-ae8f-069ac6734aba"
            }
          ]
        },
        {
          "id": "5a33dae4-82e0-422d-a8cb-990bd9467abf",
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
              "id": "08ba260f-2171-4928-b7be-57943d5ff472"
            }
          ]
        },
        {
          "id": "e68e268a-413b-4eef-9586-12e181a25edc",
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
              "id": "7a5baee6-a607-49fb-96e5-bc4d37dec897"
            }
          ]
        },
        {
          "id": "4c1fdeab-4024-4001-9517-ffc5bba0e535",
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
              "id": "719c2d99-ce7d-4f4f-8e22-c6ac7a3207c1"
            }
          ]
        },
        {
          "id": "2d11a5d0-d774-4a36-ba67-06e5157dd7f8",
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
              "id": "16b634c5-52e8-49e7-9ba0-7e7408b63ecf"
            }
          ]
        },
        {
          "id": "76de34e2-a5d3-4c3c-8227-e54654040d5e",
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
              "id": "0d8e17be-5d78-460b-a01b-b1e39ff0eec0"
            }
          ]
        },
        {
          "id": "94121624-9e08-4188-9b69-ae44e4a381ff",
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
              "id": "aacb1a4d-9e5f-4881-92b7-0e9b8a67fb1f"
            }
          ]
        }
      ]
    }
  ]
}