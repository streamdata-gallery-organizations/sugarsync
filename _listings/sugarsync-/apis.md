---
name: SugarSync
x-slug: sugarsync-
description: SugarSync is a cloud file sharing, file sync and online backup service
  that is simple, powerful and easy to use. Unlike Dropbox, SugarSync enables you
  to back up your existing folder structure. Try it for FREE for 30 days and get started
  today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
x-kinRank: "8"
x-alexaRank: "64898"
tags: 'SugarSync '
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/apis.md
specificationVersion: "0.14"
apis:
- name: Sugar Sync  API - Retrieving Album Information
  x-api-slug: album-get
  description: To retrieve information about an album, an application submits an HTTP
    GET request to then          album resource that represents the album.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/album-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/album-get-openapi.md
- name: Sugar Sync  API - Creating a Refresh Token
  x-api-slug: appauthorization-post
  description: An application needs to be authorized to access a users SugarSync resources
    through the Platform API.nTo do that, the app needs to create a refresh token.
    When a user first runs the application, it creates a refresh tokennby submitting
    a POST request that includes the users credentials to the API.nIf the request
    is successful, the SugarSync service grants the application permission to access
    the users account and returns a refresh token.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/appauthorization-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/appauthorization-post-openapi.md
- name: Sugar Sync  API - Creating an Access Token
  x-api-slug: authorization-post
  description: An application needs to be authorized to access a users SugarSync resources
    through the Platform API. To do that,nthe app needs to create an access token,
    which allows the app to access files, folders,nand other resources within a users
    account. After the token is created, the app needs to specify it in the HTTP request
    header when it makes a request through the API to access a resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/authorization-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/authorization-post-openapi.md
- name: Sugar Sync  API - Retrieving Contact Information
  x-api-slug: contact-get
  description: A contact represents another SugarSync user who has shared a folder
    or folders with this user.n          To retrieve information about a contact,
    an application submits an HTTP GET request to then          contact resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/contact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/contact-get-openapi.md
- name: Sugar Sync  API - Retrieving File Data
  x-api-slug: file-get
  description: To retrieve file data, an application submits an HTTP GET request to
    then          file data resource that represents the data for the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-get-openapi.md
- name: Sugar Sync  API - Uploading File Data
  x-api-slug: file-put
  description: An application can upload data to a file by issuing an HTTP PUT request
    to thenfile data resource that represents the data for the file.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-put-openapi.md
- name: Sugar Sync  API - Deleting a File
  x-api-slug: file-delete
  description: An application can permanently delete a file by issuing an HTTP DELETE
    request to the URL of thenfile resource.nIts a good idea to precede DELETE requests
    like this with a caution note in your applications user interface.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-delete-openapi.md
- name: Sugar Sync  API - Retrieving File Information
  x-api-slug: file-get
  description: To retrieve information about a file, an application submits an HTTP
    GET request to then          file resource that represents the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-get-openapi.md
- name: Sugar Sync  API - Creating a New File Version
  x-api-slug: file-post
  description: nAn application can create a new version of a file by submitting an
    HTTP POST request to the URL that represents the version history. The version
    history URL is returned in the &lt;versions&gt; element whenn retrieving information
    about a file.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-post-openapi.md
- name: Sugar Sync  API - Updating File Information
  x-api-slug: file-put
  description: An application can update various attributes of a file by issuing an
    HTTP PUT request to the URL thatnrepresents the file resource. In addition, the
    app needs to provide as input, XML that identifies the new attribute values for
    the file. Upon receiving the PUT request, the SugarSync service examines the input
    and updates any of the attributes that have been modified.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/file-put-openapi.md
- name: Sugar Sync  API - Retrieving Folder Information
  x-api-slug: folder-get
  description: To retrieve information about a folder, an application submits an HTTP
    GET request to then          folder resource that represents the folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-get-openapi.md
- name: Sugar Sync  API - Deleting a Folder
  x-api-slug: folder-delete
  description: An application can permanantly delete a folder by issuing an HTTP DELETE
    request to the URL of thenfolder resource.nIts a good idea to precede DELETE requests
    like this with a caution note in your applications user interface.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-delete-openapi.md
- name: Sugar Sync  API - Retrieving Folder Contents
  x-api-slug: folder-get
  description: To retrieve the contents of a folder, an application submits an HTTP
    GET request to the URLn          that represents the folder contents.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-get-openapi.md
