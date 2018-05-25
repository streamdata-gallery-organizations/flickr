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
x-alexaRank: ""
tags: Flickr
created: "2018-05-25"
modified: "2018-05-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/apis.md
specificationVersion: "0.14"
apis:
- name: Flickr Get Favorite List
  x-api-slug: flickr
  description: Returns a list of the user's favorite photos. Only photos which the
    calling user has permission to see are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.favorites.getList
  tags: Photos,Favorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getlist-get-openapi.md
- name: Flickr Get People Photos
  x-api-slug: flickr
  description: Return photos from the given user's photostream
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.people.getPhotos
  tags: Photos,People
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getphotos-get-openapi.md
- name: Flickr Get Photo Sets
  x-api-slug: flickr
  description: Returns the albums belonging to the specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photosets.getList
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getlist-get-openapi.md
- name: Flickr Get Favorite Context
  x-api-slug: flickr
  description: Returns next and previous favorites for a photo in a user's favorites
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.favorites.getContext
  tags: Photos,Favorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-favorites-getcontext-get-openapi.md
- name: Flickr Get Groups
  x-api-slug: flickr
  description: Get information about a group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.getInfo
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-getinfo-get-openapi.md
- name: Flickr Get Group Pool Photos
  x-api-slug: flickr
  description: Returns a list of pool photos for a given group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.pools.getPhotos
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-openapi.md
- name: Flickr Get Group Topic List
  x-api-slug: flickr
  description: Get a list of discussion topics in a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.discuss.topics.getList
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-topics-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-topics-getlist-get-openapi.md
- name: Flickr Get Group Replies
  x-api-slug: flickr
  description: Get information on a group topic reply
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.discuss.replies.getInfo
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-replies-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-replies-getinfo-get-openapi.md
- name: Flickr Get Group Topic Info
  x-api-slug: flickr
  description: Get information about a group discussion topic
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.discuss.topics.getInfo
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-topics-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-discuss-topics-getinfo-get-openapi.md
- name: Flickr Get Group Pools
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a group pool
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.groups.pools.getContext
  tags: Photos,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-groups-pools-getcontext-get-openapi.md
- name: Flickr Get Photo Lists
  x-api-slug: flickr
  description: Returns next and previous photos in a photo list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photolist.getContext
  tags: Photos,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photolist-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photolist-getcontext-get-openapi.md
- name: Flickr Get Photos
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a photostream
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.getContext
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getcontext-get-openapi.md
- name: Flickr Get Photo Licenses
  x-api-slug: flickr
  description: Fetches a list of available photo licenses for Flickr
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.licenses.getInfo
  tags: Photos,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-openapi.md
- name: Flickr Get People
  x-api-slug: flickr
  description: Returns a person
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.people.getInfo
  tags: Photos,People
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-people-getinfo-get-openapi.md
- name: Flickr Get Photo Exif
  x-api-slug: flickr
  description: Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling
    user must have permission to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.getExif
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getexif-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getexif-get-openapi.md
- name: Flickr Get Photo
  x-api-slug: flickr
  description: Returns a photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.getInfo
  tags: Photos,Licensing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getinfo-get-openapi.md
- name: Flickr Get Photo Set
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a set
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photosets.getContext
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-openapi.md
- name: Flickr Get Photo Set Photos
  x-api-slug: flickr
  description: Returns a list of photos in an album.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photosets.getPhotos
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-openapi.md
- name: Flickr Get Gallery Photos
  x-api-slug: flickr
  description: Returns a list of photos in a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.galleries.getPhotos
  tags: Photos,Galleries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-openapi.md
- name: Flickr Photo Search
  x-api-slug: flickr
  description: Return a list of photos matching some criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.search
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-search-get-openapi.md
- name: Flickr Upload Photo
  x-api-slug: flickr
  description: Uploads a new photo to Flickr
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//upload
  tags: Photo,Upload
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/upload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/upload-post-openapi.md
- name: 'Flickr '
  x-api-slug: flickr
  description: Returns photo sizes
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.photos.getSizes
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getsizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-photos-getsizes-get-openapi.md
- name: 'Flickr '
  x-api-slug: flickr
  description: Echos the input parameters back in the response
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//rest?method=flickr.test.echo
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-echo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/restmethodflickr-test-echo-get-openapi.md
- name: 'Flickr '
  x-api-slug: flickr
  description: Returns an oauth token and oauth token secret
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//oauth/request_token
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/oauthrequest-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/oauthrequest-token-get-openapi.md
- name: 'Flickr '
  x-api-slug: flickr
  description: Returns an access token
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services//oauth/access_token
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/oauthaccess-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/flickr/master/_listings/flickr/oauthaccess-token-get-openapi.md
- name: Flickr
  x-api-slug: flickr
  description: Flickr (pronounced flicker) is an image hosting and video hosting website,
    and web services suite that was created by Ludicorp in 2004 and acquired by Yahoo
    in 2005. In addition to being a popular website for users to share and embed personal
    photographs, and effectively an online community, the service is widely used by
    photo researchers and by bloggers to host images that they embed in blogs and
    social media.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: ://api.flickr.com//services
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
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---