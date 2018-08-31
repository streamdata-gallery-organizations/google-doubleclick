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
  /userprofiles/{profileId}/reports/{reportId}/run:
    post:
      summary: Run Report
      description: Runs a report
      operationId: dfareporting.reports.run
      parameters:
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the report
      - in: query
        name: synchronous
        description: If set and true, tries to run the report synchronously
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