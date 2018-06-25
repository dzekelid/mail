---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Mail
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Get Access Settings Activity
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all of the IP addresses that recently attempted to access your account either through the User Interface or the API.**

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/activity
  tags: Email,Access, Settings, Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingsactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingsactivity-get-openapi.md
- name: SendGrid Delete Access Settings Whitelist
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove one or more IPs from your IP whitelist.**

    You can remove one IP at a time, or you can remove multiple IP addresses.

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/whitelist
  tags: Email,Access, Settings, Whitelist
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelist-delete-openapi.md
- name: SendGrid Get Access Settings Whitelist
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of IP addresses that are currently whitelisted.**

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/whitelist
  tags: Email,Access, Settings, Whitelist
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelist-get-openapi.md
- name: SendGrid Add Access Settings Whitelist
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add one or more IP addresses to your IP whitelist.**

    When adding an IP to your whitelist, include the IP address in an array. You can whitelist one IP at a time, or you can whitelist multiple IPs at once.

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/whitelist
  tags: Email,Access, Settings, Whitelist
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelist-post-openapi.md
- name: SendGrid Delete Access Settings Whitelist Rule
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove a specific IP address from your IP whitelist.**

    When removing a specific IP address from your whitelist, you must include the ID in your call.

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/whitelist/{rule_id}
  tags: Email,Access, Settings, Whitelist, Rule
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelistrule-id-delete-openapi.md
- name: SendGrid Get Access Settings Whitelist Rule
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retreive a specific IP address that has been whitelisted.**

    You must include the ID for the specific IP address you want to retrieve in your call.

    IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

    For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//access_settings/whitelist/{rule_id}
  tags: Email,Access, Settings, Whitelist, Rule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelistrule-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/access-settingswhitelistrule-id-get-openapi.md
- name: SendGrid Get Alerts
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retieve all of your alerts.**\n\nAlerts
    allow you to specify an email address to receive notifications regarding your
    email usage or statistics. \n* Usage alerts allow you to set the threshold at
    which an alert will be sent.\n* Stats notifications allow you to set how frequently
    you would like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//alerts
  tags: Email,Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alerts-get-openapi.md
- name: SendGrid Add Alerts
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new alert.**

    Alerts allow you to specify an email address to receive notifications regarding your email usage or statistics. There are two types of alerts that can be created with this endpoint:

    * `usage_limit` allows you to set the threshold at which an alert will be sent.
    * `stats_notification` allows you to set how frequently you would like to receive email statistics reports. For example, "daily", "weekly", or "monthly".

    For more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//alerts
  tags: Email,Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alerts-post-openapi.md
- name: SendGrid Delete Alerts Alert
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete an alert.**\n\nAlerts allow you
    to specify an email address to receive notifications regarding your email usage
    or statistics. \n* Usage alerts allow you to set the threshold at which an alert
    will be sent.\n* Stats notifications allow you to set how frequently you would
    like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//alerts/{alert_id}
  tags: Email,Alerts, Alert
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alertsalert-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alertsalert-id-delete-openapi.md
- name: SendGrid Get Alerts Alert
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific alert.**\n\nAlerts
    allow you to specify an email address to receive notifications regarding your
    email usage or statistics. \n* Usage alerts allow you to set the threshold at
    which an alert will be sent.\n* Stats notifications allow you to set how frequently
    you would like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//alerts/{alert_id}
  tags: Email,Alerts, Alert
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alertsalert-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alertsalert-id-get-openapi.md
- name: SendGrid Patch Alerts Alert
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update an alert.**\n\nAlerts allow you
    to specify an email address to receive notifications regarding your email usage
    or statistics. \n* Usage alerts allow you to set the threshold at which an alert
    will be sent.\n* Stats notifications allow you to set how frequently you would
    like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//alerts/{alert_id}
  tags: Email,Alerts, Alert
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/alertsalert-id-patch-openapi.md
- name: SendGrid Get Api Keys
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys
  tags: Email,Api, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keys-get-openapi.md
- name: SendGrid Add Api Keys
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new random API Key for the user.**

    A JSON request body containing a "name" property is required. If number of maximum keys is reached, HTTP 403 will be returned.

    There is a limit of 100 API Keys on your account.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    See the [API Key Permissions List](https://sendgrid.com/docs/API_Reference/Web_API_v3/API_Keys/api_key_permissions_list.html) for a list of all available scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys
  tags: Email,Api, Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keys-post-openapi.md
- name: SendGrid Delete Api Keys Api Key
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to revoke an existing API Key**

    Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    ## URI Parameters

    | URI Parameter   | Type  | Required?  | Description  |
    |---|---|---|---|
    |api_key_id |string | required | The ID of the API Key you are deleting.|
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys/{api_key_id}
  tags: Email,Api, Keys, Api, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-delete-openapi.md
- name: SendGrid Get Api Keys Api Key
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single api key.**

    If the API Key ID does not exist an HTTP 404 will be returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys/{api_key_id}
  tags: Email,Api, Keys, Api, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-get-openapi.md
- name: SendGrid Patch Api Keys Api Key
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the name of an existing API Key.**

    A JSON request body with a "name" property is required.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    ## URI Parameters

    | URI Parameter   | Type  | Required?  | Description  |
    |---|---|---|---|
    |api_key_id |string | required | The ID of the API Key you are updating.|
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys/{api_key_id}
  tags: Email,Api, Keys, Api, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-patch-openapi.md
- name: SendGrid Put Api Keys Api Key
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the name and scopes of a given API key.**

    A JSON request body with a "name" property is required.
    Most provide the list of all the scopes an api key should have.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//api_keys/{api_key_id}
  tags: Email,Api, Keys, Api, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/api-keysapi-key-id-put-openapi.md
- name: SendGrid Get Asm Groups
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve information about multiple suppression groups.**

    This endpoint will return information for each group ID that you include in your request. To add a group ID to your request, simply append `&id=` followed by the group ID.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).

    Suppression groups, or [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html), allow you to label a category of content that you regularly send. This gives your recipients the ability to opt out of a specific set of your email. For example, you might define a group for your transactional email, and one for your marketing email so that your users can continue recieving your transactional email witout having to receive your marketing content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups
  tags: Email,Asm, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroups-get-openapi.md
- name: SendGrid Add Asm Groups
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups
  tags: Email,Asm, Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroups-post-openapi.md
- name: SendGrid Delete Asm Groups Group
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a suppression group.**

    You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}
  tags: Email,Asm, Groups, Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-id-delete-openapi.md
- name: SendGrid Get Asm Groups Group
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}
  tags: Email,Asm, Groups, Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-id-get-openapi.md
- name: SendGrid Patch Asm Groups Group
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update or change a suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}
  tags: Email,Asm, Groups, Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-id-patch-openapi.md
- name: SendGrid Get Asm Groups Group  Suppressions
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}/suppressions
  tags: Email,Asm, Groups, Group, , Suppressions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-openapi.md
- name: SendGrid Add Asm Groups Group  Suppressions
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add email addresses to an unsubscribe group.**

    If you attempt to add suppressions to a group that has been deleted or does not exist, the suppressions will be added to the global suppressions list.

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}/suppressions
  tags: Email,Asm, Groups, Group, , Suppressions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-post-openapi.md
- name: SendGrid Add Asm Groups Group  Suppressions Search
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to search a suppression group for multiple suppressions.**

    When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}/suppressions/search
  tags: Email,Asm, Groups, Group, , Suppressions, Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-idsuppressionssearch-post-openapi.md
- name: SendGrid Delete Asm Groups Group  Suppressions Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove a suppressed email address from the given suppression group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/groups/{group_id}/suppressions/{email}
  tags: Email,Asm, Groups, Group, , Suppressions, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmgroupsgroup-idsuppressionsemail-delete-openapi.md
- name: SendGrid Get Asm Suppressions
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all suppressions.**

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/suppressions
  tags: Email,Asm, Suppressions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmsuppressions-get-openapi.md
- name: SendGrid Add Asm Suppressions Global
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add one or more email addresses to the global suppressions group.**

    A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/suppressions/global
  tags: Email,Asm, Suppressions, Global
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmsuppressionsglobal-post-openapi.md
- name: SendGrid Delete Asm Suppressions Global Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove an email address from the global suppressions group.**

    A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/suppressions/global/{email}
  tags: Email,Asm, Suppressions, Global, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmsuppressionsglobalemail-delete-openapi.md
- name: SendGrid Get Asm Suppressions Global Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a global suppression. You can also use this endpoint to confirm if an email address is already globally suppresed.**

    If the email address you include in the URL path parameter `{email}` is alreayd globally suppressed, the response will include that email address. If the address you enter for `{email}` is not globally suppressed, an empty JSON object `{}` will be returned.

    A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/suppressions/global/{email}
  tags: Email,Asm, Suppressions, Global, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmsuppressionsglobalemail-get-openapi.md
- name: SendGrid Get Asm Suppressions Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint returns the list of all groups that the given email address has been unsubscribed from.**

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//asm/suppressions/{email}
  tags: Email,Asm, Suppressions, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/asmsuppressionsemail-get-openapi.md
- name: SendGrid Get Browsers Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your email statistics segmented by browser type.**

    **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

    Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//browsers/stats
  tags: Email,Browsers, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/browsersstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/browsersstats-get-openapi.md
- name: SendGrid Get Campaigns
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all of your campaigns.**

    Returns campaigns in reverse order they were created (newest first).

    Returns an empty array if no campaigns exist.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns
  tags: Email,Campaigns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaigns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaigns-get-openapi.md
