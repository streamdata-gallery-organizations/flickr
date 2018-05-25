---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Get Favorite List
  description: Returns a list of the user's favorite photos. Only photos which the
    calling user has permission to see are returned.
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
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: "200"
  last_run: ~
  days_run: ~
  minute_run: ~
---