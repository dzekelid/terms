---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TerminateEnvironment:
    get:
      summary: Terminate Environment
      description: Terminates the specified environment.
      operationId: terminateEnvironment
      x-api-path-slug: actionterminateenvironment-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to terminate
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to terminate
        type: string
      - in: query
        name: ForceTerminate
        description: Terminates the target environment even if another environment
          in the same group is      dependent on it
        type: string
      - in: query
        name: TerminateResources
        description: 'Indicates whether the associated AWS resources should shut down
          when the environment is      terminated:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
---