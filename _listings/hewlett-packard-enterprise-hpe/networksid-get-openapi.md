---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Networks
  description: Returns a network based on its id. It requires any project role or
    non-'consumer' global role.
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