- name: Sugar Sync  API - Creating a Folder
  x-api-slug: folder-post
  description: An application can create a folder within another folder by issuing
    an HTTP POST request to the URL ofnthe containing folder resource.nIn addition,
    the application needs to provide as input, XML that identifies the display name
    of the folder to be created.nNote that an application can create a folder only
    within another folder, and not directly in a workspace.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-post-openapi.md
- name: Sugar Sync  API - Updating Folder Information
  x-api-slug: folder-put
  description: An application can update various attributes of a folder by issuing
    an HTTP PUT request to the URL thatnrepresents the folder resource. In addition,
    the app needs to provide as input, XML that identifies the new attribute values
    for the folder. Upon receiving the PUT request, the SugarSync service examines
    the input and updates any of the attributes that have been modified.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/folder-put-openapi.md
- name: Sugar Sync  API - Retrieving Received Share Information
  x-api-slug: receivedshare-get
  description: To retrieve information about a received share (that is, a shared folder
    owned by another user and to whichnthis user has been granted access privileges
    by the owner), an application submits an HTTP GET request to the URLnthat represents
    the received share resource. The URL is referenced in the &lt;receivedShare&gt;
    element for the received share in the received shares list.nSee Retrieving the
    Received Shares List.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/receivedshare-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/receivedshare-get-openapi.md
- name: Sugar Sync  API - Retrieving User Information
  x-api-slug: user-get
  description: To retrieve information about a SugarSync user, an application submits
    an HTTP GET request to thenuser resource that represents the user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/user-get-openapi.md
- name: Sugar Sync  API - Retrieving Received Shares List
  x-api-slug: user-get
  description: One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe
    element contains a link to a list that describes the shared folders that are owned
    by other users and to which this user has been granted access privileges by those
    owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To
    retrieve the list, an application submits an HTTP GET request to the link in the
    &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The
    URL that represents the received shares list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/user-get-openapi.md
- name: Sugar Sync  API - Retrieving Workspace Information
  x-api-slug: workspace-get
  description: To retrieve information about a workspace, an application submits an
    HTTP GET request to then          workspace resource that represents the workspace.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-get-openapi.md
- name: Sugar Sync  API - Retrieving Workspace Contents
  x-api-slug: workspace-get
  description: To retrieve the contents of a workspace, an application submits an
    HTTP GET request to the URLn          that represents the workspace contents.
    Note that the contents of a workspace are the sync folders that are mappedntt  to
    that workspace in SugarSync.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-get-openapi.md
- name: Sugar Sync  API - Updating Workspace Information
  x-api-slug: workspace-put
  description: An application can update attributes of a workspace by issuing an HTTP
    PUT request to the URL that representsnthe workspace resource. In addition, the
    app needs to provide as input, XML that identifies the new attribute values for
    the workspace.nUpon receiving the PUT request, the SugarSync service examines
    the input and updates any of the attributes that have been modified.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/sugarsync-/master/_listings/sugarsync-/workspace-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://stripe.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sugarsync..stack.network
- type: x-application-gallery
  url: https://www.sugarsync.com/partners/
- type: x-base
  url: https://api.sugarsync.com
- type: x-best-practices
  url: https://www.sugarsync.com/dev/best-practices.html
- type: x-blog
  url: http://www.sugarsync.com/blog
- type: x-blog-rss
  url: http://blog.sugarsync.com/blog/feed
- type: x-crunchbase
  url: https://crunchbase.com/organization/sugarsync
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sugarsync
- type: x-developer
  url: https://www.sugarsync.com/developer
- type: x-forum
  url: https://groups.google.com/a/developers.sugarsync.com/forum/#!forum/platform-api/join
- type: x-getting-started
  url: https://www.sugarsync.com/dev/getting-started.html
- type: x-glossary
  url: https://www.sugarsync.com/dev/glossary.html
- type: x-linkedin
  url: https://www.linkedin.com/company/sugarsync
- type: x-pricing
  url: https://www.sugarsync.com/
- type: x-selfservice-registration
  url: https://www.sugarsync.com/developer/signup
- type: x-terms-of-service
  url: https://www.sugarsync.com/dev/terms.html
- type: x-twitter
  url: https://twitter.com/SugarSync
- type: x-website
  url: http://sugarsync.com
- type: x-website
  url: http://www.sugarsync.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---