{
  "info": {
    "name": "Azure Virtual Network API Virtual Networks Get",
    "_postman_id": "463b3f1a-576a-42c1-a066-f96f8c761854",
    "description": "Gets the specified virtual network by resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "5e63c1a1-4409-4869-94f8-d0181f889d6a",
          "name": "VirtualNetworks_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/virtualNetworks/:virtualNetworkName"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualNetworkName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets the specified virtual network by resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc64caec-8f3f-4f2e-9108-b0d6b79f8fb8"
            }
          ]
        }
      ]
    }
  ]
}