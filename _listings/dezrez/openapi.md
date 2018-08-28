swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branch/createscheduledmailmerge:
    post:
      summary: Save a scheduled mail merge.
      description: Save a scheduled mail merge..
      operationId: Branch_CreateScheduledMailMergeByscheduledMailMerge
      x-api-path-slug: apibranchcreatescheduledmailmerge-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: scheduledMailMerge
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - Scheduled
      - Mail
      - Merge
  /api/branch/scheduledmailmerges:
    get:
      summary: Get all scheduled mail merges for the logged in branch.
      description: Get all scheduled mail merges for the logged in branch..
      operationId: Branch_GetScheduledMailMergesBypageSizeBypageNumber
      x-api-path-slug: apibranchscheduledmailmerges-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Scheduled
      - Mail
      - Mergesthe
      - Logged
      - In
      - Branch
  /api/sync/mailsyncanddraftenabled:
    get:
      summary: "check if they user has setup their credentials for smap services\r\nthis
        could be used to enabled/disable the mail sync button"
      description: "Check if they user has setup their credentials for smap services\r\nthis
        could be used to enabled/disable the mail sync button."
      operationId: Sync_MailSyncAndDraftEnabled
      x-api-path-slug: apisyncmailsyncanddraftenabled-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - They
      - User
      - Has
      - Setup
      - Their
      - Credentialssmap
      - "Services\r\nThis"
      - Could
      - Be
      - Used
      - To
      - Enabled
      - Disable
      - Mail
      - Sync
      - Button