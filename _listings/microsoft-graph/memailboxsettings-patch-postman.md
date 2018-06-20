{
  "info": {
    "name": "Microsoft Graph API Update User Mailbox Settings",
    "_postman_id": "94ac9b59-21ad-4a9b-8180-207813839463",
    "description": "Update user mailbox settings Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user",
      "item": [
        {
          "id": "6fde4f94-ff47-457b-8a68-6cd22c236a81",
          "name": "UpdateUserMailboxSettings",
          "request": {
            "url": "http://graph.microsoft.com/me/mailboxSettings",
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
              "id": "6fdf0e22-79ed-410e-81ca-ee25105c29d1"
            }
          ]
        }
      ]
    }
  ]
}