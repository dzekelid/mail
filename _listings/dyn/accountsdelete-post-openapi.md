---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 0
info:
  title: Dyn Deleting an Email Sub-Account
  version: 1.0.0
  description: Deleting an Email Sub-Account
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  accounts:
    get:
      summary: Retrieve email sub-accounts
      description: Retrieving a list of up to 25 Email Sub-Accounts
      operationId: getAccounts
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: startindex
        description: An integer to indicate the starting index of where to begin the
          list of sub-accounts
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Accounts
    post:
      summary: Create an Email Sub-Account (API)
      description: Creating an Email Sub-Account using the API requires specific syntax
        for the REST API.
      operationId: postAccounts
      x-api-path-slug: accounts-post
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounceurl
        description: Bounce Postback URL
      - in: query
        name: city
        description: City
      - in: query
        name: companyname
        description: Required
      - in: query
        name: country
        description: Two-letter English abbreviation, based on the ISO 3166 standard
      - in: query
        name: generatenewapikey
        description: Used to create a new API key for an existing account (1 or 0)
      - in: query
        name: password
        description: Required
      - in: query
        name: phone
        description: Required
      - in: query
        name: spamurl
        description: Spam Postback URL
      - in: query
        name: state
        description: State
      - in: query
        name: timezone
        description: The timezone of the account, in [+/-]h
      - in: query
        name: tracklinks
        description: Toggle click tracking (1 or 0)
      - in: query
        name: trackopens
        description: Toggle open tracking (1 or 0)
      - in: query
        name: trackunsubscribes
        description: Toggle automatic list-unsubscribe support (1 or 0)
      - in: query
        name: username
        description: Required
      - in: query
        name: zipcode
        description: Zip
      responses:
        200:
          description: OK
      tags:
      - Create.Email
      - Accounts
      - (API)
    put:
      summary: Updating an Email Sub-Account
      description: Updating an Email Sub-Account
      operationId: putAccounts
      x-api-path-slug: accounts-put
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounceurl
        description: Bounce Postback URL
      - in: query
        name: city
        description: City
      - in: query
        name: companyname
        description: Required
      - in: query
        name: country
        description: Two-letter English abbreviation, based on the ISO 3166 standard
      - in: query
        name: generatenewapikey
        description: Used to create a new API key for an existing account (1 or 0)
      - in: query
        name: password
        description: Required
      - in: query
        name: phone
        description: Required
      - in: query
        name: spamurl
        description: Spam Postback URL
      - in: query
        name: state
        description: State
      - in: query
        name: timezone
        description: The timezone of the account, in [+/-]h
      - in: query
        name: tracklinks
        description: Toggle click tracking (1 or 0)
      - in: query
        name: trackopens
        description: Toggle open tracking (1 or 0)
      - in: query
        name: trackunsubscribes
        description: Toggle automatic list-unsubscribe support
      - in: query
        name: unsubscribeurl
        description: Unsubscribe postback URL
      - in: query
        name: username
        description: Required
      - in: query
        name: zipcode
        description: Zip
      responses:
        200:
          description: OK
      tags:
      - Updating.Email
      - Accounts
  accounts/delete:
    post:
      summary: Deleting an Email Sub-Account
      description: Deleting an Email Sub-Account
      operationId: postAccountsDelete
      x-api-path-slug: accountsdelete-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: username
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Deleting.Email
      - Accounts
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---