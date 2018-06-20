{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "ab387893-ebb1-4b77-8400-55876a7388ff",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "d6da03df-8cd5-484a-ac9e-fcf85c5763d1",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": "http://graph.microsoft.com/me/mailboxSettings",
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
              "id": "5d04eb63-1e5b-4374-8c8f-40954b95bd39"
            }
          ]
        }
      ]
    }
  ]
}