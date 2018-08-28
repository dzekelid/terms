{
  "info": {
    "name": "AWS Elastic MapReduce API Set Termination Protection",
    "_postman_id": "98953e09-1e2a-4674-a9c1-041342578980",
    "description": "SetTerminationProtection locks a job flow so the EC2 instances in the cluster cannot be terminated by user intervention, an API call, or in the event of a job-flow error.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instance Groups",
      "item": [
        {
          "id": "60a3222b-951d-4291-820b-22e29576a509",
          "name": "addInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=AddInstanceGroups?InstanceGroups=InstanceGroups&JobFlowId=JobFlowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more instance groups to a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "810a4363-52f1-41c5-9bdc-eda474606aa3"
            }
          ]
        },
        {
          "id": "2e2a9da1-f2d3-4642-9eff-c4b0d969a70b",
          "name": "listInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListInstanceGroups?ClusterId=ClusterId&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides all available details about the instance groups in a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afd22665-f6a6-4f5c-8ee1-94580eee7c49"
            }
          ]
        },
        {
          "id": "3cd9e704-6bc7-4151-8597-fbb5646dc03b",
          "name": "modifyInstanceGroups",
          "request": {
            "url": "http://example.com/api/?Action=ModifyInstanceGroups?ClusterId=ClusterId&InstanceGroups=InstanceGroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "ModifyInstanceGroups modifies the number of nodes and configuration settings of an instance group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ac643dd-d052-416d-9755-b01ebf904dd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "d8efca3f-64e6-45d7-a3d3-f8efbdb372a2",
          "name": "addJobFlowSteps",
          "request": {
            "url": "http://example.com/api/?Action=AddJobFlowSteps?JobFlowId=JobFlowId&Steps=Steps",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AddJobFlowSteps adds new steps to a running job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7c467f0-e6a2-406b-ae64-906ddc955825"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "2eafa319-b13e-46b4-9891-31ab509a3f2b",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tags to an Amazon EMR resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "775e344b-e492-48cb-ad77-87ea85e43171"
            }
          ]
        },
        {
          "id": "35a66207-9ed9-49a4-b43e-344a4755a099",
          "name": "removeTags",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTags?ResourceId=ResourceId&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from an Amazon EMR resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48f0a14b-35c6-492a-84d7-54a464b900f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "43120bea-ad71-4cc7-bc8d-c1d80314c1f7",
          "name": "cancelSteps",
          "request": {
            "url": "http://example.com/api/?Action=CancelSteps?ClusterId=ClusterId&StepIds=StepIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending step or steps in a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53d84b7d-dacc-402a-97e4-02663be46e48"
            }
          ]
        },
        {
          "id": "751c1b02-c3e0-42c1-b6b5-6bb247178710",
          "name": "describeStep",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStep?ClusterId=ClusterId&StepId=StepId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides more detail about the cluster step."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a11472d-568d-4518-818d-4dfeaae1ec54"
            }
          ]
        },
        {
          "id": "77da7204-b9ee-47db-abc8-b7ab6b61b8d6",
          "name": "listSteps",
          "request": {
            "url": "http://example.com/api/?Action=ListSteps?ClusterId=ClusterId&Marker=Marker&StepIds=StepIds&StepStates=StepStates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a list of steps for the cluster in reverse order unless you specify stepIds with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3771686e-e730-4715-ad93-927a2ad4bd9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Configurations",
      "item": [
        {
          "id": "0ffe9f20-883d-406e-943f-f4667e518742",
          "name": "createSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateSecurityConfiguration?Name=Name&SecurityConfiguration=SecurityConfiguration",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a security configuration, which is stored in the service and can be specified when a cluster is created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1b7b4a3-e8b8-431b-b2eb-fbf9958c7fec"
            }
          ]
        },
        {
          "id": "e71ed04b-b904-4aea-835b-8078f373a798",
          "name": "deleteSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSecurityConfiguration?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a security configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f5cc04b-161f-48a6-9d8d-76d99974e119"
            }
          ]
        },
        {
          "id": "1088a3e8-f771-406c-92d5-c24cf123ea96",
          "name": "describeSecurityConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSecurityConfiguration?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the details of a security configuration by returning the configuration JSON."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dded452c-521f-40eb-b54c-3f82463696e1"
            }
          ]
        },
        {
          "id": "51e6c440-a0a7-4bec-b6d5-ac6f67f7df95",
          "name": "listSecurityConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=ListSecurityConfigurations?Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the security configurations visible to this account, providing their creation dates and times, and their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cde2224-c53a-4280-8c9b-9fe3e11ee0a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "513c1a91-9d31-49cb-95b7-b904c00279f7",
          "name": "describeCluster",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides cluster-level details including status, hardware and software configuration, VPC settings, and so on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a1885c5-1008-4ab0-83ba-ce7a07589a4b"
            }
          ]
        },
        {
          "id": "ace307e1-7c41-4e73-b4cd-1a6ad30648c6",
          "name": "listClusters",
          "request": {
            "url": "http://example.com/api/?Action=ListClusters?ClusterStates=ClusterStates&CreatedAfter=CreatedAfter&CreatedBefore=CreatedBefore&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the status of all clusters visible to this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90dfda10-8b5a-44d4-96ea-9e1ca41a26ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Flows",
      "item": [
        {
          "id": "49dfb04a-5380-4416-a586-2eb3e6e23b7e",
          "name": "describeJobFlows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJobFlows?CreatedAfter=CreatedAfter&CreatedBefore=CreatedBefore&JobFlowIds=JobFlowIds&JobFlowStates=JobFlowStates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API is deprecated and will eventually be removed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "706cb726-d26d-46aa-8921-2a461a0a6ef4"
            }
          ]
        },
        {
          "id": "80a22ec5-3545-470f-8be3-0eaf779a2d51",
          "name": "runJobFlow",
          "request": {
            "url": "http://example.com/api/?Action=RunJobFlow?AdditionalInfo=AdditionalInfo&AmiVersion=AmiVersion&Applications=Applications&AutoScalingRole=AutoScalingRole&BootstrapActions=BootstrapActions&Configurations=Configurations&Instances=Instances&JobFlowRole=JobFlowRole&LogUri=LogUri&Name=Name&NewSupportedProducts=NewSupportedProducts&ReleaseLabel=ReleaseLabel&ScaleDownBehavior=ScaleDownBehavior&SecurityConfiguration=SecurityConfiguration&ServiceRole=ServiceRole&Steps=Steps&SupportedProducts=SupportedProducts&Tags=Tags&VisibleToAllUsers=VisibleToAllUsers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "RunJobFlow creates and starts running a new job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ae670f1-822d-4cc1-9432-18f3adde5e6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Bootstrap Actions",
      "item": [
        {
          "id": "54a80c0a-064b-4d45-bd83-eb2a1a26c847",
          "name": "listBootstrapActions",
          "request": {
            "url": "http://example.com/api/?Action=ListBootstrapActions?ClusterId=ClusterId&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the bootstrap actions associated with a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c898595-6ac5-4aa6-a999-eef4c5cccd2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "a8fd127c-05f1-4cb0-a308-af1062c92e77",
          "name": "listInstances",
          "request": {
            "url": "http://example.com/api/?Action=ListInstances?ClusterId=ClusterId&InstanceGroupId=InstanceGroupId&InstanceGroupTypes=InstanceGroupTypes&InstanceStates=InstanceStates&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the cluster instances that Amazon EMR provisions on behalf of a user \n         when it creates the cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "482719c2-b07c-4be9-9099-55a2fae44d78"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Policies",
      "item": [
        {
          "id": "4176e107-799b-4c14-ad4d-9e6862ea04eb",
          "name": "putAutoScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutAutoScalingPolicy?AutoScalingPolicy=AutoScalingPolicy&ClusterId=ClusterId&InstanceGroupId=InstanceGroupId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates an automatic scaling policy for a core instance group or task instance group in an Amazon EMR cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86c2c44b-c469-4f69-bbf7-8c279c5cd18c"
            }
          ]
        },
        {
          "id": "b00bfc7d-db7a-48eb-b301-dd58b75dcea4",
          "name": "removeAutoScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAutoScalingPolicy?ClusterId=ClusterId&InstanceGroupId=InstanceGroupId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an automatic scaling policy from a specified instance group within an EMR cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8997a8f-93bc-4440-b0d0-5f8cd4ec0e1f"
            }
          ]
        }
      ]
    },
    {
      "name": "Termination Protection",
      "item": [
        {
          "id": "fd95e166-0cd1-4ed2-8e9e-9c27b79af4e7",
          "name": "setTerminationProtection",
          "request": {
            "url": "http://example.com/api/?Action=SetTerminationProtection?JobFlowIds=JobFlowIds&TerminationProtected=TerminationProtected",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "SetTerminationProtection locks a job flow so the EC2 instances in the cluster cannot be terminated by user intervention, an API call, or in the event of a job-flow error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17297ac2-c75a-49c5-adc8-bd464cba496e"
            }
          ]
        }
      ]
    }
  ]
}