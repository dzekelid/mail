{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "99726f86-a855-4b44-a4e1-60f464a4da82",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "59c8dfdc-87d8-4b84-9e88-f84408681a3b",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id|userPrincipalName/mailboxSettings/automaticRepliesSetting"
              ],
              "variable": [
                {
                  "id": "id|userPrincipalName",
                  "value": "id|userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer &lt;token&gt;",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get user mailbox settings Get the user's mailboxSettings"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "09cd3025-f978-4d37-92ac-591a502bb350"
            }
          ]
        }
      ]
    }
  ]
}