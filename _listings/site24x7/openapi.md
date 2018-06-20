---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 1
info:
  title: Email Template API
  description: the-email-template-api-
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email_templates/{template_id}:
    get:
      summary: Retrieve Email Template
      description: Retrieve configuration of a Email Template.
      operationId: retrieve-email-template
      x-api-path-slug: email-templatestemplate-id-get
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Email Templates
    delete:
      summary: Delete Email Template
      description: Delete an existing Email Template.
      operationId: delete-email-template
      x-api-path-slug: email-templatestemplate-id-delete
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Email Templates
---