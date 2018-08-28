---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Asm Groups Group  Suppressions Email
  description: |-
    **This endpoint allows you to remove a suppressed email address from the given suppression group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /access_settings/activity:
    get:
      summary: Get Access Settings Activity
      description: |-
        **This endpoint allows you to retrieve a list of all of the IP addresses that recently attempted to access your account either through the User Interface or the API.**

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.activity.get
      x-api-path-slug: access-settingsactivity-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of IPs to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Activity
  /access_settings/whitelist:
    delete:
      summary: Delete Access Settings Whitelist
      description: |-
        **This endpoint allows you to remove one or more IPs from your IP whitelist.**

        You can remove one IP at a time, or you can remove multiple IP addresses.

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.whitelist.delete
      x-api-path-slug: access-settingswhitelist-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Whitelist
    get:
      summary: Get Access Settings Whitelist
      description: |-
        **This endpoint allows you to retrieve a list of IP addresses that are currently whitelisted.**

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.whitelist.get
      x-api-path-slug: access-settingswhitelist-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Whitelist
    post:
      summary: Add Access Settings Whitelist
      description: |-
        **This endpoint allows you to add one or more IP addresses to your IP whitelist.**

        When adding an IP to your whitelist, include the IP address in an array. You can whitelist one IP at a time, or you can whitelist multiple IPs at once.

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.whitelist.post
      x-api-path-slug: access-settingswhitelist-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Whitelist
  /access_settings/whitelist/{rule_id}:
    delete:
      summary: Delete Access Settings Whitelist Rule
      description: |-
        **This endpoint allows you to remove a specific IP address from your IP whitelist.**

        When removing a specific IP address from your whitelist, you must include the ID in your call.

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.whitelist.rule_id.delete
      x-api-path-slug: access-settingswhitelistrule-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Whitelist
      - Rule
    get:
      summary: Get Access Settings Whitelist Rule
      description: |-
        **This endpoint allows you to retreive a specific IP address that has been whitelisted.**

        You must include the ID for the specific IP address you want to retrieve in your call.

        IP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.

        For more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).
      operationId: access_settings.whitelist.rule_id.get
      x-api-path-slug: access-settingswhitelistrule-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Access
      - Settings
      - Whitelist
      - Rule
  /alerts:
    get:
      summary: Get Alerts
      description: "**This endpoint allows you to retieve all of your alerts.**\n\nAlerts
        allow you to specify an email address to receive notifications regarding your
        email usage or statistics. \n* Usage alerts allow you to set the threshold
        at which an alert will be sent.\n* Stats notifications allow you to set how
        frequently you would like to receive email statistics reports. For example,
        \"daily\", \"weekly\", or \"monthly\".\n\nFor more information about alerts,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: GET_alerts
      x-api-path-slug: alerts-get
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
    post:
      summary: Add Alerts
      description: |-
        **This endpoint allows you to create a new alert.**

        Alerts allow you to specify an email address to receive notifications regarding your email usage or statistics. There are two types of alerts that can be created with this endpoint:

        * `usage_limit` allows you to set the threshold at which an alert will be sent.
        * `stats_notification` allows you to set how frequently you would like to receive email statistics reports. For example, "daily", "weekly", or "monthly".

        For more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html).
      operationId: POST_alerts
      x-api-path-slug: alerts-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: on-behalf-of
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
  /alerts/{alert_id}:
    delete:
      summary: Delete Alerts Alert
      description: "**This endpoint allows you to delete an alert.**\n\nAlerts allow
        you to specify an email address to receive notifications regarding your email
        usage or statistics. \n* Usage alerts allow you to set the threshold at which
        an alert will be sent.\n* Stats notifications allow you to set how frequently
        you would like to receive email statistics reports. For example, \"daily\",
        \"weekly\", or \"monthly\".\n\nFor more information about alerts, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.delete
      x-api-path-slug: alertsalert-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
    get:
      summary: Get Alerts Alert
      description: "**This endpoint allows you to retrieve a specific alert.**\n\nAlerts
        allow you to specify an email address to receive notifications regarding your
        email usage or statistics. \n* Usage alerts allow you to set the threshold
        at which an alert will be sent.\n* Stats notifications allow you to set how
        frequently you would like to receive email statistics reports. For example,
        \"daily\", \"weekly\", or \"monthly\".\n\nFor more information about alerts,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.get
      x-api-path-slug: alertsalert-id-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
    patch:
      summary: Patch Alerts Alert
      description: "**This endpoint allows you to update an alert.**\n\nAlerts allow
        you to specify an email address to receive notifications regarding your email
        usage or statistics. \n* Usage alerts allow you to set the threshold at which
        an alert will be sent.\n* Stats notifications allow you to set how frequently
        you would like to receive email statistics reports. For example, \"daily\",
        \"weekly\", or \"monthly\".\n\nFor more information about alerts, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.patch
      x-api-path-slug: alertsalert-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
  /api_keys:
    get:
      summary: Get Api Keys
      description: |-
        **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: GET_api_keys
      x-api-path-slug: api-keys-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
    post:
      summary: Add Api Keys
      description: |-
        **This endpoint allows you to create a new random API Key for the user.**

        A JSON request body containing a "name" property is required. If number of maximum keys is reached, HTTP 403 will be returned.

        There is a limit of 100 API Keys on your account.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        See the [API Key Permissions List](https://sendgrid.com/docs/API_Reference/Web_API_v3/API_Keys/api_key_permissions_list.html) for a list of all available scopes.
      operationId: api_keys.post
      x-api-path-slug: api-keys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
  /api_keys/{api_key_id}:
    delete:
      summary: Delete Api Keys Api Key
      description: |-
        **This endpoint allows you to revoke an existing API Key**

        Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are deleting.|
      operationId: api_keys.api_key_id.delete
      x-api-path-slug: api-keysapi-key-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
    get:
      summary: Get Api Keys Api Key
      description: |-
        **This endpoint allows you to retrieve a single api key.**

        If the API Key ID does not exist an HTTP 404 will be returned.
      operationId: api_keys.api_key_id.get
      x-api-path-slug: api-keysapi-key-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
    patch:
      summary: Patch Api Keys Api Key
      description: |-
        **This endpoint allows you to update the name of an existing API Key.**

        A JSON request body with a "name" property is required.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are updating.|
      operationId: api_keys.api_key_id.patch
      x-api-path-slug: api-keysapi-key-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
    put:
      summary: Put Api Keys Api Key
      description: |-
        **This endpoint allows you to update the name and scopes of a given API key.**

        A JSON request body with a "name" property is required.
        Most provide the list of all the scopes an api key should have.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: api_keys.api_key_id.put
      x-api-path-slug: api-keysapi-key-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
  /asm/groups:
    get:
      summary: Get Asm Groups
      description: |-
        **This endpoint allows you to retrieve information about multiple suppression groups.**

        This endpoint will return information for each group ID that you include in your request. To add a group ID to your request, simply append `&id=` followed by the group ID.

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).

        Suppression groups, or [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html), allow you to label a category of content that you regularly send. This gives your recipients the ability to opt out of a specific set of your email. For example, you might define a group for your transactional email, and one for your marketing email so that your users can continue recieving your transactional email witout having to receive your marketing content.
      operationId: asm.groups.get
      x-api-path-slug: asmgroups-get
      parameters:
      - in: query
        name: id
        description: The ID of a suppression group that you want to retrieve information
          for
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
    post:
      summary: Add Asm Groups
      description: |-
        **This endpoint allows you to create a new suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.post
      x-api-path-slug: asmgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
  /asm/groups/{group_id}:
    delete:
      summary: Delete Asm Groups Group
      description: |-
        **This endpoint allows you to delete a suppression group.**

        You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.delete
      x-api-path-slug: asmgroupsgroup-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
    get:
      summary: Get Asm Groups Group
      description: |-
        **This endpoint allows you to retrieve a single suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.get
      x-api-path-slug: asmgroupsgroup-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
    patch:
      summary: Patch Asm Groups Group
      description: |-
        **This endpoint allows you to update or change a suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.patch
      x-api-path-slug: asmgroupsgroup-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
  /asm/groups/{group_id}/suppressions:
    get:
      summary: Get Asm Groups Group  Suppressions
      description: |-
        **This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**

        Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
      operationId: asm.groups.group_id.suppressions.get
      x-api-path-slug: asmgroupsgroup-idsuppressions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
      - ""
      - Suppressions
    post:
      summary: Add Asm Groups Group  Suppressions
      description: |-
        **This endpoint allows you to add email addresses to an unsubscribe group.**

        If you attempt to add suppressions to a group that has been deleted or does not exist, the suppressions will be added to the global suppressions list.

        Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
      operationId: asm.groups.group_id.suppressions.post
      x-api-path-slug: asmgroupsgroup-idsuppressions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
      - ""
      - Suppressions
  /asm/groups/{group_id}/suppressions/search:
    post:
      summary: Add Asm Groups Group  Suppressions Search
      description: |-
        **This endpoint allows you to search a suppression group for multiple suppressions.**

        When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
      operationId: asm.groups.group_id.suppressions.search.post
      x-api-path-slug: asmgroupsgroup-idsuppressionssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
      - ""
      - Suppressions
      - Search
  /asm/groups/{group_id}/suppressions/{email}:
    delete:
      summary: Delete Asm Groups Group  Suppressions Email
      description: |-
        **This endpoint allows you to remove a suppressed email address from the given suppression group.**

        Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
      operationId: asm.groups.group_id.suppressions.email.delete
      x-api-path-slug: asmgroupsgroup-idsuppressionsemail-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
      - ""
      - Suppressions
      - Email
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