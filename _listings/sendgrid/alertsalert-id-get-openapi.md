---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Alerts Alert
  description: "**This endpoint allows you to retrieve a specific alert.**\n\nAlerts
    allow you to specify an email address to receive notifications regarding your
    email usage or statistics. \n* Usage alerts allow you to set the threshold at
    which an alert will be sent.\n* Stats notifications allow you to set how frequently
    you would like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
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