{
  "info": {
    "name": "Plentymarkets Send mail",
    "_postman_id": "0d61e9e4-2624-44d9-a881-308dd090c7db",
    "description": "Send mail from booted plugins.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Send",
      "item": [
        {
          "id": "1cbbbe03-5246-4745-a383-d50c412b9a6e",
          "name": "putRestAccountsContactsContactAccessDataNewPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/access_data/new_password"
              ],
              "query": [
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email to a contact with a link to change the password. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce850079-8d19-4363-a9a9-a243b344aa43"
            }
          ]
        },
        {
          "id": "0603ec09-cc9e-4fc0-8184-f7d8c0269e3a",
          "name": "postRestPluginsMail",
          "request": {
            "url": "http://example.com/rest/plugins_mail",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Send mail from booted plugins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f776900a-86b8-4589-91cb-c894e1977b34"
            }
          ]
        }
      ]
    }
  ]
}