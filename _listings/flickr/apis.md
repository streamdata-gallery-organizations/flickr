---
name: Flickr
x-slug: flickr
description: Flickr (pronounced flicker) is an image hosting and video hosting website,
  and web services suite that was created by Ludicorp in 2004 and acquired by Yahoo
  in 2005. In addition to being a popular website for users to share and embed personal
  photographs, and effectively an online community, the service is widely used by
  photo researchers and by bloggers to host images that they embed in blogs and social
  media.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Flickr
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/apis.md
specificationVersion: "0.14"
apis:
- name: Flickr Upload
  x-api-slug: flickr
  description: Uploads a photo. Uploading apps can call the flickr.people.getUploadStatus
    method in the regular API to obtain file and bandwidth limits for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///upload
  tags: Upload
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/upload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/upload-post-openapi.md
- name: Flickr Replace
  x-api-slug: flickr
  description: Replaces a photo that has already been uploaded to Flickr. Uploading
    apps can call the flickr.people.getUploadStatus method in the regular API to obtain
    file and bandwidth limits for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///replace
  tags: Replace
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/replace-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/replace-post-openapi.md
- name: Flickr Activity User Comments
  x-api-slug: flickr
  description: Returns a list of recent activity on photos commented on by the calling
    user. Do not poll this method more than once an hour.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.activity.userComments
  tags: Activity,UserComments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-activity-usercomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-activity-usercomments-get-openapi.md
- name: Flickr Activity User Photos
  x-api-slug: flickr
  description: Returns a list of recent activity on photos commented on by the calling
    user. Do not poll this method more than once an hour.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.activity.userPhotos
  tags: Activity,UserPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-activity-userphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-activity-userphotos-get-openapi.md
- name: Flickr Auth Check Token
  x-api-slug: flickr
  description: Returns the credentials attached to an authentication token. This call
    must be signed as specified in the authentication API spec.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.auth.checkToken
  tags: Auth,CheckToken
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-checktoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-checktoken-get-openapi.md
- name: Flickr Auth Get Frob
  x-api-slug: flickr
  description: Returns a frob to be used during authentication. This method call must
    be signed, and is deprecated in favour of OAuth.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.auth.getFrob
  tags: Auth,GetFrob
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-getfrob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-getfrob-get-openapi.md
- name: Flickr Auth Get Full Token
  x-api-slug: flickr
  description: Get the full authentication token for a mini-token. This method call
    must be signed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.auth.getFullToken
  tags: Auth,GetFullToken
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-getfulltoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-getfulltoken-get-openapi.md
- name: Flickr Auth Get Token
  x-api-slug: flickr
  description: Returns the auth token for the given frob, if one has been attached.
    This method call must be signed, and is deprecated in favour of OAuth.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.auth.getToken
  tags: Auth,GetToken
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-gettoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-gettoken-get-openapi.md
- name: Flickr Auth Oauth Get Access Token
  x-api-slug: flickr
  description: Exchange an auth token from the old Authentication API, to an OAuth
    access token. Calling this method will delete the auth token used to make the
    request. The request must be signed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.auth.oauth.getAccessToken
  tags: Auth,Oauth,GetAccessToken
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-oauth-getaccesstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-auth-oauth-getaccesstoken-get-openapi.md
- name: Flickr Blogs Get List
  x-api-slug: flickr
  description: Get a list of configured blogs for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.blogs.getList
  tags: Blogs,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-getlist-get-openapi.md
- name: Flickr Blogs Get Services
  x-api-slug: flickr
  description: Returns a list of Flickr supported blogging services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.blogs.getServices
  tags: Blogs,GetServices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-getservices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-getservices-get-openapi.md
- name: Flickr Blogs Add Photo
  x-api-slug: flickr
  description: Posts a photo to a blog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.blogs.postPhoto
  tags: Blogs,PostPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-postphoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-blogs-postphoto-get-openapi.md
- name: Flickr Collections Get Info
  x-api-slug: flickr
  description: Returns information for a single collection. Currently can only be
    called by the collection owner, this may change.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.collections.getInfo
  tags: Collections,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-collections-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-collections-getinfo-get-openapi.md
- name: Flickr Collections Get Tree
  x-api-slug: flickr
  description: Returns a tree (or sub tree) of collections belonging to a given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.collections.getTree
  tags: Collections,GetTree
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-collections-gettree-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-collections-gettree-get-openapi.md
- name: Flickr Commons Get Institutions
  x-api-slug: flickr
  description: Retrieves a list of the current Commons institutions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.commons.getInstitutions
  tags: Commons,GetInstitutions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-commons-getinstitutions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-commons-getinstitutions-get-openapi.md
- name: Flickr Contacts Get List
  x-api-slug: flickr
  description: Get a list of contacts for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.contacts.getList
  tags: Contacts,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getlist-get-openapi.md
- name: Flickr Contacts Get List Recently Uploaded
  x-api-slug: flickr
  description: Return a list of contacts for a user who have recently uploaded photos
    along with the total count of photos uploaded. This method is still considered
    experimental. We don't plan for it to change or to go away but so long as this
    notice is present you should write your code accordingly.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.contacts.getListRecentlyUploaded
  tags: Contacts,GetListRecentlyUploaded
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getlistrecentlyuploaded-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getlistrecentlyuploaded-get-openapi.md
- name: Flickr Contacts Get Public List
  x-api-slug: flickr
  description: Get the contact list for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.contacts.getPublicList
  tags: Contacts,GetPublicList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getpubliclist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-contacts-getpubliclist-get-openapi.md
- name: Flickr Favorites Add
  x-api-slug: flickr
  description: Adds a photo to a user's favorites list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.favorites.add
  tags: Favorites,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-add-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-add-get-openapi.md
- name: Flickr Favorites Get List
  x-api-slug: flickr
  description: Returns a list of the user's favorite photos. Only photos which the
    calling user has permission to see are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.favorites.getList
  tags: Favorites,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getlist-get-openapi.md
- name: Flickr Favorites Get Public List
  x-api-slug: flickr
  description: Returns a list of favorite public photos for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.favorites.getPublicList
  tags: Favorites,GetPublicList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getpubliclist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getpubliclist-get-openapi.md
- name: Flickr Favorites Remove
  x-api-slug: flickr
  description: Adds a photo to a user's favorites list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.favorites.remove
  tags: Favorites,Remove
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-remove-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-remove-get-openapi.md
- name: Flickr Galleries Add Photo
  x-api-slug: flickr
  description: Add a photo to a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.addPhoto
  tags: Galleries,AddPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-addphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-addphoto-post-openapi.md
- name: Flickr Galleries Create
  x-api-slug: flickr
  description: Create a new gallery for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.create
  tags: Galleries,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-create-post-openapi.md
- name: Flickr Galleries Edit Meta
  x-api-slug: flickr
  description: Modify the metadata for a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.editMeta
  tags: Galleries,EditMeta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editmeta-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editmeta-post-openapi.md
- name: Flickr Galleries Edit Photo
  x-api-slug: flickr
  description: Edit the comment for a gallery photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.editPhoto
  tags: Galleries,EditPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editphoto-post-openapi.md
- name: Flickr Galleries Edit Photos
  x-api-slug: flickr
  description: Modify the photos in a gallery. Use this method to add, remove and
    re-order photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.editPhotos
  tags: Galleries,EditPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-editphotos-post-openapi.md
- name: Flickr Galleries Get Info
  x-api-slug: flickr
  description: Returns information about a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.getInfo
  tags: Galleries,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getinfo-get-openapi.md
- name: Flickr Galleries Get List
  x-api-slug: flickr
  description: Return the list of galleries created by a user. Sorted from newest
    to oldest.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.getList
  tags: Galleries,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getlist-get-openapi.md
- name: Flickr Galleries Get List For Photo
  x-api-slug: flickr
  description: Return the list of galleries to which a photo has been added. Galleries
    are returned sorted by date which the photo was added to the gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.getListForPhoto
  tags: Galleries,GetListForPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getlistforphoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getlistforphoto-get-openapi.md
- name: Flickr Galleries Get Photos
  x-api-slug: flickr
  description: Return the list of photos for a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.getPhotos
  tags: Galleries,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-openapi.md
- name: Flickr Groups Browse
  x-api-slug: flickr
  description: Browse the group category tree, finding groups and sub-categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.browse
  tags: Groups,Browse
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-browse-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-browse-get-openapi.md
- name: Flickr Groups Get Info
  x-api-slug: flickr
  description: Get information about a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.getInfo
  tags: Groups,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-getinfo-get-openapi.md
- name: Flickr Groups Search
  x-api-slug: flickr
  description: Search for groups. 18+ groups will only be returned for authenticated
    calls where the authenticated user is over 18.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.search
  tags: Groups,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-search-get-openapi.md
- name: Flickr Groups Members Get List
  x-api-slug: flickr
  description: Get a list of the members of a group. The call must be signed on behalf
    of a Flickr member, and the ability to see the group membership will be determined
    by the Flickr member's group privileges.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.members.getList
  tags: Groups,Members,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-members-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-members-getlist-get-openapi.md
- name: Flickr Groups Pools Add
  x-api-slug: flickr
  description: Add a photo to a group's pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.add
  tags: Groups,Pools,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-add-post-openapi.md
- name: Flickr Groups Pools Get Context
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a group pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.getContext
  tags: Groups,Pools,GetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getcontext-get-openapi.md
- name: Flickr Groups Pools Get Groups
  x-api-slug: flickr
  description: Returns a list of groups to which you can add photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.getGroups
  tags: Groups,Pools,GetGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getgroups-get-openapi.md
- name: Flickr Groups Pools Get Photos
  x-api-slug: flickr
  description: Returns a list of pool photos for a given group, based on the permissions
    of the group and the user logged in (if any).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.getPhotos
  tags: Groups,Pools,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-openapi.md
- name: Flickr Groups Pools Remove
  x-api-slug: flickr
  description: Remove a photo from a group pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.remove
  tags: Groups,Pools,Remove
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-remove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-remove-post-openapi.md
- name: Flickr Interestingness Get List
  x-api-slug: flickr
  description: Returns the list of interesting photos for the most recent day or a
    user-specified date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.interestingness.getList
  tags: Interestingness,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-interestingness-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-interestingness-getlist-get-openapi.md
- name: Flickr Machinetags Get Namespaces
  x-api-slug: flickr
  description: Return a list of unique namespaces, optionally limited by a given predicate,
    in alphabetical order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.machinetags.getNamespaces
  tags: Machinetags,GetNamespaces
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getnamespaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getnamespaces-get-openapi.md
- name: Flickr Machinetags Get Pairs
  x-api-slug: flickr
  description: Return a list of unique namespace and predicate pairs, optionally limited
    by predicate or namespace, in alphabetical order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.machinetags.getPairs
  tags: Machinetags,GetPairs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getpairs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getpairs-get-openapi.md
