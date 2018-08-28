{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "a3dc58ae-c008-43b2-8190-4dc8f4e11669",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "6407c22d-bb59-4d5e-894d-4f66ac214867",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": "http://graph.microsoft.com/me/mailboxSettings/timeZone",
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
              "id": "b155a0e9-397a-49a7-9593-0a521c0af3e0"
            }
          ]
        }
      ]
    }
  ]
}