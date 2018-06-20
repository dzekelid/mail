{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "512bf435-b2c8-40b7-8545-3e4006daade7",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "b35fc8c5-c320-4a22-a082-3f6fb5e884b5",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": "http://graph.microsoft.com/me/mailboxSettings/language",
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
              "id": "1794442f-37c3-4acc-a975-543a88d50608"
            }
          ]
        }
      ]
    }
  ]
}