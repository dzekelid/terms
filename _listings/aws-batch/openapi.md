swagger: "2.0"
x-collection-name: AWS Batch
x-complete: 1
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TerminateJob:
    get:
      summary: Terminate Job
      description: Terminates jobs in a job queue.
      operationId: terminateJob
      x-api-path-slug: actionterminatejob-get
      parameters:
      - in: query
        name: jobId
        description: Job IDs to be terminated
        type: string
      - in: query
        name: reason
        description: A message to attach to the job that explains the reason for cancelling
          it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs