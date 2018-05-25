---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Get Photo Sets
  description: Returns the albums belonging to the specified user
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
      x-api-path-slug: restmethodflickr-favorites-getlist-get
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
      x-api-path-slug: restmethodflickr-people-getphotos-get
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
      x-api-path-slug: restmethodflickr-photosets-getlist-get
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