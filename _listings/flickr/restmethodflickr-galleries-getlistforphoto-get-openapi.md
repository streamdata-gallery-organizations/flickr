---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Galleries Get List For Photo
  description: Return the list of galleries to which a photo has been added. Galleries
    are returned sorted by date which the photo was added to the gallery.
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
  /rest/?method=flickr.collections.getTree:
    get:
      summary: Collections Get Tree
      description: Returns a tree (or sub tree) of collections belonging to a given
        user.
      operationId: getRestMethodFlickr.collections.gettree
      x-api-path-slug: restmethodflickr-collections-gettree-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The ID of the collection to fetch a tree for, or zero to fetch
          the root collection
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The ID of the account to fetch the collection tree for
      responses:
        200:
          description: OK
      tags:
      - Collections
      - GetTree
  /rest/?method=flickr.commons.getInstitutions:
    get:
      summary: Commons Get Institutions
      description: Retrieves a list of the current Commons institutions.
      operationId: getRestMethodFlickr.commons.getinstitutions
      x-api-path-slug: restmethodflickr-commons-getinstitutions-get
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
      - Commons
      - GetInstitutions
  /rest/?method=flickr.contacts.getList:
    get:
      summary: Contacts Get List
      description: Get a list of contacts for the calling user.
      operationId: getRestMethodFlickr.contacts.getlist
      x-api-path-slug: restmethodflickr-contacts-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: filter
        description: An optional filter of the results
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - GetList
  /rest/?method=flickr.contacts.getListRecentlyUploaded:
    get:
      summary: Contacts Get List Recently Uploaded
      description: Return a list of contacts for a user who have recently uploaded
        photos along with the total count of photos uploaded. This method is still
        considered experimental. We don't plan for it to change or to go away but
        so long as this notice is present you should write your code accordingly.
      operationId: getRestMethodFlickr.contacts.getlistrecentlyuploaded
      x-api-path-slug: restmethodflickr-contacts-getlistrecentlyuploaded-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date_lastupload
        description: Limits the resultset to contacts that have uploaded photos since
          this date
      - in: query
        name: filter
        description: Limit the result set to all contacts or only those who are friends
          or family
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - GetListRecentlyUploaded
  /rest/?method=flickr.contacts.getPublicList:
    get:
      summary: Contacts Get Public List
      description: Get the contact list for a user.
      operationId: getRestMethodFlickr.contacts.getpubliclist
      x-api-path-slug: restmethodflickr-contacts-getpubliclist-get
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
        description: Number of photos to return per page
      - in: query
        name: user_id
        description: The NSID of the user to fetch the contact list for
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - GetPublicList
  /rest/?method=flickr.favorites.add:
    get:
      summary: Favorites Add
      description: Adds a photo to a user's favorites list.
      operationId: getRestMethodFlickr.favorites.add
      x-api-path-slug: restmethodflickr-favorites-add-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to add to the users favorites
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - Add
  /rest/?method=flickr.favorites.getList:
    get:
      summary: Favorites Get List
      description: Returns a list of the user's favorite photos. Only photos which
        the calling user has permission to see are returned.
      operationId: getRestMethodFlickr.favorites.getlist
      x-api-path-slug: restmethodflickr-favorites-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_fave_date
        description: Maximum date that a photo was favorited on
      - in: query
        name: min_fave_date
        description: Minimum date that a photo was favorited on
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - GetList
  /rest/?method=flickr.favorites.getPublicList:
    get:
      summary: Favorites Get Public List
      description: Returns a list of favorite public photos for the given user.
      operationId: getRestMethodFlickr.favorites.getpubliclist
      x-api-path-slug: restmethodflickr-favorites-getpubliclist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_fave_date
        description: Maximum date that a photo was favorited on
      - in: query
        name: min_fave_date
        description: Minimum date that a photo was favorited on
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: user_id
        description: The user to fetch the favorites list for
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - GetPublicList
  /rest/?method=flickr.favorites.remove:
    get:
      summary: Favorites Remove
      description: Adds a photo to a user's favorites list.
      operationId: getRestMethodFlickr.favorites.remove
      x-api-path-slug: restmethodflickr-favorites-remove-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to remove to the users favorites
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - Remove
  /rest/?method=flickr.galleries.addPhoto:
    post:
      summary: Galleries Add Photo
      description: Add a photo to a gallery.
      operationId: postRestMethodFlickr.galleries.addphoto
      x-api-path-slug: restmethodflickr-galleries-addphoto-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment
        description: A short comment or story to accompany the photo
      - in: query
        name: gallery_id
        description: The ID of the gallery to add a photo to
      - in: query
        name: photo_id
        description: The photo ID to add to the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - AddPhoto
  /rest/?method=flickr.galleries.create:
    post:
      summary: Galleries Create
      description: Create a new gallery for the calling user.
      operationId: postRestMethodFlickr.galleries.create
      x-api-path-slug: restmethodflickr-galleries-create-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: description
        description: A short description for the gallery
      - in: query
        name: format
        description: Response format
      - in: query
        name: primary_photo_id
        description: The first photo to add to your gallery
      - in: query
        name: title
        description: The title of the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - Create
  /rest/?method=flickr.galleries.editMeta:
    post:
      summary: Galleries Edit Meta
      description: Modify the metadata for a gallery.
      operationId: postRestMethodFlickr.galleries.editmeta
      x-api-path-slug: restmethodflickr-galleries-editmeta-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: description
        description: The new description for the gallery
      - in: query
        name: gallery_id
        description: The gallery ID to update
      - in: query
        name: title
        description: The new title for the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - EditMeta
  /rest/?method=flickr.galleries.editPhoto:
    post:
      summary: Galleries Edit Photo
      description: Edit the comment for a gallery photo.
      operationId: postRestMethodFlickr.galleries.editphoto
      x-api-path-slug: restmethodflickr-galleries-editphoto-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment
        description: The updated comment the photo
      - in: query
        name: gallery_id
        description: The ID of the gallery to add a photo to
      - in: query
        name: photo_id
        description: The photo ID to add to the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - EditPhoto
  /rest/?method=flickr.galleries.editPhotos:
    post:
      summary: Galleries Edit Photos
      description: Modify the photos in a gallery. Use this method to add, remove
        and re-order photos.
      operationId: postRestMethodFlickr.galleries.editphotos
      x-api-path-slug: restmethodflickr-galleries-editphotos-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: gallery_id
        description: The id of the gallery to modify
      - in: query
        name: photo_ids
        description: A comma-delimited list of photo ids to include in the gallery
      - in: query
        name: primary_photo_id
        description: The id of the photo to use as the primary photo for the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - EditPhotos
  /rest/?method=flickr.galleries.getInfo:
    get:
      summary: Galleries Get Info
      description: Returns information about a gallery.
      operationId: getRestMethodFlickr.galleries.getinfo
      x-api-path-slug: restmethodflickr-galleries-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: gallery_id
        description: The gallery ID you are requesting information for
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - GetInfo
  /rest/?method=flickr.galleries.getList:
    get:
      summary: Galleries Get List
      description: Return the list of galleries created by a user. Sorted from newest
        to oldest.
      operationId: getRestMethodFlickr.galleries.getlist
      x-api-path-slug: restmethodflickr-galleries-getlist-get
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
        description: Number of galleries to return per page
      - in: query
        name: user_id
        description: The NSID of the user to get a galleries list for
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - GetList
  /rest/?method=flickr.galleries.getListForPhoto:
    get:
      summary: Galleries Get List For Photo
      description: Return the list of galleries to which a photo has been added. Galleries
        are returned sorted by date which the photo was added to the gallery.
      operationId: getRestMethodFlickr.galleries.getlistforphoto
      x-api-path-slug: restmethodflickr-galleries-getlistforphoto-get
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
        description: Number of galleries to return per page
      - in: query
        name: photo_id
        description: The ID of the photo to fetch a list of galleries for
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - GetListForPhoto
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