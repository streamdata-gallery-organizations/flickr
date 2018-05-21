{
  "info": {
    "name": "Flickr ",
    "_postman_id": "8b92df84-b38d-4ce2-ab13-9c655303ed45",
    "description": "Echos the input parameters back in the response",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "06cece11-ddcf-4fec-94c2-af333bbfbd97",
          "name": "getFavoritesByPersonID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.favorites.getList?api_key=%7B%7D&max_fave_date=%7B%7D&min_fave_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
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
              "id": "57ae63fe-aa41-424b-93b6-6e77f2979f8c"
            }
          ]
        },
        {
          "id": "09d018d9-53ac-49f2-b324-240c46aec990",
          "name": "getMediaByPersonID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.people.getPhotos?api_key=%7B%7D&content_type=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&privacy_filter=%7B%7D&safe_search=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return photos from the given user's photostream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "045246b9-09b5-4545-bab7-5662b1bdd080"
            }
          ]
        },
        {
          "id": "0e3803a9-01af-4e97-8ca3-b01f9267aa39",
          "name": "getAlbumsByPersonID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getList?api_key=%7B%7D&page=%7B%7D&per_page=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the albums belonging to the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fa6c680-a335-4654-a40d-3f5c05cbe5c1"
            }
          ]
        },
        {
          "id": "28d4a89b-437e-44a6-a14c-f57bcbf55aa8",
          "name": "getFavoritesContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.favorites.getContext?api_key=%7B%7D&photo_id=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous favorites for a photo in a user's favorites"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0275399b-2b7d-436e-8862-319afff672d7"
            }
          ]
        },
        {
          "id": "07c8e366-694b-4e98-a6f5-23f05553920c",
          "name": "getGroupByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.getInfo?api_key=%7B%7D&group_id=%7B%7D&group_path_alias=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70693403-2654-40c3-b557-64ee2e375cc6"
            }
          ]
        },
        {
          "id": "85a54e85-bfb7-4764-89f7-301f58702deb",
          "name": "getGroupPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.pools.getPhotos?api_key=%7B%7D&group_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of pool photos for a given group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d1e1cc9-011b-474c-80cb-4a79778ae663"
            }
          ]
        },
        {
          "id": "8db44f13-4ef7-4b13-a7e5-4a165ea24605",
          "name": "getGroupDiscussionsByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.topics.getList?api_key=%7B%7D&group_id=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of discussion topics in a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "299726da-9178-4854-8fb1-d7a781781624"
            }
          ]
        },
        {
          "id": "c6f8fb49-70fa-4969-a14a-5bc3f1686cca",
          "name": "getGroupTopicRepliesByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.replies.getInfo?api_key=%7B%7D&group_id=%7B%7D&reply_id=%7B%7D&topic_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information on a group topic reply"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bee50271-eb69-46a8-9658-792a64e8e7f6"
            }
          ]
        },
        {
          "id": "d4712ae9-e787-4c58-b1ff-e6d041e0abde",
          "name": "getGroupTopicByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.discuss.topics.getInfo?api_key=%7B%7D&group_id=%7B%7D&topic_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group discussion topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe0b1136-ae9c-40cd-9d23-7d6bce183ddb"
            }
          ]
        },
        {
          "id": "a7d3f3c2-e226-4faf-981d-eb802dcd96d6",
          "name": "getGroupPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.groups.pools.getContext?api_key=%7B%7D&group_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a group pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f97bc44-e44c-4314-bd10-e374d646e790"
            }
          ]
        },
        {
          "id": "181ed30c-a40a-4bd2-81f7-3248873127ec",
          "name": "getPhotolistContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photolist.getContext?api_key=%7B%7D&photolist_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos in a photo list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d43d3a7d-abd7-4e66-b7e5-cc4800c0a1f8"
            }
          ]
        },
        {
          "id": "3a9428ef-b0c7-40b4-b08e-994c60528e1b",
          "name": "getPhotostreamContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getContext?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a photostream"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5aff7be9-c83b-480e-9fd5-4c0aeb1b6ed3"
            }
          ]
        },
        {
          "id": "e166b121-b0ee-4d33-a8a6-ecbcdfbc38a5",
          "name": "getLicenseByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.licenses.getInfo?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a list of available photo licenses for Flickr"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f00ac2a-4776-439d-8d94-20b418ec74a5"
            }
          ]
        },
        {
          "id": "758f1d90-0c43-434b-a1b7-5be9a2830b4b",
          "name": "getPersonByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.people.getInfo?api_key=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a person"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18b02910-33bd-4d7f-ad7a-18325c856c3b"
            }
          ]
        },
        {
          "id": "13d64210-9e77-4826-85ad-50c03b2c1466",
          "name": "getPhotoExifByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getExif?api_key=%7B%7D&photo_id=%7B%7D&secret=%7B%7D",
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
              "id": "d5b2a035-d721-4793-811d-fe5d8b3da60d"
            }
          ]
        },
        {
          "id": "65b0eddf-0c38-4112-bc9c-c478906d4301",
          "name": "getPhotoByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getInfo?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12a73004-f879-4695-ac47-aaf935c1668e"
            }
          ]
        },
        {
          "id": "49a5612c-71d6-4003-b510-a0a6b0f6acc5",
          "name": "getAlbumContextByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getContext?api_key=%7B%7D&photoset_id=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns next and previous photos for a photo in a set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5df4c2a-f92e-401c-bff3-67d4fdd9c54e"
            }
          ]
        },
        {
          "id": "5e98a10d-3b0a-4f7e-8872-7c2e8fc6f26b",
          "name": "getAlbumByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photosets.getPhotos?api_key=%7B%7D&photoset_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos in an album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eefb9806-1fbe-4252-8b59-4cc3aa4d76ca"
            }
          ]
        },
        {
          "id": "b4520657-93a5-4a79-a0b9-4df10ecb5a20",
          "name": "getGalleryPhotosByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.galleries.getPhotos?api_key=%7B%7D&gallery_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of photos in a gallery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25c39a9c-46a7-4380-ad3e-025065fcc843"
            }
          ]
        },
        {
          "id": "be613a62-9cef-43f8-abc7-ec1338920b5d",
          "name": "getMediaBySearch",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.search?accuracy=%7B%7D&api_key=%7B%7D&bbox=%7B%7D&contacts=%7B%7D&content_type=%7B%7D&geo_context=%7B%7D&group_id=%7B%7D&has_geo=%7B%7D&in_gallery=%7B%7D&is_commons=%7B%7D&is_getty=%7B%7D&lat=%7B%7D&license=%7B%7D&lon=%7B%7D&machine_tags=%7B%7D&machine_tag_mode=%7B%7D&max_taken_date=%7B%7D&max_upload_date=%7B%7D&media=%7B%7D&min_taken_date=%7B%7D&min_upload_date=%7B%7D&page=%7B%7D&per_page=%7B%7D&place_id=%7B%7D&privacy_filter=%7B%7D&radius=%7B%7D&radius_units=%7B%7D&safe_search=%7B%7D&sort=%7B%7D&tags=%7B%7D&text=%7B%7D&user_id=%7B%7D&woe_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of photos matching some criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec2a2244-aad9-4cd2-8f6b-6a2b780ab958"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "9bae0f60-cf05-400e-9797-14908788683b",
          "name": "uploadPhoto",
          "request": {
            "url": "http://api.flickr.com/services/upload",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "content_type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "hidden",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "is_family",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "is_friend",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "is_public",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "photo",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "safety_level",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tags",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Uploads a new photo to Flickr"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50c820d7-9aba-48bc-add9-b11ccc861153"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "5b748ba1-c50c-497e-8f0d-6f99f003ee5e",
          "name": "getPhotoSizesByID",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.photos.getSizes?api_key=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns photo sizes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9557ef0-6d60-497d-b457-7c9eb8437318"
            }
          ]
        },
        {
          "id": "fb21b3d8-67cb-448a-b99b-c12352e71ff9",
          "name": "echo",
          "request": {
            "url": "http://api.flickr.com/services/rest?method=flickr.test.echo?api_key=%7B%7D&echo=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Echos the input parameters back in the response"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fafc904f-64e7-49b1-ae59-964589a82426"
            }
          ]
        }
      ]
    }
  ]
}