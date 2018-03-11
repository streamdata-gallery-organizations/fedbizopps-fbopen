---
swagger: "2.0"
info:
  title: FBOpen API
  description: This is the API documentation for the FBOpen API, a search API of opportunities
    to work with the U.S. government.
  version: 1.0.0
host: api.data.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gsa/fbopen/v0/opp:
    post:
      summary: Search Opportunities
      description: Individual opportunities can be modified if POST functionality
        is enabled in the API
      operationId: postOpportunity
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - business opportunities
definitions: []
x-collection-name: FedBizOpps (FBOpen)
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