{
  "info": {
    "name": "Sugar Sync  API Retrieving Album Information",
    "_postman_id": "7fce5f90-2b36-4d8e-aacd-45d8443eb206",
    "description": "To retrieve information about an album, an application submits an HTTP GET request to then          album resource that represents the album.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "03a8bf0e-0a46-4883-9c32-9d86e31bc7b1",
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
              "id": "701b426b-492e-4402-9d90-0f2ca1e3ba98"
            }
          ]
        }
      ]
    }
  ]
}