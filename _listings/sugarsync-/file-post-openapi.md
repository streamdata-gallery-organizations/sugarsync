---
swagger: "2.0"
x-collection-name: SugarSync
x-complete: 0
info:
  title: Sugar Sync  API Creating a New File Version
  description: nAn application can create a new version of a file by submitting an
    HTTP POST request to the URL that represents the version history. The version
    history URL is returned in the &lt;versions&gt; element whenn retrieving information
    about a file.n
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