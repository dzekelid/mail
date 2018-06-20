---
name: AWS Simple Email Service
x-slug: aws-simple-email-service
description: Amazon Simple Email Service (Amazon SES) is a cost-effective email service
  built on the reliable and scalable infrastructure that Amazon.com developed to serve
  its own customer base. With Amazon SES, you can send and receive email with no required
  minimum commitments &ndash; you pay as you go, and you only pay for what you use.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Mail
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Email Service API Delete Verified Email Address
  x-api-slug: aws-simple-email-service-api
  description: Deletes the specified email address from the list of verified addresses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=DeleteVerifiedEmailAddress
  tags: Verified Email Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actiondeleteverifiedemailaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actiondeleteverifiedemailaddress-get-openapi.md
- name: AWS Simple Email Service API List Verified Email Addresses
  x-api-slug: aws-simple-email-service-api
  description: Returns a list containing all of the email addresses that have been
    verified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=ListVerifiedEmailAddresses
  tags: 'Verified Email Addresses '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionlistverifiedemailaddresses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionlistverifiedemailaddresses-get-openapi.md
- name: AWS Simple Email Service API Send Email
  x-api-slug: aws-simple-email-service-api
  description: Composes an email message based on input data, and then immediately
    queues the message for sending.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=SendEmail
  tags: Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionsendemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionsendemail-get-openapi.md
- name: AWS Simple Email Service API Send Raw Email
  x-api-slug: aws-simple-email-service-api
  description: Sends an email message, with header and content specified by the client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=SendRawEmail
  tags: Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionsendrawemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionsendrawemail-get-openapi.md
- name: AWS Simple Email Service API Verify Email Address
  x-api-slug: aws-simple-email-service-api
  description: Verifies an email address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: ://///?Action=VerifyEmailAddress
  tags: Email Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionverifyemailaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/actionverifyemailaddress-get-openapi.md
- name: AWS Simple Email Service API
  x-api-slug: aws-simple-email-service-api
  description: Amazon Simple Email Service (Amazon SES) is a cost-effective email
    service built on the reliable and scalable infrastructure that Amazon.com developed
    to serve its own customer base. With Amazon SES, you can send and receive email
    with no required minimum commitments &ndash; you pay as you go, and you only pay
    for what you use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSES.png
  humanURL: https://aws.amazon.com/ses/
  baseURL: :///
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/aws-simple-email-service/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SES
- type: x-documentation
  url: http://docs.aws.amazon.com/ses/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/ses/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=90
- type: x-getting-started
  url: https://aws.amazon.com/ses/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/ses/pricing/
- type: x-sdk
  url: http://aws.amazon.com/tools
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-tools
  url: http://aws.amazon.com/developertools/Amazon-SES
- type: x-website
  url: https://aws.amazon.com/ses/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---