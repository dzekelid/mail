{
  "info": {
    "name": "Elastic Email SMTP API Send Email",
    "_postman_id": "58c01b54-fe02-49be-963a-2d1e83c77f7c",
    "description": "api.elasticemail.com",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "548b8661-a82b-4cf6-8c95-0927909dc567",
          "name": "getAttachmentsUpload",
          "request": {
            "url": "http://api.elasticemail.com/attachments/upload/?api_key=%7B%7D&file=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The upload attachment command is used to upload an attachment for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c460ac6a-8322-4dc5-99b7-37d818a536b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "de6b7754-0257-4c54-9dd1-cb90a0549011",
          "name": "getListsAddContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/add-contact?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add Existing Subscriber To List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c42e06f7-8b3a-4cca-8295-2e2672b1b767"
            }
          ]
        },
        {
          "id": "dcc85bd2-0803-4dd7-b9a4-d03cb9288758",
          "name": "getListsCreateContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/create-contact?api_key=%7B%7D&birthdate=%7B%7D&city=%7B%7D&country=%7B%7D&email=%7B%7D&firstname=%7B%7D&gender=%7B%7D&lastname=%7B%7D&listname=%7B%7D&organizationname=%7B%7D&phone=%7B%7D&postalcode=%7B%7D&state=%7B%7D&the zip or postal code of the subscriber=%7B%7D&title=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create New Subscriber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0160cb9c-9816-4eea-9f12-3039edd2fd3f"
            }
          ]
        },
        {
          "id": "e035363c-716c-4938-aae1-b270790e348c",
          "name": "getListsCreateLists",
          "request": {
            "url": "http://api.elasticemail.com/lists/create-lists?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create New List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af6f0ad3-8941-48d1-b063-52bce7ff1b95"
            }
          ]
        },
        {
          "id": "ea05a652-99b2-4ae6-9fc0-d12d020dc1ca",
          "name": "getListsDelete",
          "request": {
            "url": "http://api.elasticemail.com/lists/delete?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Existing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "487d8634-dd6c-4fbb-86d0-946d172cb897"
            }
          ]
        },
        {
          "id": "bc3073e1-ddbc-4b8c-8263-05e3df1ecaf3",
          "name": "getListsDeleteContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/delete-contact?api_key=%7B%7D&email=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Existing Subscriber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96047758-8f68-497e-9be9-43d426b8830d"
            }
          ]
        },
        {
          "id": "d9bdf462-f081-49d8-a584-12e46ed5902e",
          "name": "getListsRemoveContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/remove-contact?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Remove Existing Subscriber From List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b899084c-a23c-4384-8f43-d6dd922e0adf"
            }
          ]
        },
        {
          "id": "b8a17bce-3795-45e2-af57-02bedb73a344",
          "name": "getListsUploadContacts",
          "request": {
            "url": "http://api.elasticemail.com/lists/upload-contacts?api_key=%7B%7D&birthdate=%7B%7D&city=%7B%7D&country=%7B%7D&email=%7B%7D&firstname=%7B%7D&gender=%7B%7D&lastname=%7B%7D&listname=%7B%7D&organizationname=%7B%7D&phone=%7B%7D&postalcode=%7B%7D&state=%7B%7D&title=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create Multiple Subscriber From CSV File"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46bf4cd9-99a6-47b7-a425-6a163fb127a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "167ba94f-2f08-43a4-9a97-fa67616ea3d6",
          "name": "getMailerAccountDetails",
          "request": {
            "url": "http://api.elasticemail.com/mailer/account-details?api_key=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Account Details command is used to determine how much credit you have left."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "934810a4-f8fb-4420-a3e5-2bcbd8edd101"
            }
          ]
        },
        {
          "id": "2e6ba97b-2dee-4994-9037-ad967603541f",
          "name": "getMailerChannelDelete",
          "request": {
            "url": "http://api.elasticemail.com/mailer/channel/delete?api_key=%7B%7D&format=%7B%7D&name=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting Channel"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9478b0e6-709c-4b39-8626-2581d5fec66a"
            }
          ]
        },
        {
          "id": "742608f3-07ec-48d9-9965-ae691ce82340",
          "name": "getMailerChannelList",
          "request": {
            "url": "http://api.elasticemail.com/mailer/channel/list?api_key=%7B%7D&format=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Listing of Active Channels"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9e0deff-50c1-4f28-b32d-e0e1be39e798"
            }
          ]
        },
        {
          "id": "15e9d5e4-35ed-42ae-9255-409ed676e4ad",
          "name": "getMailerListBounced",
          "request": {
            "url": "http://api.elasticemail.com/mailer/list/bounced?api_key=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This api will return you the list of email addresses which are currently in your block list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bf418b7-b47e-4fb1-99a3-6428f9fb0e8d"
            }
          ]
        },
        {
          "id": "141c3bf0-e43a-453b-a07d-015dd00fdfad",
          "name": "getMailerListComplaint",
          "request": {
            "url": "http://api.elasticemail.com/mailer/list/complaint?api_key=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This api will return you the list of email addresses which are currently in your block list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "208bd7d7-ce3d-4fc0-a400-426051d5319a"
            }
          ]
        },
        {
          "id": "9b82bf6b-5ebf-44fb-b7f0-ce5d8f766a36",
          "name": "getMailerListsUnsubscribed",
          "request": {
            "url": "http://api.elasticemail.com/mailer/lists/unsubscribed?api_key=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This api will return you the list of email addresses which are currently in your block list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fff3c239-b4d5-4262-87c2-ade2ccf57da0"
            }
          ]
        },
        {
          "id": "b1af1b0b-a34e-4274-9cb3-f841d9166101",
          "name": "getMailerSend",
          "request": {
            "url": "http://api.elasticemail.com/mailer/send/?api_key=%7B%7D&body_html=%7B%7D&body_text=%7B%7D&channel=%7B%7D&charset=%7B%7D&encodingtype=%7B%7D&from=%7B%7D&from_name=%7B%7D&lists=%7B%7D&merge_firstname=%7B%7D&merge_lastname=%7B%7D&reply_to=%7B%7D&reply_to_name=%7B%7D&sender=%7B%7D&sender_name=%7B%7D&subject=%7B%7D&template=%7B%7D&time_offset_minutes=%7B%7D&total=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "api.elasticemail.com"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d47545a3-e0ec-4895-8873-e47ef3705387"
            }
          ]
        }
      ]
    }
  ]
}