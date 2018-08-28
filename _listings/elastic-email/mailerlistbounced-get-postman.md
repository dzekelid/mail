{
  "info": {
    "name": "Elastic Email SMTP API Bounced",
    "_postman_id": "4248cc68-689c-4b8f-9473-90e572bd0db6",
    "description": "This api will return you the list of email addresses which are currently in your block list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "946da7fa-465d-463f-8746-5d84cd8de372",
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
              "id": "7adf5d73-c97e-48d0-aea7-83cee8299667"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "2ecb46f9-b3dd-4664-a606-6155dede75ce",
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
              "id": "e9478260-61d9-4406-a4f7-2a137ded407a"
            }
          ]
        },
        {
          "id": "5bbf9986-8ad7-4e57-b9cc-ee92ffedae95",
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
              "id": "b4101a35-bd97-4201-bd46-c29336824e15"
            }
          ]
        },
        {
          "id": "decfc26e-8ceb-4cf4-b8d0-d7d8c95820a6",
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
              "id": "aa9f086a-5a27-4581-a4f7-6a996cc86ba3"
            }
          ]
        },
        {
          "id": "cf6a7932-2ea7-44f1-ae1e-d1ab68db492a",
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
              "id": "c898cf0e-11cf-42db-ba77-f341c23049c0"
            }
          ]
        },
        {
          "id": "28b7793c-2fd5-4749-8432-ed2dd81639b4",
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
              "id": "322f812b-1402-4ec2-9f51-389ddcd0d048"
            }
          ]
        },
        {
          "id": "2efd4c48-7ea0-4fd2-ba6b-9175cec9c7b6",
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
              "id": "c9d6ab24-05a8-49ef-9bd2-9b09c5b31033"
            }
          ]
        },
        {
          "id": "3ec2eb65-2b7d-4d36-9e4f-dbccb2607165",
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
              "id": "eefbed82-4a13-4ccd-9bf5-55a94bba6a3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailer",
      "item": [
        {
          "id": "3f45d9fa-b4f5-4a4c-850d-6a21181227c8",
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
              "id": "74e3edcd-7c75-4db6-ac73-dbfde891d3c9"
            }
          ]
        },
        {
          "id": "2ff9d575-c018-4b8a-9423-f0cce31f4041",
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
              "id": "2b547e98-1699-4b25-a85f-7c5059db4771"
            }
          ]
        },
        {
          "id": "2e7a11a8-cd27-4ac8-9c4e-a66bb532626f",
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
              "id": "410ca75b-5b70-4b0e-95aa-5f49a7e4cf22"
            }
          ]
        },
        {
          "id": "f5e9cd19-6757-488e-97ba-8f64b1f4684a",
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
              "id": "d95d1065-0945-4084-8e75-b30135cddee6"
            }
          ]
        }
      ]
    }
  ]
}