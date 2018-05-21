{
  "info": {
    "name": "Flickr ",
    "_postman_id": "26c1e971-fb62-473c-9088-b3a4bcc2701e",
    "description": "Returns an access token",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "87e6d7e4-90ba-4509-a33c-0785cc9c80e9",
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
              "id": "2ad354ed-b6f0-4c33-bf7c-96a3f79c98e1"
            }
          ]
        },
        {
          "id": "6e05f315-4bed-4c51-956f-5656b0d094a8",
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
              "id": "319884bc-bdf1-424b-b9a3-366bebf41cae"
            }
          ]
        },
        {
          "id": "d8b5476a-f752-48a1-b62c-196cd79559cb",
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
              "id": "e3cfce16-fe15-4b38-b6a3-a7cb9f1bfbbb"
            }
          ]
        },
        {
          "id": "04f5b3ab-c762-4c00-8983-cff47d6680ee",
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
              "id": "2bad0e28-acb1-41cb-91fc-df71200ca4c5"
            }
          ]
        },
        {
          "id": "c3a921d3-04a1-4e39-b6a4-280ecc452cc3",
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
              "id": "c306fde9-dd2b-4577-9912-b7ef47a777f3"
            }
          ]
        },
        {
          "id": "ded42740-6f6c-4385-9cfa-8c17a84627fb",
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
              "id": "0964e1ec-0f51-417f-9f27-bd8237b3c636"
            }
          ]
        },
        {
          "id": "4655d22c-7794-4447-a0cd-94d9bd03d884",
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
              "id": "74f926b3-6bbe-4d98-b29d-22a2a2b13a8c"
            }
          ]
        },
        {
          "id": "b976df7c-a43e-4fbc-bd97-a4f6f88eb340",
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
              "id": "b26cd517-4314-4c2f-8e8c-aedf68d3dd0a"
            }
          ]
        },
        {
          "id": "d4e0b5ad-cbbd-471d-91c3-4e9b1f23cbe2",
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
              "id": "a730f539-8312-4e35-be58-e2187b0d3899"
            }
          ]
        },
        {
          "id": "a48fc0ec-c19e-4672-b1fc-4583ff46bea1",
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
              "id": "e7f3e3d6-183c-4577-a57a-153cbc53c434"
            }
          ]
        },
        {
          "id": "eb21e1c2-9597-47ae-a282-65272ffc68eb",
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
              "id": "0f18a02e-c203-4cba-8bdd-867433d3c83f"
            }
          ]
        },
        {
          "id": "4130f8a1-da0f-4477-9ffb-b32b85a36b02",
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
              "id": "fac3bde0-1617-4a1a-9173-163f4a7403fe"
            }
          ]
        },
        {
          "id": "bde8f0df-8459-4b0e-88d3-b98ba714c39c",
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
              "id": "1cc84a8e-5a2b-4a7b-b1c0-8edf46811db5"
            }
          ]
        },
        {
          "id": "45ddeb76-fbc8-4548-a682-72f6b1a8a601",
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
              "id": "2f0b9d91-843e-4fa3-9c94-b40bd1e6567b"
            }
          ]
        },
        {
          "id": "cbac9000-0df7-49d4-839e-827da655e863",
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
              "id": "35168056-90c8-45a2-afc0-5a1b3de9fba1"
            }
          ]
        },
        {
          "id": "8d5120f3-9fee-4426-8768-3e7aebb47a55",
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
              "id": "38fdd654-9884-43dd-8a5d-3fea7906985b"
            }
          ]
        },
        {
          "id": "4cffb048-1e64-44be-8a8d-c35d8d41c38d",
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
              "id": "3eead0c1-746f-41ee-8a95-faf9b7fe32ff"
            }
          ]
        },
        {
          "id": "7220976e-748b-44f4-ba8b-03c2ca449b06",
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
              "id": "d5d7868f-7dc7-424b-b365-8e8eed490b22"
            }
          ]
        },
        {
          "id": "25d5f4b3-2671-44ac-a3e4-18a50034e0b7",
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
              "id": "6b5925b1-3b96-4ff2-8085-8b202151e3f8"
            }
          ]
        },
        {
          "id": "9d1c8db6-bb38-452e-bbb2-6e831a6671b8",
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
              "id": "c170e6dc-3b43-44c6-a6b5-8e62d460a6ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "823b4730-b718-479e-a71d-0583c2b8bd17",
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
              "id": "57a24e84-69dd-4e63-b96b-dabc492261a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "525bd7e7-0779-4c96-b599-b3ee79b6b349",
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
              "id": "acc4ee69-afa2-4ba5-8bd1-e3fb0996fce2"
            }
          ]
        },
        {
          "id": "96a71eef-8294-4295-9d3c-fb8b98bb7306",
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
              "id": "a970f6de-3450-4e78-8740-c56fb9930321"
            }
          ]
        },
        {
          "id": "75ed9279-cc05-4c2f-a836-1fc3a83a4791",
          "name": "getRequestToken",
          "request": {
            "url": "http://api.flickr.com/services/oauth/request_token?oauth_callback=%7B%7D&oauth_consumer_key=%7B%7D&oauth_nonce=%7B%7D&oauth_signature=%7B%7D&oauth_signature_method=%7B%7D&oauth_timestamp=%7B%7D&oauth_version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an oauth token and oauth token secret"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd4e5558-b0d0-40a6-b911-b585cfcdfa5e"
            }
          ]
        },
        {
          "id": "f6af7b87-d13f-4d39-a626-20574a613ed9",
          "name": "getAccessToken",
          "request": {
            "url": "http://api.flickr.com/services/oauth/access_token?oauth_consumer_key=%7B%7D&oauth_nonce=%7B%7D&oauth_signature=%7B%7D&oauth_signature_method=%7B%7D&oauth_timestamp=%7B%7D&oauth_token=%7B%7D&oauth_verifier=%7B%7D&oauth_version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an access token"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e9a14be-0cc0-4089-a29e-93a21ec9b05f"
            }
          ]
        }
      ]
    }
  ]
}