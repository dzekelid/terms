swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TerminateWorkspaces:
    get:
      summary: Terminate Workspaces
      description: Terminates the specified WorkSpaces.
      operationId: terminateWorkspaces
      x-api-path-slug: actionterminateworkspaces-get
      parameters:
      - in: query
        name: TerminateWorkspaceRequests
        description: An array of structures that specify the WorkSpaces to terminate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces