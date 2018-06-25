{
  "info": {
    "name": "Flickr Tags Get List User Raw",
    "_postman_id": "f6c8ccc9-fce3-41bc-830b-4ac168bb20ae",
    "description": "Get the raw versions of a given tag (or all tags) for the currently logged-in user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "523c3731-3a04-4593-85cf-7d9e97248b16",
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
              "id": "f165d4b5-08b2-4749-b1b9-c2fd40ec121d"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "52c294b9-087b-48b4-bb7f-801510a3ed7e",
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
              "id": "c78750ef-979c-4f4d-8315-31cb95b36faa"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "8d945ece-08a0-4309-81bc-8768761413c5",
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
              "id": "fb1b19bc-3644-4115-831a-a8671902276c"
            }
          ]
        },
        {
          "id": "e6ad7e2a-d495-414c-8461-65e19443f0da",
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
              "id": "6e73f758-6055-4bea-8975-1669503ea1b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "a93614bb-e9bc-4f98-ad94-c355a459746a",
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
              "id": "c068abfa-606a-416a-99ec-df30fb8463e2"
            }
          ]
        },
        {
          "id": "5f49e92e-2e91-4925-8c51-c67068981ad2",
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
              "id": "ecc47d98-1d1c-4e0a-bb61-c614367009b9"
            }
          ]
        },
        {
          "id": "c63e4f47-ab4a-4b50-a98c-ec861622351d",
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
              "id": "63365101-1fc9-430a-ab64-e55cbf03269e"
            }
          ]
        },
        {
          "id": "4859389a-cf31-4d47-9a82-4170aecb26cc",
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
              "id": "f814ebff-9e2b-4e53-9a24-1834ff86b1fc"
            }
          ]
        },
        {
          "id": "2bb68cf6-6f83-4e10-9fcf-e4ecf045a828",
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
              "id": "3cda2a25-8fa5-48ef-829b-374b69a899cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "778347a3-186f-4850-bbe6-f11d381d9362",
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
              "id": "591fe7de-6009-4066-96d9-c184032785ca"
            }
          ]
        },
        {
          "id": "45d671f0-b71e-439c-adcf-d60f0d46c235",
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
              "id": "e837fee4-59d5-4012-ae69-82fa7aba59c5"
            }
          ]
        },
        {
          "id": "8657616f-7e85-4243-ac14-52108ad144f7",
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
              "id": "fe55ae44-475f-43d7-85f3-9397f8487d07"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "98269388-0a38-4f87-aaa2-06c635ee9e44",
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
              "id": "f8f70937-ae77-45f3-beba-3c5c70435503"
            }
          ]
        },
        {
          "id": "2fb5f4c4-b3a5-4a33-a851-d862e10e7b1c",
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
              "id": "87f2788c-9ca5-4789-b3f4-7ff606178b9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "80caf2de-0c0b-4b95-afeb-20180d870f83",
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
              "id": "6a5589d7-e940-49f0-aec2-b369daf3df8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "f09b75c2-377a-4b4b-b610-415c951bd85e",
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
              "id": "56719c11-70cb-43a6-9df9-98e4d9efa840"
            }
          ]
        },
        {
          "id": "7353069b-a0b5-4235-bed2-1c1b768e5ccb",
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
              "id": "6c5d5bab-90af-4c7c-b80d-ce4a90eb9f4a"
            }
          ]
        },
        {
          "id": "b43237ca-923f-4c57-bdc0-1297c01bea75",
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
              "id": "29711be4-2246-4182-bba5-dfcb280e6a3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "e04a522a-37be-4576-9bc3-c4270a2be600",
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
              "id": "707ce4a5-ba3a-40d2-b9e0-0d34707de981"
            }
          ]
        },
        {
          "id": "5b30deb1-ebb3-43e6-9bb9-474401364d1b",
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
              "id": "070e0145-0fd2-4d7a-85e8-56bc80715faf"
            }
          ]
        },
        {
          "id": "b1def813-5fc1-4261-84e0-64c8a187795a",
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
              "id": "3ac70898-298f-4b14-a9d1-12e047f8ef38"
            }
          ]
        },
        {
          "id": "724db18b-1b6a-4096-aec5-b97c3938e1be",
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
              "id": "44778add-2876-4db4-a140-bd4b97a27e72"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "3b19bb33-f4c2-4884-98e7-e411dba491f8",
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
              "id": "f0c2c644-bc87-40c8-8c1a-429f5a35345d"
            }
          ]
        },
        {
          "id": "77df3a81-3558-44f8-a3ee-feb30150c5a1",
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
              "id": "9883ae28-9945-478f-9bff-fb5c0d9f6c4e"
            }
          ]
        },
        {
          "id": "7576f9ec-c92e-4e27-b39a-4428d67beabc",
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
              "id": "ff208fca-b264-49bf-9e37-fb1f5265f248"
            }
          ]
        },
        {
          "id": "08770bfd-7347-4ec5-beb1-db6d4bade31e",
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
              "id": "5bcaa98c-1847-4a4a-a459-44f7228ab047"
            }
          ]
        },
        {
          "id": "c435e796-f705-46f5-a7d4-ce9f0aaace9a",
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
              "id": "ff2cacd9-401e-4ff1-a7b4-17f1b1f3e4d6"
            }
          ]
        },
        {
          "id": "8ad5b1ee-482f-45ac-9686-d69fe635058c",
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
              "id": "4dfd0141-914a-43a8-b27d-b436c97b6720"
            }
          ]
        },
        {
          "id": "af0017d1-f30c-4e40-b1c9-f4f148e2d271",
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
              "id": "940edfc0-3c1c-44b9-a47b-2af776c296ff"
            }
          ]
        },
        {
          "id": "eed7a2fc-fc62-4b59-94e0-97d23661757a",
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
              "id": "9789dcc8-0423-44d3-82cc-fd88a78107cf"
            }
          ]
        },
        {
          "id": "d5ff2a37-4dc2-44bb-b255-3b99f7c123a2",
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
              "id": "258473dc-7dc2-4577-ba90-17466aa82001"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "c16c1f1e-8c83-46b3-b6f1-2db13e7a8617",
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
              "id": "a5740928-5137-4305-9582-37cd3aa33f41"
            }
          ]
        },
        {
          "id": "f558990c-51f5-45d0-9c2e-9de482ce6727",
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
              "id": "eb660d0f-9ef0-422e-8fb3-c1473fbb74e2"
            }
          ]
        },
        {
          "id": "c826279d-eef5-42bc-97e6-c17c29c2502f",
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
              "id": "c71b4947-1ed7-4268-b317-1113e3bbbd40"
            }
          ]
        },
        {
          "id": "111d9fc0-5dc3-4838-8a3a-b9c27279cea2",
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
              "id": "9cda7f19-09d5-4637-90fb-685e30bac8b4"
            }
          ]
        },
        {
          "id": "6e6b9228-0dd6-4f10-8972-4fc12de3c5c9",
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
              "id": "fed7f675-d5c9-4643-993d-12fb4883f2c0"
            }
          ]
        },
        {
          "id": "c9b9b93e-514e-40f3-a6b7-5e2a91e7aa93",
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
              "id": "44ab38bf-2843-4fe0-a9f9-751e7c7d17bd"
            }
          ]
        },
        {
          "id": "9d369390-8dd8-47d2-a2f4-9b600c3b422d",
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
              "id": "460d7fd7-ee18-4b8c-9281-f89de75ec426"
            }
          ]
        },
        {
          "id": "62a246de-82a7-44c9-be01-dcead2afeacb",
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
              "id": "7b3798be-bb7f-420b-ace1-a23ec3a5db28"
            }
          ]
        },
        {
          "id": "b8686614-f2f9-4910-ac8a-edcac2a89f85",
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
              "id": "df6dca12-7263-4f62-bc94-16b57be7a2a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "cc68b04c-3c7a-413c-974f-32514ce4258b",
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
              "id": "ab0289c6-2e3b-4137-bc34-217aa31786b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "9a2e01ff-f65a-4914-ac8b-147a69266cd4",
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
              "id": "dfde77fd-b8cf-43c0-ba07-3958e510856e"
            }
          ]
        },
        {
          "id": "1c98ba54-4b66-4d48-ade0-7b631213c921",
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
              "id": "3d9f78b0-b4d3-4f1e-8de0-ee413d2761c9"
            }
          ]
        },
        {
          "id": "3b2c53dc-d1fa-42a1-95bf-d70c072ca0dd",
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
              "id": "81f9740c-bbf1-495c-bedc-b18aabec0efd"
            }
          ]
        },
        {
          "id": "19c82153-82c4-45fe-8fe0-cbe7c08d373d",
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
              "id": "a2e7d0c0-c271-4972-b658-b5c2fe1208ce"
            }
          ]
        },
        {
          "id": "06adefb8-e40d-4418-b065-afd5fb8ccd26",
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
              "id": "f3655821-64d7-47c8-88bd-221834602735"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "13083539-b181-40d9-9d80-02f6580e86ab",
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
              "id": "7f7869dc-5fe3-4860-b63a-ac7c8eb80bc6"
            }
          ]
        },
        {
          "id": "f30a406a-403b-4bea-a7a8-c67e9523c242",
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
              "id": "4be94c01-028a-489e-8d8c-fb3f45bafd30"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "688569ff-b7f4-4f9b-a6bc-11458aeaeffa",
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
              "id": "ef6b29ec-6de1-4657-bdc5-d00215e6150e"
            }
          ]
        },
        {
          "id": "5eb2486b-0f11-46ee-9741-762727f6a747",
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
              "id": "2a1ed3ca-a9c2-485f-a761-61d0e2832d5c"
            }
          ]
        },
        {
          "id": "2d87c55e-a05b-4e14-b5a2-4d15bdd6ccfc",
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
              "id": "641eac65-c077-4c52-bd8e-78de6e5bec55"
            }
          ]
        },
        {
          "id": "428ade09-9eef-4048-adcf-47c5c3471d26",
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
              "id": "32d298bb-ad86-479a-9cfa-0bdcc207469c"
            }
          ]
        },
        {
          "id": "e9cd1310-ef6b-4cbb-b2a8-8c48c9d082aa",
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
              "id": "3439088a-0820-412c-8c42-4ab66aface6c"
            }
          ]
        },
        {
          "id": "43f3c152-bc2c-42e8-890c-2d5aea99afca",
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
              "id": "eba60e05-3b1f-4906-bba2-99e2a9b21f20"
            }
          ]
        },
        {
          "id": "ce184c03-e4d4-4a7d-8599-4f9984cb090d",
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
              "id": "eafb440c-eac9-424c-9b84-fc760f7fb2a7"
            }
          ]
        },
        {
          "id": "bac85db6-78c6-4f2a-aaad-5590b8d48778",
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
              "id": "cd11140e-c8c6-4aa2-afac-9d964bf42fcb"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "f4dd6703-4a56-4cab-bf10-e4a5ff43fccb",
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
              "id": "968774e1-1b3e-4df7-b2e5-3b721ce91690"
            }
          ]
        },
        {
          "id": "9931e1e7-b133-4e0c-bba9-cfd636c17574",
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
              "id": "e6a1b941-ed33-4f3a-8e12-02a8993d3dbc"
            }
          ]
        },
        {
          "id": "977c6cb6-77bf-4da4-ba24-6d28b9e588fd",
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
              "id": "9beefa89-2920-4cfc-a6a3-a1b6a8ce1d98"
            }
          ]
        },
        {
          "id": "f7c37d58-e411-476f-a88d-bf9bce6d9815",
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
              "id": "3bcf8e3a-3a93-4270-8ae6-d544514a0efc"
            }
          ]
        },
        {
          "id": "459374ae-9c2e-410d-b3ee-1c4b338e2ff7",
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
              "id": "bf8c32dc-18b5-4e5e-9b28-434e707f90b2"
            }
          ]
        },
        {
          "id": "8cf1c7c4-574c-4dec-ae30-461142026250",
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
              "id": "0c3b3562-1391-4284-aecd-5cc5e71e5a0b"
            }
          ]
        },
        {
          "id": "2bd0ee06-6f97-4d88-a495-543ce04cd763",
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
              "id": "696c110e-8834-45ca-9769-31e93043ec72"
            }
          ]
        },
        {
          "id": "006cd951-e39b-4471-adbd-f482576aadb3",
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
              "id": "25422163-1b2e-47e8-b983-c23268bb4ee7"
            }
          ]
        },
        {
          "id": "4dc8a8ae-d985-4250-b16a-0ac2f7740d4d",
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
              "id": "9c7f3db4-8728-40d6-88de-91c965e7155a"
            }
          ]
        },
        {
          "id": "9d743d84-40b0-4f1a-9181-661311271d24",
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
              "id": "43c9eb24-fb53-4900-a463-e7deb3778ddf"
            }
          ]
        },
        {
          "id": "b8f304b9-01f7-480a-b057-95d09c692474",
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
              "id": "d990acbf-eca3-4f39-8fa2-9e334ecb9bc9"
            }
          ]
        },
        {
          "id": "74db8e08-1b20-472b-a570-f3797b62cd3e",
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
              "id": "5cf54c59-102b-4c07-bf91-d4c5f24f9e03"
            }
          ]
        },
        {
          "id": "50e9a156-421a-42f9-b14c-2f5aaae90d04",
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
              "id": "4ff98b3f-15df-41a1-b0fd-1dc5e01ebd86"
            }
          ]
        },
        {
          "id": "7b5a24bb-195b-4a75-a63c-df0b94ec2781",
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
              "id": "4ccef796-1872-4502-a1d5-2463b33b1307"
            }
          ]
        },
        {
          "id": "6c252f54-3251-40ae-bdd7-2dff542bad76",
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
              "id": "f6bc6390-4820-4b11-8427-1354a47e42cf"
            }
          ]
        },
        {
          "id": "26440326-744e-45dd-b8d4-ba6d8061422f",
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
              "id": "5699b499-4fa6-4537-b95c-a829c9f349f2"
            }
          ]
        },
        {
          "id": "7de991b6-35d2-4c92-bf1d-a4b4be55f0e4",
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
              "id": "f62f7357-b0f7-4ffb-a71a-f7b836e76427"
            }
          ]
        },
        {
          "id": "e62f0e7c-fb8b-45e1-b6d4-e8880fbceb5a",
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
              "id": "01097d4b-bb40-48b6-99fd-8c59e4236555"
            }
          ]
        },
        {
          "id": "1d8f5f8a-fe33-4f4b-a47a-d9acf4b7b0a4",
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
              "id": "6954e589-eecc-4b19-b34e-4c350a035da6"
            }
          ]
        },
        {
          "id": "a609b55e-8a61-4f3f-83ba-1d82d3588a92",
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
              "id": "ddb875c7-8b28-46d8-a4a2-abd50b6a01f6"
            }
          ]
        },
        {
          "id": "41779204-3208-4e9b-8eda-6ac774da31b9",
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
              "id": "94ec25e8-0887-432d-931c-9b2acbc5f906"
            }
          ]
        },
        {
          "id": "b84e11f1-7a4f-4dd2-9b35-e4304cfd41fb",
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
              "id": "cdecf46a-8915-4f86-aa3f-657f550f70b2"
            }
          ]
        },
        {
          "id": "0e44e82f-f2fd-48d3-9b5a-4df12ddda681",
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
              "id": "93938485-aba7-4924-b71f-bea5d6f8309c"
            }
          ]
        },
        {
          "id": "2599f96f-e37a-490f-a14a-8c477eb69182",
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
              "id": "1d1b783f-4f33-4867-84c4-a24b58349641"
            }
          ]
        },
        {
          "id": "464c062b-17a8-4774-a561-7a850e111ae9",
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
              "id": "9594ed8a-958f-46e3-bd29-8e69f18d901d"
            }
          ]
        },
        {
          "id": "5a93db5f-864d-4324-a292-824914560060",
          "name": "postRestMethodFlickr.photos.settags",
          "request": 