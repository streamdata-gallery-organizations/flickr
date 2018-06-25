{
  "info": {
    "name": "Flickr Test Login",
    "_postman_id": "1f5f9108-158a-4d80-8abe-d5e03cd2fc6d",
    "description": "A testing method which checks if the caller is logged in then returns their username.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "c1a0ebe1-cbce-4ddc-9a77-15c207596c9c",
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
              "id": "371f48d9-906c-4855-911d-0bb556af80d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "4e0a34dc-1be1-4359-802e-9b8e1ec66866",
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
              "id": "ed88d412-dfbf-49cc-9cf9-48d18c2e136e"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "44fe8d15-6879-4f17-8dce-6aad93ecce9a",
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
              "id": "eecee080-de0c-4c9e-a53b-6386c45949a5"
            }
          ]
        },
        {
          "id": "92ecb1b8-c994-4860-9a09-f8f693597c70",
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
              "id": "45f550ef-6638-4993-bc21-7573f6314f91"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "2559975d-909a-407a-a52f-117956c736de",
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
              "id": "8853cf21-d0ee-4f62-b1f9-01503d1e3bb0"
            }
          ]
        },
        {
          "id": "f100b628-380a-47f4-a885-705218436a59",
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
              "id": "dfc1dc38-d343-49e4-b1e7-5cade6770865"
            }
          ]
        },
        {
          "id": "8ac3fad7-4935-4a0b-beac-6d925a261dd6",
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
              "id": "823d56a3-3dac-4737-8e4c-48a5f7080054"
            }
          ]
        },
        {
          "id": "6f4d58b9-4911-4cfe-bd40-d34892bfb5f4",
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
              "id": "8b4cd646-bda7-443e-9807-dceb2e305075"
            }
          ]
        },
        {
          "id": "cd92af46-4a01-4095-bb19-2ada34210009",
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
              "id": "5cb8e5e2-a5f6-48c1-80ff-1391137b2c10"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "53755bde-00e1-48c5-ab88-a27ea2c3a1f5",
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
              "id": "72f25af6-0a10-418d-8884-94e5a847e28c"
            }
          ]
        },
        {
          "id": "7de7738b-847e-4898-b542-5a81fcb7687a",
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
              "id": "3232c2a3-c03b-46f6-9ade-419f2e82228a"
            }
          ]
        },
        {
          "id": "3eacab39-071e-4de8-a042-9e78c808f173",
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
              "id": "f6a96607-cc94-4bad-86ad-35863d3d9e7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "d84e7cd9-47ca-4e35-9312-67843a96d157",
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
              "id": "f57e79cc-99be-492b-8bed-97c9e0f8b85b"
            }
          ]
        },
        {
          "id": "a864007c-46fa-4c73-bab1-c680fef0d3ea",
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
              "id": "5187cf6d-0d3e-40d6-aaa3-a56cc86a8e93"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "52735f5d-4739-4fe6-8919-e62ab67ce193",
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
              "id": "db8fe38a-e726-4101-b4e8-696bfa8ec707"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "5adcfa28-7ff3-4334-bbfc-81f4d0be7467",
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
              "id": "5e4af25d-92e4-42f8-a664-26e25e5eabe6"
            }
          ]
        },
        {
          "id": "68206370-00b7-49a0-bd65-eb87dac22ef7",
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
              "id": "7c76dded-1b00-4c13-8b3a-8e466b73db07"
            }
          ]
        },
        {
          "id": "7ed81f00-b9ac-4efe-a8d3-48363921e507",
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
              "id": "3c067a17-b7c2-427c-8115-c4f67be1d72f"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "10d59df8-7c8f-4a95-88c1-7e4bebbf6b1f",
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
              "id": "c2119f32-47f7-4a85-8b11-ed894e0d31b4"
            }
          ]
        },
        {
          "id": "05ac67ca-febf-4624-bcc7-7a1ad401b366",
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
              "id": "1bef823f-2acf-4859-baf5-891703aaafd6"
            }
          ]
        },
        {
          "id": "fca4127d-66da-4b22-99fa-f2639ddb1d6e",
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
              "id": "acefa330-a184-4282-9bcb-d9c35a85cc36"
            }
          ]
        },
        {
          "id": "8ddc74da-6be2-49fe-bb8c-26abf363cdf6",
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
              "id": "bc3bc896-ef1a-4376-b4e3-1100e778f235"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "3bc3c5d2-eace-45a3-8ebe-3fedd1e90d93",
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
              "id": "fd6f5413-3e94-4495-a619-5cdf6d794aeb"
            }
          ]
        },
        {
          "id": "b6beddfe-3ff7-40c0-94b8-a086e7067262",
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
              "id": "67478336-f800-4b38-ba1f-bfae2111c7e4"
            }
          ]
        },
        {
          "id": "b721a737-c3ae-43ef-b625-683107461961",
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
              "id": "0f795e0f-9b3f-4158-8885-d307da96c34e"
            }
          ]
        },
        {
          "id": "d0a59695-3c35-4970-a8da-5e206a074c0e",
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
              "id": "bcb9e9b3-151c-4214-8be5-5bd664616595"
            }
          ]
        },
        {
          "id": "3f88e096-abd5-42f8-ac47-181e03b6a7ee",
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
              "id": "c7f6892f-14af-4727-87e5-b563e39f83aa"
            }
          ]
        },
        {
          "id": "1a96207e-8fbd-42f0-8e65-1ddc954770bd",
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
              "id": "a1c0a131-c5c1-4dcd-81c0-f1de5e7135b1"
            }
          ]
        },
        {
          "id": "86fd90ed-64e7-40e9-aaa7-0c427c260fe2",
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
              "id": "8b15ebc7-f527-44db-ac6c-ff219f0ed999"
            }
          ]
        },
        {
          "id": "eb1e74ba-4976-468e-858e-5410067a96ca",
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
              "id": "d77d1eba-7efd-4fc2-8757-da0d31346ac6"
            }
          ]
        },
        {
          "id": "33348082-dfd2-4202-a77b-bb4066f6947a",
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
              "id": "9d566c55-a3dc-480f-8258-108799ad8417"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "4a2ae6d3-241a-4452-a37f-66a82739b07f",
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
              "id": "e75af388-77dc-489a-bea2-4e47b87f301a"
            }
          ]
        },
        {
          "id": "7bea2c81-e206-416a-b7f6-2b3933e92d3e",
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
              "id": "0b242261-f607-408c-808a-229f426e7d7f"
            }
          ]
        },
        {
          "id": "1efdf753-1796-444c-9857-3324bb81e212",
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
              "id": "0c8de52d-8f0b-4cee-92f2-3d942093440b"
            }
          ]
        },
        {
          "id": "24481ce6-73ec-4c0d-860a-a373be5990f0",
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
              "id": "d53b8f2b-91dd-4a56-a609-a250526b9189"
            }
          ]
        },
        {
          "id": "5fd7e413-d844-4470-b850-a21f7838e1eb",
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
              "id": "a4b3b83e-db6d-4b1a-819c-fa66e073429e"
            }
          ]
        },
        {
          "id": "79fb4a5d-3540-49ba-b858-b548c4ec5eb7",
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
              "id": "75273759-c630-4de8-8ad1-e4f94c4b0df5"
            }
          ]
        },
        {
          "id": "86a961ae-9583-407c-b622-f0818d7bdbe7",
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
              "id": "f56f1df2-f59c-4989-ae08-37e272451a5d"
            }
          ]
        },
        {
          "id": "725337a6-4813-43d3-a440-e3798734a121",
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
              "id": "35b4e967-56e2-402a-bcf1-35bbcfb8d202"
            }
          ]
        },
        {
          "id": "6230a86f-41c6-4211-b355-0767457ccb8d",
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
              "id": "1f439c2f-e20b-4910-b59b-1803427dbca1"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "16ae6e1c-4b7c-4f1a-8961-44304f1727d6",
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
              "id": "0396524d-cfdc-48b9-801e-2539d71bbd1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "244c7f14-1481-41f0-849c-b3b852db632f",
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
              "id": "6c0085f6-742c-4e70-a04c-48f4b021617d"
            }
          ]
        },
        {
          "id": "421cd687-7c5f-475c-a1a4-c9b8abfb2416",
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
              "id": "5caf9276-a4c5-4ed9-ad1e-e063fcf0e62b"
            }
          ]
        },
        {
          "id": "ba0023bb-7c32-4e0e-912a-b4473a8133af",
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
              "id": "b52bf360-38a1-454f-8e53-a990d5908061"
            }
          ]
        },
        {
          "id": "09c3f77c-5c20-4760-b02c-5a7c33a0ad26",
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
              "id": "7150a20c-b033-433b-aabc-b3e8c287e172"
            }
          ]
        },
        {
          "id": "2eb3f981-e693-4f89-930b-db9c8461f003",
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
              "id": "6aa5c69e-2385-48ff-9aa4-3a548c7730e3"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "f2a0144e-82c8-47d3-990b-5caa927eafa3",
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
              "id": "0c6c7699-3e00-4392-9e8e-49c5f15cd3d3"
            }
          ]
        },
        {
          "id": "f814bbb7-75f5-4ec3-be0d-2fc3722dc0a5",
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
              "id": "da062d1e-37ed-4f6e-b173-0448cf90275b"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "1ec1f623-5751-4a69-a16a-1fe4fc6cedb2",
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
              "id": "ce3605f8-0cc9-45ac-a3bb-55c86ca66ef3"
            }
          ]
        },
        {
          "id": "c6e0638b-50b8-4c46-b831-8f9750edfb58",
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
              "id": "fe61a702-fe11-4c00-b97c-e944ef380d8c"
            }
          ]
        },
        {
          "id": "b41fdc7f-4138-43cb-9265-7ff4346eba6b",
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
              "id": "6112b8a4-ce24-4901-985d-e91a225be7e1"
            }
          ]
        },
        {
          "id": "1e77d83f-3442-4e82-83a2-0aae256be978",
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
              "id": "8cd8e545-6a0a-41e4-90a4-9a4f13854349"
            }
          ]
        },
        {
          "id": "9a77b734-f190-4a64-b159-6eaee95cd48c",
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
              "id": "f3fc7b66-2a48-4110-a8c3-8b4c023f9a37"
            }
          ]
        },
        {
          "id": "90a85f1b-4b3c-4b1b-b1be-51a2e3062b31",
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
              "id": "a14cab01-591b-40d2-8d7d-8775b767360d"
            }
          ]
        },
        {
          "id": "30242510-1b3c-4410-91dc-f971d3df0496",
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
              "id": "ee7b5682-bb7b-41a4-955e-d5772e6ffe63"
            }
          ]
        },
        {
          "id": "b432c5c1-59b1-4893-b591-6cd9f92999e6",
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
              "id": "217d5101-0795-4726-9a64-96500d092b2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "e7ad4a3a-eaa4-4b78-ae95-59c673e6a144",
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
              "id": "be3bdd52-5922-4432-837b-fb3cbbbb80c3"
            }
          ]
        },
        {
          "id": "f0053df3-07e5-4432-ae6d-844e02c9cac6",
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
              "id": "f8596af3-04b1-49a0-a26b-c1091ca371d6"
            }
          ]
        },
        {
          "id": "0b40e15a-8f9b-42a4-afe2-b1196dbf9527",
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
              "id": "84fa15f7-8ed1-4bc6-bf3b-bda1250d3c36"
            }
          ]
        },
        {
          "id": "2e01c48a-6e51-4f61-a4c1-4e9ca25f87fb",
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
              "id": "b4b47e31-0acb-4f96-8687-936c545e4bd3"
            }
          ]
        },
        {
          "id": "6fc7d225-fe14-441d-87b0-a15e3114361d",
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
              "id": "28c3aa16-73dd-4d80-be5a-f8455c63a2b1"
            }
          ]
        },
        {
          "id": "46176109-56d4-41c5-bc72-265728aa79d0",
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
              "id": "b2de6223-4ae2-4f38-acc6-929f01cbf9ca"
            }
          ]
        },
        {
          "id": "d55e9b73-ae52-4c6b-99ae-9eaa0687089c",
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
              "id": "19672dfe-21b1-4e62-b7e9-ff767c23bbc5"
            }
          ]
        },
        {
          "id": "43493dce-35ec-4a5e-bebe-45bb6ed1636d",
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
              "id": "74712408-306b-4c68-816e-8e20ca55543a"
            }
          ]
        },
        {
          "id": "5fc4b5a3-6f08-4d49-9f43-8e0b1a9a92cd",
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
              "id": "91bf9d07-1991-4419-9796-b8f169bbdcd4"
            }
          ]
        },
        {
          "id": "1a349dfa-731d-41b7-a2d8-e8240518b171",
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
              "id": "81226391-97bd-46e1-b74f-2e42bf767154"
            }
          ]
        },
        {
          "id": "5ad67239-040e-4f59-a0b5-2e1e051203a7",
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
              "id": "ec1988ae-daae-4bae-96fe-bb94e9f61b92"
            }
          ]
        },
        {
          "id": "ac2badaf-45ad-4b8c-b789-aea6ba197b23",
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
              "id": "393f7f3c-239a-4579-8537-cca56f31eaa2"
            }
          ]
        },
        {
          "id": "b9452bca-ba07-4a63-a0e1-efedea053c2b",
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
              "id": "eeb7e8ac-01ba-431a-98d8-3b368c72e705"
            }
          ]
        },
        {
          "id": "e41e72d9-ee50-45d7-8eff-4f7d22da9e2f",
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
              "id": "249ffeee-ee1c-4752-9382-2340297f1151"
            }
          ]
        },
        {
          "id": "dfbd1a43-fd5f-40e1-a146-3ef35430240a",
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
              "id": "799da3b5-8d0f-4905-89b0-cee0605688e9"
            }
          ]
        },
        {
          "id": "aab6c92d-3036-4eb4-a9e4-e3d82908dc87",
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
              "id": "7b9baf1d-1cdf-4c9a-b37f-9dcd1ec1a354"
            }
          ]
        },
        {
          "id": "c4134707-9b3e-4816-8bda-d27f68f81a5d",
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
              "id": "4a304186-79b6-4a52-ac49-24d2e29728e4"
            }
          ]
        },
        {
          "id": "472be413-ef96-4b7e-a5d4-828fc1b0ed4d",
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
              "id": "0db5ec7d-1b64-4360-901f-7d5cc51a04a4"
            }
          ]
        },
        {
          "id": "7f6501d2-61cd-4aa9-a241-0149226843ba",
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
              "id": "35e3527b-38d4-45dc-8873-40e708ea0a8e"
            }
          ]
        },
        {
          "id": "cc69545f-0f2d-4cad-b1ba-191745391a0a",
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
              "id": "0dd271aa-beb5-4166-bb30-0ba34fa6d2c7"
            }
          ]
        },
        {
          "id": "b7cef1d5-a939-48a8-8255-85fe9228f3a9",
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
              "id": "4ba6d790-245b-4d7b-9fa2-add36fba6c12"
            }
          ]
        },
        {
          "id": "f97d8237-8606-40a1-9d7e-b86dbd5001dc",
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
              "id": "e71b8d9d-e384-4d17-80ba-07b3458defc3"
            }
          ]
        },
        {
          "id": "4e27ee37-3c46-4087-8861-ef18ad8b17fd",
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
              "id": "48ac5948-ce1a-446d-84fb-503c7d4f869b"
            }
          ]
        },
        {
          "id": "fe8d1fa5-095f-47d1-a875-80576a630c69",
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
              "id": "0947d060-4532-457d-98ca-27e50dc7696a"
            }
          ]
        },
        {
          "id": "486387d4-2f89-4d37-ab0c-52c7132d73d3",
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
              "id": "412c715c-d991-4a30-a671-0893c8f026ba"
            }
          ]
        },
        {
          "id": "77aecebb-8d6a-442a-b57b-355c10d759eb",
          "name": "postRestMethodFlickr.photos.settags",
          "request": {
       