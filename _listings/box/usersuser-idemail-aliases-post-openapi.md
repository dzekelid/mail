---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Add Email Alias
  description: "Adds a new email alias to the given user\u2019s account."
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/email_aliases:
    get:
      summary: Get Email Aliases
      description: Retrieves all email aliases for this user. The collection of email
        aliases does not include the primary login for the user; use GET /users/USER_ID
        to retrieve the login email address.
      operationId: getEmailAliases
      x-api-path-slug: usersuser-idemail-aliases-get
      parameters:
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
    post:
      summary: Add Email Alias
      description: "Adds a new email alias to the given user\u2019s account."
      operationId: addEmailAlias
      x-api-path-slug: usersuser-idemail-aliases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Email
      - Aliases
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