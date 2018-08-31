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
  /userprofiles/{profileId}/creatives:
    get:
      summary: Get Creatives
      description: Retrieves a list of creatives, possibly filtered
      operationId: dfareporting.creatives.list
      parameters:
      - in: query
        name: active
        description: Select only active creatives
      - in: query
        name: advertiserId
        description: Select only creatives with this advertiser ID
      - in: query
        name: archived
        description: Select only archived creatives
      - in: query
        name: campaignId
        description: Select only creatives with this campaign ID
      - in: query
        name: companionCreativeIds
        description: Select only in-stream video creatives with these companion IDs
      - in: query
        name: creativeFieldIds
        description: Select only creatives with these creative field IDs
      - in: query
        name: ids
        description: Select only creatives with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: renderingIds
        description: Select only creatives with these rendering IDs
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sizeIds
        description: Select only creatives with these size IDs
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: studioCreativeId
        description: Select only creatives corresponding to this Studio creative ID
      - in: query
        name: types
        description: Select only creatives with these creative types
      responses:
        200:
          description: OK
      tags:
      - advertising
      - creative
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