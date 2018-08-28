---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Describe Termination Policy Types
  version: 1.0.0
  description: Describes the termination policies supported by Auto Scaling.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTerminationPolicyTypes:
    get:
      summary: Describe Termination Policy Types
      description: Describes the termination policies supported by Auto Scaling.
      operationId: describeTerminationPolicyTypes
      x-api-path-slug: actiondescribeterminationpolicytypes-get
      parameters:
      - in: query
        name: TerminationPolicyTypes.member.N
        description: The termination policies supported by Auto Scaling (OldestInstance,
          OldestLaunchConfiguration,             NewestInstance, ClosestToNextInstanceHour,
          and Default)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Termination Policies
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