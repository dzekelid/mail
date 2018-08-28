---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Add Mail Send
  description: "This endpoint allows you to send email over SendGrid???s v3 Web API,
    the most recent version of our API. If you are looking for documentation about
    the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
    Top level parameters are referred to as \"global\".\n* Individual fields within
    the personalizations array will override any other global, or ???message level???,
    parameters that are defined outside of personalizations.\n \n**SendGrid provides
    libraries to help you quickly and easily integrate with the v3 Web API in 7 different
    languages: [C#](https://github.com/sendgrid/sendgrid-csharp), [Go](https://github.com/sendgrid/sendgrid-go),
    [Java](https://github.com/sendgrid/sendgrid-java), [Node JS](https://github.com/sendgrid/sendgrid-nodejs),
    [PHP](https://github.com/sendgrid/sendgrid-php), [Python](https://github.com/sendgrid/sendgrid-python),
    and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor more detailed
    information about how to use the v3 Mail Send endpoint, please visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
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
  /mail/batch/{batch_id}:
    get:
      summary: Get Mail Batch Batch
      description: "**This endpoint allows you to validate a batch ID.**\n\nIf you
        set the SMTPAPI header `batch_id`, it allows you to then associate multiple
        scheduled mail/send requests together with the same ID. Then at anytime up
        to 10 minutes before the schedule date, you can cancel all of the mail/send
        requests that have this batch ID by calling the Cancel Scheduled Send endpoint.
        \n\nMore Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
      operationId: mail.batch.batch_id.get
      x-api-path-slug: mailbatchbatch-id-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Batch
      - Batch
  /mail/send:
    post:
      summary: Add Mail Send
      description: "This endpoint allows you to send email over SendGrid???s v3 Web
        API, the most recent version of our API. If you are looking for documentation
        about the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
        Top level parameters are referred to as \"global\".\n* Individual fields within
        the personalizations array will override any other global, or ???message level???,
        parameters that are defined outside of personalizations.\n \n**SendGrid provides
        libraries to help you quickly and easily integrate with the v3 Web API in
        7 different languages: [C#](https://github.com/sendgrid/sendgrid-csharp),
        [Go](https://github.com/sendgrid/sendgrid-go), [Java](https://github.com/sendgrid/sendgrid-java),
        [Node JS](https://github.com/sendgrid/sendgrid-nodejs), [PHP](https://github.com/sendgrid/sendgrid-php),
        [Python](https://github.com/sendgrid/sendgrid-python), and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor
        more detailed information about how to use the v3 Mail Send endpoint, please
        visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
      operationId: mail.send.post
      x-api-path-slug: mailsend-post
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
      - Send
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