{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "2cc6c4fc-b69d-4f88-8869-167112d4ee51",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "478027a2-a3a4-4175-b9f2-9df095fb6e6d",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id|userPrincipalName/mailboxSettings/language"
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
              "id": "14a8b5dd-5d53-4d85-9d9a-4cf59db0134e"
            }
          ]
        }
      ]
    }
  ]
}