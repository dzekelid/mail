{
  "info": {
    "name": "Microsoft Graph API Get User Mailbox Settings",
    "_postman_id": "fee1b0de-d755-442c-bd02-781f5002beae",
    "description": "Get user mailbox settings Get the user's mailboxSettings. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "8d38b754-387e-4527-a839-8da1978df563",
          "name": "GetUserMailboxSettings",
          "request": {
            "url": "http://graph.microsoft.com/me/mailboxSettings/automaticRepliesSetting",
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
              "id": "89e60198-9814-4502-9d35-04ec5bfe297a"
            }
          ]
        }
      ]
    }
  ]
}