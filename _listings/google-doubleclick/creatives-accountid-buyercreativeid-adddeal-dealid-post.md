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
  /creatives/{accountId}/{buyerCreativeId}/addDeal/{dealId}:
    post:
      summary: Create Deal
      description: Add a deal id association for the creative
      operationId: adexchangebuyer.creatives.addDeal
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      - in: path
        name: dealId
        description: The id of the deal id to associate with this creative
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