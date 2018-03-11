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
  /billinginfo/{accountId}:
    get:
      summary: Get Billing Info
      description: Returns the billing information for one account specified by account
        ID
      operationId: adexchangebuyer.billingInfo.get
      parameters:
      - in: path
        name: accountId
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - advertising
      - billing
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