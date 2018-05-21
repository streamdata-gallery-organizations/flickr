---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: 'Flickr '
  description: Returns an oauth token and oauth token secret
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
  /rest?method=flickr.groups.pools.getContext:
    get:
      summary: Get Group Pools
      description: Returns next and previous photos for a photo in a group pool
      operationId: getGroupPhotosByID
      x-api-path-slug: restmethodflickrgroupspoolsgetcontext-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: group_id
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Groups
  /rest?method=flickr.photolist.getContext:
    get:
      summary: Get Photo Lists
      description: Returns next and previous photos in a photo list
      operationId: getPhotolistContextByID
      x-api-path-slug: restmethodflickrphotolistgetcontext-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photolist_id
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Lists
  /rest?method=flickr.photos.getContext:
    get:
      summary: Get Photos
      description: Returns next and previous photos for a photo in a photostream
      operationId: getPhotostreamContextByID
      x-api-path-slug: restmethodflickrphotosgetcontext-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - Photos
  /rest?method=flickr.photos.licenses.getInfo:
    get:
      summary: Get Photo Licenses
      description: Fetches a list of available photo licenses for Flickr
      operationId: getLicenseByID
      x-api-path-slug: restmethodflickrphotoslicensesgetinfo-get
      parameters:
      - in: query
        name: api_key
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Search
  /rest?method=flickr.people.getInfo:
    get:
      summary: Get People
      description: Returns a person
      operationId: getPersonByID
      x-api-path-slug: restmethodflickrpeoplegetinfo-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
  /rest?method=flickr.photos.getExif:
    get:
      summary: Get Photo Exif
      description: Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling
        user must have permission to view the photo.
      operationId: getPhotoExifByID
      x-api-path-slug: restmethodflickrphotosgetexif-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photo_id
      - in: query
        name: secret
      responses:
        200:
          description: OK
      tags:
      - Photos
  /rest?method=flickr.photos.getInfo:
    get:
      summary: Get Photo
      description: Returns a photo
      operationId: getPhotoByID
      x-api-path-slug: restmethodflickrphotosgetinfo-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Licensing
  /rest?method=flickr.photosets.getContext:
    get:
      summary: Get Photo Set
      description: Returns next and previous photos for a photo in a set
      operationId: getAlbumContextByID
      x-api-path-slug: restmethodflickrphotosetsgetcontext-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photoset_id
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - Photos
  /rest?method=flickr.photosets.getPhotos:
    get:
      summary: Get Photo Set Photos
      description: Returns a list of photos in an album.
      operationId: getAlbumByID
      x-api-path-slug: restmethodflickrphotosetsgetphotos-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photoset_id
      responses:
        200:
          description: OK
      tags:
      - Photos
  /rest?method=flickr.galleries.getPhotos:
    get:
      summary: Get Gallery Photos
      description: Returns a list of photos in a gallery.
      operationId: getGalleryPhotosByID
      x-api-path-slug: restmethodflickrgalleriesgetphotos-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: gallery_id
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Galleries
  /rest?method=flickr.photos.search:
    get:
      summary: Photo Search
      description: Return a list of photos matching some criteria.
      operationId: getMediaBySearch
      x-api-path-slug: restmethodflickrphotossearch-get
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
      - in: query
        name: api_key
      - in: query
        name: bbox
        description: A comma-delimited list of 4 values defining the Bounding Box
          of the area that will be searched
      - in: query
        name: contacts
        description: Search your contacts
      - in: query
        name: content_type
        description: 'Content Type setting:  1: photos only'
      - in: query
        name: geo_context
        description: Geo context is a numeric value representing the photos geotagginess
          beyond latitude and longitude
      - in: query
        name: group_id
        description: The id of a group whos pool to search
      - in: query
        name: has_geo
        description: Any photo that has been geotagged, or if the value is 0 any photo
          that has not been geotagged
      - in: query
        name: in_gallery
        description: Limit the scope of the search to only photos that are in a gallery?
          Default is false, search all photos
      - in: query
        name: is_commons
        description: Limit the scope of the search to only photos that are part of
          the Flickr Commons project
      - in: query
        name: is_getty
        description: Limit the scope of the search to only photos that are for sale
          on Getty
      - in: query
        name: lat
        description: A valid latitude, in decimal format, for doing radial geo queries
      - in: query
        name: license
        description: The license id for photos (for possible values see the flickr
      - in: query
        name: lon
        description: A valid longitude, in decimal format, for doing radial geo queries
      - in: query
        name: machine_tags
        description: 'Aside from passing in a fully formed machine tag, there is a
          special syntax for searching on specific properties : Find photos using
          the dc namespace : machine_tags => dc: Find photos with a title in the dc
          namespace : machine_tags => dc:title= Find photos titled mr'
      - in: query
        name: machine_tag_mode
        description: Either any for an OR combination of tags, or all for an AND combination
      - in: query
        name: max_taken_date
        description: Maximum taken date
      - in: query
        name: max_upload_date
        description: Maximum upload date
      - in: query
        name: media
        description: Filter results by media type
      - in: query
        name: min_taken_date
        description: Minimum taken date
      - in: query
        name: min_upload_date
        description: Minimum upload date
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: place_id
        description: A Flickr place id
      - in: query
        name: privacy_filter
        description: Return photos only matching a certain privacy level
      - in: query
        name: radius
        description: A valid radius used for geo queries, greater than zero and less
          than 20 miles (or 32 kilometers), for use with point-based geo queries
      - in: query
        name: radius_units
        description: The unit of measure when doing radial geo queries
      - in: query
        name: safe_search
        description: 'Safe search setting:  1: for safe,  2: for moderate,  3: for
          restricted'
      - in: query
        name: sort
        description: The order in which to sort returned photos
      - in: query
        name: tags
        description: A comma-delimited list of tags
      - in: query
        name: text
        description: A free text search
      - in: query
        name: user_id
        description: The NSID of the user whos photo to search
      - in: query
        name: woe_id
        description: A 32-bit identifier that uniquely represents spatial entities
      responses:
        200:
          description: OK
      tags:
      - Photos
  /upload:
    post:
      summary: Upload Photo
      description: Uploads a new photo to Flickr
      operationId: uploadPhoto
      x-api-path-slug: upload-post
      parameters:
      - in: formData
        name: api_key
      - in: formData
        name: content_type
      - in: formData
        name: description
      - in: formData
        name: hidden
      - in: formData
        name: is_family
      - in: formData
        name: is_friend
      - in: formData
        name: is_public
      - in: formData
        name: photo
      - in: formData
        name: safety_level
      - in: formData
        name: tags
      - in: formData
        name: title
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Upload
  /rest?method=flickr.photos.getSizes:
    get:
      summary: ""
      description: Returns photo sizes
      operationId: getPhotoSizesByID
      x-api-path-slug: restmethodflickrphotosgetsizes-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: photo_id
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest?method=flickr.test.echo:
    get:
      summary: ""
      description: Echos the input parameters back in the response
      operationId: echo
      x-api-path-slug: restmethodflickrtestecho-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: echo
      responses:
        200:
          description: OK
      tags:
      - ""
  /oauth/request_token:
    get:
      summary: ""
      description: Returns an oauth token and oauth token secret
      operationId: getRequestToken
      x-api-path-slug: oauthrequest-token-get
      parameters:
      - in: query
        name: oauth_callback
      - in: query
        name: oauth_consumer_key
      - in: query
        name: oauth_nonce
      - in: query
        name: oauth_signature
      - in: query
        name: oauth_signature_method
      - in: query
        name: oauth_timestamp
      - in: query
        name: oauth_version
      responses:
        200:
          description: OK
      tags:
      - ""
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