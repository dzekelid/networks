{
  "info": {
    "name": "Azure Virtual Network API Virtual Networks List",
    "_postman_id": "3d990b78-0284-4239-9504-1d466ae8b1d1",
    "description": "Gets all virtual networks in a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "74107950-a8dc-4588-8d92-676efaa4e517",
          "name": "VirtualNetworks_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/virtualNetworks"
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
            "description": "Gets all virtual networks in a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e95fb335-f9d1-43ea-82a6-e2152acefcb7"
            }
          ]
        }
      ]
    }
  ]
}