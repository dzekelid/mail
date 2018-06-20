{
  "info": {
    "name": "Elastic Email SMTP API Deleting Channel",
    "_postman_id": "b5483a0f-ff70-49a7-98dc-46b5f9e593ed",
    "description": "Deleting Channel",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "d2b92a6d-cf37-4ce0-a57e-17320061c0dd",
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
              "id": "cf3cfccd-4801-41c5-91ea-e176cdc7be0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "d27e6419-40fb-48f1-95fa-32b5443ab6ce",
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
              "id": "96678a13-23f8-45f3-9294-883c6849fe4f"
            }
          ]
        },
        {
          "id": "11267f21-3f5c-4f77-9d63-9704d63d33f3",
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
              "id": "fd580116-d5f2-49ae-b75a-50e7d91a2b7b"
            }
          ]
        },
        {
          "id": "540d1d45-c35e-44f7-ade5-38655492b5da",
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
              "id": "fc4a2fae-4035-44ca-be00-ba4db82f3e45"
            }
          ]
        },
        {
          "id": "872a12cc-138b-440d-8543-b91d32e21086",
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
              "id": "47a203ae-9066-478c-ba2e-1c073a831e9a"
            }
          ]
        },
        {
          "id": "76748d06-527b-439a-bff1-e0d51888d8cb",
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
              "id": "c98e8780-c809-401a-be2a-0a9d4ecebdd6"
            }
          ]
        },
        {
          "id": "28063a2f-2373-446d-a1e0-7c45dcc564a7",
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
              "id": "b7d1fc4c-d539-476f-9d34-4e78c621eddc"
            }
          ]
        },
        {
          "id": "6f9ece32-860b-45c1-8c90-c79ba8691d05",
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
              "id": "343875ad-7bc0-4273-a2c9-7207a8406739"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "b824b7e5-bbb0-46a4-beb3-912ad5d7c999",
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
              "id": "a4e358ff-e515-4f49-94a2-8024ca81b418"
            }
          ]
        },
        {
          "id": "65426ea7-0b38-4493-87e5-66334990abdd",
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
              "id": "2695986a-c770-4cb3-829e-da049a92a6cd"
            }
          ]
        }
      ]
    }
  ]
}