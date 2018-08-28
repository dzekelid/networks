{
  "info": {
    "name": "Yammer API Get Exportable Networks",
    "_postman_id": "18d230b8-f762-4f67-95e2-7c28a7cbbcf5",
    "description": "Get Exportable Networks",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "networks",
      "item": [
        {
          "id": "d3372afc-a0b7-4f25-9082-5441f340d6b5",
          "name": "Get_Exportable Networks_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/networks/exportable.json"
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Exportable Networks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "417c2ef0-94bc-4e2b-9b4e-f23d671fc045"
            }
          ]
        }
      ]
    }
  ]
}