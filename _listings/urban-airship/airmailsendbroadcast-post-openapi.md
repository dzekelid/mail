---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post Airmail Send Broadcast
  description: Sends a message to all users (broadcast). Only message is required.
    The message will be sent out to every registered user. Badge numbers will be handled
    automatically as long as the push key is present.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /airmail/send:
    post:
      summary: Post Airmail Send
      description: "Sends a message. All fields except message are optional, but at
        least one of tags, users or aliases must be specified. Much like the push
        API, we have a batch API call that can make sending multiple messages easier.
        It\u2019s located at /api/airmail/send/batch/ and accepts a list of messages
        in the same format as the standard push call."
      operationId: airmail.send.post
      x-api-path-slug: airmailsend-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Airmail
      - Send
  /airmail/send/broadcast:
    post:
      summary: Post Airmail Send Broadcast
      description: Sends a message to all users (broadcast). Only message is required.
        The message will be sent out to every registered user. Badge numbers will
        be handled automatically as long as the push key is present.
      operationId: airmail.send.broadcast.post
      x-api-path-slug: airmailsendbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Airmail
      - Send
      - Broadcast
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