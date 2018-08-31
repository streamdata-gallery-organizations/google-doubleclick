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
  /userprofiles/{profileId}/floodlightConfigurations:
    get:
      summary: Get Floodlight Configurations
      description: Retrieves a list of floodlight configurations, possibly filtered
      operationId: dfareporting.floodlightConfigurations.list
      parameters:
      - in: query
        name: ids
        description: Set of IDs of floodlight configurations to retrieve
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - advertising
      - floodlight activity group
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