- name: SendGrid Add Campaigns
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a campaign.**

    Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

    Note: In order to send or schedule the campaign, you will be required to provide a subject, sender ID, content (we suggest both html and plain text), and at least one list or segment ID. This information is not required when you create a campaign.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns
  tags: Email,Campaigns
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaigns-post-openapi.md
- name: SendGrid Delete Campaigns Campaign
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a specific campaign.**

    Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}
  tags: Email,Campaigns, Campaign
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-id-delete-openapi.md
- name: SendGrid Get Campaigns Campaign
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific campaign.**

    Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}
  tags: Email,Campaigns, Campaign
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-id-get-openapi.md
- name: SendGrid Patch Campaigns Campaign
  x-api-slug: sendgrid
  description: |-
    Update a campaign. This is especially useful if you only set up the campaign using POST /campaigns, but didn't set many of the parameters.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}
  tags: Email,Campaigns, Campaign
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-id-patch-openapi.md
- name: SendGrid Delete Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to unschedule a campaign that has already been scheduled to be sent.**

    A successful unschedule will return a 204.
    If the specified campaign is in the process of being sent, the only option is to cancel (a different method).

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedules-delete-openapi.md
- name: SendGrid Get Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedules-get-openapi.md
- name: SendGrid Patch Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows to you change the scheduled time and date for a campaign to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedules-patch-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to schedule a specific date and time for your campaign to be sent.**

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules
  tags: Email,Campaigns, Campaign, , Schedules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedules-post-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules Now
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to immediately send a campaign at the time you make the API call.**

    Normally a POST would have a request body, but since this endpoint is telling us to send a resource that is already created, a request body is not needed.

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules/now
  tags: Email,Campaigns, Campaign, , Schedules, Now
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedulesnow-post-openapi.md
- name: SendGrid Add Campaigns Campaign  Schedules Test
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to send a test campaign.**

    To send to multiple addresses, use an array for the JSON "to" value ["one@address","two@address"]

    For more information:

    * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//campaigns/{campaign_id}/schedules/test
  tags: Email,Campaigns, Campaign, , Schedules, Test
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/campaignscampaign-idschedulestest-post-openapi.md
- name: SendGrid Get Categories
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all of your categories.**\n\nCategories
    can help organize your email analytics by enabling you to \u201Ctag\u201D emails
    by type or broad topic. You can define your own custom categories. For more information,
    please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//categories
  tags: Email,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categories-get-openapi.md
- name: SendGrid Get Categories Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

    If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

    Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//categories/stats
  tags: Email,Categories, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categoriesstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categoriesstats-get-openapi.md
- name: SendGrid Get Categories Stats Sums
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range.**

    If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

    Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//categories/stats/sums
  tags: Email,Categories, Stats, Sums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categoriesstatssums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/categoriesstatssums-get-openapi.md
- name: SendGrid Get Clients Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your email statistics segmented by client type.**

    **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

    Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//clients/stats
  tags: Email,Clients, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/clientsstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/clientsstats-get-openapi.md
- name: SendGrid Get Clients Client Type Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your email statistics segmented by a specific client type.**

    **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

    ## Available Client Types
    - phone
    - tablet
    - webmail
    - desktop

    Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//clients/{client_type}/stats
  tags: Email,Clients, Client, Type, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/clientsclient-typestats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/clientsclient-typestats-get-openapi.md
- name: SendGrid Get Contactdb Custom Fields
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all custom fields.** \n\nThe
    contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/custom_fields
  tags: Email,Contactdb, Custom, Fields
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fields-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fields-get-openapi.md
- name: SendGrid Add Contactdb Custom Fields
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a custom field.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/custom_fields
  tags: Email,Contactdb, Custom, Fields
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fields-post-openapi.md
- name: SendGrid Delete Contactdb Custom Fields Custom Field
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a custom field by ID.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/custom_fields/{custom_field_id}
  tags: Email,Contactdb, Custom, Fields, Custom, Field
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fieldscustom-field-id-delete-openapi.md
- name: SendGrid Get Contactdb Custom Fields Custom Field
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a custom field by ID.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/custom_fields/{custom_field_id}
  tags: Email,Contactdb, Custom, Fields, Custom, Field
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fieldscustom-field-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbcustom-fieldscustom-field-id-get-openapi.md
- name: SendGrid Delete Contactdb Lists
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete multiple recipient lists.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists
  tags: Email,Contactdb, Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblists-delete-openapi.md
- name: SendGrid Get Contactdb Lists
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists
  tags: Email,Contactdb, Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblists-get-openapi.md
- name: SendGrid Add Contactdb Lists
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a list for your recipients.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists
  tags: Email,Contactdb, Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblists-post-openapi.md
- name: SendGrid Delete Contactdb Lists List
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a specific recipient list with the given ID.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}
  tags: Email,Contactdb, Lists, List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-id-delete-openapi.md
- name: SendGrid Get Contactdb Lists List
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a single recipient list.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}
  tags: Email,Contactdb, Lists, List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-id-get-openapi.md
- name: SendGrid Patch Contactdb Lists List
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the name of one of your recipient lists.**


    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}
  tags: Email,Contactdb, Lists, List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-id-patch-openapi.md
- name: SendGrid Get Contactdb Lists List  Recipients
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all recipients on the list
    with the given ID.** \n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
    recipients."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients
  tags: Email,Contactdb, Lists, List, , Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-idrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-idrecipients-get-openapi.md
- name: SendGrid Add Contactdb Lists List  Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add multiple recipients to a list.**

    Adds existing recipients to a list, passing in the recipient IDs to add. Recipient IDs should be passed exactly as they are returned from recipient endpoints.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients
  tags: Email,Contactdb, Lists, List, , Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-idrecipients-post-openapi.md
- name: SendGrid Delete Contactdb Lists List  Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a single recipient from a list.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients/{recipient_id}
  tags: Email,Contactdb, Lists, List, , Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-idrecipientsrecipient-id-delete-openapi.md
- name: SendGrid Add Contactdb Lists List  Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add a single recipient to a list.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients/{recipient_id}
  tags: Email,Contactdb, Lists, List, , Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdblistslist-idrecipientsrecipient-id-post-openapi.md
- name: SendGrid Delete Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to deletes one or more recipients.**

    The body of an API call to this endpoint must include an array of recipient IDs of the recipients you want to delete.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipients-delete-openapi.md
- name: SendGrid Get Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your Marketing Campaigns recipients.**

    Batch deletion of a page makes it possible to receive an empty page of recipients before reaching the end of
    the list of recipients. To avoid this issue; iterate over pages until a 404 is retrieved.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipients-get-openapi.md
- name: SendGrid Patch Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update one or more recipients.**

    The body of an API call to this endpoint must include an array of one or more recipient objects.

    It is of note that you can add custom field data as parameters on recipient objects. We have provided an example using some of the default custom fields SendGrid provides.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipients-patch-openapi.md
- name: SendGrid Add Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add a Marketing Campaigns recipient.**

    You can add custom field data as a parameter on this endpoint. We have provided an example using some of the default custom fields SendGrid provides.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipients-post-openapi.md
- name: SendGrid Get Contactdb Recipients Billable Count
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for.**

    You are billed for marketing campaigns based on the highest number of recipients you have had in your account at one time. This endpoint will allow you to know the current billable count value.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/billable_count
  tags: Email,Contactdb, Recipients, Billable, Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsbillable-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsbillable-count-get-openapi.md
- name: SendGrid Get Contactdb Recipients Count
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/count
  tags: Email,Contactdb, Recipients, Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientscount-get-openapi.md
- name: SendGrid Get Contactdb Recipients Search
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to perform a search on all of your Marketing Campaigns recipients.**

    field_name:

    * is a variable that is substituted for your actual custom field name from your recipient.
    * Text fields must be url-encoded. Date fields are searchable only by unix timestamp (e.g. 2/2/2015 becomes 1422835200)
    * If field_name is a 'reserved' date field, such as created_at or updated_at, the system will internally convert
    your epoch time to a date range encompassing the entire day. For example, an epoch time of 1422835600 converts to
    Mon, 02 Feb 2015 00:06:40 GMT, but internally the system will search from Mon, 02 Feb 2015 00:00:00 GMT through
    Mon, 02 Feb 2015 23:59:59 GMT.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/search
  tags: Email,Contactdb, Recipients, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientssearch-get-openapi.md
- name: SendGrid Delete Contactdb Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a single recipient with the given ID from your contact database.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}
  tags: Email,Contactdb, Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsrecipient-id-delete-openapi.md
- name: SendGrid Get Contactdb Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single recipient by ID from your contact database.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}
  tags: Email,Contactdb, Recipients, Recipient
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsrecipient-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsrecipient-id-get-openapi.md
- name: SendGrid Get Contactdb Recipients Recipient  Lists
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the lists that a given recipient belongs to.**

    Each recipient can be on many lists. This endpoint gives you all of the lists that any one recipient has been added to.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}/lists
  tags: Email,Contactdb, Recipients, Recipient, , Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsrecipient-idlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbrecipientsrecipient-idlists-get-openapi.md
- name: SendGrid Get Contactdb Reserved Fields
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to list all fields that are reserved and can't be used for custom field names.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/reserved_fields
  tags: Email,Contactdb, Reserved, Fields
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbreserved-fields-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbreserved-fields-get-openapi.md
- name: SendGrid Get Contactdb Segments
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your segments.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments
  tags: Email,Contactdb, Segments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegments-get-openapi.md
- name: SendGrid Add Contactdb Segments
  x-api-slug: sendgrid
  description: "**This endpoint allows you to create a segment.**\n\nAll recipients
    in your contactdb will be added or removed automatically depending on whether
    they match the criteria for this segment.\n\nList Id:\n\n* Send this to segment
    from an existing list\n* Don't send this in order to segment from your entire
    contactdb.\n\nValid operators for create and update depend on the type of the
    field you are segmenting: \n\n* **Dates:** \"eq\", \"ne\", \"lt\" (before), \"gt\"
    (after) \n* **Text:** \"contains\", \"eq\" (is - matches the full field), \"ne\"
    (is not - matches any field where the entire field is not the condition value)
    \n* **Numbers:** \"eq\", \"lt\", \"gt\" \n* **Email Clicks and Opens:** \"eq\"
    (opened), \"ne\" (not opened) \n\nSegment conditions using \"eq\" or \"ne\" for
    email clicks and opens should provide a \"field\" of either *clicks.campaign_identifier*
    or *opens.campaign_identifier*. The condition value should be a string containing
    the id of a completed campaign. \n\nSegments may contain multiple condtions, joined
    by an \"and\" or \"or\" in the \"and_or\" field. The first condition in the conditions
    list must have an empty \"and_or\", and subsequent conditions must all specify
    an \"and_or\".\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
    recipients.\n\nFor more information about segments in Marketing Campaigns, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments
  tags: Email,Contactdb, Segments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegments-post-openapi.md
