swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /networks:
    get:
      summary: Get Networks
      description: Returns networks. It requires any project role or non-'consumer'
        global role.
      operationId: FindNetworks
      x-api-path-slug: networks-get
      parameters:
      - in: query
        name: query
        description: Filters the networks returned
      responses:
        200:
          description: OK
      tags:
      - Networks
  /networks/{id}:
    get:
      summary: Get Networks
      description: Returns a network based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetNetworkById
      x-api-path-slug: networksid-get
      parameters:
      - in: path
        name: id
        description: ID of network to fetch
      - in: query
        name: query
        description: Filters the networks returned
      responses:
        200:
          description: OK
      tags:
      - Networks
    patch:
      summary: Patch Networks
      description: Updates a network. It requires the **administrator** global role.
      operationId: ModifyNetwork
      x-api-path-slug: networksid-patch
      parameters:
      - in: path
        name: id
        description: ID of the network to update
      - in: body
        name: network
        description: Update network
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Networks