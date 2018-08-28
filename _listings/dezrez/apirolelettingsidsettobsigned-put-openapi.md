---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set the terms of business for a landlord on a PropertyLettingRole
  version: 1.0.0
  description: Set the terms of business for a landlord on a propertylettingrole.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/role/lettings/{id}/settobsigned:
    put:
      summary: Set the terms of business for a landlord on a PropertyLettingRole
      description: Set the terms of business for a landlord on a propertylettingrole.
      operationId: LettingRole_SetTOBSignedByidBydataContract
      x-api-path-slug: apirolelettingsidsettobsigned-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Terms
      - Of
      - Businessa
      - Landlord
      - "On"
      - PropertyLettingRole
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