---
swagger: "2.0"
x-collection-name: AWS Certificate Manager
x-complete: 1
info:
  title: AWS Certificate Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResendValidationEmail:
    get:
      summary: Resend Validation Email
      description: Resends the email that requests domain ownership validation.
      operationId: ResendValidationEmail
      x-api-path-slug: actionresendvalidationemail-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the requested certificate
        type: string
      - in: query
        name: Domain
        description: The Fully Qualified Domain Name (FQDN) of the certificate that
          needs to be      validated
        type: string
      - in: query
        name: ValidationDomain
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
        200:
          description: OK
      tags:
      - Validation Email
---