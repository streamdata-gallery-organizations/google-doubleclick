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
  /accounts/{accountId}/reports/saved:
    get:
      summary: Get Saved Reports
      description: List all saved reports in this Ad Exchange account
      operationId: adexchangeseller.accounts.reports.saved.list
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved reports
      - in: query
        name: maxResults
        description: The maximum number of saved reports to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through saved reports
      responses:
        200:
          description: OK
      tags:
      - advertising
      - report
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