swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /networks/{owner}/{repo}/events:
    get:
      summary: Get Networks Owner Repo Events
      description: List public events for a network of repositories.
      operationId: list-public-events-for-a-network-of-repositories
      x-api-path-slug: networksownerrepoevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of the owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Networks
      - Owner
      - Repo
      - Events