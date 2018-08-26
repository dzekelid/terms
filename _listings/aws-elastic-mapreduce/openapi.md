---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 1
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetTerminationProtection:
    get:
      summary: Set Termination Protection
      description: SetTerminationProtection locks a job flow so the EC2 instances
        in the cluster cannot be terminated by user intervention, an API call, or
        in the event of a job-flow error.
      operationId: setTerminationProtection
      x-api-path-slug: actionsetterminationprotection-get
      parameters:
      - in: query
        name: JobFlowIds
        description: A list of strings that uniquely identify the job flows to protect
        type: string
      - in: query
        name: TerminationProtected
        description: A Boolean that indicates whether to protect the job flow and
          prevent the Amazon EC2 instances in the cluster from shutting down due to
          API calls, user intervention, or job-flow error
        type: string
      responses:
        200:
          description: OK
      tags:
      - Termination Protection
  /?Action=TerminateJobFlows:
    get:
      summary: Terminate Job Flows
      description: TerminateJobFlows shuts a list of job flows down.
      operationId: terminateJobFlows
      x-api-path-slug: actionterminatejobflows-get
      parameters:
      - in: query
        name: JobFlowIds
        description: A list of job flows to be shutdown
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flows
---