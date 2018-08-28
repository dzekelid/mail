---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Add Mail Batch
  description: "**This endpoint allows you to generate a new batch ID. This batch
    ID can be associated with scheduled sends via the mail/send endpoint.**\n\nIf
    you set the SMTPAPI header `batch_id`, it allows you to then associate multiple
    scheduled mail/send requests together with the same ID. Then at anytime up to
    10 minutes before the schedule date, you can cancel all of the mail/send requests
    that have this batch ID by calling the Cancel Scheduled Send endpoint. \n\nMore
    Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mail/batch:
    post:
      summary: Add Mail Batch
      description: "**This endpoint allows you to generate a new batch ID. This batch
        ID can be associated with scheduled sends via the mail/send endpoint.**\n\nIf
        you set the SMTPAPI header `batch_id`, it allows you to then associate multiple
        scheduled mail/send requests together with the same ID. Then at anytime up
        to 10 minutes before the schedule date, you can cancel all of the mail/send
        requests that have this batch ID by calling the Cancel Scheduled Send endpoint.
        \n\nMore Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
      operationId: mail.batch.post
      x-api-path-slug: mailbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Batch
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