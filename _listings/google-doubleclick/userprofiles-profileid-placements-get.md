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
  /userprofiles/{profileId}/placements:
    get:
      summary: Get Placements
      description: Retrieves a list of placements, possibly filtered
      operationId: dfareporting.placements.list
      parameters:
      - in: query
        name: advertiserIds
        description: Select only placements that belong to these advertisers
      - in: query
        name: archived
        description: Select only archived placements
      - in: query
        name: campaignIds
        description: Select only placements that belong to these campaigns
      - in: query
        name: compatibilities
        description: Select only placements that are associated with these compatibilities
      - in: query
        name: contentCategoryIds
        description: Select only placements that are associated with these content
          categories
      - in: query
        name: directorySiteIds
        description: Select only placements that are associated with these directory
          sites
      - in: query
        name: groupIds
        description: Select only placements that belong to these placement groups
      - in: query
        name: ids
        description: Select only placements with these IDs
      - in: query
        name: maxEndDate
        description: Select only placements or placement groups whose end date is
          on or before the specified maxEndDate
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: maxStartDate
        description: Select only placements or placement groups whose start date is
          on or before the specified maxStartDate
      - in: query
        name: minEndDate
        description: Select only placements or placement groups whose end date is
          on or after the specified minEndDate
      - in: query
        name: minStartDate
        description: Select only placements or placement groups whose start date is
          on or after the specified minStartDate
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: query
        name: paymentSource
        description: Select only placements with this payment source
      - in: query
        name: placementStrategyIds
        description: Select only placements that are associated with these placement
          strategies
      - in: query
        name: pricingTypes
        description: Select only placements with these pricing types
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for placements by name or ID
      - in: query
        name: siteIds
        description: Select only placements that are associated with these sites
      - in: query
        name: sizeIds
        description: Select only placements that are associated with these sizes
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - advertising
      - placement
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