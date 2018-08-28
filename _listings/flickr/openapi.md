---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.people.findByEmail:
    get:
      summary: People Find By Email
      description: Return a user's NSID, given their email address
      operationId: getRestMethodFlickr.people.findbyemail
      x-api-path-slug: restmethodflickr-people-findbyemail-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: find_email
        description: The email address of the user to find (may be primary or secondary)
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - People
      - FindByEmail
---