- name: SendGrid Delete Contactdb Segments Segment
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a segment from your recipients database.**

    You also have the option to delete all the contacts from your Marketing Campaigns recipient database who were in this segment.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments/{segment_id}
  tags: Email,Contactdb, Segments, Segment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-id-delete-openapi.md
- name: SendGrid Get Contactdb Segments Segment
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single segment with the given ID.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments/{segment_id}
  tags: Email,Contactdb, Segments, Segment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-id-get-openapi.md
- name: SendGrid Patch Contactdb Segments Segment
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update a segment.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments/{segment_id}
  tags: Email,Contactdb, Segments, Segment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-id-patch-openapi.md
- name: SendGrid Get Contactdb Segments Segment  Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of the recipients in a segment with the given ID.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments/{segment_id}/recipients
  tags: Email,Contactdb, Segments, Segment, , Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-idrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbsegmentssegment-idrecipients-get-openapi.md
- name: SendGrid Get Contactdb Status
  x-api-slug: sendgrid
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/status
  tags: Email,Contactdb, Status
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/contactdbstatus-get-openapi.md
- name: SendGrid Get Devices Stats
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your email statistics segmented
    by the device type.**\n\n**We only store up to 7 days of email activity in our
    database.** By default, 500 items will be returned per request via the Advanced
    Stats API endpoints.\n\n## Available Device Types\n| **Device** | **Description**
    | **Example** |\n|---|---|---|\n| Desktop | Email software on desktop computer.
    | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail |\tA web-based email client.
    | I.E., Yahoo, Google, AOL, or Outlook.com. |\n| Phone | A smart phone. | iPhone,
    Android, Blackberry, etc.\n| Tablet | A tablet computer. | iPad, android based
    tablet, etc. |\n| Other | An unrecognized device. |\n\nAdvanced Stats provide
    a more in-depth view of your email statistics and the actions taken by your recipients.
    You can segment these statistics by geographic location, device type, client type,
    browser, and mailbox provider. For more information about statistics, please see
    our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//devices/stats
  tags: Email,Devices, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/devicesstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/devicesstats-get-openapi.md
- name: SendGrid Get Geo Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your email statistics segmented by country and state/province.**

    **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

    Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//geo/stats
  tags: Email,Geo, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/geostats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/geostats-get-openapi.md
- name: SendGrid Get Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all assigned and unassigned IPs.**

    Response includes warm up status, pools, assigned subusers, and whitelabel info. The start_date field corresponds to when warmup started for that IP.

    A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips
  tags: Email,Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ips-get-openapi.md
- name: SendGrid Add Ips
  x-api-slug: sendgrid
  description: This endpoint is for adding a(n) IP Address(es) to your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips
  tags: Email,Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ips-post-openapi.md
- name: SendGrid Get Ips Assigned
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve only assigned IP addresses.**

    A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/assigned
  tags: Email,Ips, Assigned
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipsassigned-get-openapi.md
- name: SendGrid Get Ips Pools
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retreive all of your IP pools.**

    IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

    IP pools can only be used with whitelabeled IP addresses.

    If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools
  tags: Email,Ips, Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspools-get-openapi.md
- name: SendGrid Add Ips Pools
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create an IP pool.**

    **Each user can create up to 10 different IP pools.**

    IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

    IP pools can only be used with whitelabeled IP addresses.

    If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools
  tags: Email,Ips, Pools
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspools-post-openapi.md
- name: SendGrid Delete Ips Pools Pool Name
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete an IP pool.**

    IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

    IP pools can only be used with whitelabeled IP addresses.

    If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools/{pool_name}
  tags: Email,Ips, Pools, Pool, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-name-delete-openapi.md
- name: SendGrid Get Ips Pools Pool Name
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to list all of the IP addresses that are in a specific IP pool.**

    IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

    IP pools can only be used with whitelabeled IP addresses.

    If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools/{pool_name}
  tags: Email,Ips, Pools, Pool, Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-name-get-openapi.md
- name: SendGrid Put Ips Pools Pool Name
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the name of an IP pool.**

    IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

    IP pools can only be used with whitelabeled IP addresses.

    If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools/{pool_name}
  tags: Email,Ips, Pools, Pool, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-name-put-openapi.md
- name: SendGrid Add Ips Pools Pool Name Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add an IP address to an IP pool.**

    You can add the same IP address to multiple pools. It may take up to 60 seconds for your IP address to be added to a pool after your request is made.

    A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools/{pool_name}/ips
  tags: Email,Ips, Pools, Pool, Name, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-nameips-post-openapi.md
- name: SendGrid Delete Ips Pools Pool Name Ips Ip
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove an IP address from an IP pool.**

    The same IP address can be added to multiple IP pools.

    A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/pools/{pool_name}/ips/{ip}
  tags: Email,Ips, Pools, Pool, Name, Ips, Ip
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipspoolspool-nameipsip-delete-openapi.md
- name: SendGrid Get Ips Remaining
  x-api-slug: sendgrid
  description: This endpoint gets amount of IP Addresses that can still be created
    during a given period and the price of those IPs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/remaining
  tags: Email,Ips, Remaining
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipsremaining-get-openapi.md
- name: SendGrid Get Ips Warmup
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your IP addresses that are currently warming up.**

    SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

    For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/warmup
  tags: Email,Ips, Warmup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipswarmup-get-openapi.md
- name: SendGrid Add Ips Warmup
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to enter an IP address into warmup mode.**

    SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

    For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/warmup
  tags: Email,Ips, Warmup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipswarmup-post-openapi.md
- name: SendGrid Delete Ips Warmup Ip Address
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to remove an IP address from warmup mode.**

    SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

    For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/warmup/{ip_address}
  tags: Email,Ips, Warmup, Ip, Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipswarmupip-address-delete-openapi.md
- name: SendGrid Get Ips Warmup Ip Address
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the warmup status for a specific IP address.**

    SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

    For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/warmup/{ip_address}
  tags: Email,Ips, Warmup, Ip, Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipswarmupip-address-get-openapi.md
- name: SendGrid Get Ips Ip Address
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to see which IP pools a particular IP address has been added to.**

    The same IP address can be added to multiple IP pools.

    A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//ips/{ip_address}
  tags: Email,Ips, Ip, Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/ipsip-address-get-openapi.md
- name: SendGrid Add Mail Batch
  x-api-slug: sendgrid
  description: "**This endpoint allows you to generate a new batch ID. This batch
    ID can be associated with scheduled sends via the mail/send endpoint.**\n\nIf
    you set the SMTPAPI header `batch_id`, it allows you to then associate multiple
    scheduled mail/send requests together with the same ID. Then at anytime up to
    10 minutes before the schedule date, you can cancel all of the mail/send requests
    that have this batch ID by calling the Cancel Scheduled Send endpoint. \n\nMore
    Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail/batch
  tags: Email,Mail, Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mailbatch-post-openapi.md
