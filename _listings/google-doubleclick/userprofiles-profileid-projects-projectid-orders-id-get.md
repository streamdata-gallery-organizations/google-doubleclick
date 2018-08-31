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
  /userprofiles/{profileId}/projects/{projectId}/orders/{id}:
    get:
      summary: Get Order
      description: Gets one order by ID
      operationId: dfareporting.orders.get
      parameters:
      - in: path
        name: id
        description: Order ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for orders
      responses:
        200:
          description: OK
      tags:
      - advertising
      - order
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