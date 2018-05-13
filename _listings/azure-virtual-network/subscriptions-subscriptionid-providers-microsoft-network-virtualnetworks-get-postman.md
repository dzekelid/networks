{
  "info": {
    "name": "Azure Virtual Network API Virtual Networks List All",
    "_postman_id": "8588286a-168c-4a1c-9de4-be4657d8a8c9",
    "description": "Gets all virtual networks in a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "3c581598-ae04-4389-be85-23ab071a0d3d",
          "name": "VirtualNetworks_ListAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/virtualNetworks"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all virtual networks in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1998bd61-f900-4c2e-82e0-60272c315cdc"
            }
          ]
        }
      ]
    }
  ]
}