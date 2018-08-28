---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Terminates a running workflow instance.
  version: 1.0.0
  description: Terminates a running workflow instance..
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
  /api/tenancy/{id}/setdates:
    post:
      summary: "Set start date, terms, end date and notice period for tenancy.\r\nassertions"
      description: "Set start date, terms, end date and notice period for tenancy.\r\nassertions."
      operationId: Tenancy_SetTenancyDatesByidBydatesDataContract
      x-api-path-slug: apitenancyidsetdates-post
      parameters:
      - in: body
        name: datesDataContract
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
      - Start
      - Date
      - ""
      - Terms
      - ""
      - End
      - Date
      - Notice
      - Periodtenancy
      - Assertions
  /api/admin/businessworkflow/{workflowName}:
    delete:
      summary: Terminates a running workflow instance.
      description: Terminates a running workflow instance..
      operationId: BusinessWorkflow_TerminateWorkflowInstanceByworkflowNameByworkflowInstanceHandleByreason
      x-api-path-slug: apiadminbusinessworkflowworkflowname-delete
      parameters:
      - in: query
        name: reason
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: workflowInstanceHandle
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Terminates
      - Running
      - Workflow
      - Instance
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