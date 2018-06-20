{
  "info": {
    "name": "Azure Virtual Network API Virtual Networks Delete",
    "_postman_id": "193712dc-15fb-4549-ac67-c4ef0f4e01bb",
    "description": "Deletes the specified virtual network.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "378f1b3e-5915-44a7-92d4-25b78ad9406c",
          "name": "VirtualNetworks_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/virtualNetworks/:virtualNetworkName"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76414c2f-48cb-4c7a-8d77-7d3c0db47086"
            }
          ]
        }
      ]
    }
  ]
}