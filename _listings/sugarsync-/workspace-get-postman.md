{
  "info": {
    "name": "Sugar Sync  API Retrieving Workspace Contents",
    "_postman_id": "da9a9dc7-ad0d-4376-9568-7707135d5142",
    "description": "To retrieve the contents of a workspace, an application submits an HTTP GET request to the URLn          that represents the workspace contents. Note that the contents of a workspace are the sync folders that are mappedntt  to that workspace in SugarSync.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "18c83bea-aef6-4b13-808c-ae8af2007274",
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
              "id": "12248c61-35dd-4d35-b180-1db094b60d7f"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "c32981f1-9fa2-435c-8672-8bd7a306db4f",
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
              "id": "d42b371f-305b-4108-9bc1-9473f5023126"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "817be6dc-9963-4e94-acec-50f1e37f3875",
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
              "id": "cdd403ee-71aa-41e4-a786-94b833201c5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "f2c725eb-9633-4aaf-bd2b-9c423bccff51",
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
              "id": "5b978935-cefc-408a-95d8-36c74d88ddf1"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "0409c688-3f10-4d24-86e4-a66246a7612b",
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
              "id": "53c7e225-c2a7-4917-8caa-8124eaa4ff78"
            }
          ]
        },
        {
          "id": "bd15e15a-3b53-4669-af5f-132e0ca25eca",
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
              "id": "65797201-5448-4e4a-aee9-0d79e417fe34"
            }
          ]
        },
        {
          "id": "ecb026af-c887-46b1-9336-a918ec02b2e6",
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
              "id": "468959ac-c1fd-4790-8aff-0665d676e449"
            }
          ]
        },
        {
          "id": "ff5a1382-2e4d-4b62-882d-f36c53811282",
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
              "id": "64420840-5de3-4bdd-bf61-cdb179e231b1"
            }
          ]
        },
        {
          "id": "66d3d242-32a9-4774-a04b-75d617b7bae6",
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
              "id": "d3e65f29-ada1-4363-a60e-e505e6c2584b"
            }
          ]
        },
        {
          "id": "c753bb19-b814-4b21-a968-8a892f96561a",
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
              "id": "12bf77b6-4e36-44b1-ab25-9e372e08bcba"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "573875f3-d077-485b-8cf8-bab4791f24e4",
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
              "id": "d7d2991d-2d82-4340-bc17-192eda50e9e2"
            }
          ]
        },
        {
          "id": "d77defca-c8ef-453a-8527-e2bba9d0290c",
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
              "id": "3267aafa-8d56-4bed-91dd-6f5198f5fae8"
            }
          ]
        },
        {
          "id": "9a3798a5-a721-47a1-8a66-376e5d1fce31",
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
              "id": "8ce1c3bb-1c5c-4354-81c7-61dd2b50c69e"
            }
          ]
        },
        {
          "id": "39a34425-dcac-4dae-a21d-3868f6a78f3f",
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
              "id": "f9686f08-a4bb-4348-82e1-de4e6b704498"
            }
          ]
        },
        {
          "id": "cf8ab4e8-a3d4-48bb-8465-25231946f0c6",
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
              "id": "f05442ac-5810-4c16-8bd1-131097fb5e6f"
            }
          ]
        }
      ]
    },
    {
      "name": "ReceivedShare",
      "item": [
        {
          "id": "5cc12ae1-76bc-454a-a9aa-c91d18bbf950",
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
              "id": "26b35498-7257-43f1-914d-5b74bf2d7d70"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "feb21ece-d4b4-4d0c-af6c-5074cb01ecc4",
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
              "id": "e0c041a2-80a6-4c55-8129-ed6375bc15cc"
            }
          ]
        },
        {
          "id": "32620f4e-3687-4a06-ae3e-dcc05bd30c3f",
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
              "id": "0f78b052-a916-464c-a342-b5fc331e8716"
            }
          ]
        }
      ]
    },
    {
      "name": "Workspace",
      "item": [
        {
          "id": "7304da9a-04fc-4ec9-a59f-a2afb6645518",
          "name": "retrieving-workspace-information",
          "request": {
            "url": "http://api.sugarsync.com/workspace",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a workspace, an application submits an HTTP GET request to then          workspace resource that represents the workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8912e0a5-3f28-4ab8-bd28-0bffee755e5e"
            }
          ]
        },
        {
          "id": "37de687f-c2f2-4754-88d1-aceed08d1c91",
          "name": "retrieving-workspace-contents",
          "request": {
            "url": "http://api.sugarsync.com/workspace/?max=%7B%7D&order=%7B%7D&start=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve the contents of a workspace, an application submits an HTTP GET request to the URLn          that represents the workspace contents. Note that the contents of a workspace are the sync folders that are mappedntt  to that workspace in SugarSync."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc1fc87a-b811-4dd1-bd02-d93304d63896"
            }
          ]
        }
      ]
    }
  ]
}