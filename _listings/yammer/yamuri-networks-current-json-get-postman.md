{
  "info": {
    "name": "Yammer API Get Network Request",
    "_postman_id": "f31252e1-d63b-4dbd-a4ed-78c840d95551",
    "description": "Facilitates switching a user between different Yammer networks. All Yammer web requests contain a network permalink in the URL (https://www.yammer.com/network_permalink/resource_path) to denote the network context. API requests use a different OAuth token for each user/network combination.\n\nParameters:\ninclude_suspended=TRUE - Optional. Include networks the user is suspended in.\n\nexclude_own_messages_from_unseen=TRUE - Optional. Exclude the user’s own messages from the unseen count. This is good for unread badges.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "networks",
      "item": [
        {
          "id": "3db13cce-9bf6-45bb-a96b-3e2082660457",
          "name": "Get_Network Request_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/networks/current.json"
              ],
              "query": [
                {
                  "key": "exclude_own_messages_from_unseen",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_suspended",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Facilitates switching a user between different Yammer networks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a989f05-7245-43a3-8fea-e97475ebee0c"
            }
          ]
        }
      ]
    }
  ]
}