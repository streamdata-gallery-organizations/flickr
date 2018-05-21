{
  "info": {
    "name": "Flickr ",
    "_postman_id": "364f2719-f98f-48c1-b67c-5d972218b2c2",
    "description": "Returns an oauth token and oauth token secret",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Photos",
      "item": [
        {
          "id": "a0c8145e-1fee-4a4d-af4f-adfbe0d98c7e",
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
              "id": "c18511ea-9001-4a5e-a7a7-e7e7e48faf7c"
            }
          ]
        },
        {
          "id": "a8262686-7ad7-4042-b805-e0a9dd238b1a",
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
              "id": "5199ae3a-0357-4401-92fa-3dd0936074cd"
            }
          ]
        },
        {
          "id": "0d9ca2b3-e648-46be-80ef-41a59c4b82f9",
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
              "id": "4d94e560-b0c3-4e54-a3e8-ddf6a8508375"
            }
          ]
        },
        {
          "id": "45d391e6-08d0-4cd2-aa8a-f7ab7fcb5089",
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
              "id": "84a98ac4-ff08-481a-8ad8-9ed16f679016"
            }
          ]
        },
        {
          "id": "1896dcf7-e43c-4b87-be01-4853ad5c99e3",
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
              "id": "bc6d0c74-66bd-4e74-93da-59a12751abcc"
            }
          ]
        },
        {
          "id": "2292a5c2-bb91-4b8d-9100-46f530201cbf",
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
              "id": "bd79c233-a9ec-450a-85a7-bf11e5501eb9"
            }
          ]
        },
        {
          "id": "8ee64a00-d89d-4101-9e5f-0f5e77da8392",
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
              "id": "39e39518-0311-4328-9e7e-efc3180e8b8a"
            }
          ]
        },
        {
          "id": "99a09b9a-6345-4c5d-ae61-25f5ac7d17a5",
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
              "id": "bd28aa54-1bc7-40e3-9c02-06d756ee10af"
            }
          ]
        },
        {
          "id": "e3c5229e-f0b1-47df-b9d8-bf608d6828f4",
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
              "id": "7bea9ec2-084c-46e9-97c0-aad24d426bef"
            }
          ]
        },
        {
          "id": "89b311d1-a02d-4226-a530-9521cc8e2dac",
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
              "id": "c384e2c6-53b7-4dd9-bda1-989ab64314d8"
            }
          ]
        },
        {
          "id": "5634d64c-bc63-46f3-86cb-cbdf69cea5ac",
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
              "id": "fdcb1e62-054a-4ac4-9e26-0d68c0b19ecc"
            }
          ]
        },
        {
          "id": "e8e7f91f-b76c-4f81-a298-0d221442b071",
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
              "id": "ca257784-a6c2-48d1-a2fb-66bebaf166cc"
            }
          ]
        },
        {
          "id": "b9bce812-7787-4bce-bf8f-bb0232c22677",
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
              "id": "49b8e991-1ecb-4432-9cec-60813c2766f2"
            }
          ]
        },
        {
          "id": "2231e8bb-c91a-4e0c-9597-448137453c22",
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
              "id": "bd1eae07-70f2-4455-9682-ea359afecb67"
            }
          ]
        },
        {
          "id": "eff7f19a-8eef-44be-b4f5-3fcc91c906d0",
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
              "id": "bc60b5f1-7b31-4039-8cec-cef438cdde68"
            }
          ]
        },
        {
          "id": "05487519-40c2-44bf-a803-0c28d5996485",
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
              "id": "d08b2571-87af-4abb-9617-798260add5e1"
            }
          ]
        },
        {
          "id": "8a8eb67d-3fd4-4de2-9409-d3a49c239733",
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
              "id": "127586c6-748f-43e1-b3e1-5e089533756d"
            }
          ]
        },
        {
          "id": "b4b46603-be17-44a8-a084-38f26851522d",
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
              "id": "c31c008d-5655-46ab-abce-68812737b6fe"
            }
          ]
        },
        {
          "id": "e22b3993-b9b1-466e-b44f-1a1c3cb7a659",
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
              "id": "82cc93e1-2c9d-49ca-a320-f56a44e2891e"
            }
          ]
        },
        {
          "id": "19335c05-ad69-48c2-94c7-9c2678d055e0",
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
              "id": "bc2ca90a-4fbf-44f9-b27e-97a65d88714e"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "bdf0bc0f-c18f-446d-aac0-e32edc6d69c9",
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
              "id": "59779103-9711-4fdc-9d02-e99dcdb3cf68"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "682c2c2b-34c0-4b9f-9b55-27a1dc1d4211",
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
              "id": "e543cb13-daa8-4e64-be2a-462edb1a3e88"
            }
          ]
        },
        {
          "id": "224c8130-f0d0-4cc1-877f-f064196095ef",
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
              "id": "eec8a62c-7719-4a37-922f-2319981a8921"
            }
          ]
        },
        {
          "id": "22fdccda-83ae-475d-80fe-5da6764aceaf",
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
              "id": "10772a74-e045-4015-9dff-a61af54ad85e"
            }
          ]
        }
      ]
    }
  ]
}