- name: Flickr Machinetags Get Predicates
  x-api-slug: flickr
  description: Return a list of unique predicates, optionally limited by a given namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.machinetags.getPredicates
  tags: Machinetags,GetPredicates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getpredicates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getpredicates-get-openapi.md
- name: Flickr Machinetags Get Recent Values
  x-api-slug: flickr
  description: Fetch recently used (or created) machine tags values.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.machinetags.getRecentValues
  tags: Machinetags,GetRecentValues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getrecentvalues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getrecentvalues-get-openapi.md
- name: Flickr Machinetags Get Values
  x-api-slug: flickr
  description: Return a list of unique values for a namespace and predicate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.machinetags.getValues
  tags: Machinetags,GetValues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getvalues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-machinetags-getvalues-get-openapi.md
- name: Flickr Panda Get List
  x-api-slug: flickr
  description: Return a list of Flickr pandas, from whom you can request photos using
    the flickr.panda.getPhotos API method. More information about the pandas can be
    found on the dev blog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.panda.getList
  tags: Panda,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-panda-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-panda-getlist-get-openapi.md
- name: Flickr Panda Get Photos
  x-api-slug: flickr
  description: Ask the Flickr Pandas for a list of recent public (and "safe") photos.
    More information about the pandas can be found on the dev blog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.panda.getPhotos
  tags: Panda,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-panda-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-panda-getphotos-get-openapi.md
- name: Flickr People Find By Email
  x-api-slug: flickr
  description: Return a user's NSID, given their email address
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.findByEmail
  tags: People,FindByEmail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-findbyemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-findbyemail-get-openapi.md
- name: Flickr People Find By Username
  x-api-slug: flickr
  description: Return a user's NSID, given their username.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.findByUsername
  tags: People,FindByUsername
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-findbyusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-findbyusername-get-openapi.md
- name: Flickr People Get Info
  x-api-slug: flickr
  description: Get information about a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getInfo
  tags: People,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getinfo-get-openapi.md
- name: Flickr People Get Photos
  x-api-slug: flickr
  description: Return photos from the given user's photostream. Only photos visible
    to the calling user will be returned. This method must be authenticated; to return
    public photos for a user, use flickr.people.getPublicPhotos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPhotos
  tags: People,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotos-get-openapi.md
- name: Flickr People Get Photos Of
  x-api-slug: flickr
  description: Returns a list of photos containing a particular Flickr member.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPhotosOf
  tags: People,GetPhotosOf
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotosof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotosof-get-openapi.md
- name: Flickr People Get Public Groups
  x-api-slug: flickr
  description: Returns the list of public groups a user is a member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPublicGroups
  tags: People,GetPublicGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getpublicgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getpublicgroups-get-openapi.md
- name: Flickr People Get Public Photos
  x-api-slug: flickr
  description: Get a list of public photos for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPublicPhotos
  tags: People,GetPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-openapi.md
- name: Flickr People Get Upload Status
  x-api-slug: flickr
  description: Returns information for the calling user related to photo uploads.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getUploadStatus
  tags: People,GetUploadStatus
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getuploadstatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getuploadstatus-get-openapi.md
- name: Flickr Photos Add Tags
  x-api-slug: flickr
  description: Add tags to a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.addTags
  tags: Photos,AddTags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-addtags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-addtags-post-openapi.md
- name: Flickr Photos Delete
  x-api-slug: flickr
  description: Delete a photo from Flickr.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.delete
  tags: Photos,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-delete-post-openapi.md
- name: Flickr Photos Get All Contexts
  x-api-slug: flickr
  description: Returns all visible sets and pools the photo belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getAllContexts
  tags: Photos,GetAllContexts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getallcontexts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getallcontexts-get-openapi.md
- name: Flickr Photos Get Contacts Photos
  x-api-slug: flickr
  description: Fetch a list of recent photos from the calling users' contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContactsPhotos
  tags: Photos,GetContactsPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontactsphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontactsphotos-get-openapi.md
- name: Flickr Photos Get Contacts Public Photos
  x-api-slug: flickr
  description: Fetch a list of recent public photos from a users' contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContactsPublicPhotos
  tags: Photos,GetContactsPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-openapi.md
- name: Flickr Photos Get Context
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContext
  tags: Photos,GetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontext-get-openapi.md
- name: Flickr Photos Get Counts
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getCounts
  tags: Photos,GetCounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcounts-get-openapi.md
- name: Flickr Photos Get Exif
  x-api-slug: flickr
  description: Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling
    user must have permission to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getExif
  tags: Photos,GetExif
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getexif-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getexif-get-openapi.md
- name: Flickr Photos Get Favorites
  x-api-slug: flickr
  description: Returns the list of people who have favorited a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getFavorites
  tags: Photos,GetFavorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getfavorites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getfavorites-get-openapi.md
- name: Flickr Photos Get Info
  x-api-slug: flickr
  description: Get information about a photo. The calling user must have permission
    to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getInfo
  tags: Photos,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getinfo-get-openapi.md
