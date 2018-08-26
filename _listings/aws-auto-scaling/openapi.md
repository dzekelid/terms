---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
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
  /?Action=TerminateInstanceInAutoScalingGroup:
    get:
      summary: Terminate Instance In Auto Scaling Group
      description: Terminates the specified instance and optionally adjusts the desired
        group size.
      operationId: terminateInstanceInAutoScalingGroup
      x-api-path-slug: actionterminateinstanceinautoscalinggroup-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If true, terminating the instance also decrements the size of
          the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Auto Scaling
---