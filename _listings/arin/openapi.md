---
swagger: "2.0"
x-collection-name: ARIN
x-complete: 1
info:
  title: Network API
  description: for-managing-network-details-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /nets:
    get:
      summary: Networks
      description: ""
      operationId: nets
      x-api-path-slug: nets-get
      parameters:
      - in: query
        name: handle
        description: the handle of the network
        type: string
        format: string
      - in: query
        name: name
        description: the name of the network
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Networks
---