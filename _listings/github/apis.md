---
name: GitHub
x-slug: github
description: GitHub brings together the worlds largest community of developers to
  discover, share, and build better software. From open source projects to private
  team repositories, were your all-in-one platform for collaborative development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "64"
tags: Mail
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Get Legacy User Email Email
  x-api-slug: github
  description: This API call is added for compatibility reasons only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////legacy/user/email/{email}
  tags: Legacy, User, Email, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/legacyuseremailemail-get-openapi.md
- name: Github Delete User Emails
  x-api-slug: github
  description: |-
    Delete email address(es).
    You can include a single email address or an array of addresses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////user/emails
  tags: User, Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/useremails-delete-openapi.md
- name: Github Get User Emails
  x-api-slug: github
  description: |-
    List email addresses for a user.
    In the final version of the API, this method will return an array of hashes
    with extended information for each email address indicating if the address
    has been verified and if it's primary email address for GitHub.
    Until API v3 is finalized, use the application/vnd.github.v3 media type to
    get other response format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////user/emails
  tags: User, Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/useremails-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/useremails-get-openapi.md
- name: Github Add User Emails
  x-api-slug: github
  description: |-
    Add email address(es).
    You can post a single email address or an array of addresses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////user/emails
  tags: User, Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/useremails-post-openapi.md
- name: Github
  x-api-slug: github
  description: GitHub brings together the worlds largest community of developers to
    discover, share, and build better software. From open source projects to private
    team repositories, were your all-in-one platform for collaborative development.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---