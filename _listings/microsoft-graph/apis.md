---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Mail
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph Group Subscribe By Mail
  x-api-slug: microsoft-graph
  description: 'group: subscribeByMail Calling this method will enable the current
    user to receive email notifications for this group, about new posts, events, and
    files in that group. Supported for only Office 365 groups.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/subscribeByMail
  tags: Group, SubscribeMail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/groupsidsubscribebymail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/groupsidsubscribebymail-post-openapi.md
- name: Microsoft Graph Group Unsubscribe By Mail
  x-api-slug: microsoft-graph
  description: 'group: unsubscribeByMail Calling this method will prevent the current
    user from receiving email notifications for this group about new posts, events,
    and files in that group. Supported for only Office 365 groups.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/unsubscribeByMail
  tags: Group, UnsubscribeMail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/groupsidunsubscribebymail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/groupsidunsubscribebymail-post-openapi.md
- name: Microsoft Graph Mail Folder Copy
  x-api-slug: microsoft-graph
  description: 'mailFolder: copy Copy a mailfolder and its contents to another mailfolder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}/copy
  tags: Mail, Folder, Copy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersidcopy-post-openapi.md
- name: Microsoft Graph Mail Folder Copy
  x-api-slug: microsoft-graph
  description: 'mailFolder: copy Copy a mailfolder and its contents to another mailfolder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}/copy
  tags: Mail, Folder, Copy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidcopy-post-openapi.md
- name: Microsoft Graph Delete Mail Folder
  x-api-slug: microsoft-graph
  description: Delete mailFolder Delete mailFolder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-delete-openapi.md
- name: Microsoft Graph Delete Mail Folder
  x-api-slug: microsoft-graph
  description: Delete mailFolder Delete mailFolder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-delete-openapi.md
- name: Microsoft Graph Get Mail Folder
  x-api-slug: microsoft-graph
  description: Get mailFolder Retrieve the properties and relationships of mailfolder
    object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-get-openapi.md
- name: Microsoft Graph Get Mail Folder
  x-api-slug: microsoft-graph
  description: Get mailFolder Retrieve the properties and relationships of mailfolder
    object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-get-openapi.md
- name: Microsoft Graph Mail Folder Move
  x-api-slug: microsoft-graph
  description: 'mailFolder: move Move a mailfolder and its contents to another mailfolder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}/move
  tags: Mail, Folder, Move
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersidmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersidmove-post-openapi.md
- name: Microsoft Graph Mail Folder Move
  x-api-slug: microsoft-graph
  description: 'mailFolder: move Move a mailfolder and its contents to another mailfolder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}/move
  tags: Mail, Folder, Move
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidmove-post-openapi.md
- name: Microsoft Graph Create Mail Folder
  x-api-slug: microsoft-graph
  description: Create MailFolder Use this API to create a new child mailfolder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}/childFolders
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersidchildfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersidchildfolders-post-openapi.md
- name: Microsoft Graph Create Mail Folder
  x-api-slug: microsoft-graph
  description: Create MailFolder Use this API to create a new child mailfolder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}/childFolders
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidchildfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersidchildfolders-post-openapi.md
- name: Microsoft Graph Update Mailfolder
  x-api-slug: microsoft-graph
  description: Update mailfolder Update the properties of mailfolder object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailFolders/{id}
  tags: Mailfolder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailfoldersid-patch-openapi.md
- name: Microsoft Graph Update Mailfolder
  x-api-slug: microsoft-graph
  description: Update mailfolder Update the properties of mailfolder object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders/{id}
  tags: Mailfolder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfoldersid-patch-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailboxSettings
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettings-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id|userPrincipalName}/mailboxSettings
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettings-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailboxSettings/automaticRepliesSetting
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingsautomaticrepliessetting-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingsautomaticrepliessetting-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingsautomaticrepliessetting-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingsautomaticrepliessetting-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailboxSettings/language
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingslanguage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingslanguage-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id|userPrincipalName}/mailboxSettings/language
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingslanguage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingslanguage-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailboxSettings/timeZone
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingstimezone-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettingstimezone-get-openapi.md
- name: Microsoft Graph Get User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Get user mailbox settings Get the user's mailboxSettings. This includes
    settings for automatic replies (notify people automatically upon receipt of their
    email), locale (language and country/region), and time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id|userPrincipalName}/mailboxSettings/timeZone
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingstimezone-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettingstimezone-get-openapi.md
- name: Microsoft Graph List Mail Folders
  x-api-slug: microsoft-graph
  description: List mailFolders Get the mail folder collection under the root folder
    of the signed-in user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders
  tags: List, Mail, Folders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfolders-get-openapi.md
- name: Microsoft Graph Create Mail Folder
  x-api-slug: microsoft-graph
  description: Create MailFolder Use this API to create a new mail folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/mailFolders
  tags: Mail, Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamemailfolders-post-openapi.md
- name: Microsoft Graph Send Mail
  x-api-slug: microsoft-graph
  description: Send mail Send the message specified in the request body. The message
    is saved in the Sent Items folder by default.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/sendMail
  tags: Send, Mail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamesendmail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersid--userprincipalnamesendmail-post-openapi.md
- name: Microsoft Graph Update User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Update user mailbox settings Update one or more settings for the user's
    mailbox. This includes settings for automatic replies (notify people automatically
    upon receipt of their email), locale, or time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/mailboxSettings
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettings-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/memailboxsettings-patch-openapi.md
- name: Microsoft Graph Update User Mailbox Settings
  x-api-slug: microsoft-graph
  description: Update user mailbox settings Update one or more settings for the user's
    mailbox. This includes settings for automatic replies (notify people automatically
    upon receipt of their email), locale, or time zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id|userPrincipalName}/mailboxSettings
  tags: User, Mailbox, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettings-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/usersiduserprincipalnamemailboxsettings-patch-openapi.md
- name: Microsoft Graph
  x-api-slug: microsoft-graph
  description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
    cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
    Graph simplifies queries that would otherwise be more complex. You can use Microsoft
    Graph to: Access data from multiple Microsoft cloud services, including Azure
    Active Directory, Exchange Online as part of Office 365, SharePoint, OneDrive,
    OneNote, and Planner. Navigate between entities and relationships. Access intelligence
    and insights from the Microsoft cloud (for commercial users).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/microsoft-graph/openapi.md
x-common:
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---