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
  /userprofiles/{profileId}/reports/{reportId}/files:
    get:
      summary: Get Report Files
      description: Lists files for a report
      operationId: dfareporting.reports.files.list
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the parent report
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is 'DESCENDING'
      responses:
        200:
          description: OK
      tags:
      - advertising
      - report file
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