---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Update User Mailbox Settings
  description: Update user mailbox settings Update one or more settings for the user's
    mailbox. This includes settings for automatic replies (notify people automatically
    upon receipt of their email), locale, or time zone.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{id}/subscribeByMail:
    post:
      summary: Group Subscribe By Mail
      description: 'group: subscribeByMail Calling this method will enable the current
        user to receive email notifications for this group, about new posts, events,
        and files in that group. Supported for only Office 365 groups.'
      operationId: Group:SubscribeByMail
      x-api-path-slug: groupsidsubscribebymail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - SubscribeMail
  /groups/{id}/unsubscribeByMail:
    post:
      summary: Group Unsubscribe By Mail
      description: 'group: unsubscribeByMail Calling this method will prevent the
        current user from receiving email notifications for this group about new posts,
        events, and files in that group. Supported for only Office 365 groups.'
      operationId: Group:UnsubscribeByMail
      x-api-path-slug: groupsidunsubscribebymail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - UnsubscribeMail
  /me/mailFolders/{id}/copy:
    post:
      summary: Mail Folder Copy
      description: 'mailFolder: copy Copy a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Copy
      x-api-path-slug: memailfoldersidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Copy
  /users/{id | userPrincipalName}/mailFolders/{id}/copy:
    post:
      summary: Mail Folder Copy
      description: 'mailFolder: copy Copy a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Copy
      x-api-path-slug: usersid--userprincipalnamemailfoldersidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Copy
  /me/mailFolders/{id}:
    delete:
      summary: Delete Mail Folder
      description: Delete mailFolder Delete mailFolder.
      operationId: DeleteMailFolder
      x-api-path-slug: memailfoldersid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
    get:
      summary: Get Mail Folder
      description: Get mailFolder Retrieve the properties and relationships of mailfolder
        object.
      operationId: GetMailFolder
      x-api-path-slug: memailfoldersid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
    patch:
      summary: Update Mailfolder
      description: Update mailfolder Update the properties of mailfolder object.
      operationId: UpdateMailfolder
      x-api-path-slug: memailfoldersid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mailfolder
  /users/{id | userPrincipalName}/mailFolders/{id}:
    delete:
      summary: Delete Mail Folder
      description: Delete mailFolder Delete mailFolder.
      operationId: DeleteMailFolder
      x-api-path-slug: usersid--userprincipalnamemailfoldersid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
    get:
      summary: Get Mail Folder
      description: Get mailFolder Retrieve the properties and relationships of mailfolder
        object.
      operationId: GetMailFolder
      x-api-path-slug: usersid--userprincipalnamemailfoldersid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
    patch:
      summary: Update Mailfolder
      description: Update mailfolder Update the properties of mailfolder object.
      operationId: UpdateMailfolder
      x-api-path-slug: usersid--userprincipalnamemailfoldersid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mailfolder
  /me/mailFolders/{id}/move:
    post:
      summary: Mail Folder Move
      description: 'mailFolder: move Move a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Move
      x-api-path-slug: memailfoldersidmove-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Move
  /users/{id | userPrincipalName}/mailFolders/{id}/move:
    post:
      summary: Mail Folder Move
      description: 'mailFolder: move Move a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Move
      x-api-path-slug: usersid--userprincipalnamemailfoldersidmove-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Move
  /me/mailFolders/{id}/childFolders:
    post:
      summary: Create Mail Folder
      description: Create MailFolder Use this API to create a new child mailfolder.
      operationId: CreateMailFolder
      x-api-path-slug: memailfoldersidchildfolders-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
  /users/{id | userPrincipalName}/mailFolders/{id}/childFolders:
    post:
      summary: Create Mail Folder
      description: Create MailFolder Use this API to create a new child mailfolder.
      operationId: CreateMailFolder
      x-api-path-slug: usersid--userprincipalnamemailfoldersidchildfolders-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
  /me/mailboxSettings:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: memailboxsettings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
    patch:
      summary: Update User Mailbox Settings
      description: Update user mailbox settings Update one or more settings for the
        user's mailbox. This includes settings for automatic replies (notify people
        automatically upon receipt of their email), locale, or time zone.
      operationId: UpdateUserMailboxSettings
      x-api-path-slug: memailboxsettings-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /users/{id|userPrincipalName}/mailboxSettings:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: usersiduserprincipalnamemailboxsettings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /me/mailboxSettings/automaticRepliesSetting:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: memailboxsettingsautomaticrepliessetting-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: usersiduserprincipalnamemailboxsettingsautomaticrepliessetting-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /me/mailboxSettings/language:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: memailboxsettingslanguage-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /users/{id|userPrincipalName}/mailboxSettings/language:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: usersiduserprincipalnamemailboxsettingslanguage-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /me/mailboxSettings/timeZone:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: memailboxsettingstimezone-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /users/{id|userPrincipalName}/mailboxSettings/timeZone:
    get:
      summary: Get User Mailbox Settings
      description: Get user mailbox settings Get the user's mailboxSettings. This
        includes settings for automatic replies (notify people automatically upon
        receipt of their email), locale (language and country/region), and time zone.
      operationId: GetUserMailboxSettings
      x-api-path-slug: usersiduserprincipalnamemailboxsettingstimezone-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer &lt;token&gt;
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Mailbox
      - Settings
  /users/{id | userPrincipalName}/mailFolders:
    get:
      summary: List Mail Folders
      description: List mailFolders Get the mail folder collection under the root
        folder of the signed-in user.
      operationId: ListMailFolders
      x-api-path-slug: usersid--userprincipalnamemailfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Mail
      - Folders
    post:
      summary: Create Mail Folder
      description: Create MailFolder Use this API to create a new mail folder.
      operationId: CreateMailFolder
      x-api-path-slug: usersid--userprincipalnamemailfolders-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
  /users/{id | userPrincipalName}/sendMail:
    post:
      summary: Send Mail
      description: Send mail Send the message specified in the request body. The message
        is saved in the Sent Items folder by default.
      operationId: SendMail
      x-api-path-slug: usersid--userprincipalnamesendmail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send
      - Mail
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