---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 0
info:
  title: Dyn Retrieve Count of Emails Delivered
  version: 1.0.0
  description: Retrieve Count of Emails Delivered
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
  opens/count:
    get:
      summary: Email Open Count
      description: Returns total number of opens for the specified account for the
        specified date range. Including a date range is highly recommended.
      operationId: getOpensCount
      x-api-path-slug: openscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: u00a0Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - .Email
      - Open
      - Count
  reports/bounces:
    get:
      summary: Retrieve Email Bounces
      description: Retrieving the Email SPAM Complaints
      operationId: getReportsBounces
      x-api-path-slug: reportsbounces-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounce_code - Indicates the code associated with the bounced Email.
      - in: query
        name: bounce_code_id - The numeric code determined by the bounce processor.
      - in: query
        name: bounce_rule - Indicates the rule that caused this email to bounce.
      - in: query
        name: bounce_type
        description: Type of bounce for filtering
      - in: query
        name: bounce_type_id - Indicates whether the bounce type is a hard or soft
          bounce.nValid Values:n1 - Hard Bouncen2 - Soft Bounce
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: noheaders
        description: Determines whether or not headers are included in the response
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: sender_id
        description: Identifying number of the sender
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Bounces
  reports/bounces/count:
    get:
      summary: Retrieve Count of Email Bounces
      description: Retrieving a total count of Email bounces using the API requires
        specific syntax for the REST API.
      operationId: getReportsBouncesCount
      x-api-path-slug: reportsbouncescount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Bounces
  reports/clicks/count:
    get:
      summary: Retrieve Count of Email Links Clicked
      description: Retrieving a total of Email links clicked
      operationId: getReportsClicksCount
      x-api-path-slug: reportsclickscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: domainu00a0
        description: Domain of the recipient, such as &#8220;gmail
      - in: query
        name: emailaddress
        description: Email address of recipient for filteringu0010
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filteringu0010
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Links
      - Clicked
  reports/clicks/count/unique:
    get:
      summary: Retrieve Count of Email Links Clicked
      description: Retrieving a total of Email links clicked
      operationId: getReportsClicksCountUnique
      x-api-path-slug: reportsclickscountunique-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: domainu00a0
        description: Domain of the recipient, such as &#8220;gmail
      - in: query
        name: emailaddress
        description: Email address of recipient for filteringu0010
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filteringu0010
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Links
      - Clicked
  reports/complaints:
    get:
      summary: Retrieve Email SPAM Complaints
      description: Retrieve Email SPAM Complaints
      operationId: getReportsComplaints
      x-api-path-slug: reportscomplaints-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - SPAM
      - Complaints
  reports/complaints/count:
    get:
      summary: Retrieve Count of Email SPAM Complaints
      description: Retrieving a total count of Email complaints
      operationId: getReportsComplaintsCount
      x-api-path-slug: reportscomplaintscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: starttime
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - SPAM
      - Complaints
  reports/delivered:
    get:
      summary: Retrieve Emails Delivered
      description: Retrieve Emails Delivered
      operationId: getReportsDelivered
      x-api-path-slug: reportsdelivered-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Emails
      - Delivered
  reports/delivered/count:
    get:
      summary: Retrieve Count of Emails Delivered
      description: Retrieve Count of Emails Delivered
      operationId: getReportsDeliveredCount
      x-api-path-slug: reportsdeliveredcount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Emails
      - Delivered
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