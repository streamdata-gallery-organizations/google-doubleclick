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
  /reports/{reportId}/files/{reportFragment}:
    get:
      summary: Download Report
      description: Downloads a report file encoded in UTF-8
      operationId: doubleclicksearch.reports.getFile
      parameters:
      - in: path
        name: reportFragment
        description: The index of the report fragment to download
      - in: path
        name: reportId
        description: ID of the report
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