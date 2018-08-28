{
  "info": {
    "name": "Azure Virtual Network API Virtual Networks Check IPAddress Availability",
    "_postman_id": "9a813bc0-8c0d-4f1b-9e6d-937e291e2273",
    "description": "Checks whether a private IP address is available for use.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "6266690e-3555-464c-960a-78fb20c9c2fe",
          "name": "VirtualNetworks_CheckIPAddressAvailability",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/virtualNetworks/:virtualNetworkName/CheckIPAddressAvailability"
              ],
              "query": [
                {
                  "key": "ipAddress",
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
            "description": "Checks whether a private IP address is available for use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6e83a71-a6c0-48b4-9c21-6202b317f799"
            }
          ]
        }
      ]
    }
  ]
}