---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Add Mailing List
  description: Add Mailing List
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/lists:
    get:
      summary: Get All Mailing Lists
      description: Get All Mailing Lists
      operationId: get-all-mailing-lists
      x-api-path-slug: usernamelists-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - Lists
    post:
      summary: Add Mailing List
      description: Add Mailing List
      operationId: add-mailing-list
      x-api-path-slug: usernamelists-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
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