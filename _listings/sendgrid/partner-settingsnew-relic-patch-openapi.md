---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Patch Partner Settings New Relic
  description: |-
    **This endpoint allows you to update or change your New Relic partner settings.**

    Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

    By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
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
  /asm/suppressions:
    get:
      summary: Get Asm Suppressions
      description: |-
        **This endpoint allows you to retrieve a list of all suppressions.**

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
      operationId: asm.suppressions.get
      x-api-path-slug: asmsuppressions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Suppressions
  /asm/suppressions/global:
    post:
      summary: Add Asm Suppressions Global
      description: |-
        **This endpoint allows you to add one or more email addresses to the global suppressions group.**

        A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
      operationId: asm.suppressions.global.post
      x-api-path-slug: asmsuppressionsglobal-post
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
      - Suppressions
      - Global
  /asm/suppressions/global/{email}:
    delete:
      summary: Delete Asm Suppressions Global Email
      description: |-
        **This endpoint allows you to remove an email address from the global suppressions group.**

        A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
      operationId: asm.suppressions.global.email.delete
      x-api-path-slug: asmsuppressionsglobalemail-delete
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
      - Suppressions
      - Global
      - Email
    get:
      summary: Get Asm Suppressions Global Email
      description: |-
        **This endpoint allows you to retrieve a global suppression. You can also use this endpoint to confirm if an email address is already globally suppresed.**

        If the email address you include in the URL path parameter `{email}` is alreayd globally suppressed, the response will include that email address. If the address you enter for `{email}` is not globally suppressed, an empty JSON object `{}` will be returned.

        A global suppression (or global unsubscribe) is an email address of a recipient who does not want to receive any of your messages. A globally suppressed recipient will be removed from any email you send. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/global_unsubscribes.html).
      operationId: asm.suppressions.global.email.get
      x-api-path-slug: asmsuppressionsglobalemail-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Suppressions
      - Global
      - Email
  /asm/suppressions/{email}:
    get:
      summary: Get Asm Suppressions Email
      description: |-
        **This endpoint returns the list of all groups that the given email address has been unsubscribed from.**

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
      operationId: asm.suppressions.email.get
      x-api-path-slug: asmsuppressionsemail-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Suppressions
      - Email
  /browsers/stats:
    get:
      summary: Get Browsers Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by browser type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: browsers.stats.get
      x-api-path-slug: browsersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the stats
      - in: query
        name: browsers
        description: The browsers to get statistics for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Browsers
      - Stats
  /campaigns:
    get:
      summary: Get Campaigns
      description: |-
        **This endpoint allows you to retrieve a list of all of your campaigns.**

        Returns campaigns in reverse order they were created (newest first).

        Returns an empty array if no campaigns exist.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: GET_campaigns
      x-api-path-slug: campaigns-get
      parameters:
      - in: query
        name: limit
        description: The number of results you would like to receive at a time
      - in: query
        name: offset
        description: The index of the first campaign to return, where 0 is the first
          campaign
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
    post:
      summary: Add Campaigns
      description: |-
        **This endpoint allows you to create a campaign.**

        Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

        Note: In order to send or schedule the campaign, you will be required to provide a subject, sender ID, content (we suggest both html and plain text), and at least one list or segment ID. This information is not required when you create a campaign.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: POST_campaigns
      x-api-path-slug: campaigns-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
  /campaigns/{campaign_id}:
    delete:
      summary: Delete Campaigns Campaign
      description: |-
        **This endpoint allows you to delete a specific campaign.**

        Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.delete
      x-api-path-slug: campaignscampaign-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
    get:
      summary: Get Campaigns Campaign
      description: |-
        **This endpoint allows you to retrieve a specific campaign.**

        Our Marketing Campaigns API lets you create, manage, send, and schedule campaigns.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.get
      x-api-path-slug: campaignscampaign-id-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
    patch:
      summary: Patch Campaigns Campaign
      description: |-
        Update a campaign. This is especially useful if you only set up the campaign using POST /campaigns, but didn't set many of the parameters.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.patch
      x-api-path-slug: campaignscampaign-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
  /campaigns/{campaign_id}/schedules:
    delete:
      summary: Delete Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to unschedule a campaign that has already been scheduled to be sent.**

        A successful unschedule will return a 204.
        If the specified campaign is in the process of being sent, the only option is to cancel (a different method).

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.delete
      x-api-path-slug: campaignscampaign-idschedules-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    get:
      summary: Get Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to retrieve the date and time that the given campaign has been scheduled to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.get
      x-api-path-slug: campaignscampaign-idschedules-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    patch:
      summary: Patch Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows to you change the scheduled time and date for a campaign to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.patch
      x-api-path-slug: campaignscampaign-idschedules-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
    post:
      summary: Add Campaigns Campaign  Schedules
      description: |-
        **This endpoint allows you to schedule a specific date and time for your campaign to be sent.**

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.post
      x-api-path-slug: campaignscampaign-idschedules-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
  /campaigns/{campaign_id}/schedules/now:
    post:
      summary: Add Campaigns Campaign  Schedules Now
      description: |-
        **This endpoint allows you to immediately send a campaign at the time you make the API call.**

        Normally a POST would have a request body, but since this endpoint is telling us to send a resource that is already created, a request body is not needed.

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.now.post
      x-api-path-slug: campaignscampaign-idschedulesnow-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
      - Now
  /campaigns/{campaign_id}/schedules/test:
    post:
      summary: Add Campaigns Campaign  Schedules Test
      description: |-
        **This endpoint allows you to send a test campaign.**

        To send to multiple addresses, use an array for the JSON "to" value ["one@address","two@address"]

        For more information:

        * [User Guide > Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
      operationId: campaigns.campaign_id.schedules.test.post
      x-api-path-slug: campaignscampaign-idschedulestest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Campaigns
      - Campaign
      - ""
      - Schedules
      - Test
  /categories:
    get:
      summary: Get Categories
      description: "**This endpoint allows you to retrieve a list of all of your categories.**\n\nCategories
        can help organize your email analytics by enabling you to \u201Ctag\u201D
        emails by type or broad topic. You can define your own custom categories.
        For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html)."
      operationId: GET_categories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: category
        description: Allows you to perform a prefix search on this particular category
      - in: query
        name: limit
        description: The number of categories to display per page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The point in the list that you would like to begin displaying
          results
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
  /categories/stats:
    get:
      summary: Get Categories Stats
      description: |-
        **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.get
      x-api-path-slug: categoriesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: categories
        description: The individual categories that you want to retrieve statistics
          for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
  /categories/stats/sums:
    get:
      summary: Get Categories Stats Sums
      description: |-
        **This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.sums.get
      x-api-path-slug: categoriesstatssums-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: Limits the number of results returned
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The point in the list to begin retrieving results
      - in: query
        name: sort_by_direction
        description: The direction you want to sort
      - in: query
        name: sort_by_metric
        description: The metric that you want to sort by
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
      - Sums
  /clients/stats:
    get:
      summary: Get Clients Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by client type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: clients.stats.get
      x-api-path-slug: clientsstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: No Name
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Clients
      - Stats
  /clients/{client_type}/stats:
    get:
      summary: Get Clients Client Type Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by a specific client type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        ## Available Client Types
        - phone
        - tablet
        - webmail
        - desktop

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: clients.client_type.stats.get
      x-api-path-slug: clientsclient-typestats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: No Name
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Clients
      - Client
      - Type
      - Stats
  /contactdb/custom_fields:
    get:
      summary: Get Contactdb Custom Fields
      description: "**This endpoint allows you to retrieve all custom fields.** \n\nThe
        contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)."
      operationId: contactdb.custom_fields.get
      x-api-path-slug: contactdbcustom-fields-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Custom
      - Fields
    post:
      summary: Add Contactdb Custom Fields
      description: |-
        **This endpoint allows you to create a custom field.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.custom_fields.post
      x-api-path-slug: contactdbcustom-fields-post
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
      - Contactdb
      - Custom
      - Fields
  /contactdb/custom_fields/{custom_field_id}:
    delete:
      summary: Delete Contactdb Custom Fields Custom Field
      description: |-
        **This endpoint allows you to delete a custom field by ID.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.custom_fields.custom_field_id.delete
      x-api-path-slug: contactdbcustom-fieldscustom-field-id-delete
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
      - Contactdb
      - Custom
      - Fields
      - Custom
      - Field
    get:
      summary: Get Contactdb Custom Fields Custom Field
      description: |-
        **This endpoint allows you to retrieve a custom field by ID.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.custom_fields.custom_field_id.get
      x-api-path-slug: contactdbcustom-fieldscustom-field-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Custom
      - Fields
      - Custom
      - Field
  /contactdb/lists:
    delete:
      summary: Delete Contactdb Lists
      description: |-
        **This endpoint allows you to delete multiple recipient lists.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.delete
      x-api-path-slug: contactdblists-delete
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
      - Contactdb
      - Lists
    get:
      summary: Get Contactdb Lists
      description: |-
        **This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.get
      x-api-path-slug: contactdblists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
    post:
      summary: Add Contactdb Lists
      description: |-
        **This endpoint allows you to create a list for your recipients.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.post
      x-api-path-slug: contactdblists-post
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
      - Contactdb
      - Lists
  /contactdb/lists/{list_id}:
    delete:
      summary: Delete Contactdb Lists List
      description: |-
        **This endpoint allows you to delete a specific recipient list with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.delete
      x-api-path-slug: contactdblistslist-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: delete_contacts
        description: Adds the ability to delete all contacts on the list in addition
          to deleting the list
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
    get:
      summary: Get Contactdb Lists List
      description: |-
        This endpoint allows you to retrieve a single recipient list.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.get
      x-api-path-slug: contactdblistslist-id-get
      parameters:
      - in: query
        name: list_id
        description: The ID of the list to retrieve
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
    patch:
      summary: Patch Contactdb Lists List
      description: |-
        **This endpoint allows you to update the name of one of your recipient lists.**


        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.patch
      x-api-path-slug: contactdblistslist-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: list_id
        description: The ID of the list you are updating
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
  /contactdb/lists/{list_id}/recipients:
    get:
      summary: Get Contactdb Lists List  Recipients
      description: "**This endpoint allows you to retrieve all recipients on the list
        with the given ID.** \n\nThe Contacts API helps you manage your [Marketing
        Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
        recipients."
      operationId: contactdb.lists.list_id.recipients.get
      x-api-path-slug: contactdblistslist-idrecipients-get
      parameters:
      - in: query
        name: list_id
        description: The ID of the list whose recipients you are requesting
      - in: query
        name: No Name
      - in: query
        name: page
        description: Page index of first recipient to return (must be a positive integer)
      - in: query
        name: page_size
        description: Number of recipients to return at a time (must be a positive
          integer between 1 and 1000)
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
    post:
      summary: Add Contactdb Lists List  Recipients
      description: |-
        **This endpoint allows you to add multiple recipients to a list.**

        Adds existing recipients to a list, passing in the recipient IDs to add. Recipient IDs should be passed exactly as they are returned from recipient endpoints.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.post
      x-api-path-slug: contactdblistslist-idrecipients-post
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
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
  /contactdb/lists/{list_id}/recipients/{recipient_id}:
    delete:
      summary: Delete Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to delete a single recipient from a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.delete
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: list_id
        description: The ID of the list you are taking this recipient away from
      - in: query
        name: No Name
      - in: query
        name: recipient_id
        description: The ID of the recipient to take off the list
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
      - Recipient
    post:
      summary: Add Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to add a single recipient to a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.post
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-post
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
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
      - Recipient
  /contactdb/recipients:
    delete:
      summary: Delete Contactdb Recipients
      description: |-
        **This endpoint allows you to deletes one or more recipients.**

        The body of an API call to this endpoint must include an array of recipient IDs of the recipients you want to delete.

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.delete
      x-api-path-slug: contactdbrecipients-delete
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
      - Contactdb
      - Recipients
    get:
      summary: Get Contactdb Recipients
      description: |-
        **This endpoint allows you to retrieve all of your Marketing Campaigns recipients.**

        Batch deletion of a page makes it possible to receive an empty page of recipients before reaching the end of
        the list of recipients. To avoid this issue; iterate over pages until a 404 is retrieved.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.get
      x-api-path-slug: contactdbrecipients-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: page
        description: Page index of first recipients to return (must be a positive
          integer)
      - in: query
        name: page_size
        description: Number of recipients to return at a time (must be a positive
          integer between 1 and 1000)
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
    patch:
      summary: Patch Contactdb Recipients
      description: |-
        **This endpoint allows you to update one or more recipients.**

        The body of an API call to this endpoint must include an array of one or more recipient objects.

        It is of note that you can add custom field data as parameters on recipient objects. We have provided an example using some of the default custom fields SendGrid provides.

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.patch
      x-api-path-slug: contactdbrecipients-patch
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
      - Contactdb
      - Recipients
    post:
      summary: Add Contactdb Recipients
      description: |-
        **This endpoint allows you to add a Marketing Campaigns recipient.**

        You can add custom field data as a parameter on this endpoint. We have provided an example using some of the default custom fields SendGrid provides.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.post
      x-api-path-slug: contactdbrecipients-post
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
      - Contactdb
      - Recipients
  /contactdb/recipients/billable_count:
    get:
      summary: Get Contactdb Recipients Billable Count
      description: |-
        **This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for.**

        You are billed for marketing campaigns based on the highest number of recipients you have had in your account at one time. This endpoint will allow you to know the current billable count value.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.billable_count.get
      x-api-path-slug: contactdbrecipientsbillable-count-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Billable
      - Count
  /contactdb/recipients/count:
    get:
      summary: Get Contactdb Recipients Count
      description: |-
        **This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.count.get
      x-api-path-slug: contactdbrecipientscount-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Count
  /contactdb/recipients/search:
    get:
      summary: Get Contactdb Recipients Search
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
      operationId: contactdb.recipients.search.get
      x-api-path-slug: contactdbrecipientssearch-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: '{field_name}'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Search
  /contactdb/recipients/{recipient_id}:
    delete:
      summary: Delete Contactdb Recipients Recipient
      description: |-
        **This endpoint allows you to delete a single recipient with the given ID from your contact database.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.recipient_id.delete
      x-api-path-slug: contactdbrecipientsrecipient-id-delete
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
      - Contactdb
      - Recipients
      - Recipient
    get:
      summary: Get Contactdb Recipients Recipient
      description: |-
        **This endpoint allows you to retrieve a single recipient by ID from your contact database.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.recipient_id.get
      x-api-path-slug: contactdbrecipientsrecipient-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Recipient
  /contactdb/recipients/{recipient_id}/lists:
    get:
      summary: Get Contactdb Recipients Recipient  Lists
      description: |-
        **This endpoint allows you to retrieve the lists that a given recipient belongs to.**

        Each recipient can be on many lists. This endpoint gives you all of the lists that any one recipient has been added to.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.recipient_id.lists.get
      x-api-path-slug: contactdbrecipientsrecipient-idlists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Recipient
      - ""
      - Lists
  /contactdb/reserved_fields:
    get:
      summary: Get Contactdb Reserved Fields
      description: |-
        **This endpoint allows you to list all fields that are reserved and can't be used for custom field names.**

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.reserved_fields.get
      x-api-path-slug: contactdbreserved-fields-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Reserved
      - Fields
  /contactdb/segments:
    get:
      summary: Get Contactdb Segments
      description: |-
        **This endpoint allows you to retrieve all of your segments.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.get
      x-api-path-slug: contactdbsegments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
    post:
      summary: Add Contactdb Segments
      description: "**This endpoint allows you to create a segment.**\n\nAll recipients
        in your contactdb will be added or removed automatically depending on whether
        they match the criteria for this segment.\n\nList Id:\n\n* Send this to segment
        from an existing list\n* Don't send this in order to segment from your entire
        contactdb.\n\nValid operators for create and update depend on the type of
        the field you are segmenting: \n\n* **Dates:** \"eq\", \"ne\", \"lt\" (before),
        \"gt\" (after) \n* **Text:** \"contains\", \"eq\" (is - matches the full field),
        \"ne\" (is not - matches any field where the entire field is not the condition
        value) \n* **Numbers:** \"eq\", \"lt\", \"gt\" \n* **Email Clicks and Opens:**
        \"eq\" (opened), \"ne\" (not opened) \n\nSegment conditions using \"eq\" or
        \"ne\" for email clicks and opens should provide a \"field\" of either *clicks.campaign_identifier*
        or *opens.campaign_identifier*. The condition value should be a string containing
        the id of a completed campaign. \n\nSegments may contain multiple condtions,
        joined by an \"and\" or \"or\" in the \"and_or\" field. The first condition
        in the conditions list must have an empty \"and_or\", and subsequent conditions
        must all specify an \"and_or\".\n\nThe Contacts API helps you manage your
        [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
        recipients.\n\nFor more information about segments in Marketing Campaigns,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment)."
      operationId: contactdb.segments.post
      x-api-path-slug: contactdbsegments-post
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
      - Contactdb
      - Segments
  /contactdb/segments/{segment_id}:
    delete:
      summary: Delete Contactdb Segments Segment
      description: |-
        **This endpoint allows you to delete a segment from your recipients database.**

        You also have the option to delete all the contacts from your Marketing Campaigns recipient database who were in this segment.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.delete
      x-api-path-slug: contactdbsegmentssegment-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: delete_contacts
        description: True to delete all contacts matching the segment in addition
          to deleting the segment
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
    get:
      summary: Get Contactdb Segments Segment
      description: |-
        **This endpoint allows you to retrieve a single segment with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.get
      x-api-path-slug: contactdbsegmentssegment-id-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: segment_id
        description: The ID of the segment you want to request
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
    patch:
      summary: Patch Contactdb Segments Segment
      description: |-
        **This endpoint allows you to update a segment.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.patch
      x-api-path-slug: contactdbsegmentssegment-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: segment_id
        description: The ID of the segment you are updating
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
  /contactdb/segments/{segment_id}/recipients:
    get:
      summary: Get Contactdb Segments Segment  Recipients
      description: |-
        **This endpoint allows you to retrieve all of the recipients in a segment with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.recipients.get
      x-api-path-slug: contactdbsegmentssegment-idrecipients-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: page
      - in: query
        name: page_size
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
      - ""
      - Recipients
  /contactdb/status:
    get:
      summary: Get Contactdb Status
      description: ""
      operationId: contactdb.status.get
      x-api-path-slug: contactdbstatus-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Status
  /devices/stats:
    get:
      summary: Get Devices Stats
      description: "**This endpoint allows you to retrieve your email statistics segmented
        by the device type.**\n\n**We only store up to 7 days of email activity in
        our database.** By default, 500 items will be returned per request via the
        Advanced Stats API endpoints.\n\n## Available Device Types\n| **Device** |
        **Description** | **Example** |\n|---|---|---|\n| Desktop | Email software
        on desktop computer. | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail
        |\tA web-based email client. | I.E., Yahoo, Google, AOL, or Outlook.com. |\n|
        Phone | A smart phone. | iPhone, Android, Blackberry, etc.\n| Tablet | A tablet
        computer. | iPad, android based tablet, etc. |\n| Other | An unrecognized
        device. |\n\nAdvanced Stats provide a more in-depth view of your email statistics
        and the actions taken by your recipients. You can segment these statistics
        by geographic location, device type, client type, browser, and mailbox provider.
        For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html)."
      operationId: devices.stats.get
      x-api-path-slug: devicesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: How many results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: How many results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Devices
      - Stats
  /geo/stats:
    get:
      summary: Get Geo Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by country and state/province.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: geo.stats.get
      x-api-path-slug: geostats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How you would like the statistics to be grouped
      - in: query
        name: country
        description: The country you would like to see statistics for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: How many results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: How many results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Geo
      - Stats
  /ips:
    get:
      summary: Get Ips
      description: |-
        **This endpoint allows you to retrieve a list of all assigned and unassigned IPs.**

        Response includes warm up status, pools, assigned subusers, and whitelabel info. The start_date field corresponds to when warmup started for that IP.

        A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
      operationId: GET_ips
      x-api-path-slug: ips-get
      parameters:
      - in: query
        name: exclude_whitelabels
        description: Should we exclude whitelabels?
      - in: query
        name: ip
        description: The IP address to get
      - in: query
        name: limit
        description: The number of IPs you want returned at the same time
      - in: query
        name: offset
        description: The offset for the number of IPs that you are requesting
      - in: query
        name: sort_by_direction
        description: The direction to sort the results
      - in: query
        name: subuser
        description: The subuser you are requesting for
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
    post:
      summary: Add Ips
      description: This endpoint is for adding a(n) IP Address(es) to your account.
      operationId: POST_ips
      x-api-path-slug: ips-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
  /ips/assigned:
    get:
      summary: Get Ips Assigned
      description: |-
        **This endpoint allows you to retrieve only assigned IP addresses.**

        A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
      operationId: ips.assigned.get
      x-api-path-slug: ipsassigned-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Assigned
  /ips/pools:
    get:
      summary: Get Ips Pools
      description: |-
        **This endpoint allows you to retreive all of your IP pools.**

        IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

        IP pools can only be used with whitelabeled IP addresses.

        If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
      operationId: ips.pools.get
      x-api-path-slug: ipspools-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
    post:
      summary: Add Ips Pools
      description: |-
        **This endpoint allows you to create an IP pool.**

        **Each user can create up to 10 different IP pools.**

        IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

        IP pools can only be used with whitelabeled IP addresses.

        If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
      operationId: ips.pools.post
      x-api-path-slug: ipspools-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
  /ips/pools/{pool_name}:
    delete:
      summary: Delete Ips Pools Pool Name
      description: |-
        **This endpoint allows you to delete an IP pool.**

        IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

        IP pools can only be used with whitelabeled IP addresses.

        If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
      operationId: ips.pools.pool_name.delete
      x-api-path-slug: ipspoolspool-name-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
      - Pool
      - Name
    get:
      summary: Get Ips Pools Pool Name
      description: |-
        **This endpoint allows you to list all of the IP addresses that are in a specific IP pool.**

        IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

        IP pools can only be used with whitelabeled IP addresses.

        If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
      operationId: ips.pools.pool_name.get
      x-api-path-slug: ipspoolspool-name-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
      - Pool
      - Name
    put:
      summary: Put Ips Pools Pool Name
      description: |-
        **This endpoint allows you to update the name of an IP pool.**

        IP Pools allow you to group your dedicated SendGrid IP addresses together. For example, you could create separate pools for your transactional and marketing email. When sending marketing emails, specify that you want to use the marketing IP pool. This allows you to maintain separate reputations for your different email traffic.

        IP pools can only be used with whitelabeled IP addresses.

        If an IP pool is NOT specified for an email, it will use any IP available, including ones in pools.
      operationId: ips.pools.pool_name.put
      x-api-path-slug: ipspoolspool-name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
      - Pool
      - Name
  /ips/pools/{pool_name}/ips:
    post:
      summary: Add Ips Pools Pool Name Ips
      description: |-
        **This endpoint allows you to add an IP address to an IP pool.**

        You can add the same IP address to multiple pools. It may take up to 60 seconds for your IP address to be added to a pool after your request is made.

        A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
      operationId: ips.pools.pool_name.ips.post
      x-api-path-slug: ipspoolspool-nameips-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
      - Pool
      - Name
      - Ips
  /ips/pools/{pool_name}/ips/{ip}:
    delete:
      summary: Delete Ips Pools Pool Name Ips Ip
      description: |-
        **This endpoint allows you to remove an IP address from an IP pool.**

        The same IP address can be added to multiple IP pools.

        A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
      operationId: ips.pools.pool_name.ips.ip.delete
      x-api-path-slug: ipspoolspool-nameipsip-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Pools
      - Pool
      - Name
      - Ips
      - Ip
  /ips/remaining:
    get:
      summary: Get Ips Remaining
      description: This endpoint gets amount of IP Addresses that can still be created
        during a given period and the price of those IPs.
      operationId: ips.remaining.get
      x-api-path-slug: ipsremaining-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Remaining
  /ips/warmup:
    get:
      summary: Get Ips Warmup
      description: |-
        **This endpoint allows you to retrieve all of your IP addresses that are currently warming up.**

        SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

        For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
      operationId: ips.warmup.get
      x-api-path-slug: ipswarmup-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Warmup
    post:
      summary: Add Ips Warmup
      description: |-
        **This endpoint allows you to enter an IP address into warmup mode.**

        SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

        For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
      operationId: ips.warmup.post
      x-api-path-slug: ipswarmup-post
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
      - Ips
      - Warmup
  /ips/warmup/{ip_address}:
    delete:
      summary: Delete Ips Warmup Ip Address
      description: |-
        **This endpoint allows you to remove an IP address from warmup mode.**

        SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

        For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
      operationId: ips.warmup.ip_address.delete
      x-api-path-slug: ipswarmupip-address-delete
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
      - Ips
      - Warmup
      - Ip
      - Address
    get:
      summary: Get Ips Warmup Ip Address
      description: |-
        **This endpoint allows you to retrieve the warmup status for a specific IP address.**

        SendGrid can automatically warm up dedicated IP addresses by limiting the amount of mail that can be sent through them per hour, with the limit determined by how long the IP address has been in warmup. See the [warmup schedule](https://sendgrid.com/docs/API_Reference/Web_API_v3/IP_Management/ip_warmup_schedule.html) for more details on how SendGrid limits your email traffic for IPs in warmup.

        For more general information about warming up IPs, please see our [Classroom](https://sendgrid.com/docs/Classroom/Deliver/Delivery_Introduction/warming_up_ips.html).
      operationId: ips.warmup.ip_address.get
      x-api-path-slug: ipswarmupip-address-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Warmup
      - Ip
      - Address
  /ips/{ip_address}:
    get:
      summary: Get Ips Ip Address
      description: |-
        **This endpoint allows you to see which IP pools a particular IP address has been added to.**

        The same IP address can be added to multiple IP pools.

        A single IP address or a range of IP addresses may be dedicated to an account in order to send email for multiple domains. The reputation of this IP is based on the aggregate performance of all the senders who use it.
      operationId: ips.ip_address.get
      x-api-path-slug: ipsip-address-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Ips
      - Ip
      - Address
  /mail/batch:
    post:
      summary: Add Mail Batch
      description: "**This endpoint allows you to generate a new batch ID. This batch
        ID can be associated with scheduled sends via the mail/send endpoint.**\n\nIf
        you set the SMTPAPI header `batch_id`, it allows you to then associate multiple
        scheduled mail/send requests together with the same ID. Then at anytime up
        to 10 minutes before the schedule date, you can cancel all of the mail/send
        requests that have this batch ID by calling the Cancel Scheduled Send endpoint.
        \n\nMore Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
      operationId: mail.batch.post
      x-api-path-slug: mailbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Batch
  /mail/batch/{batch_id}:
    get:
      summary: Get Mail Batch Batch
      description: "**This endpoint allows you to validate a batch ID.**\n\nIf you
        set the SMTPAPI header `batch_id`, it allows you to then associate multiple
        scheduled mail/send requests together with the same ID. Then at anytime up
        to 10 minutes before the schedule date, you can cancel all of the mail/send
        requests that have this batch ID by calling the Cancel Scheduled Send endpoint.
        \n\nMore Information:\n\n* [Scheduling Parameters > Batch ID](https://sendgrid.com/docs/API_Reference/SMTP_API/scheduling_parameters.html)"
      operationId: mail.batch.batch_id.get
      x-api-path-slug: mailbatchbatch-id-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Batch
      - Batch
  /mail/send:
    post:
      summary: Add Mail Send
      description: "This endpoint allows you to send email over SendGrid\u2019s v3
        Web API, the most recent version of our API. If you are looking for documentation
        about the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
        Top level parameters are referred to as \"global\".\n* Individual fields within
        the personalizations array will override any other global, or \u201Cmessage
        level\u201D, parameters that are defined outside of personalizations.\n \n**SendGrid
        provides libraries to help you quickly and easily integrate with the v3 Web
        API in 7 different languages: [C#](https://github.com/sendgrid/sendgrid-csharp),
        [Go](https://github.com/sendgrid/sendgrid-go), [Java](https://github.com/sendgrid/sendgrid-java),
        [Node JS](https://github.com/sendgrid/sendgrid-nodejs), [PHP](https://github.com/sendgrid/sendgrid-php),
        [Python](https://github.com/sendgrid/sendgrid-python), and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor
        more detailed information about how to use the v3 Mail Send endpoint, please
        visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
      operationId: mail.send.post
      x-api-path-slug: mailsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Send
  /mail_settings:
    get:
      summary: Get Mail Settings
      description: "**This endpoint allows you to retrieve a list of all mail settings.**\n\nMail
        settings allow you to tell SendGrid specific things to do to every email that
        you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: GET_mail_settings
      x-api-path-slug: mail-settings-get
      parameters:
      - in: query
        name: limit
        description: The number of settings to return
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Where in the list of results to begin displaying settings
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
  /mail_settings/address_whitelist:
    get:
      summary: Get Mail Settings Address Whitelist
      description: "**This endpoint allows you to retrieve your current email address
        whitelist settings.**\n\nThe address whitelist setting whitelists a specified
        email address or domain for which mail should never be suppressed. For example,
        you own the domain \u201Cexample.com,\u201D and one or more of your recipients
        use email@example.com addresses, by placing example.com in the address whitelist
        setting, all bounces, blocks, and unsubscribes logged for that domain will
        be ignored and sent as if under normal sending conditions.\n\nMail settings
        allow you to tell SendGrid specific things to do to every email that you send
        to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.address_whitelist.get
      x-api-path-slug: mail-settingsaddress-whitelist-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Address
      - Whitelist
    patch:
      summary: Patch Mail Settings Address Whitelist
      description: "**This endpoint allows you to update your current email address
        whitelist settings.**\n\nThe address whitelist setting whitelists a specified
        email address or domain for which mail should never be suppressed. For example,
        you own the domain \u201Cexample.com,\u201D and one or more of your recipients
        use email@example.com addresses, by placing example.com in the address whitelist
        setting, all bounces, blocks, and unsubscribes logged for that domain will
        be ignored and sent as if under normal sending conditions.\n\nMail settings
        allow you to tell SendGrid specific things to do to every email that you send
        to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.address_whitelist.patch
      x-api-path-slug: mail-settingsaddress-whitelist-patch
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
      - Mail
      - Settings
      - Address
      - Whitelist
  /mail_settings/bcc:
    get:
      summary: Get Mail Settings Bcc
      description: "**This endpoint allows you to retrieve your current BCC mail settings.**\n\nWhen
        the BCC mail setting is enabled, SendGrid will automatically send a blind
        carbon copy (BCC) to an address for every email sent without adding that address
        to the header. Please note that only one email address may be entered in this
        field, if you wish to distribute BCCs to multiple addresses you will need
        to create a distribution group or use forwarding rules.\n\nMail settings allow
        you to tell SendGrid specific things to do to every email that you send to
        your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.bcc.get
      x-api-path-slug: mail-settingsbcc-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Bcc
    patch:
      summary: Patch Mail Settings Bcc
      description: "**This endpoint allows you to update your current BCC mail settings.**\n\nWhen
        the BCC mail setting is enabled, SendGrid will automatically send a blind
        carbon copy (BCC) to an address for every email sent without adding that address
        to the header. Please note that only one email address may be entered in this
        field, if you wish to distribute BCCs to multiple addresses you will need
        to create a distribution group or use forwarding rules.\n\nMail settings allow
        you to tell SendGrid specific things to do to every email that you send to
        your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.bcc.patch
      x-api-path-slug: mail-settingsbcc-patch
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
      - Mail
      - Settings
      - Bcc
  /mail_settings/bounce_purge:
    get:
      summary: Get Mail Settings Bounce Purge
      description: "**This endpoint allows you to retrieve your current bounce purge
        settings.**\n\nThis setting allows you to set a schedule for SendGrid to automatically
        delete contacts from your soft and hard bounce suppression lists.\n\nMail
        settings allow you to tell SendGrid specific things to do to every email that
        you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.bounce_purge.get
      x-api-path-slug: mail-settingsbounce-purge-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Bounce
      - Purge
    patch:
      summary: Patch Mail Settings Bounce Purge
      description: "**This endpoint allows you to update your current bounce purge
        settings.**\n\nThis setting allows you to set a schedule for SendGrid to automatically
        delete contacts from your soft and hard bounce suppression lists.\n\nMail
        settings allow you to tell SendGrid specific things to do to every email that
        you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.bounce_purge.patch
      x-api-path-slug: mail-settingsbounce-purge-patch
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
      - Mail
      - Settings
      - Bounce
      - Purge
  /mail_settings/footer:
    get:
      summary: Get Mail Settings Footer
      description: "**This endpoint allows you to retrieve your current Footer mail
        settings.**\n\nThe footer setting will insert a custom footer at the bottom
        of the text and HTML bodies. Use the embedded HTML editor and plain text entry
        fields to create the content of the footers to be inserted into your emails.\n\nMail
        settings allow you to tell SendGrid specific things to do to every email that
        you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.footer.get
      x-api-path-slug: mail-settingsfooter-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Footer
    patch:
      summary: Patch Mail Settings Footer
      description: "**This endpoint allows you to update your current Footer mail
        settings.**\n\nThe footer setting will insert a custom footer at the bottom
        of the text and HTML bodies. Use the embedded HTML editor and plain text entry
        fields to create the content of the footers to be inserted into your emails.\n\nMail
        settings allow you to tell SendGrid specific things to do to every email that
        you send to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.footer.patch
      x-api-path-slug: mail-settingsfooter-patch
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
      - Mail
      - Settings
      - Footer
  /mail_settings/forward_bounce:
    get:
      summary: Get Mail Settings Forward Bounce
      description: "**This endpoint allows you to retrieve your current bounce forwarding
        mail settings.**\n\nActivating this setting allows you to specify an email
        address to which bounce reports are forwarded.\n\nMail settings allow you
        to tell SendGrid specific things to do to every email that you send to your
        recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.forward_bounce.get
      x-api-path-slug: mail-settingsforward-bounce-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Forward
      - Bounce
    patch:
      summary: Patch Mail Settings Forward Bounce
      description: "**This endpoint allows you to update your current bounce forwarding
        mail settings.**\n\nActivating this setting allows you to specify an email
        address to which bounce reports are forwarded.\n\nMail settings allow you
        to tell SendGrid specific things to do to every email that you send to your
        recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.forward_bounce.patch
      x-api-path-slug: mail-settingsforward-bounce-patch
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
      - Mail
      - Settings
      - Forward
      - Bounce
  /mail_settings/forward_spam:
    get:
      summary: Get Mail Settings Forward Spam
      description: "**This endpoint allows you to retrieve your current Forward Spam
        mail settings.**\n\nEnabling the forward spam setting allows you to specify
        an email address to which spam reports will be forwarded.\n\nMail settings
        allow you to tell SendGrid specific things to do to every email that you send
        to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.forward_spam.get
      x-api-path-slug: mail-settingsforward-spam-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Forward
      - Spam
    patch:
      summary: Patch Mail Settings Forward Spam
      description: "**This endpoint allows you to update your current Forward Spam
        mail settings.**\n\nEnabling the forward spam setting allows you to specify
        an email address to which spam reports will be forwarded.\n\nMail settings
        allow you to tell SendGrid specific things to do to every email that you send
        to your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.forward_spam.patch
      x-api-path-slug: mail-settingsforward-spam-patch
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
      - Mail
      - Settings
      - Forward
      - Spam
  /mail_settings/plain_content:
    get:
      summary: Get Mail Settings Plain Content
      description: "**This endpoint allows you to retrieve your current Plain Content
        mail settings.**\n\nThe plain content setting will automatically convert any
        plain text emails that you send to HTML before sending.\n\nMail settings allow
        you to tell SendGrid specific things to do to every email that you send to
        your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.plain_content.get
      x-api-path-slug: mail-settingsplain-content-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Plain
      - Content
    patch:
      summary: Patch Mail Settings Plain Content
      description: "**This endpoint allows you to update your current Plain Content
        mail settings.**\n\nThe plain content setting will automatically convert any
        plain text emails that you send to HTML before sending.\n\nMail settings allow
        you to tell SendGrid specific things to do to every email that you send to
        your recipients over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.plain_content.patch
      x-api-path-slug: mail-settingsplain-content-patch
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
      - Mail
      - Settings
      - Plain
      - Content
  /mail_settings/spam_check:
    get:
      summary: Get Mail Settings Spam Check
      description: "**This endpoint allows you to retrieve your current Spam Checker
        mail settings.**\n\nThe spam checker filter notifies you when emails are detected
        that exceed a predefined spam threshold.\n\nMail settings allow you to tell
        SendGrid specific things to do to every email that you send to your recipients
        over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.spam_check.get
      x-api-path-slug: mail-settingsspam-check-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Spam
      - Check
    patch:
      summary: Patch Mail Settings Spam Check
      description: "**This endpoint allows you to update your current spam checker
        mail settings.**\n\nThe spam checker filter notifies you when emails are detected
        that exceed a predefined spam threshold.\n\nMail settings allow you to tell
        SendGrid specific things to do to every email that you send to your recipients
        over SendGrid\u2019s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
        or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.spam_check.patch
      x-api-path-slug: mail-settingsspam-check-patch
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
      - Mail
      - Settings
      - Spam
      - Check
  /mail_settings/template:
    get:
      summary: Get Mail Settings Template
      description: "**This endpoint allows you to retrieve your current legacy email
        template settings.**\n\nThis setting refers to our original email templates.
        We currently support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
        \n\nThe legacy email template setting wraps an HTML template around your email
        content. This can be useful for sending out marketing email and/or other HTML
        formatted messages.\n\nMail settings allow you to tell SendGrid specific things
        to do to every email that you send to your recipients over SendGrid\u2019s
        [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
        Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.template.get
      x-api-path-slug: mail-settingstemplate-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Template
    patch:
      summary: Patch Mail Settings Template
      description: "**This endpoint allows you to update your current legacy email
        template settings.**\n\nThis setting refers to our original email templates.
        We currently support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
        \n\nThe legacy email template setting wraps an HTML template around your email
        content. This can be useful for sending out marketing email and/or other HTML
        formatted messages.\n\nMail settings allow you to tell SendGrid specific things
        to do to every email that you send to your recipients over SendGrid\u2019s
        [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP
        Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.template.patch
      x-api-path-slug: mail-settingstemplate-patch
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
      - Mail
      - Settings
      - Template
  /mailbox_providers/stats:
    get:
      summary: Get Mailbox Provers Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by recipient mailbox provider.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: mailbox_providers.stats.get
      x-api-path-slug: mailbox-providersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the stats
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include on each page
      - in: query
        name: mailbox_providers
        description: The mail box providers to get statistics for
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mailbox
      - Provers
      - Stats
  /partner_settings:
    get:
      summary: Get Partner Settings
      description: |-
        **This endpoint allows you to retrieve a list of all partner settings that you can enable.**

        Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).
      operationId: GET_partner_settings
      x-api-path-slug: partner-settings-get
      parameters:
      - in: query
        name: limit
        description: The number of settings to return per page
      - in: query
        name: offset
        description: The paging offset
      responses:
        200:
          description: OK
      tags:
      - Email
      - Partner
      - Settings
  /partner_settings/new_relic:
    get:
      summary: Get Partner Settings New Relic
      description: |-
        **This endpoint allows you to retrieve your current New Relic partner settings.**

        Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

        By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
      operationId: partner_settings.new_relic.get
      x-api-path-slug: partner-settingsnew-relic-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Partner
      - Settings
      - New
      - Relic
    patch:
      summary: Patch Partner Settings New Relic
      description: |-
        **This endpoint allows you to update or change your New Relic partner settings.**

        Our partner settings allow you to integrate your SendGrid account with our partners to increase your SendGrid experience and functionality. For more information about our partners, and how you can begin integrating with them, please visit our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/partners.html).

        By integrating with New Relic, you can send your SendGrid email statistics to your New Relic Dashboard. If you enable this setting, your stats will be sent to New Relic every 5 minutes. You will need your New Relic License Key to enable this setting. For more information, please see our [Classroom](https://sendgrid.com/docs/Classroom/Track/Collecting_Data/new_relic.html).
      operationId: partner_settings.new_relic.patch
      x-api-path-slug: partner-settingsnew-relic-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Partner
      - Settings
      - New
      - Relic
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