{
  "info": {
    "name": "Flickr Stats Get Photo Referrers",
    "_postman_id": "7f99f147-29a1-4328-bc75-1abee603db43",
    "description": "Get a list of referring domains for a photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "a70761e4-449c-43b1-a142-1899e51fdead",
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
              "id": "f53e6c4a-76d2-4c5a-bdf4-8c567aed64f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "95ae19a2-edce-4955-aa99-f5c8c1e9a74c",
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
              "id": "74a6305c-d129-4cbb-9283-a2a4661fefd8"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "687c2748-45c4-44c6-8512-dd556e7e40be",
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
              "id": "741b5862-53de-4523-91e6-80e652db7e44"
            }
          ]
        },
        {
          "id": "f90ac8c7-1b5f-41d5-bd7b-c7655d296b9a",
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
              "id": "d41b14d6-020a-49f7-9137-ecbb82218d55"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "3f3adf0c-b5e5-4ef3-a96e-f2b4e18c4ae6",
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
              "id": "2687afbf-b2a9-472c-8af7-c9a93c0d47f4"
            }
          ]
        },
        {
          "id": "c13c8b66-0305-442f-81a1-a88d962d7838",
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
              "id": "ce9a7ae9-d27f-4d23-9718-9d399264a807"
            }
          ]
        },
        {
          "id": "18abfa8e-b551-4fa8-ae3b-054cf4744dfc",
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
              "id": "87cd3374-4e16-448d-9907-c4c3520870fd"
            }
          ]
        },
        {
          "id": "d18dc832-90d6-4b5a-afb7-6d366afa2ea2",
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
              "id": "85e8f8ec-4b45-47af-b12e-64673f8194db"
            }
          ]
        },
        {
          "id": "de0efbae-8aeb-48b2-a845-acbfaeb58f37",
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
              "id": "1d898aaf-1507-4189-9daf-db86a333c138"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "3eb23374-96d9-4bf2-9d74-55a8ba06e226",
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
              "id": "9959bdd3-8b85-4cc1-9be9-db76c3f791de"
            }
          ]
        },
        {
          "id": "ead2e837-c6b2-4930-9cc1-20f32e4e070f",
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
              "id": "e021ab5c-baf6-4d86-be87-cbdf78ab3283"
            }
          ]
        },
        {
          "id": "3241ceb2-f757-420f-94c2-c600908d8640",
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
              "id": "9e49cfc6-7e1d-4ef5-a1b9-18b46e4b0135"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "5857974a-17b6-45c7-b20f-15d60f3990d0",
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
              "id": "044e46cb-95ee-4295-a4ee-3a466388066d"
            }
          ]
        },
        {
          "id": "b76efa27-a206-42ff-acc6-4a5486cdf670",
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
              "id": "692c0112-bbdb-4d9e-a374-ddb3dc725521"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "8909ab9d-9e0e-4920-a436-44bc6fbb2233",
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
              "id": "2d76b149-02d4-4710-9a8b-bd5ab477baf3"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "b739d77f-80ae-49c2-8b87-35b842dad92f",
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
              "id": "c78d0396-50eb-42bc-8ea2-ebf6949bc8a4"
            }
          ]
        },
        {
          "id": "28e11676-ec43-46b5-9d00-dc9e41550d4b",
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
              "id": "bb99ab07-f04b-4f7b-ad68-8b4338468a01"
            }
          ]
        },
        {
          "id": "3086b522-a3d8-42de-8428-8b31ae0c7ead",
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
              "id": "7981e117-97c6-4f9e-817a-3ecbb5474198"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "31b8b969-9f45-4225-920b-81f46bafeec4",
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
              "id": "3311ffe1-ab12-4341-8319-3c9e7c94a479"
            }
          ]
        },
        {
          "id": "3a8a269e-c75a-4702-8f83-98a0e2434f76",
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
              "id": "dd0a1cb6-878b-4a74-adc7-300fd2a0b0b3"
            }
          ]
        },
        {
          "id": "cb11e276-50f4-4793-90dc-03b808beb828",
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
              "id": "ee0e8a9e-a0a5-4714-914d-4c5087ee00a0"
            }
          ]
        },
        {
          "id": "165b0583-ac0e-4a00-b682-d7fdcefbe23d",
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
              "id": "fef7e4c2-8535-4c85-bcbf-af4c2e3ae4b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "b0b5b501-1f1d-461f-b244-7b46bdce43e5",
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
              "id": "3f6f3adb-3eb6-48a2-a512-d3c23a006ac9"
            }
          ]
        },
        {
          "id": "ae9b9a2b-421b-488a-8972-a06148c2ed3f",
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
              "id": "df8a128e-3066-43f7-b31d-49927d6977f9"
            }
          ]
        },
        {
          "id": "b24a2843-ec8c-47af-b3fa-34c34514fcb9",
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
              "id": "6044d3d7-d523-449c-b265-7ce623cfe6fd"
            }
          ]
        },
        {
          "id": "da84bdca-f25b-4527-8668-70af787e6176",
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
              "id": "4a1f6fd3-3ab3-4918-a98a-da7d69040524"
            }
          ]
        },
        {
          "id": "abdcebcd-604b-4ecb-bb68-60858e91f2ff",
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
              "id": "0f81b3a9-8f3b-48f4-84e5-c2b5119f4870"
            }
          ]
        },
        {
          "id": "1b692dce-5ff3-48af-8083-1c8c2568d6cc",
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
              "id": "ec37ec3e-891b-4ba0-92c5-cd3a0417d727"
            }
          ]
        },
        {
          "id": "9b93c98e-95ec-4d20-8044-4fc638b9c458",
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
              "id": "7f52b017-f0f9-4fd2-a6cc-8d9912cdfc26"
            }
          ]
        },
        {
          "id": "4e50cace-e9fa-4ba0-aece-764dd28922e7",
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
              "id": "a875b673-378f-47df-9b6a-1f5dd98d3813"
            }
          ]
        },
        {
          "id": "e897c496-54d5-4dd5-b15c-565607f9bd6f",
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
              "id": "987de0ad-da99-4540-8395-670ede601e56"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "aae1af42-320d-4750-846d-d9f74516a5ec",
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
              "id": "96b306d1-3b51-4c9e-968f-ea296e9c4592"
            }
          ]
        },
        {
          "id": "428eb2f7-5023-4611-a24d-63e158fae923",
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
              "id": "68c12b5a-e50e-4987-8786-31290d965e8e"
            }
          ]
        },
        {
          "id": "6703a3e8-75e1-4c89-96d1-0315ff5b2cdf",
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
              "id": "61bebf91-a085-4a77-a609-e12658952d08"
            }
          ]
        },
        {
          "id": "ff521f0d-df19-499c-8655-916579a7519c",
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
              "id": "3196c978-83bf-4a12-b08b-736518e179c9"
            }
          ]
        },
        {
          "id": "9d8c79df-aee7-4ebf-8f2f-907b17894d29",
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
              "id": "a03faa75-f0f0-4080-a115-3dcb63415d48"
            }
          ]
        },
        {
          "id": "3f498f0a-b1bf-4a64-ba7d-7d936a4ba02c",
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
              "id": "4f457668-39e7-4e20-bb1c-756acf895889"
            }
          ]
        },
        {
          "id": "a3818797-b386-4709-a669-2b3bd77ba372",
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
              "id": "491cc5c9-619c-4768-88b7-584eacb1f691"
            }
          ]
        },
        {
          "id": "69a854f4-5984-4a7e-a681-7cf4a23ef2d5",
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
              "id": "9d88e9c8-464d-4d41-aabe-0e80437cfd54"
            }
          ]
        },
        {
          "id": "1517032b-b7c7-4eae-aac4-005c29636269",
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
              "id": "aaf9ad65-7941-4975-b48b-caf536c6f3f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "253f1e51-a7a8-449f-99ee-443ef55d589c",
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
              "id": "51f04150-a700-4c0c-ac98-9bce202fa6fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "ecfa4eee-6c48-4774-b4e2-ac8e39109b1a",
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
              "id": "279be814-5905-44f5-9fae-db9ae44e904e"
            }
          ]
        },
        {
          "id": "5c86f253-a265-499b-aba9-87160b1a2537",
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
              "id": "8b02c0bc-29d7-4c32-b214-ad07bcaa410c"
            }
          ]
        },
        {
          "id": "78975e42-a26e-4cc7-bb8e-0142f77d62b6",
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
              "id": "1a818e10-1a0e-44ac-a16d-688a3e1a4aca"
            }
          ]
        },
        {
          "id": "c4edbe30-e33e-41be-93dc-dc1ac01818b8",
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
              "id": "c5b88524-b0c5-4802-9daa-a8543d346972"
            }
          ]
        },
        {
          "id": "705c4e17-754b-46f7-8537-a35041ce053b",
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
              "id": "d316e18b-7b8d-482c-b9e7-a1f3724df37d"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "f899ab3b-2724-449a-bf0b-ff3d5885a16e",
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
              "id": "6efd6194-c77a-425c-9328-c75330512b48"
            }
          ]
        },
        {
          "id": "207df82b-c7f4-4d5d-938c-2fb2aa2fdf5d",
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
              "id": "8ac093fc-2fc9-45cc-8ffe-cf454e44158b"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "4619f34a-79a3-4ddb-bc18-2e285555ad1c",
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
              "id": "435510ce-6a18-4eef-aecc-c7db9c46678e"
            }
          ]
        },
        {
          "id": "0b5c61e1-c24d-4c81-b8fd-b50b876012e8",
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
              "id": "45495352-b8a7-4502-9f2b-c120f7590082"
            }
          ]
        },
        {
          "id": "8503fd9f-8c58-4a54-ab24-c17959ba7a37",
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
              "id": "b230d2f4-6b3c-4272-975b-c60657696ebc"
            }
          ]
        },
        {
          "id": "7091375c-3068-424a-a796-6d3dc0d493ca",
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
              "id": "69483835-21fa-4856-acfb-a82e0c0cde05"
            }
          ]
        },
        {
          "id": "7cd33d38-5301-4d5e-8d9a-a2160bbf7702",
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
              "id": "d78a470c-e6d2-41c8-9a16-22be61f8b4db"
            }
          ]
        },
        {
          "id": "018dbcb9-acdb-4227-b37b-1dcc7cc7170f",
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
              "id": "621f9539-2d40-47d4-b924-354f70446275"
            }
          ]
        },
        {
          "id": "fa10c829-98c9-402e-ba36-60f2dfffa477",
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
              "id": "9955925c-5ff8-4b97-b715-175bfd08412b"
            }
          ]
        },
        {
          "id": "b4a74399-ab5b-4fe8-a4d0-2cb52187e6dd",
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
              "id": "a1ecc5b6-2901-41a2-a4d3-4046634e1485"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "76e902c6-a5a0-4cb0-b4ce-062d01b505f3",
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
              "id": "1e927b5e-60f0-48e4-bced-21726c64fbbb"
            }
          ]
        },
        {
          "id": "5d819855-a525-47f3-abe9-2846b9a285b5",
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
              "id": "5c687534-3877-4643-bbec-8ae1260578ba"
            }
          ]
        },
        {
          "id": "d43089e4-83f1-4839-9cff-503dc221fdee",
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
              "id": "f6df121a-6e2a-4297-b2c6-2c1eb515f9b1"
            }
          ]
        },
        {
          "id": "af21bcd2-be5f-4c77-a31e-6f57e90641d8",
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
              "id": "6e99d6b7-3d39-4489-9151-764cb09f980b"
            }
          ]
        },
        {
          "id": "7b675930-30c5-461d-8d14-830435dbe461",
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
              "id": "cc2eb085-6cf2-435b-a9c1-7beb36be208f"
            }
          ]
        },
        {
          "id": "52e8dfe3-c0e4-413e-b0ff-32d6f2fb6cec",
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
              "id": "47e2780a-5c53-42cb-a9ae-8d2a191b35da"
            }
          ]
        },
        {
          "id": "69e56aee-e0d8-4dd2-9e1f-6f332a56ceae",
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
              "id": "cf1a3047-4d1d-4d05-a5e7-b24a9c6ea453"
            }
          ]
        },
        {
          "id": "a336bede-7a16-4ccd-93a2-a21b8b4369fd",
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
              "id": "6c1b37fc-f3d7-4be2-a00f-ef058dd1364d"
            }
          ]
        },
        {
          "id": "e960fc95-9e36-4dd1-a802-57ca97f6df61",
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
              "id": "458c9249-f36a-4e6e-842b-46a1bc2c367f"
            }
          ]
        },
        {
          "id": "56dffd78-9a10-435d-937b-3d5539ffd8c1",
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
              "id": "3979297d-7d98-4cc9-acfe-19e69829a649"
            }
          ]
        },
        {
          "id": "bd30658c-605d-4dd9-b461-c4b7b2efccd2",
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
              "id": "3d7bad5b-47f0-4240-9cae-324817532390"
            }
          ]
        },
        {
          "id": "b63c58f8-61cc-4fd5-8bc0-9a826d28aa1f",
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
              "id": "e80c1f87-dd73-45ea-9f89-b78d1a561cb9"
            }
          ]
        },
        {
          "id": "8fb28086-effa-442d-ba1b-2bd9a496ed18",
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
              "id": "218d8148-8e6b-449e-959f-d4a52a9e95ca"
            }
          ]
        },
        {
          "id": "0f31756c-b977-4940-a2da-b8e2a73c3bd6",
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
              "id": "99e58662-0e81-4dfc-999e-ba5f720d3594"
            }
          ]
        },
        {
          "id": "3d2ab544-b3ea-424e-a575-db6247058da6",
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
              "id": "5c8ab3d6-fcd7-4620-a4ba-0e40c0e153b8"
            }
          ]
        },
        {
          "id": "fff22d88-9d06-47b1-9074-cafdea3b7696",
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
              "id": "6a516fb1-ab3a-4af3-8545-cf578b99a27c"
            }
          ]
        },
        {
          "id": "cfdb620e-334f-4769-bd0d-54d4eccc9064",
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
              "id": "8eb4c753-85fb-4cdb-81e0-9e7f99e5e764"
            }
          ]
        },
        {
          "id": "6d86d5a7-7a37-41ae-b825-ff043dc97f35",
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
              "id": "e19b6c25-3189-43f8-8fa1-a0cb85c17278"
            }
          ]
        },
        {
          "id": "a299c7b7-ba67-48f8-966d-1724b35a0446",
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
              "id": "41bff20b-8b1a-4422-9654-fcefecff3ac2"
            }
          ]
        },
        {
          "id": "59fdcfa8-f6b1-40db-b8ad-32820ffef3d3",
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
              "id": "8ab6256f-76a0-4643-bc17-08675061e709"
            }
          ]
        },
        {
          "id": "513e8f09-4d95-4ab7-972a-6a52e52cdafc",
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
              "id": "8a1cf608-3a24-43d1-b65a-62a0a975bb8c"
            }
          ]
        },
        {
          "id": "2aca30c1-4966-4154-bd61-df6fffb9da37",
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
              "id": "d996e6fd-9907-4d9b-a24d-91b07b53e134"
            }
          ]
        },
        {
          "id": "046e5a2c-8a99-4d6b-a946-a9c9c6320220",
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
              "id": "934f8497-0874-4081-acac-995f1ea66f14"
            }
          ]
        },
        {
          "id": "9a1d5e9d-06a3-43dc-9ba6-3426c60c36d6",
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
              "id": "960854d6-69a2-4799-af45-08529f100f21"
            }
          ]
        },
        {
          "id": "6e5e32ba-d0df-473d-a974-fa3cb60d6332",
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
              "id": "a250190f-42f9-4d45-b4ae-a07ece19918b"
            }
          ]
        },
        {
          "id": "f8582c15-acfc-47b3-a9ed-c2cf83b86d1c",
          "name": "postRestMethodFlickr.photos.settags",
          "request": {
            "url": "http://api.fl