- name: Flickr Photos Get Not In Set
  x-api-slug: flickr
  description: Returns a list of your photos that are not part of any sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getNotInSet
  tags: Photos,GetNotInSet
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getnotinset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getnotinset-get-openapi.md
- name: Flickr Photos Get Perms
  x-api-slug: flickr
  description: Get permissions for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getPerms
  tags: Photos,GetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getperms-get-openapi.md
- name: Flickr Photos Get Recent
  x-api-slug: flickr
  description: Returns the list of people who have favorited a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getRecent
  tags: Photos,GetRecent
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getrecent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getrecent-get-openapi.md
- name: Flickr Photos Get Sizes
  x-api-slug: flickr
  description: Returns the available sizes for a photo. The calling user must have
    permission to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getSizes
  tags: Photos,GetSizes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getsizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getsizes-get-openapi.md
- name: Flickr Photos Get Untagged
  x-api-slug: flickr
  description: Returns a list of your photos that are not tagged.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getUntagged
  tags: Photos,GetUntagged
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getuntagged-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getuntagged-get-openapi.md
- name: Flickr Photos Get With Geo Data
  x-api-slug: flickr
  description: Returns a list of your geo-tagged photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getWithGeoData
  tags: Photos,GetWithGeoData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getwithgeodata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getwithgeodata-get-openapi.md
- name: Flickr Photos Get Without Geo Data
  x-api-slug: flickr
  description: Returns a list of your photos which haven't been geo-tagged.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getWithoutGeoData
  tags: Photos,GetWithoutGeoData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getwithoutgeodata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getwithoutgeodata-get-openapi.md
- name: Flickr Photos Get Recently Updated
  x-api-slug: flickr
  description: Return a list of your photos that have been recently created or which
    have been recently modified. Recently modified may mean that the photo's metadata
    (title, description, tags) may have been changed or a comment has been added (or
    just modified somehow :-)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getRecentlyUpdated
  tags: Photos,GetRecentlyd
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getrecentlyupdated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getrecentlyupdated-get-openapi.md
- name: Flickr Photos Remove Tag
  x-api-slug: flickr
  description: Remove a tag from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.removeTag
  tags: Photos,RemoveTag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-removetag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-removetag-post-openapi.md
- name: Flickr Photos Search
  x-api-slug: flickr
  description: Return a list of photos matching some criteria. Only photos visible
    to the calling user will be returned. To return private or semi-private photos,
    the caller must be authenticated with 'read' permissions, and have permission
    to view the photos. Unauthenticated calls will only return public photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.search
  tags: Photos,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-search-get-openapi.md
- name: Flickr Photos Set Content Type
  x-api-slug: flickr
  description: Set the content type of a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setContentType
  tags: Photos,SetContentType
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setcontenttype-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setcontenttype-post-openapi.md
- name: Flickr Photos Set Dates
  x-api-slug: flickr
  description: Set one or both of the dates for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setDates
  tags: Photos,SetDates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setdates-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setdates-post-openapi.md
- name: Flickr Photos Set Meta
  x-api-slug: flickr
  description: Set the meta information for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setMeta
  tags: Photos,SetMeta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setmeta-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setmeta-post-openapi.md
- name: Flickr Photos Set Perms
  x-api-slug: flickr
  description: Set permissions for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setPerms
  tags: Photos,SetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setperms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setperms-post-openapi.md
- name: Flickr Photos Set Safety Level
  x-api-slug: flickr
  description: Set the safety level of a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setSafetyLevel
  tags: Photos,SetSafetyLevel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setsafetylevel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-setsafetylevel-post-openapi.md
- name: Flickr Photos Set Tags
  x-api-slug: flickr
  description: Set the tags for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setTags
  tags: Photos,SetTags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-settags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-settags-post-openapi.md
- name: Flickr Photos Comments Add Comment
  x-api-slug: flickr
  description: Add comment to a photo as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.addComment
  tags: Photos,Comments,AddComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-addcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-addcomment-post-openapi.md
- name: Flickr Photos Comments Delete Comment
  x-api-slug: flickr
  description: Delete comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.deleteComment
  tags: Photos,Comments,DeleteComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-deletecomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-deletecomment-post-openapi.md
- name: Flickr Photos Comments Edit Comment
  x-api-slug: flickr
  description: Edit the text of a comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.editComment
  tags: Photos,Comments,EditComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-editcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-editcomment-post-openapi.md
- name: Flickr Photos Comments Get List
  x-api-slug: flickr
  description: Returns the comments for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.getList
  tags: Photos,Comments,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-getlist-get-openapi.md
- name: Flickr Photos Comments Get Recent For Contacts
  x-api-slug: flickr
  description: Return the list of photos belonging to your contacts that have been
    commented on recently.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.getRecentForContacts
  tags: Photos,Comments,GetRecentForContacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-getrecentforcontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-comments-getrecentforcontacts-get-openapi.md
- name: Flickr Photos Geo Batch Correct Location
  x-api-slug: flickr
  description: Correct the places hierarchy for all the photos for a user at a given
    latitude, longitude and accuracy. Batch corrections are processed in a delayed
    queue so it may take a few minutes before the changes are reflected in a user's
    photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.batchCorrectLocation
  tags: Photos,Geo,BatchCorrectLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-batchcorrectlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-batchcorrectlocation-post-openapi.md
- name: Flickr Photos Geo Correct Location
  x-api-slug: flickr
  description: Corrects a photo's location.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.correctLocation
  tags: Photos,Geo,CorrectLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-correctlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-correctlocation-post-openapi.md
