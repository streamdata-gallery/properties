---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List properties
  description: Lists all properties.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/properties:
    get:
      summary: List properties
      description: Lists all properties.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemsproperties-get
      parameters:
      - in: query
        name: groupId
        description: Filter restricts the list of results to items linked to a specified
          property group
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified property information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
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