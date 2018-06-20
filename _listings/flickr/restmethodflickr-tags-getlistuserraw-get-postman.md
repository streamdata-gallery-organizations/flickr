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
              "id": "2c5b30f6-c487-42d9-b4dd-759ac02256c6"
            }
          ]
        },
        {
          "id": "0cb1b746-64bd-4193-a559-dfa60ad2acee",
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
              "id": "61904720-599b-4316-97d0-05289a0ee67d"
            }
          ]
        },
        {
          "id": "17066df3-e93e-4f09-8245-871777aa2661",
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
              "id": "35b7cfaf-cec2-4c3c-abed-8178ec4ea1bd"
            }
          ]
        },
        {
          "id": "85dae8ce-3054-4703-9a51-07ec3e9842e2",
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
              "id": "b9244b44-43ef-475e-85c6-c1d0d47289f7"
            }
          ]
        },
        {
          "id": "398d4aad-8316-4ae0-b466-71519d058d90",
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
              "id": "26c68d99-d976-49fe-add7-89d0c1ba69f1"
            }
          ]
        },
        {
          "id": "5e913fed-d783-4491-aeb1-28feeaef5273",
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
              "id": "981a99c2-b016-479a-9651-bba4fbf247c1"
            }
          ]
        },
        {
          "id": "9c839fc6-6af3-4f40-bf22-b0b686f61d6b",
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
              "id": "b774aa51-7cce-4a67-a511-739351fd1e7d"
            }
          ]
        },
        {
          "id": "286ef1c9-76ca-45de-87ba-c7fe8467edcb",
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
              "id": "d3f31956-8748-4245-82a0-6a340a1198ff"
            }
          ]
        },
        {
          "id": "d4b3a841-c92b-44ac-8f56-799994185a4c",
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
              "id": "b7f014ac-8530-4dbf-9cf0-71eb8289d0f8"
            }
          ]
        },
        {
          "id": "58db3fac-d289-48ce-8ae9-68ea2b2c511a",
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
              "id": "0848eea9-c1ed-4a47-a59a-6acbec93c039"
            }
          ]
        },
        {
          "id": "5342953f-f2f8-47d7-a1c4-b6fb9c6fe186",
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
              "id": "e5419e4c-bf3f-4194-8e06-eb2bf428a45e"
            }
          ]
        },
        {
          "id": "6e419486-b967-42f0-ab4f-68bf18342607",
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
              "id": "16e0622c-30f2-4005-83a1-a904d8ee510d"
            }
          ]
        },
        {
          "id": "b9819f66-df0f-400e-8aa7-01e04592cdc2",
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
              "id": "4d2b39f8-c0d3-4979-b21e-ad18b4ba87d8"
            }
          ]
        },
        {
          "id": "e52423bc-a96f-46af-a20e-6e4f4eaa1263",
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
              "id": "d03688e6-2615-4fca-80f1-11b25dc9e854"
            }
          ]
        },
        {
          "id": "e83c6a58-ed0d-40aa-b0a9-eea53fb60e0e",
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
              "id": "578e4f40-6cd9-4ec8-940d-0ada001018a3"
            }
          ]
        },
        {
          "id": "4b4895ee-a334-48c7-9850-e894fd10049a",
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
              "id": "71c6079b-a721-431a-addb-0fe4cc3b073b"
            }
          ]
        },
        {
          "id": "7a22da37-8378-4f4b-b275-16dc584ddc4b",
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
              "id": "207e3fb8-c655-4333-9ffe-d1de6d7cea0b"
            }
          ]
        },
        {
          "id": "da65d78e-7992-4a49-9c9a-488f99cb777e",
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
              "id": "4ea14d99-9b48-4f05-a88d-ca3df0d6b005"
            }
          ]
        },
        {
          "id": "a24d61ba-5152-480a-9de9-7db83496c487",
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
              "id": "e44e3dcb-02cf-4619-bcf8-5e1f1b7055a6"
            }
          ]
        },
        {
          "id": "896ba4c8-10cd-49c0-9134-cbc4d83e28b9",
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
              "id": "ed4d7cdd-f623-459a-ab59-5665a96583c8"
            }
          ]
        },
        {
          "id": "5ecf6577-3d16-42d6-91b0-d28d566c75db",
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
              "id": "bd0a5848-034b-4da4-875b-96560da3056f"
            }
          ]
        },
        {
          "id": "ec955686-4050-455b-b093-9b1666dadb19",
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
              "id": "9be4e63d-e5d8-4b4b-a3ff-98e52fa1225a"
            }
          ]
        },
        {
          "id": "365c858c-d1da-41ab-97e0-47e8f25072e5",
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
              "id": "2535bdf5-417b-4948-b21a-2b477cee10f4"
            }
          ]
        },
        {
          "id": "8749f5bf-fedf-4a18-b7e8-a8bcfe5e187d",
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
              "id": "3d4236b9-cd89-4ae3-bdaa-3b7dd1b7c0ca"
            }
          ]
        },
        {
          "id": "1b3506f9-885a-4d92-8f65-43353165460b",
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
              "id": "04f15447-8de2-4a77-8a16-20884150d6e4"
            }
          ]
        },
        {
          "id": "d31b47d0-11b9-48ad-ae32-dc60a187f4a1",
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
              "id": "8d274b8b-2326-43a6-a615-785f02782134"
            }
          ]
        },
        {
          "id": "3cbc5245-d455-456b-bd20-c865287e8f2b",
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
              "id": "33e90fba-0d5c-4ae5-a997-1a084f8cdfd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "8a84afbe-5d27-43f2-ba5d-bf3226ce03af",
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
              "id": "c7c8b56a-6a81-4cc1-aba4-198d46d38923"
            }
          ]
        },
        {
          "id": "5a6ced81-f20c-4cbb-b0ad-e8ccd28e46d2",
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
              "id": "d94f0568-230c-4d56-840c-bc2078725257"
            }
          ]
        },
        {
          "id": "572dd444-2378-412a-a2b6-eca9634bd7d5",
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
              "id": "70d3d65e-efad-4e55-89d4-22f6178671d3"
            }
          ]
        },
        {
          "id": "b399ab1c-4828-4cd7-8745-146a10dd7b8d",
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
              "id": "c2e01c8d-3088-4bd6-80d2-5b6cb3f5c36d"
            }
          ]
        },
        {
          "id": "b8b7656a-08ca-425e-893c-ab5c8bb75d74",
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
              "id": "ac5ead1c-1070-4e75-ac62-1e543834366b"
            }
          ]
        },
        {
          "id": "0729d047-0f93-409c-8645-8126d8e0f97c",
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
              "id": "850e4225-121d-495a-9042-5067fccd1154"
            }
          ]
        },
        {
          "id": "5254ee82-ed99-44d2-a067-c45ff6605b36",
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
              "id": "237e58ff-cb73-4fc0-97f8-2dcb1e776a38"
            }
          ]
        },
        {
          "id": "e713db56-3bae-4cd3-a761-e90628fedc35",
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
              "id": "7805c3af-0c8b-420f-ad1d-d00ab6a26919"
            }
          ]
        },
        {
          "id": "53576dcc-cae5-408c-a87e-4706b0fb6fee",
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
              "id": "8b608d7a-5d4f-4176-b2df-d0e9eac6f9d8"
            }
          ]
        },
        {
          "id": "975effe4-dd8b-43b0-939b-83c42ad5bf21",
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
              "id": "979e40ab-febd-4efc-bc92-efd43e9abeda"
            }
          ]
        },
        {
          "id": "d7e52730-1de9-49d8-b5c0-36559963fc24",
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
              "id": "8e0e143b-be26-4e60-93d2-50cb8bda8ab9"
            }
          ]
        },
        {
          "id": "7e3f50a6-ceba-46fa-a17d-bd0b9e4b98cb",
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
              "id": "557a7f61-1839-4919-a784-03ffce93cbde"
            }
          ]
        },
        {
          "id": "23d59ea3-62b5-4139-bc8f-856f088cdeec",
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
              "id": "206372bd-4c59-4fa9-be21-c97f50c66c4c"
            }
          ]
        },
        {
          "id": "974e03e0-9d4a-4be2-8e0a-7c58773f2f24",
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
              "id": "b0c00481-41c9-46fd-94dc-9eb1170d6224"
            }
          ]
        },
        {
          "id": "7573b5f3-8ec7-49e8-9fae-c97f8654719f",
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
              "id": "e8457928-a2ac-4eb9-8dcf-b9bc90cdd3dd"
            }
          ]
        },
        {
          "id": "fc1d12a2-ec39-400b-9a5e-2b2df1ae6fb7",
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
              "id": "d9618d8d-9434-4042-a7b6-89abbc03adb4"
            }
          ]
        },
        {
          "id": "381bd710-13ce-4ce5-80fa-4658314fd1a8",
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
              "id": "d8652658-6a31-4427-b66d-ab88052a968e"
            }
          ]
        },
        {
          "id": "ed4f074a-6646-469d-b1d4-15dac1f25bbc",
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
              "id": "4aeaa4e7-5835-4e28-985f-897a16bb5939"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "503f0e4d-74a9-4e46-b38a-26c672b6e60b",
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
              "id": "51a5efd3-a366-40ff-b880-0aebdba74118"
            }
          ]
        },
        {
          "id": "91479a4c-eb41-4fd3-97e4-4cc7232163b2",
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
              "id": "a09656ff-cb41-42c2-bd77-e4aa492df44f"
            }
          ]
        },
        {
          "id": "f3c42633-49e6-4f5a-9537-34d3d954c75c",
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
              "id": "fc470cf9-436e-4577-9335-321c0250080b"
            }
          ]
        },
        {
          "id": "afccaac6-d798-4a7f-8034-1a9404fef5ee",
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
              "id": "08470249-2f90-46b9-91ab-5b435c373381"
            }
          ]
        },
        {
          "id": "5340a5e0-eaab-4ba2-8b8f-59a5a36d77ab",
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
              "id": "127cde51-61b9-4cc1-8eed-bad98f4a2535"
            }
          ]
        },
        {
          "id": "60e71366-482f-483f-9c59-62f5cb88d24d",
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
              "id": "0d7ae4f6-1a7d-458a-bd43-fca6e5d818d0"
            }
          ]
        },
        {
          "id": "5fed6901-60cd-491c-b1ae-3a1e3211173a",
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
              "id": "a710235d-7ecd-43f0-9d7b-49964615e2d6"
            }
          ]
        },
        {
          "id": "85b499e2-eeb7-41c6-a560-eaf25c275147",
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
              "id": "d5e7c56d-fde9-4dbc-aaa3-657fe739a281"
            }
          ]
        },
        {
          "id": "6d5bc0fe-675e-4caa-96a6-8c4d5adcea14",
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
              "id": "fe76bcc6-bc4b-4ed2-9f24-0733a23d6f9b"
            }
          ]
        },
        {
          "id": "d15202f0-eaa5-4302-8024-fdf78db0d4d5",
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
              "id": "e006dac7-c269-4442-abb4-ed3326e3a787"
            }
          ]
        },
        {
          "id": "401e6ab7-1b27-4db6-8533-93035f9bf252",
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
              "id": "31892e97-85d2-4c10-a3ca-a15c3f128b90"
            }
          ]
        },
        {
          "id": "97b5a595-5812-4bf8-a15e-924d9eec8f27",
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
              "id": "2c31d2f1-ee76-4837-b069-5da1a25b8e84"
            }
          ]
        },
        {
          "id": "ebb1da5d-6947-4095-8a9b-797d93720177",
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
              "id": "141a1a8a-47e9-4ae3-9131-c6ce7e5f2d6a"
            }
          ]
        },
        {
          "id": "88cf96fd-0778-4342-a5bb-2796c3262b92",
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
              "id": "91866f9a-d086-4ad4-9698-dff985773cfa"
            }
          ]
        },
        {
          "id": "275894d0-7822-478a-a9fe-06307be6b51b",
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
              "id": "01266157-3a53-459b-a924-0af6dd816756"
            }
          ]
        }
      ]
    },
    {
      "name": "Prefs",
      "item": [
        {
          "id": "af2f270a-eca2-4d9e-94e7-2a17e9115052",
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
              "id": "16e67cbb-ffe5-4eb4-854d-e4cb85750aa9"
            }
          ]
        },
        {
          "id": "4eeca005-bef5-4f65-963a-feb222a138ba",
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
              "id": "c5f6503b-6096-4976-bedb-e25a8e683d81"
            }
          ]
        },
        {
          "id": "77486e58-9db4-48d1-88eb-4a23560caa18",
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
              "id": "02da174a-4d0c-4a09-9205-c87283c19a26"
            }
          ]
        },
        {
          "id": "e76285d6-5e51-4260-8e38-10e528e1347f",
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
              "id": "8d5aa9eb-3d7b-45c2-98e7-a4d27b7c775e"
            }
          ]
        },
        {
          "id": "c9bfd056-4d79-4757-ad82-0da8514720d6",
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
              "id": "30f590d4-a092-4b6e-999b-22e67294ba8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Reflection",
      "item": [
        {
          "id": "b4c89011-aeae-448f-adf9-92ff8524d0e7",
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
              "id": "cea96914-dffd-401b-98a2-f5ff1b38acfd"
            }
          ]
        },
        {
          "id": "9e457866-8e5b-49eb-b656-849482134ec3",
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
              "id": "2616578d-58d5-4ddc-80a3-8730e96acf63"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "762dc850-3324-4961-9b88-01060560f12f",
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
              "id": "17c51715-14cd-44a5-ba5d-506e285a5c17"
            }
          ]
        },
        {
          "id": "cee81eab-2d81-4250-9f57-b874506c1724",
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
              "id": "3d6469f2-d032-4d1a-8711-b35706786d51"
            }
          ]
        },
        {
          "id": "2d7957d4-4700-4d96-84c1-0f8d18932f54",
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
              "id": "6de32c0d-8a6c-4ea3-890d-99bc198a241c"
            }
          ]
        },
        {
          "id": "02ea2f2a-ccb7-4c02-beee-fef6f570403f",
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
              "id": "98e2379b-4509-48d5-bf72-f55e93e70849"
            }
          ]
        },
        {
          "id": "c5645a71-ad32-4f98-afa9-e1d0348a27c4",
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
              "id": "8c76f838-2718-44e9-93f7-50de2fc104a5"
            }
          ]
        },
        {
          "id": "640cf3c5-e80b-48e3-ac97-0bf6ab1b29c3",
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
              "id": "b9406f46-f4ab-4b81-a86f-ecb6ce113518"
            }
          ]
        },
        {
          "id": "2074ab31-bf28-45f1-9e97-dd66434ad3f5",
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
              "id": "430425fa-87ab-41e6-bd5a-cf0c6fc56915"
            }
          ]
        },
        {
          "id": "20db61f0-7ef6-438a-ae51-dc372b4733d2",
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
              "id": "925c9d06-7182-4d2e-8d43-8cddd7cf430a"
            }
          ]
        },
        {
          "id": "0c2538bb-5246-4438-8855-e3cf64977eba",
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
              "id": "69980666-0330-4dd3-9bcb-c3030b12b83f"
            }
          ]
        },
        {
          "id": "72116dd8-974f-4e26-ae8b-badf31304601",
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
              "id": "199fe3e6-168b-46f4-a3e4-93d82547ff0b"
            }
          ]
        },
        {
          "id": "dfd9cef5-e96f-4ced-8ab3-31fe1269d453",
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
              "id": "26d84b06-99e4-4ae6-be1a-f59a38b53d17"
            }
          ]
        },
        {
          "id": "27935119-73be-4b31-84f7-66b00c53c8c4",
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
              "id": "b75d9cb4-aed7-4324-acfb-413a5b49afbb"
            }
          ]
        },
        {
          "id": "2d607368-86ef-4bc0-87b2-66a1b86866b9",
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
              "id": "b5d2678a-0927-4270-9247-68741616596b"
            }
          ]
        },
        {
          "id": "68ce8e19-3b77-49f3-96c4-1b7a08cce5b5",
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
              "id": "e1ea94a9-4c1c-4291-a550-25f9eccb4551"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "41855641-7187-4fa7-8e56-18672e2c0ecd",
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
              "id": "d68248bf-0d2d-4571-b7e1-ff57740d4d85"
            }
          ]
        },
        {
          "id": "662ff52d-fd13-434b-954b-e9cfc8e15066",
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
              "id": "d229c898-3ba8-47f2-930f-e4b792233096"
            }
          ]
        },
        {
          "id": "c7825802-d26f-4584-8f4f-59481b200e84",
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
              "id": "16ffff55-3ea4-4656-842e-bf43f2b2a38b"
            }
          ]
        },
        {
          "id": "384323b4-be91-489e-8989-6033c1491cae",
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
              "id": "25e2c136-5276-4ab4-996a-e638f1a2d14d"
            }
          ]
        },
        {
          "id": "900c21d4-08e6-4e3f-a8d0-4bdb82c398b3",
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
              "id": "c7e8da94-8cae-46ee-a638-0095b73ea41e"
            }
          ]
        },
        {
          "id": "723bc610-b68b-4741-b55d-fc11b6b84a06",
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
              "id": "dad06003-a7a6-412b-9442-2c1e0e5d4955"
            }
          ]
        },
        {
          "id": "947608b3-0ca1-4a8b-9d62-62f19a1219ef",
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
              "id": "903b8e77-a887-4bf9-99ee-5c2014ee4f3f"
            }
          ]
        }
      ]
    }
  ]
}