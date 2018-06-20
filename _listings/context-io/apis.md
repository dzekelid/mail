---
name: Context.IO
x-slug: context-io
description: Create simple email webhooks and code against a free, RESTful, IMAP API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
x-kinRank: "9"
x-alexaRank: "569975"
tags: Mail
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/apis.md
specificationVersion: "0.14"
apis:
- name: Context.IO Get Accounts Contacts Email
  x-api-slug: context-io
  description: Gets information about a given contact.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}
  tags: Accounts,Contacts,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemail-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Files
  x-api-slug: context-io
  description: Lists files exchanged with a contact. Returns the latest attachments
    exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
    any file attached to an email received from Mr. X, sent to Mr. X or sent by anyone
    to both Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/files
  tags: Accounts,Contacts,Email,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailfiles-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Messages
  x-api-slug: context-io
  description: Lists messages where a contact is present. Returns the latest email
    messages exchanged with one or more email addresses. By "exchanged with Mr. X"
    we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both
    Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/messages
  tags: Accounts,Contacts,Email,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailmessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailmessages-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Threads
  x-api-slug: context-io
  description: Lists threads where a contact is present. Returns the latest email
    threads exchanged with one or more email addresses. By "exchanged with Mr. X"
    we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both
    Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/threads
  tags: Accounts,Contacts,Email,Threads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailthreads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidcontactsemailthreads-get-openapi.md
- name: Context.IO Get Accounts Email Addresses
  x-api-slug: context-io
  description: Lists email addresses used by an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses
  tags: Accounts,Email,Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addresses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addresses-get-openapi.md
- name: Context.IO Post Accounts Email Addresses
  x-api-slug: context-io
  description: Adds a new email address as an alias for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses
  tags: Accounts,Email,Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addresses-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addresses-post-openapi.md
- name: Context.IO Post Accounts Email Addresses Email
  x-api-slug: context-io
  description: Makes this email address the primary one for the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses/{email}
  tags: Accounts,Email,Addresses,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addressesemail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addressesemail-post-openapi.md
- name: Context.IO Delete Accounts Email Addresses Email
  x-api-slug: context-io
  description: Removes an email address form the aliases of an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses/{email}
  tags: Accounts,Email,Addresses,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addressesemail-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/accountsidemail-addressesemail-delete-openapi.md
- name: Context.IO
  x-api-slug: context-io
  description: Context.IO is the missing email API that makes it easy and fastto integrate
    your users email data in your application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/context-io/openapi.md
x-common:
- type: x-base
  url: https://api.context.io/
- type: x-blog
  url: http://blog.context.io/
- type: x-blog-rss
  url: http://blog.context.io/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/product/context-io
- type: x-crunchbase
  url: https://crunchbase.com/organization/context-io
- type: x-documentation
  url: http://context.io/docs/2.0
- type: x-email
  url: hello@context.io
- type: x-email
  url: support@context.io
- type: x-email
  url: business@context.io
- type: x-faq
  url: http://context.io/privacy-faq
- type: x-github
  url: https://github.com/contextio
- type: x-ios-library
  url: https://github.com/contextio/contextio-ios
- type: x-node-js-library
  url: https://github.com/contextio/ContextIO-node
- type: x-php-library
  url: https://github.com/contextio/PHP-ContextIO
- type: x-pricing
  url: http://context.io/pricing
- type: x-privacy
  url: http://www.returnpath.com/privacy-policy-data
- type: x-python-library
  url: https://github.com/contextio/Python-ContextIO
- type: x-ruby-library
  url: https://github.com/contextio/contextio-ruby
- type: x-selfservice-registration
  url: http://context.io/#signup
- type: x-terms-of-service
  url: http://context.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/contextio
- type: x-website
  url: http://context.io/
- type: x-website
  url: http://context.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---