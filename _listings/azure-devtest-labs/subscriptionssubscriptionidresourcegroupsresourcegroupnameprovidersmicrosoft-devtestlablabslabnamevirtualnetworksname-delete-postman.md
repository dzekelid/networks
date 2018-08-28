{
  "info": {
    "name": "Azure DevTest Labs API Virtual Networks Delete",
    "_postman_id": "fc078ed3-f923-4145-95a6-3c018f827005",
    "description": "Delete virtual network. This operation can take a while to complete.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "virtual networks",
      "item": [
        {
          "id": "e189751f-2582-49e5-ab7c-ffb38136649b",
          "name": "VirtualNetworks_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/virtualnetworks/:name"
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
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete virtual network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2e4ae9a-6e66-438f-b480-e614aeb23160"
            }
          ]
        }
      ]
    }
  ]
}