- name: Flickr Photos Geo Get Location
  x-api-slug: flickr
  description: Get the geo data (latitude and longitude and the accuracy level) for
    a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.getLocation
  tags: Photos,Geo,GetLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-getlocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-getlocation-get-openapi.md
- name: Flickr Photos Geo Get Perms
  x-api-slug: flickr
  description: Get permissions for who may view geo data for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.getPerms
  tags: Photos,Geo,GetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-getperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-getperms-get-openapi.md
- name: Flickr Photos Geo Photos For Location
  x-api-slug: flickr
  description: Return a list of photos for the calling user at a specific latitude,
    longitude and accuracy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.photosForLocation
  tags: Photos,Geo,PhotosForLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-photosforlocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-photosforlocation-get-openapi.md
- name: Flickr Photos Geo Remove Location
  x-api-slug: flickr
  description: Removes the geo data associated with a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.removeLocation
  tags: Photos,Geo,RemoveLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-removelocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-removelocation-post-openapi.md
- name: Flickr Photos Geo Set Context
  x-api-slug: flickr
  description: 'Indicate the state of a photo''s geotagginess beyond latitude and
    longitude. Note : photos passed to this method must already be geotagged (using
    the flickr.photos.geo.setLocation method).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setContext
  tags: Photos,Geo,SetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setcontext-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setcontext-post-openapi.md
- name: Flickr Photos Geo Set Location
  x-api-slug: flickr
  description: Sets the geo data (latitude and longitude and, optionally, the accuracy
    level) for a photo. Before users may assign location data to a photo they must
    define who, by default, may view that information. Users can edit this preference
    at http://www.flickr.com/account/geo/privacy/. If a user has not set this preference,
    the API method will return an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setLocation
  tags: Photos,Geo,SetLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setlocation-post-openapi.md
- name: Flickr Photos Geo Set Perms
  x-api-slug: flickr
  description: Set the permission for who may view the geo data associated with a
    photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setPerms
  tags: Photos,Geo,SetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-geo-setperms-get-openapi.md
- name: Flickr Photos Licenses Get Info
  x-api-slug: flickr
  description: Fetches a list of available photo licenses for Flickr.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.licenses.getInfo
  tags: Photos,Licenses,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-openapi.md
- name: Flickr Photos Licenses Set Info
  x-api-slug: flickr
  description: Sets the license for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.licenses.setInfo
  tags: Photos,Licenses,SetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-setinfo-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-setinfo-post-openapi.md
- name: Flickr Photos Notes Add
  x-api-slug: flickr
  description: Add a note to a photo. Coordinates and sizes are in pixels, based on
    the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.add
  tags: Photos,Notes,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-add-post-openapi.md
- name: Flickr Photos Notes Delete
  x-api-slug: flickr
  description: Delete a note from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.delete
  tags: Photos,Notes,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-delete-post-openapi.md
- name: Flickr Photos Notes Edit
  x-api-slug: flickr
  description: Edit a note on a photo. Coordinates and sizes are in pixels, based
    on the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.edit
  tags: Photos,Notes,Edit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-edit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-notes-edit-post-openapi.md
- name: Flickr Photos People Add
  x-api-slug: flickr
  description: Add a person to a photo. Coordinates and sizes are in pixels, based
    on the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.add
  tags: Photos,People,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-add-post-openapi.md
- name: Flickr Photos People Delete
  x-api-slug: flickr
  description: Remove a person from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.delete
  tags: Photos,People,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-delete-post-openapi.md
- name: Flickr Photos People Delete Coords
  x-api-slug: flickr
  description: Remove the bounding box from a person in a photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.deleteCoords
  tags: Photos,People,DeleteCoords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-deletecoords-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-deletecoords-post-openapi.md
- name: Flickr Photos People Edit Coords
  x-api-slug: flickr
  description: Edit the bounding box of an existing person on a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.editCoords
  tags: Photos,People,EditCoords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-editcoords-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-editcoords-post-openapi.md
- name: Flickr Photos People Get List
  x-api-slug: flickr
  description: Get a list of people in a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.getList
  tags: Photos,People,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-people-getlist-get-openapi.md
- name: Flickr Photos Transform Rotate
  x-api-slug: flickr
  description: Rotate a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.transform.rotate
  tags: Photos,Transform,Rotate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-transform-rotate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-transform-rotate-post-openapi.md
- name: Flickr Photos Upload Check Tickets
  x-api-slug: flickr
  description: Checks the status of one or more asynchronous photo upload tickets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.upload.checkTickets
  tags: Photos,Upload,CheckTickets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-upload-checktickets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-upload-checktickets-get-openapi.md
- name: Flickr Photosets Add Photo
  x-api-slug: flickr
  description: Add a photo to the end of an existing photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.addPhoto
  tags: Photosets,AddPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-addphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-addphoto-post-openapi.md
- name: Flickr Photosets Create
  x-api-slug: flickr
  description: Create a new photoset for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.create
  tags: Photosets,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-create-post-openapi.md
- name: Flickr Photosets Delete
  x-api-slug: flickr
  description: Delete a new photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.delete
  tags: Photosets,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-delete-post-openapi.md
- name: Flickr Photosets Edit Meta
  x-api-slug: flickr
  description: Modify the meta-data for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.editMeta
  tags: Photosets,EditMeta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-editmeta-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-editmeta-post-openapi.md
