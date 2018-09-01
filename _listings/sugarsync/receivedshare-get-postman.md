{
  "info": {
    "name": "Sugar Sync  API Retrieving Received Share Information",
    "_postman_id": "cc01805a-3b0c-49c1-b643-ef423d06824a",
    "description": "To retrieve information about a received share (that is, a shared folder owned by another user and to whichnthis user has been granted access privileges by the owner), an application submits an HTTP GET request to the URLnthat represents the received share resource. The URL is referenced in the &lt;receivedShare&gt; element for the received share in the received shares list.nSee Retrieving the Received Shares List.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "8288bc2e-b5e3-4682-ae09-5291711d6868",
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
              "id": "ae3b4d3c-5e6f-4293-9c95-6fcb1a0c6690"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "db5566a6-a9fb-450f-9caf-358e60f94bf6",
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
              "id": "04df6656-9735-4fb0-9c80-8fc67d4b0ae2"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "f2fdf2e2-c734-4e76-8b97-1a7547fcf88f",
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
              "id": "dda3c58c-a89b-4c75-b921-94b223870885"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "06ecd264-be7b-49e3-b547-544e4bbf467a",
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
              "id": "0b270ec8-0518-40ee-8c0e-b1126da0681d"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "70595a2b-e3cb-4f11-893a-fb2523b96be6",
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
              "id": "551823db-c679-44af-9f62-8fca149aa1e4"
            }
          ]
        },
        {
          "id": "2bab0e74-feca-4647-a109-a9279e3c9eae",
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
              "id": "457a1531-435a-49f7-9b8f-aeb8164cca0b"
            }
          ]
        },
        {
          "id": "cae9b0e5-bf4e-4fb4-a530-75a3ce3627a7",
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
              "id": "a33f5593-0b3d-4934-a086-ccb91923f403"
            }
          ]
        },
        {
          "id": "9b356749-e2a8-4817-b140-dc667df85207",
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
              "id": "4e2c2321-5e64-4a8d-a846-e6f91df89be4"
            }
          ]
        },
        {
          "id": "2d7440f7-e0aa-4fc6-89ff-448b4f0f82bc",
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
              "id": "29497b07-b1c8-43cd-92ae-c9644fd8394c"
            }
          ]
        },
        {
          "id": "ad00f9ae-5fea-43ff-8b48-f34569c25ba5",
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
              "id": "e27ae488-d87e-4f83-8679-2ab53cdc6d8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "cc2fb148-8c68-42b1-88c4-02fbfc3548f7",
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
              "id": "a0cce2a6-301a-49a6-bd61-3c142260f7e1"
            }
          ]
        },
        {
          "id": "b1edf576-cf45-4bd2-a652-8582409b0fbe",
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
              "id": "23b097c5-9eec-4934-91b3-2e19de5ea364"
            }
          ]
        },
        {
          "id": "999e7f88-cf22-4403-9927-3bbaabf0e3e7",
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
              "id": "36605e02-3528-4c8a-8783-27c3e5166089"
            }
          ]
        },
        {
          "id": "a61312a9-ae07-4034-96fd-45d93e610db2",
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
              "id": "990fe05a-864d-4609-98f6-85f80b612636"
            }
          ]
        },
        {
          "id": "9ddb4d6c-1d5e-411b-99c1-af66ac0ae19d",
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
              "id": "349bfe4f-918c-436f-bb1f-efc8b2e1d6e7"
            }
          ]
        }
      ]
    },
    {
      "name": "ReceivedShare",
      "item": [
        {
          "id": "f9ef07de-768e-47e5-8616-d810ba8dce79",
          "name": "retrieving-received-share-information",
          "request": {
            "url": "http://api.sugarsync.com/receivedShare/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a received share (that is, a shared folder owned by another user and to whichnthis user has been granted access privileges by the owner), an application submits an HTTP GET request to the URLnthat represents the received share resource. The URL is referenced in the &lt;receivedShare&gt; element for the received share in the received shares list.nSee Retrieving the Received Shares List."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd8bf08c-2a68-4e71-8ee4-4637d0690f61"
            }
          ]
        }
      ]
    }
  ]
}