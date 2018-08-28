---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Unsubscribed
  description: This api will return you the list of email addresses which are currently
    in your block list.
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  mailer/account-details:
    get:
      summary: Account Details
      description: The Account Details command is used to determine how much credit
        you have left.
      operationId: getMailerAccountDetails
      x-api-path-slug: maileraccountdetails-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Account
      - Details
  mailer/channel/delete:
    get:
      summary: Deleting Channel
      description: Deleting Channel
      operationId: getMailerChannelDelete
      x-api-path-slug: mailerchanneldelete-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: format
        description: csv or xml
      - in: query
        name: name
        description: channel name to delete
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Channel
      - Delete
  mailer/channel/list:
    get:
      summary: Listing of Active Channels
      description: Listing of Active Channels
      operationId: getMailerChannelList
      x-api-path-slug: mailerchannellist-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: format
        description: csv or xml
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Channel
      - List
  mailer/list/bounced:
    get:
      summary: Bounced
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListBounced
      x-api-path-slug: mailerlistbounced-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - List
      - Bounced
  mailer/list/complaint:
    get:
      summary: Complaint
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListComplaint
      x-api-path-slug: mailerlistcomplaint-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - List
      - Complaint
  mailer/lists/unsubscribed:
    get:
      summary: Unsubscribed
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListsUnsubscribed
      x-api-path-slug: mailerlistsunsubscribed-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Lists
      - Unsubscribed
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