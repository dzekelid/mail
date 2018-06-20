{
  "info": {
    "name": "Elastic Email SMTP API Listing of Active Channels",
    "_postman_id": "fe85b4b1-dd75-4fcf-b0cb-07db745bb8a3",
    "description": "Listing of Active Channels",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "604b50b8-94ad-4578-b208-42fe25b85b30",
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
              "id": "b42d91a0-dcb7-438f-9859-c76c87fe08e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "89bdcd08-a404-46bd-9f8d-f9e1cda27f67",
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
              "id": "ccf09190-0c50-430c-9e6b-89aca6718a62"
            }
          ]
        },
        {
          "id": "e2461672-95b5-4518-8a85-fa5ff4fb0991",
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
              "id": "e28c4728-c363-4869-bf61-e339c263661c"
            }
          ]
        },
        {
          "id": "6c668e6c-de50-4c71-a29f-b351d2892240",
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
              "id": "15638a4a-95b2-48b5-b99e-fdf6df03dfa5"
            }
          ]
        },
        {
          "id": "11f7e54a-f9c4-4615-a96b-0942f2f13ce0",
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
              "id": "aaaecd4e-23a9-4661-b2e5-d5d020f2f2d3"
            }
          ]
        },
        {
          "id": "d8e8b52a-2d04-4f1b-b30b-85223b284588",
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
              "id": "2e0248be-d6ff-4189-a560-bfb89fd2c619"
            }
          ]
        },
        {
          "id": "e0fb4d52-7982-47d6-8465-59dc3cfca5a5",
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
              "id": "ae5ab3a0-3f33-4be2-a815-46e0004379ec"
            }
          ]
        },
        {
          "id": "dc9ee33f-74f3-4b89-b47c-e4b3603aec39",
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
              "id": "527deb33-2e85-438b-8a23-c262fa195f3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "de412d98-d8a9-46ba-9f55-aeda68597340",
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
              "id": "2e949623-f908-4758-bb84-abbed8f63cea"
            }
          ]
        },
        {
          "id": "38beed40-2a5f-4378-abc6-aedad4288c0b",
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
              "id": "7b927aec-d0fa-447c-84b5-81966c336f8b"
            }
          ]
        },
        {
          "id": "0fb54722-f367-4e50-a274-c22cd54075c9",
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
              "id": "08bd2fcc-3b09-4f8e-aeba-e58f420cede9"
            }
          ]
        }
      ]
    }
  ]
}