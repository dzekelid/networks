---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Switc hto Network Mode
  description: Switches the network mode from auto subnet mode to custom subnet mode.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/networks:
    get:
      summary: Get Networks
      description: Retrieves the list of networks available to the specified project.
      operationId: compute.networks.list
      x-api-path-slug: projectglobalnetworks-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Network
    post:
      summary: Create Network
      description: Creates a network in the specified project using the data included
        in the request.
      operationId: compute.networks.insert
      x-api-path-slug: projectglobalnetworks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Network
  /{project}/global/networks/{network}:
    delete:
      summary: Delete Network
      description: Deletes the specified network.
      operationId: compute.networks.delete
      x-api-path-slug: projectglobalnetworksnetwork-delete
      parameters:
      - in: path
        name: network
        description: Name of the network to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Network
    get:
      summary: Get Network
      description: Returns the specified network. Get a list of available networks
        by making a list() request.
      operationId: compute.networks.get
      x-api-path-slug: projectglobalnetworksnetwork-get
      parameters:
      - in: path
        name: network
        description: Name of the network to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Network
  /{project}/global/networks/{network}/switchToCustomMode:
    post:
      summary: Switc hto Network Mode
      description: Switches the network mode from auto subnet mode to custom subnet
        mode.
      operationId: compute.networks.switchToCustomMode
      x-api-path-slug: projectglobalnetworksnetworkswitchtocustommode-post
      parameters:
      - in: path
        name: network
        description: Name of the network to be updated
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Network
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