{
  "info": {
    "name": "Elastic Email SMTP API Unsubscribed",
    "_postman_id": "c8255df4-bc2c-4049-8bf1-c39fb3047199",
    "description": "This api will return you the list of email addresses which are currently in your block list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "e5599f87-38d4-4904-a968-68d0e81486b1",
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
              "id": "b2f0ca46-0046-4f46-bbc7-1f2f1870345a"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "12dd0eb5-2974-44ce-971b-0c64374a94f9",
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
              "id": "93644b8e-373f-48fb-974f-4c8dc336245e"
            }
          ]
        },
        {
          "id": "a20e2a6b-1e2c-4bc2-a627-1e9e1f8d0eef",
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
              "id": "824e9c46-5647-4091-9582-eb1fcb405cee"
            }
          ]
        },
        {
          "id": "a98677dd-ec01-495b-acb8-af5db27318a9",
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
              "id": "31a21620-821b-41d2-b383-3f1611dfc704"
            }
          ]
        },
        {
          "id": "afa8c403-fa73-47d1-aaa0-ca1ed5a441ae",
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
              "id": "200df82f-7ce6-4a95-87f2-46400d6d9339"
            }
          ]
        },
        {
          "id": "c5e20310-40c8-4eaf-b64c-977880f6de7c",
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
              "id": "278042a7-5246-465c-9a3d-a5f0efeacf7c"
            }
          ]
        },
        {
          "id": "cf6a6d03-4257-4dd2-8804-dd8496f0e334",
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
              "id": "0b3767f0-5542-4c5d-9e46-621848c0dfab"
            }
          ]
        },
        {
          "id": "3b3ce2d7-f5e3-4cbe-9b1b-36d04c60309d",
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
              "id": "381ef1dd-939f-4db2-b8c3-6da8fe9bc1d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "da106440-c2f2-471e-a46f-db65c273042d",
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
              "id": "4e1a92e5-3c89-4372-a0ec-079ed258f809"
            }
          ]
        },
        {
          "id": "d35e8307-5554-4a94-a8cb-b8dde964b3aa",
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
              "id": "d70b2239-d3cd-4565-b667-479408a6c34f"
            }
          ]
        },
        {
          "id": "b5430648-c52d-4e65-9372-e26578104b69",
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
              "id": "e75c740f-723e-49a6-a662-e5814518b7b8"
            }
          ]
        },
        {
          "id": "e401d1df-8b23-4b8d-a6d7-9c515f893d72",
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
              "id": "73e02409-b735-4cc9-ae11-e62b8039c8ca"
            }
          ]
        },
        {
          "id": "7dd96ae8-a400-4ed8-90d6-ca6f42ff4ca8",
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
              "id": "5223d33e-a42d-4bc3-9660-cb07c519cc60"
            }
          ]
        },
        {
          "id": "09407bc3-7222-43d0-a510-410aa1d96ba4",
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
              "id": "20226c73-4ead-4aad-acd0-05436968aae8"
            }
          ]
        }
      ]
    }
  ]
}