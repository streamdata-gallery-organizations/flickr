---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Upload
  description: Uploads a photo. Uploading apps can call the flickr.people.getUploadStatus
    method in the regular API to obtain file and bandwidth limits for the user.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /upload:
    post:
      summary: Upload
      description: Uploads a photo. Uploading apps can call the flickr.people.getUploadStatus
        method in the regular API to obtain file and bandwidth limits for the user.
      operationId: postUpload
      x-api-path-slug: upload-post
      parameters:
      - in: query
        name: async
        description: Flickr can process photos in async mode, for applications that
          need to post multiple photos and dont want to wait around for each one to
          complete, leaving a socket connection open the whole time
      - in: query
        name: content_type
        description: Set to 1 for Photo, 2 for Screenshot, or 3 for Other
      - in: query
        name: description
        description: A description of the photo
      - in: query
        name: hidden
        description: Set to 1 to keep the photo in global search results, 2 to hide
          from public searches
      - in: query
        name: is_family
        description: Set to 0 for no, 1 for yes
      - in: query
        name: is_friend
        description: Set to 0 for no, 1 for yes
      - in: query
        name: is_public
        description: Set to 0 for no, 1 for yes
      - in: query
        name: safety_level
        description: Set to 1 for Safe, 2 for Moderate, or 3 for Restricted
      - in: query
        name: tags
        description: A space-seperated list of tags to apply to the photo
      - in: query
        name: title
        description: The title of the photo
      responses:
        200:
          description: OK
      tags:
      - Upload
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