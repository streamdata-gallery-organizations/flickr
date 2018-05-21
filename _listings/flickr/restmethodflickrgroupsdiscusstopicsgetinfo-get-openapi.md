---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Get Group Topic Info
  description: Get information about a group discussion topic
  termsOfService: https://www.flickr.com/services/api/tos/
  version: 1.0.0
host: api.flickr.com
basePath: /services
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest?method=flickr.favorites.getList:
    get:
      summary: Get Favorite List
      description: Returns a list of the user's favorite photos. Only photos which
        the calling user has permission to see are returned.
      operationId: getFavoritesByPersonID
      x-api-path-slug: restmethodflickrfavoritesgetlist-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: max_fave_date
      - in: query
        name: min_fave_date
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Favorites
  /rest?method=flickr.people.getPhotos:
    get:
      summary: Get People Photos
      description: Return photos from the given user's photostream
      operationId: getMediaByPersonID
      x-api-path-slug: restmethodflickrpeoplegetphotos-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: content_type
      - in: query
        name: max_taken_date
      - in: query
        name: max_upload_date
      - in: query
        name: min_taken_date
      - in: query
        name: min_upload_date
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: privacy_filter
      - in: query
        name: safe_search
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
  /rest?method=flickr.photosets.getList:
    get:
      summary: Get Photo Sets
      description: Returns the albums belonging to the specified user
      operationId: getAlbumsByPersonID
      x-api-path-slug: restmethodflickrphotosetsgetlist-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Photos
  /rest?method=flickr.favorites.getContext:
    get:
      summary: Get Favorite Context
      description: Returns next and previous favorites for a photo in a user's favorites
      operationId: getFavoritesContextByID
      x-api-path-slug: restmethodflickrfavoritesgetcontext-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photo_id
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Favorites
  /rest?method=flickr.groups.getInfo:
    get:
      summary: Get Groups
      description: Get information about a group
      operationId: getGroupByID
      x-api-path-slug: restmethodflickrgroupsgetinfo-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      - in: query
        name: group_path_alias
      - in: query
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
  /rest?method=flickr.groups.pools.getPhotos:
    get:
      summary: Get Group Pool Photos
      description: Returns a list of pool photos for a given group
      operationId: getGroupPhotosByID
      x-api-path-slug: restmethodflickrgroupspoolsgetphotos-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
  /rest?method=flickr.groups.discuss.topics.getList:
    get:
      summary: Get Group Topic List
      description: Get a list of discussion topics in a group.
      operationId: getGroupDiscussionsByID
      x-api-path-slug: restmethodflickrgroupsdiscusstopicsgetlist-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
  /rest?method=flickr.groups.discuss.replies.getInfo:
    get:
      summary: Get Group Replies
      description: Get information on a group topic reply
      operationId: getGroupTopicRepliesByID
      x-api-path-slug: restmethodflickrgroupsdiscussrepliesgetinfo-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      - in: query
        name: reply_id
      - in: query
        name: topic_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
  /rest?method=flickr.groups.discuss.topics.getInfo:
    get:
      summary: Get Group Topic Info
      description: Get information about a group discussion topic
      operationId: getGroupTopicByID
      x-api-path-slug: restmethodflickrgroupsdiscusstopicsgetinfo-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      - in: query
        name: topic_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---