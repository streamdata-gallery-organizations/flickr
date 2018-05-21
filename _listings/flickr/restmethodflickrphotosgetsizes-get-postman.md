{
  "info": {
    "name": "Flickr ",
    "_postman_id": "fb942e26-b046-4225-af13-43fc11923c63",
    "description": "Returns photo sizes",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "79716106-bb8a-47f7-8e8e-077d09af8ecf",
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
              "id": "50808705-4e35-4294-9274-c4d2a397f77f"
            }
          ]
        },
        {
          "id": "d0b7c8fa-aa6b-43cf-b0f6-c64ef7675703",
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
              "id": "c62f2bc9-338b-4069-9ff0-d3ccf75bdd89"
            }
          ]
        },
        {
          "id": "b23460b3-5c00-4481-b3ba-a0592e780c58",
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
              "id": "791cba8a-3992-474a-8bca-2ded2e907cc4"
            }
          ]
        },
        {
          "id": "8b7623b4-0624-424c-8eec-651de6f34d70",
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
              "id": "8455fe1b-8d06-49c4-895c-f6c160b1a122"
            }
          ]
        },
        {
          "id": "0080af66-8d90-4c3f-b1bb-0b632c104a60",
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
              "id": "b2447949-68b9-4f1a-badc-5711b8ff065c"
            }
          ]
        },
        {
          "id": "79b8d45e-800e-479c-9d1c-19015890acc6",
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
              "id": "b4fdae4b-41fd-4f02-beca-b21520ebdddf"
            }
          ]
        },
        {
          "id": "bc139417-cf5b-4976-8526-19d73b483393",
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
              "id": "5551bd14-92cf-4199-a6c2-e80182998b18"
            }
          ]
        },
        {
          "id": "45a11a54-cd36-48fe-8b25-24afe2e2d8a2",
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
              "id": "35e631fd-ef80-4edd-ba3c-8aa0b4ce624f"
            }
          ]
        },
        {
          "id": "32e5d1f6-ae03-4bf4-8cde-f5e0e5f17d5a",
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
              "id": "1da0919c-193b-45cf-941e-5a9172d65107"
            }
          ]
        },
        {
          "id": "83799f4b-3256-4d32-b1bc-8396bc3f8e90",
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
              "id": "e322f77c-b752-452a-849e-533e2664d70f"
            }
          ]
        },
        {
          "id": "a1fa2e85-3768-40bf-9fe4-99e2399ed54f",
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
              "id": "8dd4988c-14a1-4e80-8c6a-34f3b5cd7fa3"
            }
          ]
        },
        {
          "id": "a98813a5-fa8b-4fa0-972e-89cd9d073f45",
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
              "id": "f6351532-336d-43f7-b021-b8f94dff22da"
            }
          ]
        },
        {
          "id": "5d17dd16-e1b1-42d6-8ad5-102c89a029a8",
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
              "id": "68f84899-4172-4cdc-a136-5f751b7de3ec"
            }
          ]
        },
        {
          "id": "664c7195-5322-422e-a571-d2c91d0dfd6f",
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
              "id": "77ddea30-8c91-45c2-a913-0cc73fda23da"
            }
          ]
        },
        {
          "id": "38db3a29-4f0c-4b82-9026-25de0cdd61cf",
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
              "id": "e8e90132-b57e-4539-bcab-339a9a458626"
            }
          ]
        },
        {
          "id": "4073956e-364d-43c8-a07f-8732cdb1cea3",
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
              "id": "a50e3ca9-15db-491c-aae3-d5735987166f"
            }
          ]
        },
        {
          "id": "533558b2-ce00-4f96-b0eb-a5ed5e5f64e4",
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
              "id": "6062f790-9c8f-4c6e-af9f-3e5ccec44e56"
            }
          ]
        },
        {
          "id": "8e2e95d0-f79e-4f5f-82e8-9400cea1b98d",
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
              "id": "e6dcf952-fb09-480e-9735-d0aa665ceaef"
            }
          ]
        },
        {
          "id": "f02e43f4-ee8e-42bc-841e-d1135f9bfa12",
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
              "id": "fcd3ba07-22cb-4708-84c9-c07961233167"
            }
          ]
        },
        {
          "id": "4f3582e9-5832-4847-afa2-bd5296752b9c",
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
              "id": "32ae9779-4622-437f-a309-ed83594192eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "8d681460-3a5b-44f5-bd07-5b587896cb9e",
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
              "id": "b02e44c7-2941-4698-b0a0-a5adba385e81"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "b5cfda82-6d09-4cee-a760-ac1f9b5265e3",
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
              "id": "891229a4-4cac-4baa-98fa-43cd86d0a757"
            }
          ]
        }
      ]
    }
  ]
}