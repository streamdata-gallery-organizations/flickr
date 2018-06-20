{
  "info": {
    "name": "Flickr Urls Lookup User",
    "_postman_id": "8ee51cfc-289d-4452-a23e-29d769e1e66d",
    "description": "Returns a user NSID, given the url to a user's photos or profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "e6de926a-2392-4875-b435-f987eae15bcf",
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
              "id": "fc194416-57d0-40df-8695-9050106bd56a"
            }
          ]
        }
      ]
    },
    {
      "name": "Replace",
      "item": [
        {
          "id": "51e853b4-d54b-409f-b601-9912ec855fb8",
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
              "id": "d14d45bc-d36e-46e3-94f0-c1a145294812"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "a8d8d874-fb50-4479-8e42-107350675b4e",
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
              "id": "029072bc-8892-42b7-9afd-d53767cbbfbf"
            }
          ]
        },
        {
          "id": "ef8b4564-3237-4d4d-b0cc-7114893b86dd",
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
              "id": "05891530-03d6-4d24-98e3-810bc926fe4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "eb31bb28-4940-40ea-a218-b576eb9d1843",
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
              "id": "66e63c82-192a-427d-ae38-32b43dad63ef"
            }
          ]
        },
        {
          "id": "9b74ccb4-b3c8-430b-8660-2e22f66689a6",
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
              "id": "f4d18e3f-96e7-4e42-ab34-c2f9817455c7"
            }
          ]
        },
        {
          "id": "551e9ba0-844a-4454-b86a-8619ecc6b9eb",
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
              "id": "86610b3a-5e68-46e8-8e33-67e4bbd4a44a"
            }
          ]
        },
        {
          "id": "a4c69dcc-a818-46a4-9df4-2a39c107693a",
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
              "id": "8b5206bb-3cc8-41e5-82a6-e0dddd964618"
            }
          ]
        },
        {
          "id": "73aac441-08ab-4d95-8660-7825d87e42e7",
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
              "id": "6dfdea27-afd3-4358-83fa-133102ef6e69"
            }
          ]
        }
      ]
    },
    {
      "name": "Blogs",
      "item": [
        {
          "id": "1352a936-86bb-4eaf-b1f3-067640fd5630",
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
              "id": "2541525e-3324-43f5-9f09-4de6c756f877"
            }
          ]
        },
        {
          "id": "16a0ce9a-902f-4623-b103-308a65f965af",
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
              "id": "67bca98c-5ab7-4e89-9efa-0bd42250f558"
            }
          ]
        },
        {
          "id": "a08189a4-91c9-4954-a399-286a1e4a7f56",
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
              "id": "48b694fc-d749-4fe4-a5db-e9722f1fe7cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "48db276b-0e2b-4d9b-b8a2-4af8eeb4985a",
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
              "id": "99d24da7-5a03-4c7f-a35e-48374181f3d3"
            }
          ]
        },
        {
          "id": "b4edc6ed-5e76-457d-bceb-11a24558fbc2",
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
              "id": "c137f789-66de-450f-bf5d-0d479124a53a"
            }
          ]
        }
      ]
    },
    {
      "name": "Commons",
      "item": [
        {
          "id": "7be5efd0-40b2-4d2f-a1a1-023f24217dea",
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
              "id": "20627a9d-2c0b-471d-bd6f-a6aa6308f164"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "5dad716a-d0a8-4e43-99b0-d7779a7889e7",
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
              "id": "5e8b164a-4c76-4081-bde7-69564ccc28ff"
            }
          ]
        },
        {
          "id": "45c67913-4f06-49f2-9897-7e6f18f91c3b",
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
              "id": "0d1aa1e9-b651-4a38-b59d-13f2a0c7ca19"
            }
          ]
        },
        {
          "id": "ca4a053d-ab1b-4d7f-a032-d0eafcdf4a9c",
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
              "id": "007f8b74-06d3-4d5c-b8c7-9cf5c3e1708c"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorites",
      "item": [
        {
          "id": "ac423f8a-b9a6-413c-9b91-60b88b39b4de",
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
              "id": "c9547168-0f7b-4e90-a349-26ee442b0e7d"
            }
          ]
        },
        {
          "id": "28bee831-9912-486d-bef1-b25c28b26f38",
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
              "id": "beefef0d-75cd-4cb2-9b31-a449e6d10dae"
            }
          ]
        },
        {
          "id": "72d47e85-3c5d-4eca-a395-33289e6f916f",
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
              "id": "1da2aa49-a285-4775-99a2-840cf12f8299"
            }
          ]
        },
        {
          "id": "0bf44862-f717-451b-8cba-cdd7cdd2f334",
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
              "id": "6f315d13-9324-4230-984e-adb59439a8f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Galleries",
      "item": [
        {
          "id": "88e799d7-f49f-40b3-89e7-6e1c45559a0f",
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
              "id": "06e89986-26c2-420d-839f-7091067de58c"
            }
          ]
        },
        {
          "id": "4a599a1e-7d8b-459a-a55e-274a96324b39",
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
              "id": "f234dffc-f93d-4b19-9835-255c02f205e8"
            }
          ]
        },
        {
          "id": "9edff235-fdc3-4c1e-84ab-36cce62a878b",
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
              "id": "721f19b0-e837-4eb8-8a15-b49225e6e70b"
            }
          ]
        },
        {
          "id": "00be95e3-d133-4ffe-8c99-9b56ea944cda",
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
              "id": "917cbe7b-ebd9-4d15-8824-c16f6e816f33"
            }
          ]
        },
        {
          "id": "d04f6039-ffe2-4e8b-a4e5-b328b93831c3",
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
              "id": "376fe52e-39df-4d0b-bf65-c484f6176097"
            }
          ]
        },
        {
          "id": "f6bd0813-2de5-4a08-9af8-d4d85e322a9b",
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
              "id": "187a9d58-a875-46ad-8f93-1eda333adb0b"
            }
          ]
        },
        {
          "id": "80ab87cb-ac13-4442-a331-2501b93ca349",
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
              "id": "e877e531-33c1-4e19-88da-194d9f529cd3"
            }
          ]
        },
        {
          "id": "ed05ba32-cad6-45cb-80c7-7b0e1bdb0b7d",
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
              "id": "b7f45cba-e22b-4a21-9bcc-2440ac2e5142"
            }
          ]
        },
        {
          "id": "599fa7fc-f630-48ae-9091-5cdad0382c27",
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
              "id": "ff8c345e-f372-4e9b-b3a0-141e0c0b6be3"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "6674d57d-39a2-41b3-9314-d6474bbaa83d",
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
              "id": "6b006e34-7c3a-4453-b1db-2a9e2c77c8f2"
            }
          ]
        },
        {
          "id": "b636548c-8121-441d-b57c-dc066b828351",
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
              "id": "66ed4692-97a3-493c-aba7-64fba48de629"
            }
          ]
        },
        {
          "id": "90600507-ec0d-4f72-81e2-6eb601c31e25",
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
              "id": "c0795210-3c75-4dee-bd9c-a190603fef53"
            }
          ]
        },
        {
          "id": "41c64fe4-844e-4ba5-8321-229aae617f50",
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
              "id": "5d20cb55-239f-4e2b-8321-4aacf69117dd"
            }
          ]
        },
        {
          "id": "717c099d-7e9b-4ee0-b55b-b315d491a3f3",
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
              "id": "62934ced-b522-45da-9ff8-498477c5ec40"
            }
          ]
        },
        {
          "id": "b79e5eb1-2f99-439c-9f6a-ed9f957b173b",
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
              "id": "005bc0ca-620e-4c51-a723-2a676e7cad77"
            }
          ]
        },
        {
          "id": "e1f0b178-f56a-4432-af3c-49e61011cfc3",
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
              "id": "232497b9-f98f-4d88-9bae-e55c6ea2a124"
            }
          ]
        },
        {
          "id": "b1395fee-a4d5-4407-9056-a32928e0b3d6",
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
              "id": "bcc1a8bb-678f-4b1d-b31a-d367c436c547"
            }
          ]
        },
        {
          "id": "5954a5e8-12f2-4430-85cf-49408e463345",
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
              "id": "d05c8a9d-6af6-490b-bfd4-34fe2ba9ca2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Interestingness",
      "item": [
        {
          "id": "1582d450-77d6-4e02-b37d-dee0d041839a",
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
              "id": "9e79512f-150d-4622-b5e1-73880b6e7960"
            }
          ]
        }
      ]
    },
    {
      "name": "Machinetags",
      "item": [
        {
          "id": "6ec5008d-e2d5-410b-ac29-ab1f004a82b8",
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
              "id": "eb9e970b-f541-4ab6-9543-561b185eaf63"
            }
          ]
        },
        {
          "id": "ca1731c7-68d0-4e12-83df-0d54536393dc",
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
              "id": "cd3ce936-5bad-4ca7-955b-56508cee0a07"
            }
          ]
        },
        {
          "id": "5569722f-5730-472a-bd1e-ac2eebcc6baf",
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
              "id": "83f8b0d6-445e-4b37-bf36-43ab5320cb66"
            }
          ]
        },
        {
          "id": "ec8fd837-0d56-4cb0-8031-026cbdd88f25",
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
              "id": "e79885f2-dc9f-497c-adab-fdd2e37bfd28"
            }
          ]
        },
        {
          "id": "b6717315-d14a-45de-b0a5-efa7ebd52bb6",
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
              "id": "451203f4-1854-4b7c-b7c7-7331f013f546"
            }
          ]
        }
      ]
    },
    {
      "name": "Panda",
      "item": [
        {
          "id": "9dda5155-fa91-4524-adb0-88c46e269643",
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
              "id": "d86aeea0-8f6a-4801-93bb-d0fd6baac094"
            }
          ]
        },
        {
          "id": "0caedae9-1421-48b7-8641-64190e3b4b7b",
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
              "id": "5e93412a-96a5-479b-8d41-b1ed9c2966cc"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "4384d739-9500-44c5-b8fc-13ccc67cdc9e",
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
              "id": "c8c00e64-4451-4f29-9b5f-4367e1585b21"
            }
          ]
        },
        {
          "id": "022ec4f8-eed8-433d-b9a7-dddeb1fadd35",
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
              "id": "d60e9175-81d7-4ab1-bea8-1511d699adf4"
            }
          ]
        },
        {
          "id": "2d315537-8560-42fb-bc16-6ac7ef0c18cd",
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
              "id": "4362071f-4521-4e6d-9c53-9d7ba0be8c32"
            }
          ]
        },
        {
          "id": "2d1d6b71-a487-4745-b8ee-87e8d269df4b",
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
              "id": "e9b0cf93-997d-4ad1-afe8-bd680f7f6e0a"
            }
          ]
        },
        {
          "id": "a57c6576-cfe8-4ce0-816d-046966a2b18f",
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
              "id": "7dc57b7b-cb03-4c09-92a9-176ce0a37348"
            }
          ]
        },
        {
          "id": "f364518a-7f8c-49aa-b536-6fe2d7897ff1",
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
              "id": "ae399275-38fd-48fc-b355-345b7b488594"
            }
          ]
        },
        {
          "id": "bba23896-ce19-450e-9391-a4bd658ce4cd",
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
              "id": "e1827930-c9a9-49df-9dea-51f65a124b50"
            }
          ]
        },
        {
          "id": "24d82e4a-78b1-4654-ad5c-56f44ce69fd0",
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
              "id": "356c9a70-b0e9-46bd-b52f-ad0d6d7817de"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "c747bfff-89f7-42ca-96eb-a30ceb3320f6",
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
              "id": "7d128ec4-980f-4cdf-932c-c4a16bae7f41"
            }
          ]
        },
        {
          "id": "067cdd62-f4ad-4f4f-849e-25638130240f",
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
              "id": "feceab08-2208-42d7-94d3-ca08e081f577"
            }
          ]
        },
        {
          "id": "d36401f0-deb6-4518-ad37-cea9fd5deaaa",
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
              "id": "7ec69efa-249e-4659-88fb-6eabd8154e3e"
            }
          ]
        },
        {
          "id": "27a13890-fbc9-4cb6-9edd-64e8b2811f90",
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
              "id": "34518c62-aee8-457f-85ce-1bad3d6e3bd1"
            }
          ]
        },
        {
          "id": "ca46b30e-b53a-41d5-81cc-b787c8507dec",
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
              "id": "e7b3457b-7d0d-4f18-a6ff-7090e571e5df"
            }
          ]
        },
        {
          "id": "1efc6cce-ad1e-469b-b049-2c9c093bc437",
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
              "id": "7667c262-2325-4302-9377-5d02ce1dc84c"
            }
          ]
        },
        {
          "id": "df27c090-e35b-4b74-be4e-ec4d4f611867",
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
              "id": "faabe64a-05fa-4f26-93a1-6f28c011e76e"
            }
          ]
        },
        {
          "id": "0ed20823-b68d-44fc-bbdc-ea9e40345ce7",
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
              "id": "26965d23-483f-472f-b697-547f01aabc93"
            }
          ]
        },
        {
          "id": "4dee6528-2fd0-4fe2-9dcc-ffef83ae0d83",
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
              "id": "d5660f60-1063-4920-a1c6-561167857029"
            }
          ]
        },
        {
          "id": "6a9c3834-5567-4512-a09b-08ddaba53b4b",
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
              "id": "7b29f541-3ce1-4877-9cd7-1e6f325410e6"
            }
          ]
        },
        {
          "id": "71873659-640b-49c1-a197-36bcab3e5ed3",
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
              "id": "2999b4d3-28a1-439c-ad7d-70ffe5ab0aa7"
            }
          ]
        },
        {
          "id": "7e7a724c-e03c-4e57-ace2-7eb3b0ab792c",
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
              "id": "bfab01ad-e965-4ef6-adb9-43aa42ad76c3"
            }
          ]
        },
        {
          "id": "6b8c4db5-3850-44cf-8c06-cba08908040f",
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
              "id": "e4c6d210-177a-46dd-970a-f3382dc3f79f"
            }
          ]
        },
        {
          "id": "c0d30810-2ed0-4e72-bad8-e44ae3371060",
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
              "id": "9ce7f420-3a47-47ae-8166-25a71fef5e06"
            }
          ]
        },
        {
          "id": "ca35eef3-5368-4112-9234-42d87c04ec7b",
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
              "id": "5ebe1450-61ae-462f-ad98-36ca0b39d8f8"
            }
          ]
        },
        {
          "id": "c58bb641-6bd3-4118-8f29-7ab1630c49bf",
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
              "id": "6d568fd2-3368-44d3-b18b-2524a3225fbc"
            }
          ]
        },
        {
          "id": "a715e9c0-25b5-42aa-aa7a-28fe138084e4",
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
              "id": "88871ced-5748-4529-9954-8f7d176e9605"
            }
          ]
        },
        {
          "id": "c443f9ea-0424-4a23-bf89-10d5d4924d52",
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
              "id": "ae53c332-1370-44ee-9994-5c5cd025afa7"
            }
          ]
        },
        {
          "id": "2ea335cb-909b-41c6-bb6f-fc60eadc8595",
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
              "id": "b6cb8d62-8345-4508-aaae-610d0d1b00f8"
            }
          ]
        },
        {
          "id": "d337c982-5b84-4255-b4e6-fa7d541a2131",
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
              "id": "aecda36b-69e8-4eed-b533-aa7ae3636a0f"
            }
          ]
        },
        {
          "id": "36a2dc3a-2cea-4df5-ac1b-94ac6f9ce90a",
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
              "id": "8672d252-ba3b-402b-ab89-4de5edb499a4"
            }
          ]
        },
        {
          "id": "180b152e-75e1-4eb6-98bd-7dae122d20b7",
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
              "id": "ea8ed20d-02ae-496e-9e22-4186b2795975"
            }
          ]
        },
        {
          "id": "32e369ca-98c4-4d6f-98b3-80900f6e72f6",
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
              "id": "43b7bd5f-5b2f-4c76-9474-6624cada9268"
            }
          ]
        },
        {
          "id": "e5b4735a-a03a-4edb-8dd3-18e603793c90",
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
              "id": "287f204d-8ba3-48eb-b997-76e992ad037f"
            }
          ]
        },
        {
          "id": "465f87ee-adfe-4cd3-a8f4-ed81a9f113ad",
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
              "id": "b5a2917c-cf2a-4a2c-a856-a42e611cf380"
            }
          ]
        },
        {
          "id": "b265ccf0-cf89-49b7-984f-311ed6b0b3bf",
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
              "id": "899cac86-2caa-493a-a347-bcffc870c719"
            }
          ]
        },
        {
          "id": "d1ec4176-3d6b-41fc-8060-50385d6b7693",
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
              "id": "44e5abfc-608b-435f-8959-c10591ee48c1"
            }
          ]
        },
        {
          "id": "6eed51ff-4da5-48c4-bcb3-2d0276921b1f",
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
              "id": "67705ce8-b1e0-40f5-a6ef-462fd34eb8e8"
            }
          ]
        },
        {
          "id": "07676b45-13d9-4e22-b8bf-6df5176f6afe",
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
              "id": "f9d88341-ee55-4080-9ed7-76d5bcb18ac4"
            }
          ]
        },
        {
          "id": "98b9fae1-7e33-49e8-99d7-01a4686108ea",
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
              "id": "d83d7f98-6947-4e1d-b895-1f8b3bf82577"
            }
          ]
        },
        {
          "id": "b1bb37f0-30f8-4c0e-8218-9dd2c00424aa",
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
              "id": "a17fee7f-f6cc-4575-8b1d-45a7298cd88a"
            }
          ]
        },
        {
          "id": "0b9e83c8-ea88-4c6d-8583-40c52fafed46",
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
              "id": "4d1bbb44-5c45-4619-a5b1-48727ce4dd0d"
            }
          ]
        },
        {
          "id": "492d4b2b-d7de-42fe-b8a0-c669cc9e0edc",
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
              "id": "091e65ff-a2fc-4fdc-9a92-871655051290"
            }
          ]
        },
        {
          "id": "e2dba64a-3618-41df-9853-e71681e58cce",
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
              "id": "59187239-b8ea-4aa1-87c2-9e26022db8c2"
            }
          ]
        },
        {
          "id": "4ca52dcc-5f1f-4de6-83a0-d5fbfafefacb",
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
              "id": "b1f5aed3-eaf0-44c6-91bd-f1dfc676fc22"
            }
          ]
        },
        {
          "id": "935fb9e4-bd2c-4cc6-8c24-1c47591b5d42",
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
              "id": "f9e2ce78-4015-4e60-975f-5445a825726c"
            }
          ]
        },
        {
          "id": "d53a644d-d2b6-4463-aa36-918fef754f7b",
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
              "id": "9f4caa1d-c481-4872-b203-3640d8a76e95"
            }
          ]
        },
        {
          "id": "83780eeb-114d-4dfe-9a07-4228521a1a7c",
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
              "id": "019cab08-f9a3-4996-ba6e-5e7e967853c5"
            }
          ]
        },
        {
          "id": "db5b1c22-2db8-4975-b0b8-30fdffd4f6e0",
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
              "id": "4b04be1a-80bc-4137-947c-9c7bcea93e04"
            }
          ]
        },
        {
          "id": "49e7c13f-17a6-47b1-96b6-5d70305d551e",
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
              "id": "f7a3d148-54d8-4302-99a9-5753b11abb66"
            }
          ]
        },
        {
          "id": "f310ed67-fc4d-4af0-995d-cbd5d18a7077",
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
              "id": "27de1f02-3b45-4c71-8e4b-4935160a820e"
            }
          ]
        },
        {
          "id": "8d4c09a0-73f8-4d59-bf66-31f51351c102",
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
              "id": "bb28201e-fafd-4e6f-8954-5d632174e7d3"
            }
          ]
        },
        {
          "id": "b0526739-e3ef-4075-8038-29b6a8397ca8",
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
              "id": "24db2f9c-77f7-447b-ad8e-6d26ce118a33"
            }
          ]
        },
        {
          "id": "57942f94-015c-4706-8f08-392a14ede96f",
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
              "id": "e069ef68-2cfd-4dd5-ac81-19eb7d44dd72"
            }
          ]
        },
        {
          "id": "d61956b7-85fb-4693-8579-866ba1249633",
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
              "id": "c5e63a43-1bcd-49ad-a102-e162164eb723"
            }
          ]
        },
        {
          "id": "b4d42e52-e881-4dc3-88f7-d7a91d2d897c",
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
              "id": "db75b4be-44b6-4efb-9cf6-29d33411b4c3"
            }
          ]
        },
        {
          "id": "1c4af113-fc9e-442b-985e-651e7744595d",
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
              "id": "b216496f-6ddd-403c-85ed-cbddad548edc"
            }
          ]
        },
        {
          "id": "b79b3d2b-8e45-4fc0-95fc-91853a8e2300",
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
              "id": "2453bb76-883e-496d-ae91-2b3833946eaf"
            }
          ]
        },
        {
          "id": "c1714f9d-4315-4dfd-b557-f18cad804a4a",
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
              "id": "4b315fee-b77e-4f92-9e81-d96e177e095a"
            }
          ]
        },
        {
          "id": "6fa2ba57-00a1-458f-b2c6-238ff907e840",
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
              "id": "6a73c7bd-3bd3-493e-b503-9f98109e24e6"
            }
          ]
        },
        {
          "id": "7b43fb54-e539-4cf8-b526-efb2be50ec2b",
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
              "id": "97f51a86-9916-49a9-93d8-d6901ec598a2"
            }
          ]
        },
        {
          "id": "eeb38113-d089-4e31-8d97-18487aaaa764",
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
              "id": "1772e9fe-b608-4276-9397-64fff80b9efd"
            }
          ]
        }
      ]
    },
    {
      "name": "Photosets",
      "item": [
        {
          "id": "af2ce7ed-aa54-4b96-91b2-06469670aec5",
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
              "id": "a952746d-ddce-42d6-bc11-ca9d0ad86c51"
            }
          ]
        },
        {
          "id": "351dca73-305b-40de-8a9e-7cc0559b4770",
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
              "id": "b588ffab-ee32-4290-a023-f970ce92c7dc"
            }
          ]
        },
        {
          "id": "d99d7944-5ab4-4504-8fb3-620ac3246309",
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
              "id": "cf000041-f56e-42ef-b666-62eb8dd1fc7e"
            }
          ]
        },
        {
          "id": "2c2264f2-5562-4563-90cb-a28de86b5403",
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
              "id": "9a961bf9-5abc-4f14-96cb-1557c4641b6d"
            }
          ]
        },
        {
          "id": "f76987fb-530b-467d-a89a-f773eabb9d11",
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
              "id": "59cb63ea-027e-40e0-972f-9f5813d3131b"
            }
          ]
        },
        {
          "id": "ca330300-79c6-498c-ae38-e23227918530",
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
              "id": "a8bb2e0d-4355-49c0-b6d7-dab7e778e424"
            }
          ]
        },
        {
          "id": "bb302747-8c24-4bfb-b047-a107bc620719",
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
              "id": "92c3eb60-aee0-4824-9799-33aa2aaa5cae"
            }
          ]
        },
        {
          "id": "effa2e66-a433-4218-ae47-db1c3806933e",
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
              "id": "72254109-d2ff-4ead-9f87-219053371e73"
            }
          ]
        },
        {
          "id": "7b4328b1-867a-44ad-8082-44331e08c15d",
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
              "id": "50a7c496-5eb3-43d4-b586-9508548cd96e"
            }
          ]
        },
        {
          "id": "62932709-2781-485c-b68b-c0aaee276831",
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
              "id": "b68a1784-65f2-47ea-acef-750e973ac525"
            }
          ]
        },
        {
          "id": "724132a5-edf9-444f-85a3-24618e8217f9",
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
              "id": "93f121b3-e2ee-4ff5-bd08-1160ff3bdd25"
            }
          ]
        },
        {
          "id": "02e6c22c-c30b-421e-9d8f-06041e01fcf9",
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
              "id": "f739ae71-9bc3-4014-9e1a-28ed230128d6"
            }
          ]
        },
        {
          "id": "b0fe25e1-0753-448b-b5e3-d58ee9420ed0",
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
              "id": "5925354e-321a-457f-ace6-65d12e29e309"
            }
          ]
        },
        {
          "id": "eaa5eb0d-fa94-4df2-9f6c-aa4a52641fe1",
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
              "id": "35490d8e-8bcc-458e-be79-de130ed8f789"
            }
          ]
        },
        {
          "id": "04ce722d-efc5-48dd-9ee4-a357fb492acb",
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
              "id": "4d957b1c-e8d5-41d8-8a19-7c776d39d07a"
            }
          ]
        },
        {
          "id": "8502e13e-c26b-4288-90cd-28f2905eeebc",
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
              "id": "3448e5d6-8408-4a0e-8bfe-0279b037e2d3"
            }
          ]
        },
        {
          "id": "1a181560-1d44-4811-b6f5-758cc5c688f0",
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
              "id": "8e85d433-c83f-44db-8dbf-2ac0b330f54c"
            }
          ]
        },
        {
          "id": "bcd1975b-10c6-42ca-a396-9ce948443fd3",
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
              "id": "d8ed1da7-0206-4efc-91ca-22a625f1b2d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "20701484-3a7e-4679-93d0-b0e2273a46c5",
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
              "id": "66167e24-86bb-473c-8cd1-74992c3937a6"
            }
          ]
        },
        {
          "id": "fd40d368-29d6-4c8d-b4a5-a076ec2e2717",
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
              "id": "3193afae-0334-4145-9897-e9d0bd9bf3a9"
            }
          ]
        },
        {
          "id": "8f614c64-81e8-478d-b648-7bb11702e3d0",
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
              "id": "5a3a42d9-1c39-4fbe-9e84-986c95a9c6bf"
            }
          ]
        },
        {
          "id": "9a59ef26-900c-4dc9-b637-017f140e549e",
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
              "id": "6a82c4af-0a3f-4906-b95f-fcfeba70f78f"
            }
          ]
        },
        {
          "id": "0bbdef66-aac0-4280-bdb8-c1622f933d29",
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
              "id": "790731d1-2200-4026-8fb0-11ae3600c691"
            }
          ]
        },
        {
          "id": "51e046d5-e6e7-4dab-84e8-5aa5f97515da",
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
              "id": "280bead7-6146-4448-a881-87720bfcc540"
            }
          ]
        },
        {
          "id": "31c04a98-8ad0-4e9a-b625-4683d66a5038",
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
              "id": "da2fe8a7-c303-4160-96c1-7db279c72b2e"
            }
          ]
        },
        {
          "id": "c4793fd2-a2c1-4fab-8815-1d3d3d85aed5",
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
              "id": "27607ba3-72ef-481f-89d0-1bda3d68cad5"
            }
          ]
        },
        {
          "id": "80fd5a66-2367-4649-a4af-d642ac43da30",
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
              "id": "5e89ed60-b3d6-4f12-8c03-2bd0ebc70d8a"
            }
          ]
        },
        {
          "id": "48c1355b-967d-49be-9790-2eaf71ef7ba7",
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
              "id": "cf5f516c-1b10-491c-b727-efb5beba3856"
            }
          ]
        },
        {
          "id": "413649ae-4cff-4bb6-8b4a-35188a57c99c",
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
              "id": "ad1ccbc6-b496-46d6-b6cd-f8171fb6df17"
            }
          ]
        },
        {
          "id": "69fd79c2-70b0-4b7b-bbe1-864b787ea990",
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
              "id": "c0338f4f-38af-4e2f-9056-102b0d10ed8b"
            }
          ]
        },
        {
          "id": "a65574aa-487c-46da-a1d5-15e7e7283144",
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
              "id": "65c31a49-3a7c-4c0d-b8fb-c7dca6318b2e"
            }
          ]
        },
        {
          "id": "781a45eb-9aac-4ddf-b909-8c250a1d5206",
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
              "id": "25c02a94-65c7-4ab5-862f-7dd17162403c"
            }
          ]
        },
        {
          "id": "7601ff9d-8c71-4897-968f-3193126d2387",
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
              "id": "5bf3492a-dc8e-4e2f-8a45-426274e74852"
            }
          ]
        }
      ]
    },
    {
      "name": "Prefs",
      "item": [
        {
          "id": "87c1e0fe-d42e-40c6-865a-ddc5db024b18",
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
              "id": "49fbb7ab-7783-4b33-a3cb-0f62bd40fce5"
            }
          ]
        },
        {
          "id": "8d495a58-4407-49ef-ba04-3c51369f4065",
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
              "id": "677564dd-3205-4d50-acdc-4c2b0f91390f"
            }
          ]
        },
        {
          "id": "1aedad69-7fe8-4ffb-a100-da5b48e06d38",
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
              "id": "6f34b2b9-505e-4e9e-8962-b2b8f83a80c3"
            }
          ]
        },
        {
          "id": "5b401da4-f2df-409a-8bba-0b59854bf7ce",
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
              "id": "97b43436-bf76-4f59-a38b-1d37f49ba285"
            }
          ]
        },
        {
          "id": "31075283-e958-4d2b-908a-515678c75891",
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
              "id": "1ce6317b-2691-4c7e-b7a2-18d55b80848b"
            }
          ]
        }
      ]
    },
    {
      "name": "Reflection",
      "item": [
        {
          "id": "8946265a-0b0d-47fd-a62f-e848a65eed7d",
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
              "id": "51010840-faae-4bc5-943f-f56d91079413"
            }
          ]
        },
        {
          "id": "4562afb1-53ba-49fe-9a4e-e9430acc0b25",
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
              "id": "ddbe5072-2ccc-4614-ac1c-4f278f23808d"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "392f829b-9dc5-4459-98e3-685ba028a622",
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
              "id": "d16b4fbf-02ad-40e8-a2e8-532ae7ef0535"
            }
          ]
        },
        {
          "id": "58053de1-df07-4475-b7f3-864d7f60c13b",
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
              "id": "eb4ff2c3-3ead-44e8-8c20-04792ab048a5"
            }
          ]
        },
        {
          "id": "e5f43974-7e54-4ed7-a908-cbead69c1be8",
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
              "id": "fcaae64a-8020-423d-9415-4da07b48762b"
            }
          ]
        },
        {
          "id": "d27c4693-e1d5-4eec-8d23-2497600702da",
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
              "id": "5dc4b872-661f-4c94-b94f-3d80463b5663"
            }
          ]
        },
        {
          "id": "7b3bda70-1520-404b-aaa3-095175928ce5",
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
              "id": "0b099aca-755e-482d-82e5-bec683006ae4"
            }
          ]
        },
        {
          "id": "a9c911ff-874d-420d-81b6-adad25887a3b",
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
              "id": "ed7099c1-7118-4940-8554-08a54a0e88af"
            }
          ]
        },
        {
          "id": "53ae487b-7b8f-4969-bc24-25c385b6fa6a",
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
              "id": "73d5723a-2a9c-4c40-a1ca-643048a053ed"
            }
          ]
        },
        {
          "id": "e03cea66-5f71-43c7-ba78-a38f687d4707",
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
              "id": "d49e9265-c5a3-494f-99e7-5c588e759b77"
            }
          ]
        },
        {
          "id": "45a4cd09-eff9-4dc6-a8eb-aa040bb73ff5",
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
              "id": "8eeec00b-b714-41ef-9174-d92973b85396"
            }
          ]
        },
        {
          "id": "7dbbfe43-2109-4ba2-a9c4-b4113c117271",
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
              "id": "951cdeab-9855-4986-9519-9c4a4692e530"
            }
          ]
        },
        {
          "id": "3bbdc4c1-52e2-4a5a-9b2d-dbf10de6f16c",
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
              "id": "50db3b1e-2c8c-4a18-afdc-083940194512"
            }
          ]
        },
        {
          "id": "8cfb90bb-a759-4ec6-97b5-6c6aa117b44d",
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
              "id": "97046e6a-6704-4a11-addf-92d4e07011f2"
            }
          ]
        },
        {
          "id": "ac64af8f-7d9d-4685-b401-e4b9a9033323",
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
              "id": "7c607676-f5f0-477d-b3d4-c120d0948065"
            }
          ]
        },
        {
          "id": "6494d7c6-4d93-4fbf-9c82-0bb5a2c6b296",
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
              "id": "0c3f7b12-d01a-4344-b4f5-5f8853ea57f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "a7c7e4f1-e7e1-4af2-a1a6-54d63bedaac4",
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
              "id": "4d829206-da3b-4ba9-aef8-59679dd342ba"
            }
          ]
        },
        {
          "id": "3443e17c-916c-43a8-90f4-ca96174a8d7c",
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
              "id": "b2f7c2d8-8e8c-456a-a41d-d451442e3f81"
            }
          ]
        },
        {
          "id": "95306e08-af77-46c0-8d2d-0b642ece50ae",
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
              "id": "80a90fd6-3903-45a0-a33a-347863d254cf"
            }
          ]
        },
        {
          "id": "d2af4287-8184-4b42-b843-59c073a17f85",
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
              "id": "4fb1afe7-6559-4db1-82fe-d72bd4dbbbbd"
            }
          ]
        },
        {
          "id": "127877cb-9f05-42e5-9506-24c1d548dcb8",
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
              "id": "9ed19901-1fbb-4a8d-b907-7c1dc891a4f4"
            }
          ]
        },
        {
          "id": "2cb91a7a-13fb-4e90-8742-dc3d174ac0e9",
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
              "id": "54e01a12-22b4-4b12-993d-b31c255269bb"
            }
          ]
        },
        {
          "id": "ec875c06-365a-45c2-910a-73258b677e3f",
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
              "id": "dd627757-8122-4a8f-a339-b713380630ed"
            }
          ]
        },
        {
          "id": "db96e6b1-8961-475c-be47-ff102d3807af",
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
              "id": "d3f41543-5b5f-488e-8b08-668ad081474d"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "7c2a1df8-c6cb-4346-9f1b-c55d6d41aec2",
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
              "id": "a872c500-432e-4994-b0ba-ddfec6eefdda"
            }
          ]
        },
        {
          "id": "b322d7cb-654d-4114-ae77-05c948cd5e38",
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
              "id": "89f213d7-0ddb-4377-b685-334bbeaf3b5b"
            }
          ]
        },
        {
          "id": "049f3285-d8d1-4a18-a5f9-e713e215b8b9",
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
              "id": "17f9286c-4ba7-413c-9629-5802ad366ec0"
            }
          ]
        }
      ]
    },
    {
      "name": "Urls",
      "item": [
        {
          "id": "4a57c274-7541-419b-b5d6-29cb0bcdefaa",
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
              "id": "bc4adee4-f19f-4a9a-a7b1-fa6f840cfce9"
            }
          ]
        },
        {
          "id": "75299ae7-6f88-4289-9533-8fc3379069e8",
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
              "id": "9d88ffde-421c-4a1f-9ebf-4a87c124de70"
            }
          ]
        },
        {
          "id": "7ff5c06d-d5c3-41b0-a5c8-c88bf0190379",
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
              "id": "5dccc659-aa17-4e0e-8272-f62dc5e0ec66"
            }
          ]
        },
        {
          "id": "33824dee-6269-475c-adb4-7bfcf971cb73",
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
              "id": "8357f61b-7aec-4c37-8d15-e1062c1b164b"
            }
          ]
        },
        {
          "id": "08083cfb-5d00-4463-abc9-527df8ffb92c",
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
              "id": "73c5bf95-d3cd-4653-84db-e9c845e1dc0f"
            }
          ]
        },
        {
          "id": "27d69ffb-7167-4f81-a76f-65014b64484f",
          "name": "getRestMethodFlickr.urls.lookupuser",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.urls.lookupUser?api_key=%7B%7D&format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a user NSID, given the url to a user's photos or profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43e0fd03-455c-444d-9c81-0e9ae58aa8b6"
            }
          ]
        }
      ]
    }
  ]
}