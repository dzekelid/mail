{
  "info": {
    "name": "Elastic Email SMTP API Log Activity",
    "_postman_id": "00a46c94-5e45-4864-9e00-73aae3796df4",
    "description": "The detailed activity log api allows you to get detailed information from your activity log on the emails that you have sent. Information can be narrowed by email status, channel and datetime.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "8df0ca71-b894-4f44-82f9-b383c1035255",
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
              "id": "fa2d6d1a-0bc6-4c30-8c40-b938c3e4e832"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "65d84483-1a09-44b5-b2ac-87c76c944d91",
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
              "id": "3d113267-5d57-461b-a564-0475ea0ed399"
            }
          ]
        },
        {
          "id": "5e208d85-5651-42de-9347-9164e807a1b0",
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
              "id": "e22be9bd-8d24-4e1e-a786-42d1766dbe44"
            }
          ]
        },
        {
          "id": "d59cc7d1-34f5-489a-9c69-6edbef853370",
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
              "id": "2c281cb4-a80d-4ac4-a681-d79d348b5369"
            }
          ]
        },
        {
          "id": "8da5ef5f-cee2-4fa1-ab4e-a18efa192af1",
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
              "id": "960e8d50-e8dc-4a8f-9a89-f6a88bad0126"
            }
          ]
        },
        {
          "id": "53188182-946c-440a-8f45-7e2205b19058",
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
              "id": "fbec7177-49ab-4443-9db6-c25c6cb64ab5"
            }
          ]
        },
        {
          "id": "56cb011d-762b-492f-8680-6e89a130a356",
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
              "id": "a8bb49e7-d726-4bee-91f5-fee37eb357aa"
            }
          ]
        },
        {
          "id": "1e596484-53b7-4401-b01f-63cc65109622",
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
              "id": "b2db8607-952d-4476-8ac7-324b1b5a8fc9"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "5ed14e41-3315-4141-9552-5f5d9831410c",
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
              "id": "6c7d0a88-07a7-48c8-bba2-afa46e949fc9"
            }
          ]
        },
        {
          "id": "795480a9-06d8-434f-8c50-ca4779b847bd",
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
              "id": "b3a88b96-92fe-477f-b2e2-a3de518e7b2f"
            }
          ]
        },
        {
          "id": "35ba2a90-1c87-4c54-a568-164af53b000e",
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
              "id": "ca01ea1e-18e0-4190-a314-6eb194763170"
            }
          ]
        },
        {
          "id": "e3a95130-5ffd-4650-9efd-f9cc97ddf5a4",
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
              "id": "d412f930-3717-4e38-ae1f-75211582cd70"
            }
          ]
        },
        {
          "id": "112418f9-1f74-4950-93d4-4c4b878a4d35",
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
              "id": "a9b0ea9a-3eae-4544-98b6-c836f7bc5c6b"
            }
          ]
        },
        {
          "id": "410fe82d-12b7-426d-8bb3-a32a0a2df0b3",
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
              "id": "817eda76-e9a9-47cc-9f1e-9c7adc4f8898"
            }
          ]
        },
        {
          "id": "64c306c3-24c8-419a-bee5-ca9ce2c95e8e",
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
              "id": "dbfff49b-7d28-4e9c-8df6-be88f2e52214"
            }
          ]
        },
        {
          "id": "d365c846-45af-4eff-99bc-00433959fc7e",
          "name": "getMailerStatusLog",
          "request": {
            "url": "http://api.elasticemail.com/mailer/status/log?api_key=%7B%7D&channel=%7B%7D&compress=%7B%7D&format=%7B%7D&from=%7B%7D&status=%7B%7D&to=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The detailed activity log api allows you to get detailed information from your activity log on the emails that you have sent. Information can be narrowed by email status, channel and datetime."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d7f7f9f-debf-4efd-9219-8d2be45d65aa"
            }
          ]
        }
      ]
    }
  ]
}