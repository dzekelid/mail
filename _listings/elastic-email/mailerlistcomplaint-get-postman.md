{
  "info": {
    "name": "Elastic Email SMTP API Complaint",
    "_postman_id": "92ef1c37-affd-469d-a965-580dd1cb90fe",
    "description": "This api will return you the list of email addresses which are currently in your block list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "94cf18da-4f46-4710-89c4-287da36c6b8a",
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
              "id": "3ed32a8f-2422-4256-b4ae-d158133b47c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "5b1b2651-cfa9-482b-8f1d-5e5f2acc16fc",
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
              "id": "55949c68-a316-4889-bdcb-d15b1960f56a"
            }
          ]
        },
        {
          "id": "0867f0c0-94fc-4ab4-a482-3468932c56ba",
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
              "id": "d28220e6-b064-4e70-9d87-343d1ee9de15"
            }
          ]
        },
        {
          "id": "82677ae5-5cbc-456c-922a-4ecba2989b52",
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
              "id": "f9b611a9-41ff-4898-afa1-d97143e119c4"
            }
          ]
        },
        {
          "id": "b21a20cb-3245-4bb6-8458-c15d2b024023",
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
              "id": "2f9c30b0-23b1-4641-81ad-c3bb7a37cda7"
            }
          ]
        },
        {
          "id": "5e5b7661-297d-48f6-b029-f44ddf2d8d3c",
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
              "id": "301f2587-1297-443b-b4f6-9d0933d18c59"
            }
          ]
        },
        {
          "id": "9c603ddb-f3d9-419f-a886-c6f93e989207",
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
              "id": "3cbd0d04-a0da-435b-9ab7-a27b42669b91"
            }
          ]
        },
        {
          "id": "e308c1b5-8822-4af4-9b45-4985f4128558",
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
              "id": "0a07f0d5-14b8-40dc-ac17-4b68bdd6b5e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "307f7bb6-c95c-4c2e-9541-79a6d3f137bf",
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
              "id": "da0624ca-cd29-44b8-9d8c-84421e1db168"
            }
          ]
        },
        {
          "id": "831cb22f-4854-4b59-9600-eb12d39235ba",
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
              "id": "43462cfc-43a8-4195-a298-f276426e06b3"
            }
          ]
        },
        {
          "id": "fae4d5ca-ce4f-436b-abce-10f9392e805b",
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
              "id": "0c4a13cc-aa08-463a-96da-da77738f6589"
            }
          ]
        },
        {
          "id": "d927336e-144e-4165-9ac3-52083b60df95",
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
              "id": "2ec4919f-ab6e-4dcd-a423-cdac71d31710"
            }
          ]
        },
        {
          "id": "ff5ee6dd-ccc3-46bc-b7a0-788f4fb13b36",
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
              "id": "56220f2c-7963-4383-99d7-bf4b3be5e67c"
            }
          ]
        }
      ]
    }
  ]
}