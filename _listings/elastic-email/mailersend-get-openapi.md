---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Send Email
  description: api.elasticemail.com
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
  mailer/send/:
    get:
      summary: Send Email
      description: api.elasticemail.com
      operationId: getMailerSend
      x-api-path-slug: mailersend-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: body_html
        description: html email body
      - in: query
        name: body_text
        description: text email body
      - in: query
        name: channel
        description: an id field (max 60 chars) that can be used for reporting
      - in: query
        name: charset
        description: 'text value of encoding for example: iso-8859-1, windows-1251,
          utf-8, us-ascii, windows-1250'
      - in: query
        name: encodingtype
        description: 0 for None, 1 for Raw7Bit, 2 for Raw8Bit, 3 for QuotedPrintable,
          4 for Base64 (Default), 5 for Uue  note that you can also provide the text
          version such as Raw7Bit for value 1
      - in: query
        name: from
        description: from email address
      - in: query
        name: from_name
        description: display name for from email address
      - in: query
        name: lists
        description: the name of a contact list you would like to send to
      - in: query
        name: merge_firstname
        description: if sending to a template you can send merge_ fields to merge
          data with the template
      - in: query
        name: merge_lastname
        description: if sending to a template you can send merge_ fields to merge
          data with the template
      - in: query
        name: reply_to
        description: email address to reply to
      - in: query
        name: reply_to_name
        description: display name of the reply to address
      - in: query
        name: sender
        description: email address of the sender
      - in: query
        name: sender_name
        description: display name sender
      - in: query
        name: subject
        description: email subject
      - in: query
        name: template
        description: the name of an email template you have created in your account
      - in: query
        name: time_offset_minutes
        description: number of minutes in the future this email should be sent
      - in: query
        name: total
        description: semi colon separated list of email recipients (each email is
          treated separately, like a BCC)
      - in: query
        name: username
        description: your account email address
      responses:
        200:
          description: OK
      tags:
      - Mailer
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