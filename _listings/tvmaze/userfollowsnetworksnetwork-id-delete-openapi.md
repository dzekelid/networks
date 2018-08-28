---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Delete User Follows Networks
  description: Delete user follows networks.
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/follows/networks:
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworks
      x-api-path-slug: userfollowsnetworks-get
      parameters:
      - in: query
        name: embed
        description: Embed full network info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
  /user/follows/networks/{network_id}:
    delete:
      summary: Delete User Follows Networks
      description: Delete user follows networks.
      operationId: deleteUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---