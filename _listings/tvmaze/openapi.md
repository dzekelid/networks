swagger: "2.0"
x-collection-name: TVmaze
x-complete: 1
info:
  title: TVmaze user
  description: access-to-the-user-api-is-only-possible-for-users-with-a-premiumhttpwww-tvmaze-compremium-account--a-user-can-only-access-their-own-user-data-authentication-uses-http-basic--use-the-tvmaze-username-as-authentication-username-and-the-tvmaze-api-key-as-authentication-password--your-api-key-can-be-found-on-your-dashboardhttpwww-tvmaze-comdashboard--to-try-out-these-api-calls-from-this-page-click-the-authorize-button-on-top-and-input-your-credentials-
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
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
    parameters:
      summary: Parameters User Follows Networks
      description: Parameters user follows networks.
      operationId: parametersUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Networks
    put:
      summary: Put User Follows Networks
      description: Put user follows networks.
      operationId: putUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks