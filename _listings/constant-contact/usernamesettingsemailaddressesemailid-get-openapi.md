---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Email Address Details
  description: Get Email Address Details
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
  /{username}/lists/{list-id}:
    delete:
      summary: Delete Mailing List
      description: Delete Mailing List
      operationId: delete-mailing-list
      x-api-path-slug: usernamelistslistid-delete
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
    get:
      summary: Get Mailing List
      description: Get Mailing List
      operationId: get-mailing-list
      x-api-path-slug: usernamelistslistid-get
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
    put:
      summary: Update Mailing List
      description: Update Mailing List
      operationId: update-mailing-list
      x-api-path-slug: usernamelistslistid-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
  /{username}/settings/emailaddresses:
    get:
      summary: List Account Email Addresses
      description: List Account Email Addresses
      operationId: list-account-email-addresses
      x-api-path-slug: usernamesettingsemailaddresses-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Account
      - Email
      - Resses
  /{username}/settings/emailaddresses/{email-id}:
    get:
      summary: Get Email Address Details
      description: Get Email Address Details
      operationId: get-email-address-details
      x-api-path-slug: usernamesettingsemailaddressesemailid-get
      parameters:
      - in: path
        name: email-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ress
      - Details
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