- name: SendGrid Get Mail Batch Batch
  x-api-slug: sendgrid
  description: "**This endpoint allows you to validate a batch ID.**\n\nIf you set
    the SMTPAPI header `batch_id`, it allows you to then associate multiple scheduled
    mail/send requests together with the same ID. Then at anytime up to 10 minutes
    before the schedule date, you can cancel all of the mail/send requests that have
    this batch ID by calling the Cancel Scheduled Send endpoint. \n\nMore Information:\n\n*
    [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail/batch/{batch_id}
  tags: Email,Mail, Batch, Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mailbatchbatch-id-get-openapi.md
- name: SendGrid Add Mail Send
  x-api-slug: sendgrid
  description: "This endpoint allows you to send email over SendGrid\u2019s v3 Web
    API, the most recent version of our API. If you are looking for documentation
    about the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
    Top level parameters are referred to as \"global\".\n* Individual fields within
    the personalizations array will override any other global, or \u201Cmessage level\u201D,
    parameters that are defined outside of personalizations.\n \n**SendGrid provides
    libraries to help you quickly and easily integrate with the v3 Web API in 7 different
    languages: [C#](https://github.com/sendgrid/sendgrid-csharp), [Go](https://github.com/sendgrid/sendgrid-go),
    [Java](https://github.com/sendgrid/sendgrid-java), [Node JS](https://github.com/sendgrid/sendgrid-nodejs),
    [PHP](https://github.com/sendgrid/sendgrid-php), [Python](https://github.com/sendgrid/sendgrid-python),
    and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor more detailed
    information about how to use the v3 Mail Send endpoint, please visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail/send
  tags: Email,Mail, Send
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mailsend-post-openapi.md
- name: SendGrid Get Mail Settings
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all mail settings.**\n\nMail
    settings allow you to tell SendGrid specific things to do to every email that
    you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings
  tags: Email,Mail, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settings-get-openapi.md
- name: SendGrid Get Mail Settings Address Whitelist
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current email address
    whitelist settings.**\n\nThe address whitelist setting whitelists a specified
    email address or domain for which mail should never be suppressed. For example,
    you own the domain \u201Cexample.com,\u201D and one or more of your recipients
    use email@example.com addresses, by placing example.com in the address whitelist
    setting, all bounces, blocks, and unsubscribes logged for that domain will be
    ignored and sent as if under normal sending conditions.\n\nMail settings allow
    you to tell SendGrid specific things to do to every email that you send to your
    recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/address_whitelist
  tags: Email,Mail, Settings, Address, Whitelist
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsaddress-whitelist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsaddress-whitelist-get-openapi.md
- name: SendGrid Patch Mail Settings Address Whitelist
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current email address whitelist
    settings.**\n\nThe address whitelist setting whitelists a specified email address
    or domain for which mail should never be suppressed. For example, you own the
    domain \u201Cexample.com,\u201D and one or more of your recipients use email@example.com
    addresses, by placing example.com in the address whitelist setting, all bounces,
    blocks, and unsubscribes logged for that domain will be ignored and sent as if
    under normal sending conditions.\n\nMail settings allow you to tell SendGrid specific
    things to do to every email that you send to your recipients over SendGrid\u2019s
    [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
    Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/address_whitelist
  tags: Email,Mail, Settings, Address, Whitelist
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsaddress-whitelist-patch-openapi.md
- name: SendGrid Get Mail Settings Bcc
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current BCC mail settings.**\n\nWhen
    the BCC mail setting is enabled, SendGrid will automatically send a blind carbon
    copy (BCC) to an address for every email sent without adding that address to the
    header. Please note that only one email address may be entered in this field,
    if you wish to distribute BCCs to multiple addresses you will need to create a
    distribution group or use forwarding rules.\n\nMail settings allow you to tell
    SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/bcc
  tags: Email,Mail, Settings, Bcc
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbcc-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbcc-get-openapi.md
- name: SendGrid Patch Mail Settings Bcc
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current BCC mail settings.**\n\nWhen
    the BCC mail setting is enabled, SendGrid will automatically send a blind carbon
    copy (BCC) to an address for every email sent without adding that address to the
    header. Please note that only one email address may be entered in this field,
    if you wish to distribute BCCs to multiple addresses you will need to create a
    distribution group or use forwarding rules.\n\nMail settings allow you to tell
    SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/bcc
  tags: Email,Mail, Settings, Bcc
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbcc-patch-openapi.md
- name: SendGrid Get Mail Settings Bounce Purge
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current bounce purge settings.**\n\nThis
    setting allows you to set a schedule for SendGrid to automatically delete contacts
    from your soft and hard bounce suppression lists.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/bounce_purge
  tags: Email,Mail, Settings, Bounce, Purge
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbounce-purge-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbounce-purge-get-openapi.md
- name: SendGrid Patch Mail Settings Bounce Purge
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current bounce purge settings.**\n\nThis
    setting allows you to set a schedule for SendGrid to automatically delete contacts
    from your soft and hard bounce suppression lists.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/bounce_purge
  tags: Email,Mail, Settings, Bounce, Purge
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsbounce-purge-patch-openapi.md
- name: SendGrid Get Mail Settings Footer
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current Footer mail settings.**\n\nThe
    footer setting will insert a custom footer at the bottom of the text and HTML
    bodies. Use the embedded HTML editor and plain text entry fields to create the
    content of the footers to be inserted into your emails.\n\nMail settings allow
    you to tell SendGrid specific things to do to every email that you send to your
    recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/footer
  tags: Email,Mail, Settings, Footer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsfooter-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsfooter-get-openapi.md
- name: SendGrid Patch Mail Settings Footer
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current Footer mail settings.**\n\nThe
    footer setting will insert a custom footer at the bottom of the text and HTML
    bodies. Use the embedded HTML editor and plain text entry fields to create the
    content of the footers to be inserted into your emails.\n\nMail settings allow
    you to tell SendGrid specific things to do to every email that you send to your
    recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/footer
  tags: Email,Mail, Settings, Footer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsfooter-patch-openapi.md
- name: SendGrid Get Mail Settings Forward Bounce
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current bounce forwarding
    mail settings.**\n\nActivating this setting allows you to specify an email address
    to which bounce reports are forwarded.\n\nMail settings allow you to tell SendGrid
    specific things to do to every email that you send to your recipients over SendGrid\u2019s
    [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
    Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/forward_bounce
  tags: Email,Mail, Settings, Forward, Bounce
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-bounce-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-bounce-get-openapi.md
- name: SendGrid Patch Mail Settings Forward Bounce
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current bounce forwarding
    mail settings.**\n\nActivating this setting allows you to specify an email address
    to which bounce reports are forwarded.\n\nMail settings allow you to tell SendGrid
    specific things to do to every email that you send to your recipients over SendGrid\u2019s
    [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
    Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/forward_bounce
  tags: Email,Mail, Settings, Forward, Bounce
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-bounce-patch-openapi.md
- name: SendGrid Get Mail Settings Forward Spam
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current Forward Spam mail
    settings.**\n\nEnabling the forward spam setting allows you to specify an email
    address to which spam reports will be forwarded.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/forward_spam
  tags: Email,Mail, Settings, Forward, Spam
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-spam-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-spam-get-openapi.md
- name: SendGrid Patch Mail Settings Forward Spam
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current Forward Spam mail
    settings.**\n\nEnabling the forward spam setting allows you to specify an email
    address to which spam reports will be forwarded.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/forward_spam
  tags: Email,Mail, Settings, Forward, Spam
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsforward-spam-patch-openapi.md
- name: SendGrid Get Mail Settings Plain Content
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current Plain Content
    mail settings.**\n\nThe plain content setting will automatically convert any plain
    text emails that you send to HTML before sending.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/plain_content
  tags: Email,Mail, Settings, Plain, Content
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsplain-content-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsplain-content-get-openapi.md
- name: SendGrid Patch Mail Settings Plain Content
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current Plain Content mail
    settings.**\n\nThe plain content setting will automatically convert any plain
    text emails that you send to HTML before sending.\n\nMail settings allow you to
    tell SendGrid specific things to do to every email that you send to your recipients
    over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/plain_content
  tags: Email,Mail, Settings, Plain, Content
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsplain-content-patch-openapi.md
- name: SendGrid Get Mail Settings Spam Check
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current Spam Checker mail
    settings.**\n\nThe spam checker filter notifies you when emails are detected that
    exceed a predefined spam threshold.\n\nMail settings allow you to tell SendGrid
    specific things to do to every email that you send to your recipients over SendGrid\u2019s
    [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
    Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/spam_check
  tags: Email,Mail, Settings, Spam, Check
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsspam-check-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsspam-check-get-openapi.md
- name: SendGrid Patch Mail Settings Spam Check
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current spam checker mail
    settings.**\n\nThe spam checker filter notifies you when emails are detected that
    exceed a predefined spam threshold.\n\nMail settings allow you to tell SendGrid
    specific things to do to every email that you send to your recipients over SendGrid\u2019s
    [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
    Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/spam_check
  tags: Email,Mail, Settings, Spam, Check
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingsspam-check-patch-openapi.md
- name: SendGrid Get Mail Settings Template
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current legacy email template
    settings.**\n\nThis setting refers to our original email templates. We currently
    support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
    \n\nThe legacy email template setting wraps an HTML template around your email
    content. This can be useful for sending out marketing email and/or other HTML
    formatted messages.\n\nMail settings allow you to tell SendGrid specific things
    to do to every email that you send to your recipients over SendGrid\u2019s [Web
    API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/template
  tags: Email,Mail, Settings, Template
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingstemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingstemplate-get-openapi.md
- name: SendGrid Patch Mail Settings Template
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current legacy email template
    settings.**\n\nThis setting refers to our original email templates. We currently
    support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
    \n\nThe legacy email template setting wraps an HTML template around your email
    content. This can be useful for sending out marketing email and/or other HTML
    formatted messages.\n\nMail settings allow you to tell SendGrid specific things
    to do to every email that you send to your recipients over SendGrid\u2019s [Web
    API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mail_settings/template
  tags: Email,Mail, Settings, Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mail-settingstemplate-patch-openapi.md
- name: SendGrid Get Mailbox Provers Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your email statistics segmented by recipient mailbox provider.**

    **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

    Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//mailbox_providers/stats
  tags: Email,Mailbox, Provers, Stats
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/mailbox-providersstats-get-openapi.md
- name: SendGrid Get Partner Settings
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all partner settings that you can enable.**

    Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//partner_settings
  tags: Email,Partner, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/partner-settings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/partner-settings-get-openapi.md
- name: SendGrid Get Partner Settings New Relic
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your current New Relic partner settings.**

    Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

    By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//partner_settings/new_relic
  tags: Email,Partner, Settings, New, Relic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/partner-settingsnew-relic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/partner-settingsnew-relic-get-openapi.md
- name: SendGrid Patch Partner Settings New Relic
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update or change your New Relic partner settings.**

    Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

    By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//partner_settings/new_relic
  tags: Email,Partner, Settings, New, Relic
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/partner-settingsnew-relic-patch-openapi.md
- name: SendGrid Get Scopes
  x-api-slug: sendgrid
  description: "**This endpoint returns a list of all scopes that this user has access
    to.**\n\nAPI Keys can be used to authenticate the use of [SendGrid\u2019s v3 Web
    API](https://sendgrid.com/docs/API_Reference/Web_API_v3/index.html), or the [Mail
    API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html). API
    Keys may be assigned certain permissions, or scopes, that limit which API endpoints
    they are able to access. For a more detailed explanation of how you can use API
    Key permissios, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/api_keys.html#-API-Key-Permissions)
    or [Classroom](https://sendgrid.com/docs/Classroom/Basics/API/api_key_permissions.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//scopes
  tags: Email,Scopes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopes-get-openapi.md
- name: SendGrid Get Scopes Requests
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all recent access requests.

    **Note:** The Response Header's 'link' parameter will include pagination info. For example:

    link: ```<https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=0>; rel="first"; title="1", <https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=10>; rel="last"; title="2", <https://api.sendgrid.com/v3/scopes/requests?limit=10&offset=0>; rel="prev"; title="1"```
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//scopes/requests
  tags: Email,Scopes, Requests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequests-get-openapi.md
- name: SendGrid Delete Scopes Requests Request
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to deny an attempt to access your account.

    **Note:** Only teammate admins may delete a teammate's access request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//scopes/requests/{request_id}
  tags: Email,Scopes, Requests, Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequestsrequest-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequestsrequest-id-delete-openapi.md
- name: SendGrid Patch Scopes Requests Request  Approve
  x-api-slug: sendgrid
  description: "This endpoint allows you to approve an access attempt.\n\n**Note:**
    Only teammate admins may approve another teammate\u2019s access request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//scopes/requests/{request_id}/approve
  tags: Email,Scopes, Requests, Request, , Approve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequestsrequest-idapprove-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/scopesrequestsrequest-idapprove-patch-openapi.md
- name: SendGrid Get Senders
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders
  tags: Email,Senders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senders-get-openapi.md
- name: SendGrid Add Senders
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new sender identity.**

    *You may create up to 100 unique sender identities.*

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders
  tags: Email,Senders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senders-post-openapi.md
- name: SendGrid Delete Senders Sender
  x-api-slug: sendgrid
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders/{sender_id}
  tags: Email,Senders, Sender
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid Get Senders Sender
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders/{sender_id}
  tags: Email,Senders, Sender
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid Patch Senders Sender
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders/{sender_id}
  tags: Email,Senders, Sender
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid Add Senders Sender  Resend Verification
  x-api-slug: sendgrid
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//senders/{sender_id}/resend_verification
  tags: Email,Senders, Sender, , Resend, Verification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid Get Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your global email statistics between a given date range.**

    Parent accounts will see aggregated stats for their account and all subuser accounts. Subuser accounts will only see their own stats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//stats
  tags: Email,Stats
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/stats-get-openapi.md
- name: SendGrid Get Subusers
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers
  tags: Email,Subusers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusers-get-openapi.md
- name: SendGrid Add Subusers
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers
  tags: Email,Subusers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusers-post-openapi.md
- name: SendGrid Get Subusers Reputations
  x-api-slug: sendgrid
  description: |-
    Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received. When a bounce, spam report, or other negative action happens on a sent email, it will effect your sender rating.

    This endpoint allows you to request the reputations for your subusers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/reputations
  tags: Email,Subusers, Reputations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersreputations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersreputations-get-openapi.md
- name: SendGrid Get Subusers Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the email statistics for the given subusers.**

    You may retrieve statistics for up to 10 different subusers by including an additional _subusers_ parameter for each additional subuser.

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats
  tags: Email,Subusers, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstats-get-openapi.md
- name: SendGrid Get Subusers Stats Monthly
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the monthly email statistics for all subusers over the given date range.**

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
    `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats/monthly
  tags: Email,Subusers, Stats, Monthly
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstatsmonthly-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstatsmonthly-get-openapi.md
- name: SendGrid Get Subusers Stats Sums
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the total sums of each email statistic metric for all subusers over the given date range.**


    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats/sums
  tags: Email,Subusers, Stats, Sums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstatssums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subusersstatssums-get-openapi.md
- name: SendGrid Delete Subusers Subuser Name
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to delete a subuser. This is a permanent action, once deleted a subuser cannot be retrieved.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}
  tags: Email,Subusers, Subuser, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-name-delete-openapi.md
- name: SendGrid Patch Subusers Subuser Name
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to enable or disable a subuser.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}
  tags: Email,Subusers, Subuser, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-name-patch-openapi.md
- name: SendGrid Put Subusers Subuser Name Ips
  x-api-slug: sendgrid
  description: "Each subuser should be assigned to an IP address, from which all of
    this subuser's mail will be sent. Often, this is the same IP as the parent account,
    but each subuser can have their own, or multiple, IP addresses as well. \n\nMore
    information:\n\n* [How to request more IPs](https://sendgrid.com/docs/Classroom/Basics/Account/adding_an_additional_dedicated_ip_to_your_account.html)\n*
    [IPs can be whitelabeled](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/ips.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/ips
  tags: Email,Subusers, Subuser, Name, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-nameips-put-openapi.md
- name: SendGrid Delete Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namemonitor-delete-openapi.md
- name: SendGrid Get Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namemonitor-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namemonitor-get-openapi.md
- name: SendGrid Add Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namemonitor-post-openapi.md
- name: SendGrid Put Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namemonitor-put-openapi.md
- name: SendGrid Get Subusers Subuser Name Stats Monthly
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrive the monthly email statistics for a specific subuser.**

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
    `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/stats/monthly
  tags: Email,Subusers, Subuser, Name, Stats, Monthly
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namestatsmonthly-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/subuserssubuser-namestatsmonthly-get-openapi.md
- name: SendGrid Delete Suppression Blocks
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete all email addresses on your blocks
    list.**\n\nThere are two options for deleting blocked emails: \n\n1. You can delete
    all blocked emails by setting `delete_all` to true in the request body. \n2. You
    can delete some blocked emails by specifying the email addresses in an array in
    the request body.\n\n[Blocks](https://sendgrid.com/docs/Glossary/blocks.html)
    happen when your message was rejected for a reason related to the message, not
    the recipient address. This can happen when your mail server IP address has been
    added to a blacklist or blocked by an ISP, or if the message content is flagged
    by a filter on the receiving server.\n\nFor more information, please see our [User
    Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/blocks
  tags: Email,Suppression, Blocks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionblocks-delete-openapi.md
- name: SendGrid Get Suppression Blocks
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all email addresses that are currently on your blocks list.**

    There are several causes for [blocked](https://sendgrid.com/docs/Glossary/blocks.html) emails: for example, your mail server IP address is on an ISP blacklist, or blocked by an ISP, or if the receiving server flags the message content.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/blocks
  tags: Email,Suppression, Blocks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionblocks-get-openapi.md
- name: SendGrid Delete Suppression Blocks Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a specific email address from your blocks list.**

    [Blocks](https://sendgrid.com/docs/Glossary/blocks.html) happen when your message was rejected for a reason related to the message, not the recipient address. This can happen when your mail server IP address has been added to a blacklist or blocked by an ISP, or if the message content is flagged by a filter on the receiving server.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/blocks/{email}
  tags: Email,Suppression, Blocks, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionblocksemail-delete-openapi.md
- name: SendGrid Get Suppression Blocks Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific email address from your blocks list.**

    [Blocks](https://sendgrid.com/docs/Glossary/blocks.html) happen when your message was rejected for a reason related to the message, not the recipient address. This can happen when your mail server IP address has been added to a blacklist or blocked by an ISP, or if the message content is flagged by a filter on the receiving server.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/blocks/{email}
  tags: Email,Suppression, Blocks, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionblocksemail-get-openapi.md
- name: SendGrid Delete Suppression Bounces
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete all of your bounces. You can
    also use this endpoint to remove a specific email address from your bounce list.**\n\nA
    bounced email is when the message is undeliverable and then returned to the server
    that sent it.\n\nFor more information see: \n\n* [User Guide > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html)
    for more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)\n*
    [Classroom > List Scrubbing Guide](https://sendgrid.com/docs/Classroom/Deliver/list_scrubbing.html)\n\nNote:
    the `delete_all` and `emails` parameters should be used independently of each
    other as they have different purposes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/bounces
  tags: Email,Suppression, Bounces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbounces-delete-openapi.md
- name: SendGrid Get Suppression Bounces
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all of your bounces.**\n\nA
    bounced email is when the message is undeliverable and then returned to the server
    that sent it.  \n\nFor more information see: \n\n* [User Guide > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html)
    for more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/bounces
  tags: Email,Suppression, Bounces
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbounces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbounces-get-openapi.md
- name: SendGrid Delete Suppression Bounces Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove an email address from your bounce
    list.**\n\nA bounced email is when the message is undeliverable and then returned
    to the server that sent it. This endpoint allows you to delete a single email
    addresses from your bounce list. \n\nFor more information see: \n\n* [User Guide
    > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html) for
    more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)\n*
    [Classroom > List Scrubbing Guide](https://sendgrid.com/docs/Classroom/Deliver/list_scrubbing.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/bounces/{email}
  tags: Email,Suppression, Bounces, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbouncesemail-delete-openapi.md
- name: SendGrid Get Suppression Bounces Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific bounce for a given
    email address.**\n\nA bounced email is when the message is undeliverable and then
    returned to the server that sent it.\n\nFor more information see: \n\n* [User
    Guide > Bounces](https://sendgrid.com/docs/User_Guide/Suppressions/bounces.html)
    for more information\n* [Glossary > Bounces](https://sendgrid.com/docs/Glossary/Bounces.html)\n*
    [Classroom > List Scrubbing Guide](https://sendgrid.com/docs/Classroom/Deliver/list_scrubbing.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/bounces/{email}
  tags: Email,Suppression, Bounces, Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbouncesemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionbouncesemail-get-openapi.md
- name: SendGrid Delete Suppression Inval Emails
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove email addresses from your invalid
    email address list.**\n\nThere are two options for deleting invalid email addresses:
    \n\n1) You can delete all invalid email addresses by setting `delete_all` to true
    in the request body.\n2) You can delete some invalid email addresses by specifying
    certain addresses in an array in the request body.\n\nAn invalid email occurs
    when you attempt to send email to an address that is formatted in a manner that
    does not meet internet email format standards or the email does not exist at the
    recipient\u2019s mail server.\n\nExamples include addresses without the \u201C@\u201D
    sign or addresses that include certain special characters and/or spaces. This
    response can come from our own server or the recipient mail server.\n\nFor more
    information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails
  tags: Email,Suppression, Inval, Emails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emails-delete-openapi.md
- name: SendGrid Get Suppression Inval Emails
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all invalid email
    addresses.**\n\nAn invalid email occurs when you attempt to send email to an address
    that is formatted in a manner that does not meet internet email format standards
    or the email does not exist at the recipient\u2019s mail server.\n\nExamples include
    addresses without the \u201C@\u201D sign or addresses that include certain special
    characters and/or spaces. This response can come from our own server or the recipient
    mail server.\n\nFor more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails
  tags: Email,Suppression, Inval, Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emails-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emails-get-openapi.md
- name: SendGrid Delete Suppression Inval Emails Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove a specific email address from
    the invalid email address list.**\n\nAn invalid email occurs when you attempt
    to send email to an address that is formatted in a manner that does not meet internet
    email format standards or the email does not exist at the recipient\u2019s mail
    server.\n\nExamples include addresses without the \u201C@\u201D sign or addresses
    that include certain special characters and/or spaces. This response can come
    from our own server or the recipient mail server.\n\nFor more information, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails/{email}
  tags: Email,Suppression, Inval, Emails, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emailsemail-delete-openapi.md
- name: SendGrid Get Suppression Inval Emails Email
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific invalid email addresses.**\n\nAn
    invalid email occurs when you attempt to send email to an address that is formatted
    in a manner that does not meet internet email format standards or the email does
    not exist at the recipient\u2019s mail server.\n\nExamples include addresses without
    the \u201C@\u201D sign or addresses that include certain special characters and/or
    spaces. This response can come from our own server or the recipient mail server.\n\nFor
    more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/invalid_emails.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/invalid_emails/{email}
  tags: Email,Suppression, Inval, Emails, Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emailsemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressioninvalid-emailsemail-get-openapi.md
- name: SendGrid Delete Suppression Spam Reports
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete your spam reports.**\n\nThere
    are two options for deleting spam reports: \n\n1) You can delete all spam reports
    by setting \"delete_all\" to true in the request body. \n2) You can delete some
    spam reports by specifying the email addresses in an array in the request body.\n\n[Spam
    reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient
    indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html)
    and then their email provider reports this to SendGrid.\n\nFor more information,
    please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/spam_reports
  tags: Email,Suppression, Spam, Reports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reports-delete-openapi.md
- name: SendGrid Get Suppression Spam Reports
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all spam reports.**

    [Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html) and then their email provider reports this to SendGrid.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/spam_reports
  tags: Email,Suppression, Spam, Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reports-get-openapi.md
- name: SendGrid Delete Suppression Spam Reports Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a specific spam report.**

    [Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html) and then their email provider reports this to SendGrid.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/spam_reports/{email}
  tags: Email,Suppression, Spam, Reports, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reportsemail-delete-openapi.md
- name: SendGrid Get Suppression Spam Reports Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific spam report.**

    [Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html) and then their email provider reports this to SendGrid.

    For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/spam_reports/{email}
  tags: Email,Suppression, Spam, Reports, Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reportsemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionspam-reportsemail-get-openapi.md
- name: SendGrid Get Suppression Unsubscribes
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all email address that are globally suppressed.**

    A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//suppression/unsubscribes
  tags: Email,Suppression, Unsubscribes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/suppressionunsubscribes-get-openapi.md
- name: SendGrid Get Teammates
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all current teammates.

    **Note:** The Response Header will include pagination info. For example:

    link: ```<https://api.sendgrid.com/v3/teammates?limit=10&offset=0>; rel="first"; title="1", <https://api.sendgrid.com/v3/teammates?limit=10&offset=10>; rel="last"; title="2", <https://api.sendgrid.com/v3/teammates?limit=10&offset=0>; rel="prev"; title="1"```
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates
  tags: Email,Teammates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammates-get-openapi.md
- name: SendGrid Add Teammates
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to send a teammate invitation via email with a predefined set of scopes, or permissions.

    **Note:** A teammate invite will expire after 7 days, but you may resend the invite at any time to reset the expiration date.

    Essentials, [Legacy Lite](https://sendgrid.com/docs/Classroom/Basics/Billing/legacy_lite_plan.html), and Free Trial users may create up to one teammate per account. There are no limits for how many teammates a Pro or higher account may create.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates
  tags: Email,Teammates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammates-post-openapi.md
- name: SendGrid Get Teammates Pending
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all pending teammate invitations.

    **Note:** Each teammate invitation is valid for 7 days. Users may resend the invite to refresh the expiration date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/pending
  tags: Email,Teammates, Pending
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatespending-get-openapi.md
- name: SendGrid Delete Teammates Pending Token
  x-api-slug: sendgrid
  description: This endpoint allows you to delete a pending teammate invite.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/pending/{token}
  tags: Email,Teammates, Pending, Token
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatespendingtoken-delete-openapi.md
- name: SendGrid Add Teammates Pending Token Resend
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to resend a teammate invite.

    **Note:** Teammate invitations will expire after 7 days. Resending an invite will reset the expiration date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/pending/{token}/resend
  tags: Email,Teammates, Pending, Token, Resend
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatespendingtokenresend-post-openapi.md
- name: SendGrid Delete Teammates Username
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to delete a teammate.

    **Only the parent user or an admin teammate can delete another teammate.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/{username}
  tags: Email,Teammates, Username
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatesusername-delete-openapi.md
- name: SendGrid Get Teammates Username
  x-api-slug: sendgrid
  description: This endpoint allows you to retrieve a specific teammate by username.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/{username}
  tags: Email,Teammates, Username
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatesusername-get-openapi.md
- name: SendGrid Patch Teammates Username
  x-api-slug: sendgrid
  description: "This endpoint allows you to update a teammate\u2019s permissions.\n\nTo
    turn a teammate into an admin, the request body should contain an `is_admin` set
    to `true`. Otherwise, set `is_admin` to `false` and pass in all the scopes that
    a teammate should have.\n\n**Only the parent user or other admin teammates can
    update another teammate\u2019s permissions.**\n\n**Admin users can only update
    permissions.**"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//teammates/{username}
  tags: Email,Teammates, Username
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/teammatesusername-patch-openapi.md
- name: SendGrid Get Templates
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all transactional templates.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates
  tags: Email,Templates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templates-get-openapi.md
- name: SendGrid Add Templates
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates
  tags: Email,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templates-post-openapi.md
- name: SendGrid Delete Templates Template
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}
  tags: Email,Templates, Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-id-delete-openapi.md
- name: SendGrid Get Templates Template
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}
  tags: Email,Templates, Template
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-id-get-openapi.md
- name: SendGrid Patch Templates Template
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to edit a transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}
  tags: Email,Templates, Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-id-patch-openapi.md
- name: SendGrid Add Templates Template  Versions
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new version of a template.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}/versions
  tags: Email,Templates, Template, , Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversions-post-openapi.md
- name: SendGrid Delete Templates Template  Versions Version
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete one of your transactional template versions.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string | The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}/versions/{version_id}
  tags: Email,Templates, Template, , Versions, Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversionsversion-id-delete-openapi.md
- name: SendGrid Get Templates Template  Versions Version
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific version of a template.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string |  The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}/versions/{version_id}
  tags: Email,Templates, Template, , Versions, Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversionsversion-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversionsversion-id-get-openapi.md
- name: SendGrid Patch Templates Template  Versions Version
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to edit a version of one of your transactional templates.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string | The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}/versions/{version_id}
  tags: Email,Templates, Template, , Versions, Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversionsversion-id-patch-openapi.md
- name: SendGrid Add Templates Template  Versions Version  Activate
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to activate a version of one of your templates.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.


    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string |  The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//templates/{template_id}/versions/{version_id}/activate
  tags: Email,Templates, Template, , Versions, Version, , Activate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/templatestemplate-idversionsversion-idactivate-post-openapi.md
- name: SendGrid Get Tracking Settings
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a list of all tracking settings that you can enable on your account.**

    You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

    For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings
  tags: Email,Tracking, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settings-get-openapi.md
- name: SendGrid Get Tracking Settings Click
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your current click tracking setting.**

    You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

    For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/click
  tags: Email,Tracking, Settings, Click
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsclick-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsclick-get-openapi.md
- name: SendGrid Patch Tracking Settings Click
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to change your current click tracking setting. You can enable, or disable, click tracking using this endpoint.**

    You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

    For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/click
  tags: Email,Tracking, Settings, Click
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsclick-patch-openapi.md
- name: SendGrid Get Tracking Settings Google Analytics
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current setting for Google
    Analytics.**\n\nFor more information about using Google Analytics, please refer
    to [Google\u2019s URL Builder](https://support.google.com/analytics/answer/1033867?hl=en)
    and their article on [\"Best Practices for Campaign Building\"](https://support.google.com/analytics/answer/1037445).\n\nWe
    default the settings to Google\u2019s recommendations. For more information, see
    [Google Analytics Demystified](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/google_analytics_demystified_ga_statistics_vs_sg_statistics.html).\n\nYou
    can track a variety of the actions your recipients may take when interacting with
    your emails including opening your emails, clicking on links in your emails, and
    subscribing to (or unsubscribing from) your emails.\n\nFor more information about
    tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/google_analytics
  tags: Email,Tracking, Settings, Google, Analytics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsgoogle-analytics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsgoogle-analytics-get-openapi.md
- name: SendGrid Patch Tracking Settings Google Analytics
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current setting for Google
    Analytics.**\n\nFor more information about using Google Analytics, please refer
    to [Google\u2019s URL Builder](https://support.google.com/analytics/answer/1033867?hl=en)
    and their article on [\"Best Practices for Campaign Building\"](https://support.google.com/analytics/answer/1037445).\n\nWe
    default the settings to Google\u2019s recommendations. For more information, see
    [Google Analytics Demystified](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/google_analytics_demystified_ga_statistics_vs_sg_statistics.html).\n\nYou
    can track a variety of the actions your recipients may take when interacting with
    your emails including opening your emails, clicking on links in your emails, and
    subscribing to (or unsubscribing from) your emails.\n\nFor more information about
    tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/google_analytics
  tags: Email,Tracking, Settings, Google, Analytics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsgoogle-analytics-patch-openapi.md
- name: SendGrid Get Tracking Settings Open
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current settings for open
    tracking.**\n\nOpen Tracking adds an invisible image at the end of the email which
    can track email opens. If the email recipient has images enabled on their email
    client, a request to SendGrid\u2019s server for the invisible image is executed
    and an open event is logged. These events are logged in the Statistics portal,
    Email Activity interface, and are reported by the Event Webhook.\n\nYou can track
    a variety of the actions your recipients may take when interacting with your emails
    including opening your emails, clicking on links in your emails, and subscribing
    to (or unsubscribing from) your emails.\n\nFor more information about tracking,
    please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/open
  tags: Email,Tracking, Settings, Open
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsopen-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsopen-get-openapi.md
- name: SendGrid Patch Tracking Settings Open
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current settings for open
    tracking.**\n\nOpen Tracking adds an invisible image at the end of the email which
    can track email opens. If the email recipient has images enabled on their email
    client, a request to SendGrid\u2019s server for the invisible image is executed
    and an open event is logged. These events are logged in the Statistics portal,
    Email Activity interface, and are reported by the Event Webhook.\n\nYou can track
    a variety of the actions your recipients may take when interacting with your emails
    including opening your emails, clicking on links in your emails, and subscribing
    to (or unsubscribing from) your emails.\n\nFor more information about tracking,
    please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/open
  tags: Email,Tracking, Settings, Open
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingsopen-patch-openapi.md
- name: SendGrid Get Tracking Settings Subscription
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your current settings for subscription tracking.**

    Subscription tracking adds links to the bottom of your emails that allows your recipients to subscribe to, or unsubscribe from, your emails.

    You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

    For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/subscription
  tags: Email,Tracking, Settings, Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingssubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingssubscription-get-openapi.md
- name: SendGrid Patch Tracking Settings Subscription
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update your current settings for subscription tracking.**

    Subscription tracking adds links to the bottom of your emails that allows your recipients to subscribe to, or unsubscribe from, your emails.

    You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

    For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//tracking_settings/subscription
  tags: Email,Tracking, Settings, Subscription
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/tracking-settingssubscription-patch-openapi.md
- name: SendGrid Get User Account
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your user account details.**

    Your user's account information includes the user's account type and reputation.

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/account
  tags: Email,User, Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/useraccount-get-openapi.md
- name: SendGrid Get User Credits
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the current credit balance for your account.**

    Your monthly credit allotment limits the number of emails you may send before incurring overage charges. For more information about credits and billing, please visit our [Clssroom](https://sendgrid.com/docs/Classroom/Basics/Billing/billing_info_and_faqs.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/credits
  tags: Email,User, Credits
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/usercredits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/usercredits-get-openapi.md
- name: SendGrid Get User Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the email address currently on file for your account.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/email
  tags: Email,User, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/useremail-get-openapi.md
- name: SendGrid Put User Email
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the email address currently on file for your account.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/email
  tags: Email,User, Email
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/useremail-put-openapi.md
- name: SendGrid Put User Password
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update your password.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/password
  tags: Email,User, Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userpassword-put-openapi.md
- name: SendGrid Get User Profile
  x-api-slug: sendgrid
  description: |-
    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/profile
  tags: Email,User, Profile
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userprofile-get-openapi.md
- name: SendGrid Patch User Profile
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update your current profile details.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)

    It should be noted that any one or more of the parameters can be updated via the PATCH /user/profile endpoint. The only requirement is that you include at least one when you PATCH.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/profile
  tags: Email,User, Profile
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userprofile-patch-openapi.md
- name: SendGrid Get User Scheduled Sends
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all cancel/paused scheduled send information.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/scheduled_sends
  tags: Email,User, Scheduled, Sends
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userscheduled-sends-get-openapi.md
- name: SendGrid Add User Scheduled Sends
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

    If the maximum number of cancellations/pauses are added, HTTP 400 will
    be returned.

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/scheduled_sends
  tags: Email,User, Scheduled, Sends
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userscheduled-sends-post-openapi.md
- name: SendGrid Delete User Scheduled Sends Batch
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete the cancellation/pause of a scheduled send.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/scheduled_sends/{batch_id}
  tags: Email,User, Scheduled, Sends, Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userscheduled-sendsbatch-id-delete-openapi.md
- name: SendGrid Get User Scheduled Sends Batch
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the cancel/paused scheduled send information for a specific `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/scheduled_sends/{batch_id}
  tags: Email,User, Scheduled, Sends, Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userscheduled-sendsbatch-id-get-openapi.md
- name: SendGrid Patch User Scheduled Sends Batch
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the status of a scheduled send for the given `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/scheduled_sends/{batch_id}
  tags: Email,User, Scheduled, Sends, Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userscheduled-sendsbatch-id-patch-openapi.md
- name: SendGrid Get User Settings Enforced Tls
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current Enforced TLS settings.**\n\nThe
    Enforced TLS settings specify whether or not the recipient is required to support
    TLS or have a valid certificate. See the [SMTP Ports User Guide](https://sendgrid.com/docs/Classroom/Basics/Email_Infrastructure/smtp_ports.html)
    for more information on opportunistic TLS.\n\n**Note:** If either setting is enabled
    and the recipient does not support TLS or have a valid certificate, we drop the
    message and send a block event with \u201CTLS required but not supported\u201D
    as the description."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/settings/enforced_tls
  tags: Email,User, Settings, Enforced, Tls
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/usersettingsenforced-tls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/usersettingsenforced-tls-get-openapi.md
- name: SendGrid Patch User Settings Enforced Tls
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current Enforced TLS settings.**\n\nThe
    Enforced TLS settings specify whether or not the recipient is required to support
    TLS or have a valid certificate. See the [SMTP Ports User Guide](https://sendgrid.com/docs/Classroom/Basics/Email_Infrastructure/smtp_ports.html)
    for more information on opportunistic TLS.\n\n**Note:** If either setting is enabled
    and the recipient does not support TLS or have a valid certificate, we drop the
    message and send a block event with \u201CTLS required but not supported\u201D
    as the description."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/settings/enforced_tls
  tags: Email,User, Settings, Enforced, Tls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/usersettingsenforced-tls-patch-openapi.md
- name: SendGrid Get User Username
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve your current account username.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/username
  tags: Email,User, Username
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userusername-get-openapi.md
- name: SendGrid Put User Username
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update the username for your account.**

    Keeping your user profile up to date is important. This will help SendGrid to verify who you are as well as contact you should we need to.

    For more information about your user profile:

    * [SendGrid Account Settings](https://sendgrid.com/docs/User_Guide/Settings/account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/username
  tags: Email,User, Username
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userusername-put-openapi.md
- name: SendGrid Get User Webhooks Event Settings
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve your current event webhook
    settings.**\n\nIf an event type is marked as `true`, then the event webhook will
    include information about that event.\n\nSendGrid\u2019s Event Webhook will notify
    a URL of your choice via HTTP POST with information about events that occur as
    SendGrid processes your email.\n\nCommon uses of this data are to remove unsubscribes,
    react to spam reports, determine unengaged recipients, identify bounced email
    addresses, or create advanced analytics of your email program."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/event/settings
  tags: Email,User, Webhooks, Event, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhookseventsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhookseventsettings-get-openapi.md
- name: SendGrid Patch User Webhooks Event Settings
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update your current event webhook settings.**\n\nIf
    an event type is marked as `true`, then the event webhook will include information
    about that event.\n\nSendGrid\u2019s Event Webhook will notify a URL of your choice
    via HTTP POST with information about events that occur as SendGrid processes your
    email.\n\nCommon uses of this data are to remove unsubscribes, react to spam reports,
    determine unengaged recipients, identify bounced email addresses, or create advanced
    analytics of your email program."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/event/settings
  tags: Email,User, Webhooks, Event, Settings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhookseventsettings-patch-openapi.md
- name: SendGrid Add User Webhooks Event Test
  x-api-slug: sendgrid
  description: "**This endpoint allows you to test your event webhook by sending a
    fake event notification post to the provided URL.**\n\nSendGrid\u2019s Event Webhook
    will notify a URL of your choice via HTTP POST with information about events that
    occur as SendGrid processes your email.\n\nCommon uses of this data are to remove
    unsubscribes, react to spam reports, determine unengaged recipients, identify
    bounced email addresses, or create advanced analytics of your email program."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/event/test
  tags: Email,User, Webhooks, Event, Test
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhookseventtest-post-openapi.md
- name: SendGrid Get User Webhooks Parse Settings
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your current inbound parse settings.**

    The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/settings
  tags: Email,User, Webhooks, Parse, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettings-get-openapi.md
- name: SendGrid Add User Webhooks Parse Settings
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new inbound parse setting.**

    The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the content, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/settings
  tags: Email,User, Webhooks, Parse, Settings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettings-post-openapi.md
- name: SendGrid Delete User Webhooks Parse Settings Hostname
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a specific inbound parse setting.**

    The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/settings/{hostname}
  tags: Email,User, Webhooks, Parse, Settings, Hostname
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettingshostname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettingshostname-delete-openapi.md
- name: SendGrid Get User Webhooks Parse Settings Hostname
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific inbound parse setting.**

    The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/settings/{hostname}
  tags: Email,User, Webhooks, Parse, Settings, Hostname
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettingshostname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettingshostname-get-openapi.md
- name: SendGrid Patch User Webhooks Parse Settings Hostname
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update a specific inbound parse setting.**

    The inbound parse webhook allows you to have incoming emails parsed, extracting some or all of the contnet, and then have that content POSTed by SendGrid to a URL of your choosing. For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Webhooks/parse.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/settings/{hostname}
  tags: Email,User, Webhooks, Parse, Settings, Hostname
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsesettingshostname-patch-openapi.md
- name: SendGrid Get User Webhooks Parse Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the statistics for your Parse Webhook useage.**

    SendGrid's Inbound Parse Webhook allows you to parse the contents and attachments of incomming emails. The Parse API can then POST the parsed emails to a URL that you specify. The Inbound Parse Webhook cannot parse messages greater than 20MB in size, including all attachments.

    There are a number of pre-made integrations for the SendGrid Parse Webhook which make processing events easy. You can find these integrations in the [Library Index](https://sendgrid.com/docs/Integrate/libraries.html#-Webhook-Libraries).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//user/webhooks/parse/stats
  tags: Email,User, Webhooks, Parse, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsestats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/userwebhooksparsestats-get-openapi.md
- name: SendGrid Get Whitelabel Domains
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all domain whitelabels
    you have created.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains
  tags: Email,Whitelabel, Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomains-get-openapi.md
- name: SendGrid Add Whitelabel Domains
  x-api-slug: sendgrid
  description: "**This endpoint allows you to create a whitelabel for one of your
    domains.**\n\nIf you are creating a domain whitelabel that you would like a subuser
    to use, you have two options:\n1. Use the \"username\" parameter. This allows
    you to create a whitelabel on behalf of your subuser. This means the subuser is
    able to see and modify the created whitelabel.\n2. Use the Association workflow
    (see Associate Domain section). This allows you to assign a whitelabel created
    by the parent to a subuser. This means the subuser will default to the assigned
    whitelabel, but will not be able to see or modify that whitelabel. However, if
    the subuser creates their own whitelabel it will overwrite the assigned whitelabel.\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains
  tags: Email,Whitelabel, Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomains-post-openapi.md
- name: SendGrid Get Whitelabel Domains Default
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve the default whitelabel for
    a domain.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D or
    \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    domain | string  |The domain to find a default domain whitelabel for. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/default
  tags: Email,Whitelabel, Domains, Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdefault-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdefault-get-openapi.md
- name: SendGrid Delete Whitelabel Domains Subuser
  x-api-slug: sendgrid
  description: "**This endpoint allows you to disassociate a specific whitelabel from
    a subuser.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D or
    \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nDomain
    whitelabels can be associated with (i.e. assigned to) subusers from a parent account.
    This functionality allows subusers to send mail using their parent's whitelabels.
    To associate a whitelabel with a subuser, the parent account must first create
    the whitelabel and validate it. The the parent may then associate the whitelabel
    via the subuser management tools.\n\nFor more information on whitelabeling, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Required?  | Description  |\n|---|---|---|---|\n|
    username | string  | required  | Username for the subuser to find associated whitelabels
    for. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/subuser
  tags: Email,Whitelabel, Domains, Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainssubuser-delete-openapi.md
- name: SendGrid Get Whitelabel Domains Subuser
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all of the whitelabels that
    have been assigned to a specific subuser.**\n\nA domain whitelabel allows you
    to remove the \u201Cvia\u201D or \u201Csent on behalf of\u201D message that your
    recipients see when they read your emails. Whitelabeling a domain allows you to
    replace sendgrid.net with your personal sending domain. You will be required to
    create a subdomain so that SendGrid can generate the DNS records which you must
    give to your host provider. If you choose to use Automated Security, SendGrid
    will provide you with 3 CNAME records. If you turn Automated Security off, you
    will be given 2 TXT records and 1 MX record.\n\nDomain whitelabels can be associated
    with (i.e. assigned to) subusers from a parent account. This functionality allows
    subusers to send mail using their parent's whitelabels. To associate a whitelabel
    with a subuser, the parent account must first create the whitelabel and validate
    it. The the parent may then associate the whitelabel via the subuser management
    tools.\n\nFor more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Description  |\n|---|---|---|\n| username
    | string  | Username of the subuser to find associated whitelabels for. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/subuser
  tags: Email,Whitelabel, Domains, Subuser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainssubuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainssubuser-get-openapi.md
- name: SendGrid Delete Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete a domain whitelabel.**\n\nA domain
    whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf of\u201D
    message that your recipients see when they read your emails. Whitelabeling a domain
    allows you to replace sendgrid.net with your personal sending domain. You will
    be required to create a subdomain so that SendGrid can generate the DNS records
    which you must give to your host provider. If you choose to use Automated Security,
    SendGrid will provide you with 3 CNAME records. If you turn Automated Security
    off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdomain-id-delete-openapi.md
- name: SendGrid Get Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdomain-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdomain-id-get-openapi.md
- name: SendGrid Patch Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update the settings for a domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdomain-id-patch-openapi.md
- name: SendGrid Add Whitelabel Domains Domain  Subuser
  x-api-slug: sendgrid
  description: "**This endpoint allows you to associate a specific domain whitelabel
    with a subuser.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nDomain
    whitelabels can be associated with (i.e. assigned to) subusers from a parent account.
    This functionality allows subusers to send mail using their parent's whitelabels.
    To associate a whitelabel with a subuser, the parent account must first create
    the whitelabel and validate it. The the parent may then associate the whitelabel
    via the subuser management tools.\n\nFor more information on whitelabeling, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    domain_id | integer   | ID of the domain whitelabel to associate with the subuser.
    |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}/subuser
  tags: Email,Whitelabel, Domains, Domain, , Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsdomain-idsubuser-post-openapi.md
- name: SendGrid Add Whitelabel Domains  Ips
  x-api-slug: sendgrid
  description: "**This endpoint allows you to add an IP address to a domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  |  Description  |\n|---|---|---|\n|
    id | integer  | ID of the domain to which you are adding an IP |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/ips
  tags: Email,Whitelabel, Domains, , Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsidips-post-openapi.md
- name: SendGrid Delete Whitelabel Domains  Ips Ip
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove a domain's IP address from that
    domain's whitelabel.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Description  |\n|---|---|---|\n| id
    | integer  | ID of the domain whitelabel to delete the IP from. |\n| ip | string
    | IP to remove from the domain whitelabel. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/ips/{ip}
  tags: Email,Whitelabel, Domains, , Ips, Ip
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsidipsip-delete-openapi.md
- name: SendGrid Add Whitelabel Domains  Valate
  x-api-slug: sendgrid
  description: "**This endpoint allows you to validate a domain whitelabel. If it
    fails, it will return an error message describing why the whitelabel could not
    be validated.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    id | integer  |ID of the domain whitelabel to validate. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/validate
  tags: Email,Whitelabel, Domains, , Valate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabeldomainsidvalidate-post-openapi.md
- name: SendGrid Get Whitelabel Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of the IP whitelabels that have been createdy by this account.**

    You may include a search key by using the "ip" parameter. This enables you to perform a prefix search for a given IP segment (e.g. "192.").

    A IP whitelabel consists of a subdomain and domain that will be used to generate a reverse DNS record for a given IP. Once SendGrid has verified that the appropriate A record for the IP has been created, the appropriate reverse DNS record for the IP is generated.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/ips
  tags: Email,Whitelabel, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabelips-get-openapi.md
- name: SendGrid Add Whitelabel Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create an IP whitelabel.**

    When creating an IP whitelable, you should use the same subdomain that you used when you created a domain whitelabel.

    A IP whitelabel consists of a subdomain and domain that will be used to generate a reverse DNS record for a given IP. Once SendGrid has verified that the appropriate A record for the IP has been created, the appropriate reverse DNS record for the IP is generated.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/ips
  tags: Email,Whitelabel, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabelips-post-openapi.md
- name: SendGrid Delete Whitelabel Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete an IP whitelabel.**

    A IP whitelabel consists of a subdomain and domain that will be used to generate a reverse DNS record for a given IP. Once SendGrid has verified that the appropriate A record for the IP has been created, the appropriate reverse DNS record for the IP is generated.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/ips/{id}
  tags: Email,Whitelabel, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabelipsid-delete-openapi.md
- name: SendGrid Get Whitelabel Ips
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve an IP whitelabel.**

    A IP whitelabel consists of a subdomain and domain that will be used to generate a reverse DNS record for a given IP. Once SendGrid has verified that the appropriate A record for the IP has been created, the appropriate reverse DNS record for the IP is generated.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/ips/{id}
  tags: Email,Whitelabel, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabelipsid-get-openapi.md
- name: SendGrid Add Whitelabel Ips  Valate
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to validate an IP whitelabel.**

    A IP whitelabel consists of a subdomain and domain that will be used to generate a reverse DNS record for a given IP. Once SendGrid has verified that the appropriate A record for the IP has been created, the appropriate reverse DNS record for the IP is generated.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/ips.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/ips/{id}/validate
  tags: Email,Whitelabel, Ips, , Valate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabelipsidvalidate-post-openapi.md
- name: SendGrid Get Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all link whitelabels.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links
  tags: Email,Whitelabel, Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinks-get-openapi.md
- name: SendGrid Add Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to create a new link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinks-post-openapi.md
- name: SendGrid Get Whitelabel Links Default
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the default link whitelabel.**

    Default link whitelabel is the actual link whitelabel to be used when sending messages. If there are multiple link whitelabels, the default is determined by the following order:
    <ul>
      <li>Validated link whitelabels marked as "default"</li>
      <li>Legacy link whitelabels (migrated from the whitelabel wizard)</li>
      <li>Default SendGrid link whitelabel (i.e. 100.ct.sendgrid.net)</li>
    </ul>

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/default
  tags: Email,Whitelabel, Links, Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksdefault-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksdefault-get-openapi.md
- name: SendGrid Delete Whitelabel Links Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to disassociate a link whitelabel from a subuser.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/subuser
  tags: Email,Whitelabel, Links, Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinkssubuser-delete-openapi.md
- name: SendGrid Get Whitelabel Links Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the associated link whitelabel for a subuser.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/subuser
  tags: Email,Whitelabel, Links, Subuser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinkssubuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinkssubuser-get-openapi.md
- name: SendGrid Delete Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksid-delete-openapi.md
- name: SendGrid Get Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a specific link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksid-get-openapi.md
- name: SendGrid Patch Whitelabel Links
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update a specific link whitelabel. You can use this endpoint to change a link whitelabel's default status.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}
  tags: Email,Whitelabel, Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksid-patch-openapi.md
- name: SendGrid Add Whitelabel Links  Valate
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to validate a link whitelabel.**

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{id}/validate
  tags: Email,Whitelabel, Links, , Valate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinksidvalidate-post-openapi.md
- name: SendGrid Add Whitelabel Links Link  Subuser
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to associate a link whitelabel with a subuser account.**

    Link whitelables can be associated with subusers from the parent account. This functionality allows
    subusers to send mail using their parent's linke whitelabels. To associate a link whitelabel, the parent account
    must first create a whitelabel and validate it. The parent may then associate that whitelabel with a subuser via the API or the Subuser Management page in the user interface.

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/links/{link_id}/subuser
  tags: Email,Whitelabel, Links, Link, , Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/whitelabellinkslink-idsubuser-post-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Mail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/mail/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---