- name: Flickr Photosets Edit Photos
  x-api-slug: flickr
  description: Modify the photos in a photoset. Use this method to add, remove and
    re-order photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.editPhotos
  tags: Photosets,EditPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-editphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-editphotos-post-openapi.md
- name: Flickr Photosets Get Context
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getContext
  tags: Photosets,GetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-openapi.md
- name: Flickr Photosets Get Info
  x-api-slug: flickr
  description: Gets information about a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getInfo
  tags: Photosets,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getinfo-get-openapi.md
- name: Flickr Photosets Get List
  x-api-slug: flickr
  description: Returns the photosets belonging to the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getList
  tags: Photosets,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getlist-get-openapi.md
- name: Flickr Photosets Get Photos
  x-api-slug: flickr
  description: Get the list of photos in a set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getPhotos
  tags: Photosets,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-openapi.md
- name: Flickr Photosets Order Sets
  x-api-slug: flickr
  description: Set the order of photosets for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.orderSets
  tags: Photosets,OrderSets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-ordersets-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-ordersets-post-openapi.md
- name: Flickr Photosets Remove Photo
  x-api-slug: flickr
  description: Remove a photo from a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.removePhoto
  tags: Photosets,RemovePhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-removephoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-removephoto-post-openapi.md
- name: Flickr Photosets Remove Photos
  x-api-slug: flickr
  description: Remove multiple photos from a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.removePhotos
  tags: Photosets,RemovePhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-removephotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-removephotos-post-openapi.md
- name: Flickr Photosets Reorder Photos
  x-api-slug: flickr
  description: Update the order of photos in a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.reorderPhotos
  tags: Photosets,ReorderPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-reorderphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-reorderphotos-post-openapi.md
- name: Flickr Photosets Set Primary Photo
  x-api-slug: flickr
  description: Set photoset primary photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.setPrimaryPhoto
  tags: Photosets,SetPrimaryPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-setprimaryphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-setprimaryphoto-post-openapi.md
- name: Flickr Photosets Comments Add Comment
  x-api-slug: flickr
  description: Add a comment to a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.addComment
  tags: Photosets,Comments,AddComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-addcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-addcomment-post-openapi.md
- name: Flickr Photosets Comments Delete Comment
  x-api-slug: flickr
  description: Delete a photoset comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.deleteComment
  tags: Photosets,Comments,DeleteComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-deletecomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-deletecomment-post-openapi.md
- name: Flickr Photosets Comments Edit Comment
  x-api-slug: flickr
  description: Edit the text of a comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.editComment
  tags: Photosets,Comments,EditComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-editcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-editcomment-post-openapi.md
- name: Flickr Photosets Comments Get List
  x-api-slug: flickr
  description: Returns the comments for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.getList
  tags: Photosets,Comments,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-comments-getlist-get-openapi.md
- name: Flickr Places Find
  x-api-slug: flickr
  description: Return a list of place IDs for a query string.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.find
  tags: Places,Find
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-find-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-find-get-openapi.md
- name: Flickr Places Find By Lat Lon
  x-api-slug: flickr
  description: Return a place ID for a latitude, longitude and accuracy triple.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.findByLatLon
  tags: Places,FindByLatLon
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-findbylatlon-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-findbylatlon-get-openapi.md
- name: Flickr Places Get Children With Photos Public
  x-api-slug: flickr
  description: Return a list of locations with public photos that are parented by
    a Where on Earth (WOE) or Places ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getChildrenWithPhotosPublic
  tags: Places,GetChildrenWithPhotosPublic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-openapi.md
- name: Flickr Places Get Info
  x-api-slug: flickr
  description: Get information about a place.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getInfo
  tags: Places,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getinfo-get-openapi.md
- name: Flickr Places Get Info By Url
  x-api-slug: flickr
  description: Lookup information about a place, by its flickr.com/places URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getInfoByUrl
  tags: Places,GetInfoByUrl
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getinfobyurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getinfobyurl-get-openapi.md
- name: Flickr Places Get Place Types
  x-api-slug: flickr
  description: Fetches a list of available place types for Flickr.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getPlaceTypes
  tags: Places,GetPlaceTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getplacetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getplacetypes-get-openapi.md
- name: Flickr Places Get Shape History
  x-api-slug: flickr
  description: Return an historical list of all the shape data generated for a Places
    or Where on Earth (WOE) ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getShapeHistory
  tags: Places,GetShapeHistory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getshapehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-getshapehistory-get-openapi.md
- name: Flickr Places Get Top Places List
  x-api-slug: flickr
  description: Return the top 100 most geotagged places for a day.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getTopPlacesList
  tags: Places,GetTopPlacesList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-gettopplaceslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-gettopplaceslist-get-openapi.md
- name: Flickr Places Places For Bounding Box
  x-api-slug: flickr
  description: Return all the locations of a matching place type for a bounding box.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.placesForBoundingBox
  tags: Places,PlacesForBoundingBox
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforboundingbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforboundingbox-get-openapi.md
- name: Flickr Places Places For Contacts
  x-api-slug: flickr
  description: Return a list of the top 100 unique places clustered by a given placetype
    for a user's contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.placesForContacts
  tags: Places,PlacesForContacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforcontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforcontacts-get-openapi.md
- name: Flickr Places Places For Tags
  x-api-slug: flickr
  description: Return a list of the top 100 unique places clustered by a given placetype
    for set of tags or machine tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.placesForTags
  tags: Places,PlacesForTags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesfortags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesfortags-get-openapi.md
