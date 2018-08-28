---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Delete Verified Email Address
  version: 1.0.0
  description: Deletes the specified email address from the list of verified addresses.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteVerifiedEmailAddress:
    get:
      summary: Delete Verified Email Address
      description: Deletes the specified email address from the list of verified addresses.
      operationId: deleteVerifiedEmailAddress
      x-api-path-slug: actiondeleteverifiedemailaddress-get
      parameters:
      - in: query
        name: EmailAddress
        description: An email address to be removed from the list of verified addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verified Email Addresses
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