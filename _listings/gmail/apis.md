---
name: Gmail
x-slug: gmail
description: The Gmail API is a RESTful API that can be used to access Gmail mailboxes
  and send mail. For most web applications (including mobile apps), the Gmail API
  is the best choice for authorized access to a users Gmail data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Mail
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/apis.md
specificationVersion: "0.14"
apis:
- name: Gmail Get Drafts
  x-api-slug: gmail
  description: Lists the drafts in the user's mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts
  tags: Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddrafts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddrafts-get-openapi.md
- name: Gmail Update Draft
  x-api-slug: gmail
  description: Creates a new draft with the DRAFT label.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddrafts-post-openapi.md
- name: Gmail Send Draft
  x-api-slug: gmail
  description: Sends the specified, existing draft to the recipients in the To, Cc,
    and Bcc headers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts/send
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddraftssend-post-openapi.md
- name: Gmail Delete Draft
  x-api-slug: gmail
  description: Immediately and permanently deletes the specified draft. Does not simply
    trash it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddraftsid-delete-openapi.md
- name: Gmail Get Draft
  x-api-slug: gmail
  description: Gets the specified draft.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddraftsid-get-openapi.md
- name: Gmail Update Draft
  x-api-slug: gmail
  description: Replaces a draft's content.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/drafts/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useriddraftsid-put-openapi.md
- name: Gmail Get Message
  x-api-slug: gmail
  description: Lists the messages in the user's mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessages-get-openapi.md
- name: Gmail Create Message
  x-api-slug: gmail
  description: Directly inserts a message into only this user's mailbox similar to
    IMAP APPEND, bypassing most scanning and classification. Does not send a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessages-post-openapi.md
- name: Gmail Delete Messages
  x-api-slug: gmail
  description: Deletes many messages by message ID. Provides no guarantees that messages
    were not already deleted or even existed at all.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/batchDelete
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesbatchdelete-post-openapi.md
- name: Gmail Update Label
  x-api-slug: gmail
  description: Modifies the labels on the specified messages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/batchModify
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesbatchmodify-post-openapi.md
- name: Gmail Import Message
  x-api-slug: gmail
  description: Imports a message into only this user's mailbox, with standard email
    delivery scanning and classification similar to receiving via SMTP. Does not send
    a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/import
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesimport-post-openapi.md
- name: Gmail Send Message
  x-api-slug: gmail
  description: Sends the specified message to the recipients in the To, Cc, and Bcc
    headers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/send
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagessend-post-openapi.md
- name: Gmail Delete Message
  x-api-slug: gmail
  description: Immediately and permanently deletes the specified message. This operation
    cannot be undone. Prefer messages.trash instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesid-delete-openapi.md
- name: Gmail Get Message
  x-api-slug: gmail
  description: Gets the specified message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesid-get-openapi.md
- name: Gmail Modify message
  x-api-slug: gmail
  description: Modifies the labels on the specified message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{id}/modify
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesidmodify-post-openapi.md
- name: Gmail Trash Message
  x-api-slug: gmail
  description: Moves the specified message to the trash.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{id}/trash
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesidtrash-post-openapi.md
- name: Gmail UnTrash Message
  x-api-slug: gmail
  description: Removes the specified message from the trash.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{id}/untrash
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesiduntrash-post-openapi.md
- name: Gmail Get Attachments
  x-api-slug: gmail
  description: Gets the specified message attachment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/messages/{messageId}/attachments/{id}
  tags: Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridmessagesmessageidattachmentsid-get-openapi.md
- name: Gmail Get Threads
  x-api-slug: gmail
  description: Lists the threads in the user's mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreads-get-openapi.md
- name: Gmail Delete Threads
  x-api-slug: gmail
  description: Immediately and permanently deletes the specified thread. This operation
    cannot be undone. Prefer threads.trash instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads/{id}
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreadsid-delete-openapi.md
- name: Gmail Get Threads
  x-api-slug: gmail
  description: Gets the specified thread.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads/{id}
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreadsid-get-openapi.md
- name: Gmail Modify Thread labels
  x-api-slug: gmail
  description: Modifies the labels applied to the thread. This applies to all messages
    in the thread.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads/{id}/modify
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreadsidmodify-post-openapi.md
- name: Gmail Trash Thread
  x-api-slug: gmail
  description: Moves the specified thread to the trash.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads/{id}/trash
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreadsidtrash-post-openapi.md
- name: Gmail UnTrash Threat
  x-api-slug: gmail
  description: Removes the specified thread from the trash.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users//{userId}/threads/{id}/untrash
  tags: Email Thread
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/useridthreadsiduntrash-post-openapi.md
- name: Gmail
  x-api-slug: gmail
  description: The Gmail API is a RESTful API that can be used to access Gmail mailboxes
    and send mail. For most web applications (including mobile apps), the Gmail API
    is the best choice for authorized access to a users Gmail data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gmail-icon.png
  humanURL: https://www.google.com/gmail/
  baseURL: https://www.googleapis.com//gmail/v1/users
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/gmail/openapi.md
x-common:
- type: x-auth-scopes
  url: https://developers.google.com/gmail/api/auth/scopes
- type: x-authentication
  url: https://developers.google.com/gmail/api/auth/about-auth
- type: x-developer
  url: https://developers.google.com/gmail/api/
- type: x-documentation
  url: https://developers.google.com/gmail/api/v1/reference/
- type: x-twitter
  url: https://twitter.com/gmail
- type: x-website
  url: https://www.google.com/gmail/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---