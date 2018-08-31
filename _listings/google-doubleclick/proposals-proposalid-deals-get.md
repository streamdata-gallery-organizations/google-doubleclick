---
swagger: "2.0"
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /proposals/{proposalId}/deals:
    get:
      summary: Get Proposal Deals
      description: List all the deals for a given proposal
      operationId: adexchangebuyer.marketplacedeals.list
      parameters:
      - in: query
        name: pqlQuery
        description: Query string to retrieve specific deals
      - in: path
        name: proposalId
        description: The proposalId to get deals for
      responses:
        200:
          description: OK
      tags:
      - advertising
      - deal
definitions: []
x-collection-name: Google Doubleclick
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