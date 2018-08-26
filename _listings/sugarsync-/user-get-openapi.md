---
swagger: "2.0"
x-collection-name: SugarSync
x-complete: 0
info:
  title: Sugar Sync  API Retrieving Received Shares List
  description: One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe
    element contains a link to a list that describes the shared folders that are owned
    by other users and to which this user has been granted access privileges by those
    owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To
    retrieve the list, an application submits an HTTP GET request to the link in the
    &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The
    URL that represents the received shares list.
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /album/:
    get:
      summary: Retrieving Album Information
      description: To retrieve information about an album, an application submits
        an HTTP GET request to then          album resource that represents the album.
      operationId: retrieving-album-information
      x-api-path-slug: album-get
      parameters:
      - in: query
        name: max
        description: Positive integer
      - in: query
        name: order
        description: name, last_modified, size, or extension
      - in: query
        name: start
        description: 0 or positive integer
      responses:
        200:
          description: OK
      tags:
      - Album
  /app-authorization:
    post:
      summary: Creating a Refresh Token
      description: An application needs to be authorized to access a users SugarSync
        resources through the Platform API.nTo do that, the app needs to create a
        refresh token. When a user first runs the application, it creates a refresh
        tokennby submitting a POST request that includes the users credentials to
        the API.nIf the request is successful, the SugarSync service grants the application
        permission to access the users account and returns a refresh token.n
      operationId: creating-a-refresh-token
      x-api-path-slug: appauthorization-post
      parameters:
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        200:
          description: OK
      tags:
      - App
      - Authorization
  /authorization:
    post:
      summary: Creating an Access Token
      description: An application needs to be authorized to access a users SugarSync
        resources through the Platform API. To do that,nthe app needs to create an
        access token, which allows the app to access files, folders,nand other resources
        within a users account. After the token is created, the app needs to specify
        it in the HTTP request header when it makes a request through the API to access
        a resource.
      operationId: creating-an-access-token
      x-api-path-slug: authorization-post
      parameters:
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        200:
          description: OK
      tags:
      - Authorization
  /contact/:
    get:
      summary: Retrieving Contact Information
      description: A contact represents another SugarSync user who has shared a folder
        or folders with this user.n          To retrieve information about a contact,
        an application submits an HTTP GET request to then          contact resource.
      operationId: retrieving-contact-information
      x-api-path-slug: contact-get
      responses:
        200:
          description: OK
      tags:
      - Contact
  /file:
    get:
      summary: Retrieving File Data
      description: To retrieve file data, an application submits an HTTP GET request
        to then          file data resource that represents the data for the file.
      operationId: retrieving-file-data
      x-api-path-slug: file-get
      responses:
        200:
          description: OK
      tags:
      - File
    put:
      summary: Uploading File Data
      description: An application can upload data to a file by issuing an HTTP PUT
        request to thenfile data resource that represents the data for the file.n
      operationId: uploading-file-data
      x-api-path-slug: file-put
      responses:
        200:
          description: OK
      tags:
      - File
  /file/:
    delete:
      summary: Deleting a File
      description: An application can permanently delete a file by issuing an HTTP
        DELETE request to the URL of thenfile resource.nIts a good idea to precede
        DELETE requests like this with a caution note in your applications user interface.n
      operationId: deleting-a-file
      x-api-path-slug: file-delete
      responses:
        200:
          description: OK
      tags:
      - File
    get:
      summary: Retrieving File Information
      description: To retrieve information about a file, an application submits an
        HTTP GET request to then          file resource that represents the file.
      operationId: retrieving-file-information
      x-api-path-slug: file-get
      responses:
        200:
          description: OK
      tags:
      - File
    post:
      summary: Creating a New File Version
      description: nAn application can create a new version of a file by submitting
        an HTTP POST request to the URL that represents the version history. The version
        history URL is returned in the &lt;versions&gt; element whenn retrieving information
        about a file.n
      operationId: creating-a-new-file-version
      x-api-path-slug: file-post
      responses:
        200:
          description: OK
      tags:
      - File
    put:
      summary: Updating File Information
      description: An application can update various attributes of a file by issuing
        an HTTP PUT request to the URL thatnrepresents the file resource. In addition,
        the app needs to provide as input, XML that identifies the new attribute values
        for the file. Upon receiving the PUT request, the SugarSync service examines
        the input and updates any of the attributes that have been modified.
      operationId: updating-file-information
      x-api-path-slug: file-put
      parameters:
      - in: header
        name: Authorization
        description: The access token
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        200:
          description: OK
      tags:
      - File
  /folder:
    get:
      summary: Retrieving Folder Information
      description: To retrieve information about a folder, an application submits
        an HTTP GET request to then          folder resource that represents the folder.
      operationId: retrieving-folder-information
      x-api-path-slug: folder-get
      responses:
        200:
          description: OK
      tags:
      - Folder
  /folder/:
    delete:
      summary: Deleting a Folder
      description: An application can permanantly delete a folder by issuing an HTTP
        DELETE request to the URL of thenfolder resource.nIts a good idea to precede
        DELETE requests like this with a caution note in your applications user interface.n
      operationId: deleting-a-folder
      x-api-path-slug: folder-delete
      responses:
        200:
          description: OK
      tags:
      - Folder
    get:
      summary: Retrieving Folder Contents
      description: To retrieve the contents of a folder, an application submits an
        HTTP GET request to the URLn          that represents the folder contents.
      operationId: retrieving-folder-contents
      x-api-path-slug: folder-get
      parameters:
      - in: query
        name: max
        description: Positive integer
      - in: query
        name: order
        description: name, last_modified, size, or extension
      - in: query
        name: start
        description: 0 or positive integer
      - in: query
        name: type
        description: folder or file
      responses:
        200:
          description: OK
      tags:
      - Folder
    post:
      summary: Creating a Folder
      description: An application can create a folder within another folder by issuing
        an HTTP POST request to the URL ofnthe containing folder resource.nIn addition,
        the application needs to provide as input, XML that identifies the display
        name of the folder to be created.nNote that an application can create a folder
        only within another folder, and not directly in a workspace.
      operationId: creating-a-folder
      x-api-path-slug: folder-post
      parameters:
      - in: header
        name: Authorization
        description: The access token
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        200:
          description: OK
      tags:
      - Folder
    put:
      summary: Updating Folder Information
      description: An application can update various attributes of a folder by issuing
        an HTTP PUT request to the URL thatnrepresents the folder resource. In addition,
        the app needs to provide as input, XML that identifies the new attribute values
        for the folder. Upon receiving the PUT request, the SugarSync service examines
        the input and updates any of the attributes that have been modified.
      operationId: updating-folder-information
      x-api-path-slug: folder-put
      parameters:
      - in: header
        name: Authorization
        description: The access token
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        200:
          description: OK
      tags:
      - Folder
  /receivedShare/:
    get:
      summary: Retrieving Received Share Information
      description: To retrieve information about a received share (that is, a shared
        folder owned by another user and to whichnthis user has been granted access
        privileges by the owner), an application submits an HTTP GET request to the
        URLnthat represents the received share resource. The URL is referenced in
        the &lt;receivedShare&gt; element for the received share in the received shares
        list.nSee Retrieving the Received Shares List.
      operationId: retrieving-received-share-information
      x-api-path-slug: receivedshare-get
      responses:
        200:
          description: OK
      tags:
      - ReceivedShare
  /user:
    get:
      summary: Retrieving User Information
      description: To retrieve information about a SugarSync user, an application
        submits an HTTP GET request to thenuser resource that represents the user.
      operationId: retrieving-user-information
      x-api-path-slug: user-get
      parameters:
      - in: query
        name: max
        description: The maximum number of workspaces, beginning with the workspace
          at the start index, that the clienttt  wants listed in the response
      - in: query
        name: start
        description: Specifies the index within the indexed sequence of workspaces
          in the users account where thett  client wants workspaces to be retrieved
      responses:
        200:
          description: OK
      tags:
      - User
  /user/:
    get:
      summary: Retrieving Received Shares List
      description: One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe
        element contains a link to a list that describes the shared folders that are
        owned by other users and to which this user has been granted access privileges
        by those owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To
        retrieve the list, an application submits an HTTP GET request to the link
        in the &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The
        URL that represents the received shares list.
      operationId: retrieving-received-shares-list
      x-api-path-slug: user-get
      parameters:
      - in: query
        name: max
        description: The maximum number of albums, beginning with the album at the
          start index, that the clienttt  wants listed in the response
      - in: query
        name: start
        description: Specifies the index within the indexed sequence of albums in
          the users account where thett  client wants albums to be retrieved
      responses:
        200:
          description: OK
      tags:
      - User
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