- name: Flickr Places Places For User
  x-api-slug: flickr
  description: Return a list of the top 100 unique places clustered by a given placetype
    for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.placesForUser
  tags: Places,PlacesForUser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-placesforuser-get-openapi.md
- name: Flickr Places Resolve Place Id
  x-api-slug: flickr
  description: Find Flickr Places information by Place ID. This method has been deprecated.
    It won't be removed but you should use flickr.places.getInfo instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.resolvePlaceId
  tags: Places,ResolvePlaceId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-resolveplaceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-resolveplaceid-get-openapi.md
- name: Flickr Places Resolve Place U R L
  x-api-slug: flickr
  description: Find Flickr Places information by Place URL. This method has been deprecated.
    It won't be removed but you should use flickr.places.getInfo instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.resolvePlaceURL
  tags: Places,ResolvePlaceURL
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-resolveplaceurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-resolveplaceurl-get-openapi.md
- name: Flickr Places Tags For Place
  x-api-slug: flickr
  description: Return a list of the top 100 unique tags for a Flickr Places or Where
    on Earth (WOE) ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.tagsForPlace
  tags: Places,TagsForPlace
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-tagsforplace-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-places-tagsforplace-get-openapi.md
- name: Flickr Prefs Get Content Type
  x-api-slug: flickr
  description: Returns the default content type preference for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.prefs.getContentType
  tags: Prefs,GetContentType
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getcontenttype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getcontenttype-get-openapi.md
- name: Flickr Prefs Get Geo Perms
  x-api-slug: flickr
  description: Returns the default privacy level for geographic information attached
    to the user's photos and whether or not the user has chosen to use geo-related
    EXIF information to automatically geotag their photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.prefs.getGeoPerms
  tags: Prefs,GetGeoPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getgeoperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getgeoperms-get-openapi.md
- name: Flickr Prefs Get Hden
  x-api-slug: flickr
  description: Returns the default hidden preference for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.prefs.getHidden
  tags: Prefs,GetHidden
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-gethidden-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-gethidden-get-openapi.md
- name: Flickr Prefs Get Privacy
  x-api-slug: flickr
  description: Returns the default privacy level preference for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.prefs.getPrivacy
  tags: Prefs,GetPrivacy
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getprivacy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getprivacy-get-openapi.md
- name: Flickr Prefs Get Safety Level
  x-api-slug: flickr
  description: Returns the default safety level preference for the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.prefs.getSafetyLevel
  tags: Prefs,GetSafetyLevel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getsafetylevel-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-prefs-getsafetylevel-get-openapi.md
- name: Flickr Reflection Get Method Info
  x-api-slug: flickr
  description: Returns information for a given Flickr API method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.reflection.getMethodInfo
  tags: Reflection,GetMethodInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-reflection-getmethodinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-reflection-getmethodinfo-get-openapi.md
- name: Flickr Reflection Get Methods
  x-api-slug: flickr
  description: Returns a list of available Flickr API methods.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.reflection.getMethods
  tags: Reflection,GetMethods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-reflection-getmethods-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-reflection-getmethods-get-openapi.md
- name: Flickr Stats Get Collection Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a collection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getCollectionDomains
  tags: Stats,GetCollectionDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectiondomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectiondomains-get-openapi.md
- name: Flickr Stats Get Collection Referrers
  x-api-slug: flickr
  description: Get a list of referrers from a given domain to a collection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getCollectionReferrers
  tags: Stats,GetCollectionReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectionreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectionreferrers-get-openapi.md
- name: Flickr Stats Get Collection Stats
  x-api-slug: flickr
  description: Get the number of views on a collection for a given date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getCollectionStats
  tags: Stats,GetCollectionStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectionstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getcollectionstats-get-openapi.md
- name: Flickr Stats Get Photo Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotoDomains
  tags: Stats,GetPhotoDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotodomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotodomains-get-openapi.md
- name: Flickr Stats Get Photo Referrers
  x-api-slug: flickr
  description: Get a list of referring domains for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotoReferrers
  tags: Stats,GetPhotoReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotoreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotoreferrers-get-openapi.md
- name: Flickr Stats Get Photo Stats
  x-api-slug: flickr
  description: Get the number of views, comments and favorites on a photo for a given
    date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotoStats
  tags: Stats,GetPhotoStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostats-get-openapi.md
- name: Flickr Stats Get Photoset Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetDomains
  tags: Stats,GetPhotosetDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetdomains-get-openapi.md
- name: Flickr Stats Get Photoset Referrers
  x-api-slug: flickr
  description: Get a list of referring domains for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetReferrers
  tags: Stats,GetPhotosetReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetreferrers-get-openapi.md
- name: Flickr Stats Get Photoset Stats
  x-api-slug: flickr
  description: Get the number of views on a photoset for a given date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetStats
  tags: Stats,GetPhotosetStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotosetstats-get-openapi.md
- name: Flickr Stats Get Photostream Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamDomains
  tags: Stats,GetPhotostreamDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamdomains-get-openapi.md
- name: Flickr Stats Get Photostream Referrers
  x-api-slug: flickr
  description: Get a list of referrers from a given domain to a user's photostream
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamReferrers
  tags: Stats,GetPhotostreamReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamreferrers-get-openapi.md
