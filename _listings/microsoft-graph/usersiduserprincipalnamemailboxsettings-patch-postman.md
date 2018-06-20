{
  "info": {
    "name": "Microsoft Graph API Update User Mailbox Settings",
    "_postman_id": "5bb0184a-48ad-4777-bfc6-80fa316b4b97",
    "description": "Update user mailbox settings Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "0049eb59-231d-4f29-8294-5dde4cfe42b1",
          "name": "UpdateUserMailboxSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id|userPrincipalName/mailboxSettings"
              ],
              "variable": [
                {
                  "id": "id|userPrincipalName",
                  "value": "id|userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
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
            "description": "Update user mailbox settings Update one or more settings for the user's mailbox"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "5f34eb78-a695-4f81-a5df-515751c29ca9"
            }
          ]
        }
      ]
    }
  ]
}