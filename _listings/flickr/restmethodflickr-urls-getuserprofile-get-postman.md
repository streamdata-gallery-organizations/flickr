{
  "info": {
    "name": "Flickr Urls Get User Profile",
    "_postman_id": "6b69909b-c420-448d-8b70-3ded0bb19560",
    "description": "Returns the url to a user's profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "d7df3898-eae2-42fd-ae6d-36ace97b9f25",
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
              "id": "884012a3-d597-4ab8-8a96-5e8989928aee"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "0edafbf9-0c38-4294-b92e-eb715f8b879f",
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
              "id": "3a43cece-a255-443a-af18-24b65d47df62"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "acbc421d-5ab2-4348-9800-086097967256",
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
              "id": "03411fc4-ec8d-4c25-b7eb-0b4347137122"
            }
          ]
        },
        {
          "id": "b84082e9-27e4-4c99-bfbf-2794d3bb62d6",
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
              "id": "e55e982d-8fe5-46ba-b482-c8f452a7260d"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "c4ba63e9-32da-4079-ae25-c1617289ce9a",
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
              "id": "ed91da17-468b-436e-9b4c-17def4e94af7"
            }
          ]
        },
        {
          "id": "cc50175b-daed-4d9a-b156-24b90924fe3c",
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
              "id": "97befae3-dbe1-4eb9-af0e-eed1f077f9f6"
            }
          ]
        },
        {
          "id": "98ecf28c-3fd7-4fb4-bc4d-5508e62cd8db",
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
              "id": "6d359843-c058-4e7f-a412-0b57bd3fac2f"
            }
          ]
        },
        {
          "id": "63d300b6-599c-4cea-93f9-a33588c77aee",
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
              "id": "21be182f-45fc-4563-a99b-5499ec55c86a"
            }
          ]
        },
        {
          "id": "0578776e-7eab-4967-ab34-c1f8faad6a5f",
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
              "id": "0ad14ed6-b040-4d72-abaa-2d4c11d48fc6"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "789ba33d-ae61-4c88-9599-20a889e82d6e",
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
              "id": "bb852561-ed46-4ee8-8f1a-2f51075b3e11"
            }
          ]
        },
        {
          "id": "137f94b4-c34f-4ddc-b0d2-8bd853b6941b",
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
              "id": "376a74e7-0f26-4e34-ae2f-df2d344555a7"
            }
          ]
        },
        {
          "id": "79cc8a09-2aac-4363-932e-bdecf7606492",
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
              "id": "c19c99e1-958c-485d-a64a-6dd558b7959f"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "b160785e-291f-459c-8bac-b467153e7bc9",
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
              "id": "c38ae185-89c3-4c19-844e-81c14ff9f112"
            }
          ]
        },
        {
          "id": "fc1fb81e-6082-43dd-ad15-52aae3f68991",
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
              "id": "57738ffb-ec5b-459d-94d2-a806bc2b9bb4"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "39669a97-4940-4d3c-8ee2-5e47b16a145b",
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
              "id": "db655199-35cb-4ad8-811a-e0fc606d3a96"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "af40a8e8-ef80-4367-a452-bbe48b34207f",
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
              "id": "dac791e0-5d61-48cc-830a-191dbefd41c5"
            }
          ]
        },
        {
          "id": "ef9620b3-f685-4632-a83b-5067e63a1836",
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
              "id": "51223b4e-f85c-4ff9-88b7-46601ccbebae"
            }
          ]
        },
        {
          "id": "66dcda2d-e1aa-41d2-b4b7-461e5852cfb5",
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
              "id": "8fd8c101-f7ae-4cff-b6ab-e1fecc3c6e7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "5037068f-d080-45ce-bb51-ec75bea87e24",
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
              "id": "2b620e33-4ccc-4d4c-bffa-efc22114fe6c"
            }
          ]
        },
        {
          "id": "33ca3b5d-417a-4edf-a665-cdfe38edf7ae",
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
              "id": "cf08aad4-d2e1-4082-a3df-d992fc0109ef"
            }
          ]
        },
        {
          "id": "8971295a-4322-494e-84aa-e448f321869d",
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
              "id": "5cb2e241-52b1-4927-b078-1ee2162d721a"
            }
          ]
        },
        {
          "id": "b0b8acdf-1af7-4f5f-a14e-a6aa6bbd3751",
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
              "id": "a910b1ac-9cdc-4c80-8e53-373fd890d385"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "13dc64e3-b067-4da8-9237-2906146b0ac9",
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
              "id": "0728ca9e-93c1-45bd-a29f-0f7269329678"
            }
          ]
        },
        {
          "id": "2ce75eef-cced-45e6-bae0-193f656e5439",
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
              "id": "e9308fdf-451d-47d6-ae01-35d1ffd43663"
            }
          ]
        },
        {
          "id": "66049471-968d-4e0c-b3ba-c398519e4ee2",
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
              "id": "16518361-f45e-444c-8af6-9bdd42acf511"
            }
          ]
        },
        {
          "id": "4b0f068c-fa53-4e42-9d57-a1d327dac481",
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
              "id": "57a96268-8c00-49b9-a0ba-f30370d98c30"
            }
          ]
        },
        {
          "id": "c1e78eef-d936-4438-b2a7-fd8a58bfabbc",
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
              "id": "3d882137-95b5-46d6-950d-b721be72572e"
            }
          ]
        },
        {
          "id": "a52990a1-acfd-434f-ad8f-2961b57404b6",
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
              "id": "6bb4c6d8-9111-4d76-9440-3a656344bfef"
            }
          ]
        },
        {
          "id": "54e701c4-2dd2-4b9d-9a8d-15e63662eead",
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
              "id": "ccc4e6df-c3d0-4f44-aeb3-e9ac982624d2"
            }
          ]
        },
        {
          "id": "81411ff7-4443-4727-af0e-c6370ba54687",
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
              "id": "2b3e8647-2ba4-4fb5-8df3-9ea744cc260e"
            }
          ]
        },
        {
          "id": "337c44c8-cce9-4d41-9e21-589071ff70c5",
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
              "id": "4f837711-41ef-4fbd-862e-9d5ccc170b0f"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "5311ac87-85ba-4b56-a1c7-6771e5c97b2d",
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
              "id": "42371f79-caa1-48c6-a079-cf7126077f6d"
            }
          ]
        },
        {
          "id": "4fa69558-ddf4-4e81-ba4f-7548bdf535b6",
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
              "id": "8dc04f98-7efc-4df8-b17d-25545aadb4d5"
            }
          ]
        },
        {
          "id": "85ab6e79-2398-432a-92c0-33e8103b24a0",
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
              "id": "19165d4d-ccab-4da4-baf3-9415913fa16e"
            }
          ]
        },
        {
          "id": "bc3f21b8-a95c-4147-aa19-28b64285fca8",
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
              "id": "55f52706-aacf-4afc-9613-96a053ab3a8b"
            }
          ]
        },
        {
          "id": "3b091bc9-5592-4fb2-a39c-a60070b5554d",
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
              "id": "f39c4644-6a06-41c9-be04-7879528faa3a"
            }
          ]
        },
        {
          "id": "66604f3c-ccdf-4287-be46-db0368598894",
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
              "id": "cf901a8a-9061-4530-a885-b67180e9d244"
            }
          ]
        },
        {
          "id": "3fd26911-6e45-40c6-b3fb-d588fb0c119b",
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
              "id": "3942dcf7-3e03-4238-b512-503679cc7e20"
            }
          ]
        },
        {
          "id": "ce6e14e2-a0a9-4ac3-bc3e-b34a06723b81",
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
              "id": "4723f105-8832-434d-a625-16c0ca283481"
            }
          ]
        },
        {
          "id": "30b03e82-1c13-405f-a658-3073f5234d91",
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
              "id": "f913d234-97d4-44aa-b479-d0adf30d724e"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "915a3360-7efc-4dad-8756-6e3e8f879784",
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
              "id": "9b8b02ae-059c-4a7a-bbe9-ff06719e867b"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "eeac270e-53d1-4763-8fec-6e9801f5ddcd",
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
              "id": "32e3b363-af26-41db-8d59-42667237aaa6"
            }
          ]
        },
        {
          "id": "835d2ce3-ecef-40b7-82a8-114cad7af52a",
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
              "id": "196e7f5b-94f4-4f4b-97d2-ec384c670159"
            }
          ]
        },
        {
          "id": "bed14c78-a43e-488d-8d73-dafb5966457f",
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
              "id": "bb77a20c-25a0-4cfc-a5da-147bae3cb2b2"
            }
          ]
        },
        {
          "id": "66ade1bb-62eb-4897-b445-a82fcf64b51a",
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
              "id": "661ffe92-13fc-4cf1-a29f-7bd6907e035a"
            }
          ]
        },
        {
          "id": "ea2e8e98-55e7-4e32-b1c4-1d0b5d313c09",
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
              "id": "60bace1b-a2eb-4397-b387-28f7abb5817b"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "2b5764af-ef58-463e-99d2-6f8da4c8d762",
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
              "id": "a4b11848-d5bb-4947-b49c-bab9a35f581c"
            }
          ]
        },
        {
          "id": "f4332223-5001-43ce-a4e9-981191a3652f",
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
              "id": "25fee12b-e461-44c1-9e0d-4f87960f11fb"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "c9369855-d954-49db-9f51-9b96759594e9",
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
              "id": "a5487d46-aa60-4aa0-800b-4e1c027a6966"
            }
          ]
        },
        {
          "id": "8ecd41dc-d15f-4786-bfe4-1481998a87d2",
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
              "id": "8a5751d1-0454-4940-bf29-05543eb49c4e"
            }
          ]
        },
        {
          "id": "3f2708d1-3170-41d3-a772-b2b4c37d6b18",
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
              "id": "2c9e213b-fdb3-4673-990f-5948df884179"
            }
          ]
        },
        {
          "id": "72c7a7f1-f0d1-428d-928d-32c1f5d33d99",
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
              "id": "8aad7dd2-8818-480c-be83-238903338970"
            }
          ]
        },
        {
          "id": "2dfcbdf7-b938-41e3-8a52-7465370f5da7",
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
              "id": "13108eae-623b-4933-b7d8-3a28870783ae"
            }
          ]
        },
        {
          "id": "aa9b0b02-7ad1-4db5-b82e-cb1a5309b8fd",
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
              "id": "2e981d9b-2abf-4831-a166-c71d6dcfce96"
            }
          ]
        },
        {
          "id": "84ead68e-0d2e-47ff-96a6-14398e6ec9d7",
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
              "id": "66ac7077-25c8-4856-b994-01b9741260d9"
            }
          ]
        },
        {
          "id": "861e73da-222c-4c0e-9e0a-3034f276a39b",
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
              "id": "9aee417f-cdf7-4b6c-84e5-6a19c3c5e21f"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "5966299c-e8ad-41d8-bb44-4fd675ca4186",
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
              "id": "b55cff7b-14bf-4d0a-a122-a19fcff673ff"
            }
          ]
        },
        {
          "id": "604bed0a-1dee-4892-857a-58a2ef45cee6",
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
              "id": "4d257ae8-99f8-4556-b9d0-65718b1b1eeb"
            }
          ]
        },
        {
          "id": "e071342d-3280-48b7-bc38-15a5ef7a53b8",
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
              "id": "2cb6e052-910f-465a-97e4-53c13ae73127"
            }
          ]
        },
        {
          "id": "cfc1b7c9-a57b-490b-8e93-e1b9d118e157",
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
              "id": "84138215-bcd8-428d-bd46-82b8a74c7178"
            }
          ]
        },
        {
          "id": "7ff203f5-b963-440e-8c9b-27ad80ee9330",
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
              "id": "0701ddd6-62a3-4298-9c1d-2a1ad65d88bd"
            }
          ]
        },
        {
          "id": "072716c9-3329-45a1-aba8-73410a84a757",
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
              "id": "82018cdd-3658-4774-b40b-f5fa41db1691"
            }
          ]
        },
        {
          "id": "2c2abb9b-fbde-4ed1-83ad-1515e8dac85e",
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
              "id": "fb65b0e9-795f-4ab8-9775-585d67f7dc0e"
            }
          ]
        },
        {
          "id": "e7402a8f-dc3c-4fb8-9d22-4488d2c2c0a2",
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
              "id": "0aae9c71-77a9-4daa-b34a-a8444a3bdf1c"
            }
          ]
        },
        {
          "id": "d03e68e4-6880-431e-acc4-5730dbc9f66f",
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
              "id": "4fb774ab-cc2b-4dd0-a695-1f859bcc775c"
            }
          ]
        },
        {
          "id": "53e8d8b7-9ff0-42e1-b22e-985fc320291b",
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
              "id": "81ede792-254f-4a87-8dc3-3ff609cbf186"
            }
          ]
        },
        {
          "id": "d203dcac-1d66-469e-9bab-3241a6e60d67",
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
              "id": "255ef275-1779-4149-9869-5905f7db6de7"
            }
          ]
        },
        {
          "id": "0880d713-e467-4a84-8585-32ddd3cb3e5d",
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
              "id": "67972262-beb2-47a0-8679-89628fa0369b"
            }
          ]
        },
        {
          "id": "a9099821-5abb-4ea8-ba07-c0e354023170",
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
              "id": "763c9e3b-d24a-45f8-8efa-aad2020d5d65"
            }
          ]
        },
        {
          "id": "56245231-efa1-4068-96f7-d9c5184eb75d",
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
              "id": "6a667c1f-6fff-4ff4-8df6-56e4e562172b"
            }
          ]
        },
        {
          "id": "fc50e7cf-a4e5-4360-9875-7d5531bd6460",
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
              "id": "95b42c92-03a4-4304-9e34-e2f05d19b680"
            }
          ]
        },
        {
          "id": "75f9839d-1bb4-42e7-b2b1-0efac6c831b1",
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
              "id": "03e83476-ec1f-43fc-ac63-db0feded2d52"
            }
          ]
        },
        {
          "id": "8abd8efd-e2b3-4395-910e-260030c9a994",
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
              "id": "bab3a4b9-f81f-4200-8f4b-a63fba231484"
            }
          ]
        },
        {
          "id": "b6c348cc-ad5a-4c83-8324-49cb14f5b1f7",
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
              "id": "7d747cbf-2b0f-45b5-8461-08182b5e65b1"
            }
          ]
        },
        {
          "id": "9393785f-65db-4dd1-8392-0d16de758f46",
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
              "id": "f5ee3bf6-a05d-44ae-95d5-c8a564b1eb30"
            }
          ]
        },
        {
          "id": "519d67c0-f455-413b-98ae-319370b5bbaa",
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
              "id": "67661e3a-37e7-4a33-9289-f7c34fa11379"
            }
          ]
        },
        {
          "id": "18cfb78e-bc8c-4c59-9f19-265dce6a9724",
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
              "id": "7445e28b-87d4-4584-9b1e-684fc999cf94"
            }
          ]
        },
        {
          "id": "3f29414e-05fb-4600-8888-02409ecc095f",
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
              "id": "ad897696-21ed-45aa-9fdf-7be8dc904790"
            }
          ]
        },
        {
          "id": "e4a186e9-1925-4855-8a5d-cbd1617edcef",
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
              "id": "3c6bb619-2d92-48bb-af95-1fb9fd395f0e"
            }
          ]
        },
        {
          "id": "dba3da0b-1e9b-4165-9ad4-58d29061c174",
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
              "id": "cb0a894a-cea9-4afe-98e1-8b69def62646"
            }
          ]
        },
        {
          "id": "168e2d24-fbfb-42b0-82ce-29169f4ed708",
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
              "id": "1ad8667e-a93d-423b-b832-fdee5637d9b7"
            }
          ]
        },
        {
          "id": "8e8604ac-29f6-4f8f-a347-60b7e571c74c",
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
              "id": "b2eafdb0-d741-4afe-baa7-a4fb6c0ab5e8"
            }
          ]
        },
        {
          "id": "a4eeb6e0-78be-40d9-b004-96db3bb9d1d1",
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
              "id": "b16bc484-0860-4f35-a44c-c66c7ff76471"
            }
          ]
        },
        {
          "id": "390ec0d8-0e17-47b0-b10d-091c4807a8e6",
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
              "id": "74de57cf-8e62-49d4-9289-e58c2214496d"
            }
          ]
        },
        {
          "id": "7b2633ff-9927-4412-9426-b954024c8bc3",
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
              "id": "9fd6addc-6e81-4565-ba72-9551a339a846"
            }
          ]
        },
        {
          "id": "3f335abb-d368-4b3e-b155-5f2f2aae9e60",
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
              "id": "e55861ae-41ba-4a5e-b0b6-6204bcb7fabe"
            }
          ]
        },
        {
          "id": "93342701-3cc4-4a17-9e95-02c437359c63",
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
              "id": "06479e95-82c0-4cba-9cfc-e3faef03c3da"
            }
          ]
        },
        {
          "id": "4099aae9-cb00-470a-aa24-5cfaac7d7e48",
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
              "id": "6a758755-82fb-4977-99eb-0bc1bd0c488f"
            }
          ]
        },
        {
          "id": "30b53353-6a18-4a63-9ce0-5c52e38c424b",
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
              "id": "d33b7566-1073-496a-8d9d-02117ed4a06a"
            }
          ]
        },
        {
          "id": "fa04a4fd-b46b-472b-acba-246d2b523813",
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
              "id": "c6ecb665-1ac3-4f64-8367-cd1c6e0cc5af"
            }
          ]
        },
        {
          "id": "b58d4158-e45a-4820-a93a-a9e33e3ecb26",
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
              "id": "0d75a37c-ed90-4ed3-9811-0787d50e3980"
            }
          ]
        },
        {
          "id": "c51760b6-135c-4fb8-8d0a-e9f5abc9a3c6",
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
              "id": "d5945123-a9d8-4f8c-a726-d46a9559e6fe"
            }
          ]
        },
        {
          "id": "610a2e68-cf50-4f18-9271-a944ec84bfc3",
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
              "id": "dfb1b247-dcc2-4f58-a564-7d3a1e040949"
            }
          ]
        },
        {
          "id": "2d10116d-68aa-4785-9ddd-f431a14e3b27",
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
              "id": "ee12ab8f-5735-4205-8456-88c26948710b"
            }
          ]
        },
        {
          "id": "aecedccd-8f90-4a35-8c55-d8316bd33d14",
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
              "id": "69be1f91-23e9-46d2-80f6-6e0f617800a9"
            }
          ]
        },
        {
          "id": "84ee4b35-a446-413f-8df4-480a4965f88f",
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
              "id": "1e181972-6f21-417b-8540-bf3426a2c102"
            }
          ]
        },
        {
          "id": "056ccf3e-24ef-4441-adc6-239f0e0656f5",
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
              "id": "b316db9c-26eb-4e95-944f-86ff46b13277"
            }
          ]
        },
        {
          "id": "2add57fd-6424-4f0b-9a1a-023b0f9631fe",
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
              "id": "ec582fbb-508b-44b3-970c-4f833b1417c0"
            }
          ]
        },
        {
          "id": "dd1f2133-af92-4696-b2e2-80b8ea1d6fa7",
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
              "id": "da0845f8-acf3-4b20-83e7-b1cee05f714a"
            }
          ]
        },
        {
          "id": "f9769692-0c74-41a1-8034-b24d9e4584fd",
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
              "id": "dcb161fc-6c97-4075-a368-1ebf98a9a2b9"
            }
          ]
        },
        {
          "id": "e6872659-df44-42eb-97a0-fd74c36897c3",
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
              "id": "5ae4499d-0665-4b08-97a9-e1f5961ec02a"
            }
          ]
        },
        {
          "id": "460d1beb-4cd5-4988-be5b-0c4e3aeae916",
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
              "id": "a702da90-bc17-4e0a-a9d8-fc4721c581b0"
            }
          ]
        },
        {
          "id": "5cda1001-28ac-4ef2-ac11-4eb51f108a7a",
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
              "id": "29daf156-5305-4258-b4f1-acfb9c55e3c0"
            }
          ]
        },
        {
          "id": "a79381c9-6677-4349-94ac-f64341d44989",
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
              "id": "a674ab5e-b173-4f20-bfe7-0e82db3fe35e"
            }
          ]
        },
        {
          "id": "1f86f90a-2f8b-448b-906e-478893533fcd",
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
              "id": "3aa43b71-ba8d-47a6-ad7b-0eb949a097d8"
            }
          ]
        },
        {
          "id": "f770335a-b5b7-4c41-b387-5fd750f331bf",
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
              "id": "646d3707-bb22-448a-9c6f-e36a4ede239b"
            }
          ]
        },
        {
          "id": "084f0bab-613b-400a-9710-b5bcdc4d8b1f",
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
              "id": "76b0adf2-300c-4620-8e4f-4f74bc02642d"
            }
          ]
        },
        {
          "id": "00fd4a9f-b658-4f52-81ca-41781c651ae5",
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
              "id": "bd5c5d5b-7307-4122-9c8c-f45413efba1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "80d7b712-33ac-4067-afbd-d9fb184a853d",
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
              "id": "2ed911b2-37d3-40ed-866a-2f440f116ba8"
            }
          ]
        },
        {
          "id": "2cdb3894-e1a0-460c-96a6-2c84189f9351",
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
              "id": "0388deec-9845-4e54-b06e-81b8ff678590"
            }
          ]
        },
        {
          "id": "39188d4b-86e7-4110-a727-b68a27033149",
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
              "id": "1e3e8407-807c-4dac-9524-7321cabcef2e"
            }
          ]
        },
        {
          "id": "865c9817-4fdc-4433-b2bd-e13127b51b57",
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
              "id": "909d32f4-1b09-467e-9569-2e75bd5ed6b4"
            }
          ]
        },
        {
          "id": "a35c6036-fc7c-4e34-af66-5765aa6d54d2",
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
              "id": "5b0f766e-7478-4143-b90e-494bbb8c3cdb"
            }
          ]
        },
        {
          "id": "fb91bf6b-e71f-4700-99c4-76182beea2a9",
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
              "id": "1cc7ae90-e230-4e92-a8c6-87ad5487e1a8"
            }
          ]
        },
        {
          "id": "4656145c-4772-48b5-bd93-a09b970892f3",
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
              "id": "52f43dad-dc36-4eb4-b115-c661bb81c44b"
            }
          ]
        },
        {
          "id": "12b1145a-cc8e-46ac-b51e-8f10d24da927",
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
              "id": "04a58b03-8fa5-4304-b7aa-5c4040a510ce"
            }
          ]
        },
        {
          "id": "a641b80e-8a08-4397-a6bf-f6a088f17fe9",
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
              "id": "5a2e440c-25c1-4665-9aef-6a77548f8593"
            }
          ]
        },
        {
          "id": "73f32f1b-3bac-4f91-bd40-61d4130dc1a0",
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
              "id": "b400f9f8-fe36-4139-a9a9-b5c1f57fa98a"
            }
          ]
        },
        {
          "id": "af09d116-2cde-40cf-a01a-fad1614a666c",
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
              "id": "c869dd52-a4c7-4015-9a45-062043c48d50"
            }
          ]
        },
        {
          "id": "0e1e5df2-04e5-4f8e-8f46-9f6a1641d139",
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
              "id": "592e04d7-c5ff-4d0b-b6d8-9aafcf0671bc"
            }
          ]
        },
        {
          "id": "44365846-4b0d-468c-924a-47cc913a7706",
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
              "id": "d888ff07-c829-4f2c-b8fa-91b9ca9ce11c"
            }
          ]
        },
        {
          "id": "c7da5085-ef11-450b-a0b0-2c2a2cdf0461",
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
              "id": "3f3f60dc-509c-47c7-8e1e-5d7a5125f3ab"
            }
          ]
        },
        {
          "id": "b705aa7e-d0cd-43b8-86b5-8ffe0bbe687f",
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
              "id": "be026032-ba1c-4076-a4b4-0f8b3173688d"
            }
          ]
        },
        {
          "id": "721b1086-3238-48c7-aa70-879bc7afca68",
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
              "id": "aaa005ad-a206-45f0-9fa3-614cb7ff12d5"
            }
          ]
        },
        {
          "id": "eadb8f06-1e94-439a-9f01-f7d5d7658e83",
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
              "id": "ec53e7f7-908d-49fd-8b7d-fdfbfae352ef"
            }
          ]
        },
        {
          "id": "17186716-9ba7-403a-b38e-c330313df272",
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
              "id": "a4d4880a-c041-41f1-b4e3-1e871b228368"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "6848661f-13e6-422a-85ae-e3daec865607",
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
              "id": "543fc551-c2c0-4210-86fa-c59c3698a31d"
            }
          ]
        },
        {
          "id": "b8b9a449-8dfa-4ac3-ab18-a0c0c4aa8852",
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
              "id": "6625553f-ef68-48c1-8455-2e86a66f6f72"
            }
          ]
        },
        {
          "id": "82632972-e87c-4848-a73f-37fe130ebb66",
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
              "id": "5b480f2e-a8c5-43cf-855a-131bb230ca0c"
            }
          ]
        },
        {
          "id": "b5015040-6cb0-4dc5-8433-e63ab426c39c",
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
              "id": "546680ef-2bca-473c-bbf7-6a56af0f4647"
            }
          ]
        },
        {
          "id": "9ab1486c-28ec-4ecf-94b7-c4e8d19942b2",
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
              "id": "e256f5cc-cb04-49be-944e-5e2e7cffee41"
            }
          ]
        },
        {
          "id": "bb452762-7be7-4eda-b6eb-88866da8fe50",
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
              "id": "8b032be8-1169-41a8-a6fe-cd8d61e89669"
            }
          ]
        },
        {
          "id": "9807198b-90d0-4f7c-a3b7-d6a1732afa53",
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
              "id": "247dfb13-018b-46b7-8229-10b35dbc0a18"
            }
          ]
        },
        {
          "id": "45d966ee-0f7a-45c2-acea-807b222d8570",
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
              "id": "06b12757-fa3f-4917-9d05-e50b82fcea3d"
            }
          ]
        },
        {
          "id": "dd43bd89-73d1-40e3-a7ef-3121c74f3e14",
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
              "id": "4598c61e-b77a-45b9-b60b-9d0121909d83"
            }
          ]
        },
        {
          "id": "04acd1dc-ef6c-4e99-8fb9-07a091375e6c",
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
              "id": "c4944001-98c0-4475-899e-cb62fa8b54e4"
            }
          ]
        },
        {
          "id": "44a0b94d-140f-46d7-be87-a6c26b44bbef",
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
              "id": "2de067db-cee7-47da-9901-4a22e9cb0666"
            }
          ]
        },
        {
          "id": "a5d21346-4733-44f5-acf2-6edd6c1ce99d",
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
              "id": "a90ae1f0-e698-42d7-8e1d-4cef5eed5d05"
            }
          ]
        },
        {
          "id": "137fa3bf-08b1-48b4-8792-0ae8c0001cf8",
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
              "id": "d04c6b10-cd78-405e-b02b-80f513afaef7"
            }
          ]
        },
        {
          "id": "08daa382-25f5-46ff-bba2-47e45c1f952f",
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
              "id": "5f2c11e8-3ee8-4cba-92b5-19c21d81123f"
            }
          ]
        },
        {
          "id": "29662225-5333-4b25-bc16-8e6ba5050afe",
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
              "id": "504bd3a0-2642-4629-86d2-287a26d9735e"
            }
          ]
        }
      ]
    },
    {
      "name": "Prefs",
      "item": [
        {
          "id": "ee236b26-dca6-4e28-8591-7a031eec2e95",
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
              "id": "41635184-a948-4790-98e5-1f2dd9dac27f"
            }
          ]
        },
        {
          "id": "b745918a-dd83-4a5f-b963-d8f3b19b4914",
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
              "id": "63d7678f-7e3d-4ed6-9175-090aa51d1126"
            }
          ]
        },
        {
          "id": "a23b38bf-8840-4ed6-875e-f65549e945c4",
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
              "id": "8c1885fb-8cee-48ed-8848-d819b1fddbeb"
            }
          ]
        },
        {
          "id": "99729d61-4454-49f7-8a47-1f303fa08900",
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
              "id": "c05f3a1f-978b-4e3c-b82f-5b8529c3c532"
            }
          ]
        },
        {
          "id": "46c409b7-c45e-43c0-b4f2-ed14f59e0899",
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
              "id": "0dc4842e-7e7f-496f-ab9b-f55dac2a9f38"
            }
          ]
        }
      ]
    },
    {
      "name": "Reflection",
      "item": [
        {
          "id": "3ad56c47-3400-484e-b9eb-3ebc6489cb39",
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
              "id": "20029941-f5aa-49a1-b61d-464486fa57c3"
            }
          ]
        },
        {
          "id": "fc998aea-db2e-4d1d-9804-f58577da1f50",
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
              "id": "0dc1f8b5-1c5a-4827-b55b-da68d862cf19"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "430b1731-f1d4-4457-8ea1-a5494c35eafa",
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
              "id": "5711eedc-67f6-491f-b1b5-2a3666fabe7d"
            }
          ]
        },
        {
          "id": "b4d12111-3b7a-472b-897f-f46623fa1afc",
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
              "id": "216feaf9-c427-4e6f-9879-6033f852f836"
            }
          ]
        },
        {
          "id": "976e0c0a-a8cd-440f-b045-7f0f2907550e",
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
              "id": "51e69a77-88f4-477a-8cfc-4769b3aa6f67"
            }
          ]
        },
        {
          "id": "de568cd7-8998-4d3a-9d48-5b24343f6954",
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
              "id": "77022865-0f73-48e9-8fdf-7df18e950aa7"
            }
          ]
        },
        {
          "id": "f4465d4f-de7c-428e-a797-e5954059dd65",
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
              "id": "a064fbb1-1642-45a7-aae6-8419185a0476"
            }
          ]
        },
        {
          "id": "82ce09b6-5105-4989-9a7b-0d5672233d6c",
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
              "id": "132dc2c5-5184-465a-8a81-2091366fc09a"
            }
          ]
        },
        {
          "id": "f3924d61-e4b2-4178-9897-b11be0b8cf14",
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
              "id": "d939b08d-45b0-42d3-8e42-61cd217e28eb"
            }
          ]
        },
        {
          "id": "a0919185-de87-4016-93df-3cc951984608",
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
              "id": "701c8e35-4d6f-46bb-8f36-e225fc59cd15"
            }
          ]
        },
        {
          "id": "cb8561cb-0f59-4c1b-93a6-fd1a0e69836a",
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
              "id": "97c33963-df95-469f-b08a-565119c0739d"
            }
          ]
        },
        {
          "id": "6ba4f9c5-b131-4a19-a890-9d4da4f723b6",
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
              "id": "1836f64a-e8b6-4c4b-a546-3124fc626b68"
            }
          ]
        },
        {
          "id": "429a568d-3f80-43bc-9658-96a28eff7fca",
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
              "id": "e4efdbcd-28ce-427f-b465-0bd0d7af476b"
            }
          ]
        },
        {
          "id": "9c9233b0-678e-4a84-915e-71a471bc00e4",
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
              "id": "446846fe-22c4-4e1c-afbf-9776055123c9"
            }
          ]
        },
        {
          "id": "b4e15bbd-3fb3-4f79-a95a-ade68757a08d",
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
              "id": "1ab05918-c170-4fe0-9c44-ab0c0367f25e"
            }
          ]
        },
        {
          "id": "7d3fff1b-34af-477d-bbe2-da3cef3ccf91",
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
              "id": "1d8e15a6-bcf8-49eb-8dfa-c3141a06f6f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "ead2db2e-c710-442b-a070-4ae90d62cdcb",
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
              "id": "bdf61944-2e86-419c-af21-bf46041711df"
            }
          ]
        },
        {
          "id": "9656214b-7a63-471a-821f-39ee8e0be719",
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
              "id": "2709713b-75cb-4115-9215-247074526cd1"
            }
          ]
        },
        {
          "id": "3be8846a-b9c1-4b42-a04c-d10f7db3e47c",
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
              "id": "9f45bc10-8b2c-4fa6-9e90-d2ed78d2ec6c"
            }
          ]
        },
        {
          "id": "ffb3adb2-477c-46e3-b800-93e0a1ed8448",
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
              "id": "eff12c5b-aeb3-4123-ab3d-aecf234f9161"
            }
          ]
        },
        {
          "id": "35c162f0-5441-44d1-9a00-39f7358a00a7",
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
              "id": "70cfe48b-9cb7-4a33-8f45-d63445df25ad"
            }
          ]
        },
        {
          "id": "7b6c6026-3e60-4dbd-8b0c-111f4bc4f6fb",
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
              "id": "51dbcf08-f621-411c-be63-71421bfe74df"
            }
          ]
        },
        {
          "id": "7387ef26-6b3d-49b6-a84d-32328893dd27",
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
              "id": "0c45e6e6-aeb7-4ddf-af12-db150f4f191e"
            }
          ]
        },
        {
          "id": "0a4a66ab-582d-4904-a255-bf956526c750",
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
              "id": "f011ceef-cae2-43e5-9486-32cc80afd15f"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "10306242-912d-4a14-b880-be5c192f6893",
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
              "id": "20adde42-e8d2-4987-b004-4e888a62bdd2"
            }
          ]
        },
        {
          "id": "462c2b88-a223-4311-80fc-ce52b58f214a",
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
              "id": "6fd1d4f6-9ae1-4fc8-8993-2d4d7a763b0b"
            }
          ]
        },
        {
          "id": "00b33ff6-552b-45c1-a773-4bd33f03c5e0",
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
              "id": "2df9058c-6811-40b5-9c40-c31de0ed8725"
            }
          ]
        }
      ]
    },
    {
      "name": "Urls",
      "item": [
        {
          "id": "04b67dfd-3227-4bfa-bdf7-d2b54a44748b",
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
              "id": "35ae1975-7d37-44e8-8c3e-6aaef9f8f6cb"
            }
          ]
        },
        {
          "id": "4920cb2c-4dd4-4533-a93c-9050229db1ec",
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
              "id": "200fa617-6e21-4082-a74c-8322007d616e"
            }
          ]
        },
        {
          "id": "1cc5824e-418c-4888-add4-cd4604eceab5",
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
              "id": "95ba23ff-aa23-48ea-a6b0-45ff81b5071e"
            }
          ]
        }
      ]
    }
  ]
}