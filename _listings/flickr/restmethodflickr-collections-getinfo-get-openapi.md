---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Collections Get Info
  description: Returns information for a single collection. Currently can only be
    called by the collection owner, this may change.
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
  /replace:
    post:
      summary: Replace
      description: Replaces a photo that has already been uploaded to Flickr. Uploading
        apps can call the flickr.people.getUploadStatus method in the regular API
        to obtain file and bandwidth limits for the user.
      operationId: postReplace
      x-api-path-slug: replace-post
      parameters:
      - in: query
        name: async
        description: Photos may be replaced in async mode, for applications that dont
          want to wait around for an upload to complete, leaving a socket connection
          open the whole time
      - in: query
        name: photo_id
        description: The ID of the photo to replace
      responses:
        200:
          description: OK
      tags:
      - Replace
  /rest/?method=flickr.activity.userComments:
    get:
      summary: Activity User Comments
      description: Returns a list of recent activity on photos commented on by the
        calling user. Do not poll this method more than once an hour.
      operationId: getRestMethodFlickr.activity.usercomments
      x-api-path-slug: restmethodflickr-activity-usercomments-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of items to return per page
      responses:
        200:
          description: OK
      tags:
      - Activity
      - UserComments
  /rest/?method=flickr.activity.userPhotos:
    get:
      summary: Activity User Photos
      description: Returns a list of recent activity on photos commented on by the
        calling user. Do not poll this method more than once an hour.
      operationId: getRestMethodFlickr.activity.userphotos
      x-api-path-slug: restmethodflickr-activity-userphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of items to return per page
      - in: query
        name: timeframe
        description: The timeframe in which to return updates for
      responses:
        200:
          description: OK
      tags:
      - Activity
      - UserPhotos
  /rest/?method=flickr.auth.checkToken:
    get:
      summary: Auth Check Token
      description: Returns the credentials attached to an authentication token. This
        call must be signed as specified in the authentication API spec.
      operationId: getRestMethodFlickr.auth.checktoken
      x-api-path-slug: restmethodflickr-auth-checktoken-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: auth_token
        description: The authentication token to check
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Auth
      - CheckToken
  /rest/?method=flickr.auth.getFrob:
    get:
      summary: Auth Get Frob
      description: Returns a frob to be used during authentication. This method call
        must be signed, and is deprecated in favour of OAuth.
      operationId: getRestMethodFlickr.auth.getfrob
      x-api-path-slug: restmethodflickr-auth-getfrob-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Auth
      - GetFrob
  /rest/?method=flickr.auth.getFullToken:
    get:
      summary: Auth Get Full Token
      description: Get the full authentication token for a mini-token. This method
        call must be signed.
      operationId: getRestMethodFlickr.auth.getfulltoken
      x-api-path-slug: restmethodflickr-auth-getfulltoken-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: mini_token
        description: The mini-token typed in by a user
      responses:
        200:
          description: OK
      tags:
      - Auth
      - GetFullToken
  /rest/?method=flickr.auth.getToken:
    get:
      summary: Auth Get Token
      description: Returns the auth token for the given frob, if one has been attached.
        This method call must be signed, and is deprecated in favour of OAuth.
      operationId: getRestMethodFlickr.auth.gettoken
      x-api-path-slug: restmethodflickr-auth-gettoken-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: frob
        description: The frob to check
      responses:
        200:
          description: OK
      tags:
      - Auth
      - GetToken
  /rest/?method=flickr.auth.oauth.getAccessToken:
    get:
      summary: Auth Oauth Get Access Token
      description: Exchange an auth token from the old Authentication API, to an OAuth
        access token. Calling this method will delete the auth token used to make
        the request. The request must be signed.
      operationId: getRestMethodFlickr.auth.oauth.getaccesstoken
      x-api-path-slug: restmethodflickr-auth-oauth-getaccesstoken-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Oauth
      - GetAccessToken
  /rest/?method=flickr.blogs.getList:
    get:
      summary: Blogs Get List
      description: Get a list of configured blogs for the calling user.
      operationId: getRestMethodFlickr.blogs.getlist
      x-api-path-slug: restmethodflickr-blogs-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: service
        description: Optionally only return blogs for a given service id
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - GetList
  /rest/?method=flickr.blogs.getServices:
    get:
      summary: Blogs Get Services
      description: Returns a list of Flickr supported blogging services.
      operationId: getRestMethodFlickr.blogs.getservices
      x-api-path-slug: restmethodflickr-blogs-getservices-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - GetServices
  /rest/?method=flickr.blogs.postPhoto:
    get:
      summary: Blogs Add Photo
      description: Posts a photo to a blog.
      operationId: getRestMethodFlickr.blogs.addphoto
      x-api-path-slug: restmethodflickr-blogs-postphoto-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: blog_id
        description: The ID of the blog to post to
      - in: query
        name: blog_password
        description: The password for the blog (used when the blog does not have a
          stored password)
      - in: query
        name: description
        description: The blog post body
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The ID of the photo to blog
      - in: query
        name: service
        description: A Flickr supported blogging service
      - in: query
        name: title
        description: The blog post title
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - PostPhoto
  /rest/?method=flickr.collections.getInfo:
    get:
      summary: Collections Get Info
      description: Returns information for a single collection. Currently can only
        be called by the collection owner, this may change.
      operationId: getRestMethodFlickr.collections.getinfo
      x-api-path-slug: restmethodflickr-collections-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The ID of the collection to fetch information for
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Collections
      - GetInfo
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