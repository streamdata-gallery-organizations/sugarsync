{
  "info": {
    "name": "Sugar Sync  API Updating Folder Information",
    "_postman_id": "a7701d46-c8a4-466b-94b8-6c4421b26ce3",
    "description": "An application can update various attributes of a folder by issuing an HTTP PUT request to the URL thatnrepresents the folder resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the folder. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "f83047e4-745b-45bf-b144-39ebe669cdf2",
          "name": "retrieving-album-information",
          "request": {
            "url": "http://api.sugarsync.com/album/?max=%7B%7D&order=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about an album, an application submits an HTTP GET request to then          album resource that represents the album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90ea23f3-4963-4324-ac7e-b62da939b994"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "5396fd52-4dcb-429a-9f51-b1dca0f2f2ca",
          "name": "creating-a-refresh-token",
          "request": {
            "url": "http://api.sugarsync.com/app-authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API.nTo do that, the app needs to create a refresh token. When a user first runs the application, it creates a refresh tokennby submitting a POST request that includes the users credentials to the API.nIf the request is successful, the SugarSync service grants the application permission to access the users account and returns a refresh token.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0965baf-f925-4c5a-bc9e-d38d47be4792"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "9c2b1005-18d5-417e-8439-0f50eb6c066a",
          "name": "creating-an-access-token",
          "request": {
            "url": "http://api.sugarsync.com/authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API. To do that,nthe app needs to create an access token, which allows the app to access files, folders,nand other resources within a users account. After the token is created, the app needs to specify it in the HTTP request header when it makes a request through the API to access a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fb1588d-44b2-457f-80e7-f87b21a0efe5"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "98b456f2-bf95-44e9-b629-42076b2fda4a",
          "name": "retrieving-contact-information",
          "request": {
            "url": "http://api.sugarsync.com/contact/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A contact represents another SugarSync user who has shared a folder or folders with this user.n          To retrieve information about a contact, an application submits an HTTP GET request to then          contact resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc7e51c-73fa-4bb4-b6e7-7b0ed8483edd"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "11f4ac6a-7914-4be2-bba0-b972b79fd735",
          "name": "retrieving-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve file data, an application submits an HTTP GET request to then          file data resource that represents the data for the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "877fe673-698e-4437-95b5-6c8ddf23073b"
            }
          ]
        },
        {
          "id": "16d90200-d359-40c0-a7b6-20cf1dac1dfb",
          "name": "uploading-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "An application can upload data to a file by issuing an HTTP PUT request to thenfile data resource that represents the data for the file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07386033-dcf8-45c5-b76a-e941890f48d2"
            }
          ]
        },
        {
          "id": "ab6da1f0-3ab1-45a2-a3d5-26413308170d",
          "name": "retrieving-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a file, an application submits an HTTP GET request to then          file resource that represents the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d9da167-d05f-44f2-b6ca-27065dd9f23a"
            }
          ]
        },
        {
          "id": "4e194de3-ba2f-41a6-803c-ddfa9c3d6a71",
          "name": "updating-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can update various attributes of a file by issuing an HTTP PUT request to the URL thatnrepresents the file resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the file. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94d5eaa5-0e40-4513-9c0f-8f5d11c7c438"
            }
          ]
        },
        {
          "id": "2d2ae548-69f2-41aa-a222-2735a1343177",
          "name": "creating-a-new-file-version",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "nAn application can create a new version of a file by submitting an HTTP POST request to the URL that represents the version history. The version history URL is returned in the &lt;versions&gt; element whenn retrieving information about a file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06484355-7ee3-4f80-948f-56372c4c27ba"
            }
          ]
        },
        {
          "id": "0854ad7a-0219-4369-8351-3db34204b216",
          "name": "deleting-a-file",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanently delete a file by issuing an HTTP DELETE request to the URL of thenfile resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0771b59f-3b2d-4f3e-a0cf-33855a01461d"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "db2342f0-7c12-44f3-91fc-361d0ecbe601",
          "name": "retrieving-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a folder, an application submits an HTTP GET request to then          folder resource that represents the folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c929b84-29a3-4030-95be-8accfb5f9b5c"
            }
          ]
        },
        {
          "id": "ed86ff97-9b08-4907-88c6-6b2402d3ca2a",
          "name": "retrieving-folder-contents",
          "request": {
            "url": "http://api.sugarsync.com/folder/?max=%7B%7D&order=%7B%7D&start=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve the contents of a folder, an application submits an HTTP GET request to the URLn          that represents the folder contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bd7a479-7835-437c-a276-d3823546371a"
            }
          ]
        },
        {
          "id": "4eb1b1b7-633a-4dbd-a656-ba342fd0b086",
          "name": "updating-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can update various attributes of a folder by issuing an HTTP PUT request to the URL thatnrepresents the folder resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the folder. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37c1117a-2f6c-4ab3-beb1-9106dac37acc"
            }
          ]
        },
        {
          "id": "25d19e4b-fac1-430d-8d6c-f4ce0beb9f70",
          "name": "creating-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can create a folder within another folder by issuing an HTTP POST request to the URL ofnthe containing folder resource.nIn addition, the application needs to provide as input, XML that identifies the display name of the folder to be created.nNote that an application can create a folder only within another folder, and not directly in a workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dce0e7d-3349-4646-93b2-24e9418c2c10"
            }
          ]
        },
        {
          "id": "ddf6b9f6-1611-4693-810e-45e2d6f03621",
          "name": "deleting-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanantly delete a folder by issuing an HTTP DELETE request to the URL of thenfolder resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9de5f81-e9e3-42a7-bcd7-0811c6246f48"
            }
          ]
        }
      ]
    }
  ]
}