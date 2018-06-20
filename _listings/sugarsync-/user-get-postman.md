{
  "info": {
    "name": "Sugar Sync  API Retrieving Received Shares List",
    "_postman_id": "c5a4b2d9-0869-476c-91ff-ac5c76e60676",
    "description": "One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe element contains a link to a list that describes the shared folders that are owned by other users and to which this user has been granted access privileges by those owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To retrieve the list, an application submits an HTTP GET request to the link in the &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The URL that represents the received shares list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "b8077b6c-93d8-4da7-ac54-3ce9e7514355",
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
              "id": "757bc46b-9ff2-431e-bf7f-96b4bb6192fb"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "7175fe29-5607-4ceb-8cd9-c18a5a6a210a",
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
              "id": "7c45a98f-f4a1-4547-9b6b-9e884846169b"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "e0f8c161-9d63-467b-ba66-5c7c354453c2",
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
              "id": "3d85af6f-5e6c-4e50-94cc-99f944cbd8c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "5e48384b-1992-486c-b0ef-159834c507d2",
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
              "id": "8de3c74a-5c04-45ce-9570-df7d1ec4ac48"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "13d55382-5a0e-4c76-ad90-6421bf0e9989",
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
              "id": "d9a207b3-937a-4bfc-aa21-e5d246c99f28"
            }
          ]
        },
        {
          "id": "ac8807b1-60e1-4d4e-b6d5-7b98f487c988",
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
              "id": "8207d03c-bcd4-4649-a2a3-da918c1909df"
            }
          ]
        },
        {
          "id": "8fb04cc7-80d2-4e71-a062-a2ec9b25f9f2",
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
              "id": "aec2d650-7a60-44cf-a60b-c97742dc201a"
            }
          ]
        },
        {
          "id": "6b4713ae-0853-49c0-a977-5f30a3b0707f",
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
              "id": "98283b62-8bbe-4381-8b92-53bb48837c05"
            }
          ]
        },
        {
          "id": "96efbc36-54d7-4ea0-8417-41ac2a2b0679",
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
              "id": "05e2e72f-f669-4b57-a17d-a72c3cb08f64"
            }
          ]
        },
        {
          "id": "fa509e8e-1d3e-45d9-bce4-6222d4ce4c3c",
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
              "id": "815a3bf2-5585-4d97-b54e-1a57c1970cb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "968977bf-f7b8-4b47-b6da-2f1bf1cfcd01",
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
              "id": "7931d0aa-4d38-43b1-a7ce-a7775e6b355a"
            }
          ]
        },
        {
          "id": "74ed7dc0-0985-4442-94c7-470bc560d493",
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
              "id": "9632cfcf-0622-4a5d-b40f-694bbeb0a392"
            }
          ]
        },
        {
          "id": "295d4d96-0c19-45f7-90f2-f13b1708cc5c",
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
              "id": "568ee268-a06b-4abb-be51-c6801b430e09"
            }
          ]
        },
        {
          "id": "52897be3-2b34-46fb-a20d-ae9b86439565",
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
              "id": "a4c96ce8-95ba-4c85-82b8-2fef6474644a"
            }
          ]
        },
        {
          "id": "44135f9b-42ab-4ac6-a05c-11506fa7727c",
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
              "id": "7d26a005-6f81-4eb9-984e-a840109485e2"
            }
          ]
        }
      ]
    },
    {
      "name": "ReceivedShare",
      "item": [
        {
          "id": "d49a9387-8142-4708-bc55-879da156ffc1",
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
              "id": "922a0284-d969-4ac7-a73e-a0ca92eed7b8"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "0298089d-bbf5-4f89-8ec6-7ead7ad56d75",
          "name": "retrieving-user-information",
          "request": {
            "url": "http://api.sugarsync.com/user?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a SugarSync user, an application submits an HTTP GET request to thenuser resource that represents the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b7697e9-0ada-4710-b0a0-790f7b304289"
            }
          ]
        },
        {
          "id": "540fe709-2258-4440-8d98-381cad43fe46",
          "name": "retrieving-received-shares-list",
          "request": {
            "url": "http://api.sugarsync.com/user/?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe element contains a link to a list that describes the shared folders that are owned by other users and to which this user has been granted access privileges by those owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To retrieve the list, an application submits an HTTP GET request to the link in the &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The URL that represents the received shares list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecc3a983-1f23-4b5d-92ff-4e1d5057f6b4"
            }
          ]
        }
      ]
    }
  ]
}