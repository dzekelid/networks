swagger: "2.0"
x-collection-name: Bitly
x-complete: 1
info:
  title: Bitly User Metrics API
  description: the-bitly-user-metrics-api
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/network_history:
    get:
      summary: User Network History
      description: Returns entries from a users network history in reverse chronogical
        order. (A users network history includes publicly saved links from Twitter
        and Facebook connections.)
      operationId: userNetworkHistory
      x-api-path-slug: v3usernetwork-history-get
      parameters:
      - in: query
        name: expand_client_id
        description: whether to provide additional information about encoding application
      - in: query
        name: expand_user
        description: include extra user info in response (login, avatar_url, display_name,
          profile_url, full_name)
      - in: query
        name: limit
        description: 'integer in the range of 1 to 100 that specifies the number of
          records to return (default: 20)'
      - in: query
        name: offset
        description: integer that specifies the first record to return
      responses:
        200:
          description: OK
      tags:
      - User
      - Network
      - History