---
name: Apigee
x-slug: apigee
description: Apigee Edge is a platform for developing and managing API proxies. Think
  of a proxy as an abstraction layer that fronts for your backend service APIs and
  provides value-added features like security, rate limiting, quotas, analytics, and
  more. The primary consumers of Edge API proxies are app developers who want to use
  your backend services.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Mail
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/apis.md
specificationVersion: "0.14"
apis:
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps
  x-api-slug: apigee-edge
  description: Provides an expanded view of a developer's collection of apps .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps
  tags: Organizations,Developers,Developer,Email,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps
  x-api-slug: apigee-edge
  description: Creates an app associated with a developer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps
  tags: Organizations,Developers,Developer,Email,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-post-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Gets a count of all API resources in the API products accessible by
    a developer app .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Updates the app to get a new set of consumer credentials.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-put-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Revokes a Developer App, disabling access to all API Products .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name
  x-api-slug: apigee-edge
  description: Delete a Developer's App.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key
  x-api-slug: apigee-edge
  description: Returns details for a consumer key for a developer app .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key
  x-api-slug: apigee-edge
  description: Revokes a developer app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name Keys Consumer Key
  x-api-slug: apigee-edge
  description: Deletes a consumer key that belongs to an app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Revokes the association of an API Product with a Developer App's consumer
    key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name Keys Consumer Key Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Removes an API product from a developer app key profile, and thereby
    renders the developer app unable to access the URIs defined in the API product
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Oauth1accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 1.0 access tokens for a developer's app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth1accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Oauth1accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Oauth2accesstokens
  x-api-slug: apigee-edge
  description: Get count of    OAuth 2.0 access tokens for a developer's app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth2accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Oauth2accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Oauth1accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 1.0 access tokens for a developer's app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth1accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,Oauth1accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Oauth2accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 2.0 access tokens for a developer's app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth2accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,Oauth2accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Developers Developer
    Email
  x-api-slug: apigee-edge
  description: Removes the association of a Developer with a Company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/developers/{developer_email}
  tags: Organizations,Companies,Companies,Developers,Developer,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopersdeveloper-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopersdeveloper-email-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Appfamilies
  x-api-slug: apigee-edge
  description: An expanded list of all app families in an organization, listing Apps
    in the collection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies
  tags: Organizations,Developers,Developer,Email,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Appfamilies
  x-api-slug: apigee-edge
  description: Creates an app family for developers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies
  tags: Organizations,Developers,Developer,Email,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-post-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Gets a list of apps in an appfamily.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Updates an existing app family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Deletes an App Family and all Apps it contains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-delete-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Appfamilies
    Appfamily Name Apps App Name
  x-api-slug: apigee-edge
  description: Removes an App from an App Family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-nameappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-nameappsapp-name-delete-openapi.md
- name: Apigee Edge Get Users User Email
  x-api-slug: apigee-edge
  description: Gets a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-get-openapi.md
- name: Apigee Edge Post Users User Email
  x-api-slug: apigee-edge
  description: Updates a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-post-openapi.md
- name: Apigee Edge Delete Users User Email
  x-api-slug: apigee-edge
  description: Deletes a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}
  tags: Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-email-delete-openapi.md
- name: Apigee Edge Get Users User Email Userroles
  x-api-slug: apigee-edge
  description: Gets roles for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles
  tags: Users,User,Email,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserroles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserroles-get-openapi.md
- name: Apigee Edge Post Users User Email Userroles
  x-api-slug: apigee-edge
  description: Associates a user with a organizational user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles
  tags: Users,User,Email,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserroles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserroles-post-openapi.md
- name: Apigee Edge Get Userroles Role Name Users User Email
  x-api-slug: apigee-edge
  description: Checks user in a given system role
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users/{user_email}
  tags: Userroles,Role,Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/userrolesrole-nameusersuser-email-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/userrolesrole-nameusersuser-email-get-openapi.md
- name: Apigee Edge Delete Userroles Role Name Users User Email
  x-api-slug: apigee-edge
  description: Deletes user for a role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///userroles/{role_name}/users/{user_email}
  tags: Userroles,Role,Users,User,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/userrolesrole-nameusersuser-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/userrolesrole-nameusersuser-email-delete-openapi.md
- name: Apigee Edge Delete Users User Email Userroles Role Name
  x-api-slug: apigee-edge
  description: Deletes organizational role for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}/userroles/{role_name}
  tags: Users,User,Email,Userroles,Role
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserrolesrole-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailuserrolesrole-name-delete-openapi.md
- name: Apigee Edge Get Users User Email Permissions Get
  x-api-slug: apigee-edge
  description: Checks user has particular permission for a resource at global level
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///users/{user_email}permissions/get
  tags: Users,User,Emailpermissions,Get
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailpermissionsget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/usersuser-emailpermissionsget-get-openapi.md
- name: Apigee Edge
  x-api-slug: apigee-edge
  description: Apigee Edge is a platform for developing and managing API proxies.
    Think of a proxy as an abstraction layer that fronts for your backend service
    APIs and provides value-added features like security, rate limiting, quotas, analytics,
    and more. The primary consumers of Edge API proxies are app developers who want
    to use your backend services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1/
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/apigee/openapi.md
x-common:
- type: x-website
  url: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---