- name: Flickr Stats Get Photostream Stats
  x-api-slug: flickr
  description: Get the number of views on a user's photostream for a given date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamStats
  tags: Stats,GetPhotostreamStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getphotostreamstats-get-openapi.md
- name: Flickr Stats Get Popular Photos
  x-api-slug: flickr
  description: List the photos with the most views, comments or favorites.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPopularPhotos
  tags: Stats,GetPopularPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getpopularphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-getpopularphotos-get-openapi.md
- name: Flickr Stats Get Total Views
  x-api-slug: flickr
  description: Get the overall view counts for an account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getTotalViews
  tags: Stats,GetTotalViews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-gettotalviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-stats-gettotalviews-get-openapi.md
- name: Flickr Tags Get Cluster Photos
  x-api-slug: flickr
  description: Returns the first 24 photos for a given tag cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getClusterPhotos
  tags: Tags,GetClusterPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getclusterphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getclusterphotos-get-openapi.md
- name: Flickr Tags Get Clusters
  x-api-slug: flickr
  description: Returns a list of tag clusters for the given tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getClusters
  tags: Tags,GetClusters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getclusters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getclusters-get-openapi.md
- name: Flickr Tags Get Hot List
  x-api-slug: flickr
  description: Returns a list of hot tags for the given period.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getHotList
  tags: Tags,GetHotList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-gethotlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-gethotlist-get-openapi.md
- name: Flickr Tags Get List Photo
  x-api-slug: flickr
  description: Get the tag list for a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getListPhoto
  tags: Tags,GetListPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistphoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistphoto-get-openapi.md
- name: Flickr Tags Get List User
  x-api-slug: flickr
  description: Get the tag list for a given user (or the currently logged in user).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getListUser
  tags: Tags,GetListUser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuser-get-openapi.md
- name: Flickr Tags Get List User Popular
  x-api-slug: flickr
  description: Get the popular tags for a given user (or the currently logged in user).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getListUserPopular
  tags: Tags,GetListUserPopular
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuserpopular-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuserpopular-get-openapi.md
- name: Flickr Tags Get List User Raw
  x-api-slug: flickr
  description: Get the raw versions of a given tag (or all tags) for the currently
    logged-in user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getListUserRaw
  tags: Tags,GetListUserRaw
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuserraw-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getlistuserraw-get-openapi.md
- name: Flickr Tags Get Related
  x-api-slug: flickr
  description: Returns a list of tags 'related' to the given tag, based on clustered
    usage analysis.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getRelated
  tags: Tags,GetRelated
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getrelated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-tags-getrelated-get-openapi.md
- name: Flickr Test Echo
  x-api-slug: flickr
  description: A testing method which echoes all parameters back in the response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.test.echo
  tags: Test,Echo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-echo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-echo-get-openapi.md
- name: Flickr Test Login
  x-api-slug: flickr
  description: A testing method which checks if the caller is logged in then returns
    their username.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.test.login
  tags: Test,Login
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-login-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-login-get-openapi.md
- name: Flickr Test Null
  x-api-slug: flickr
  description: This method doesn't do anything.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.test.null
  tags: Test,Null
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-null-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-null-get-openapi.md
- name: Flickr Urls Get Group
  x-api-slug: flickr
  description: Returns the url to a group's page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.getGroup
  tags: Urls,GetGroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getgroup-get-openapi.md
- name: Flickr Urls Get User Photos
  x-api-slug: flickr
  description: Returns the url to a user's photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.getUserPhotos
  tags: Urls,GetUserPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getuserphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getuserphotos-get-openapi.md
- name: Flickr Urls Get User Profile
  x-api-slug: flickr
  description: Returns the url to a user's profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.getUserProfile
  tags: Urls,GetUserProfile
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getuserprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-getuserprofile-get-openapi.md
- name: Flickr Urls Lookup Gallery
  x-api-slug: flickr
  description: Returns gallery info, by url.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.lookupGallery
  tags: Urls,LookupGallery
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupgallery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupgallery-get-openapi.md
- name: Flickr Urls Lookup Group
  x-api-slug: flickr
  description: Returns a group NSID, given the url to a group's page or photo pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.lookupGroup
  tags: Urls,LookupGroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupgroup-get-openapi.md
- name: Flickr Urls Lookup User
  x-api-slug: flickr
  description: Returns a user NSID, given the url to a user's photos or profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.lookupUser
  tags: Urls,LookupUser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-urls-lookupuser-get-openapi.md
- name: Flickr
  x-api-slug: flickr
  description: The Flickr API consists of a set of callable methods, and some API
    endpoints.  To perform an action using the Flickr API, you need to select a calling
    convention, send a request to its endpoint specifying a method and some arguments,
    and will receive a formatted response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services/
  tags: Flickr
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/openapi.md
x-common:
- type: x-authentication
  url: https://www.flickr.com/services/api/auth.oauth.html
- type: x-base
  url: https://api.flickr.com/services/
- type: x-developer
  url: https://www.flickr.com/services/api/
- type: x-getting-started
  url: https://www.flickr.com/services/developer/
- type: x-privacy
  url: https://info.yahoo.com/privacy/us/yahoo/flickr/details.html
- type: x-support
  url: https://help.yahoo.com/kb/flickr-for-desktop
- type: x-terms-of-service
  url: https://www.flickr.com/services/api/tos/
- type: x-twitter
  url: https://twitter.com/flickr
- type: x-website
  url: http://www.flickr.com/
- type: x-website
  url: http://flickr.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---