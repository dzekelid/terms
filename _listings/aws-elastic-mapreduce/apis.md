---
name: AWS Elastic MapReduce
x-slug: aws-elastic-mapreduce
description: Amazon EMR provides a managed Hadoop framework that makes it easy, fast,
  and cost-effective to process vast amounts of data across dynamically scalable Amazon
  EC2 instances. You can also run other popular distributed frameworks such as Apache
  Spark, HBase, Presto, and Flink in Amazon EMR, and interact with data in other AWS
  data stores such as Amazon S3 and Amazon DynamoDB.Amazon EMR securely and reliably
  handles a broad set of big data use cases, including log analysis, web indexing,
  data transformations (ETL), machine learning, financial analysis, scientific simulation,
  and bioinformatics.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonEMR.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Terms
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/terms/master/_listings/aws-elastic-mapreduce/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Elastic MapReduce API - Set Termination Protection
  x-api-slug: actionsetterminationprotection-get
  description: SetTerminationProtection locks a job flow so the EC2 instances in the
    cluster cannot be terminated by user intervention, an API call, or in the event
    of a job-flow error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonEMR.png
  humanURL: https://aws.amazon.com/emr/
  baseURL: :///
  tags: Amazon Web Services, Data, MapReduce, Stack Network, API Service Provider,
    API Service Provider, API Provider, Databases, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/terms/master/_listings/aws-elastic-mapreduce/actionsetterminationprotection-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/terms/master/_listings/aws-elastic-mapreduce/actionsetterminationprotection-get-openapi.md
- name: AWS Elastic MapReduce API - Terminate Job Flows
  x-api-slug: actionterminatejobflows-get
  description: TerminateJobFlows shuts a list of job flows down.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonEMR.png
  humanURL: https://aws.amazon.com/emr/
  baseURL: :///
  tags: Amazon Web Services, Data, MapReduce, Stack Network, API Service Provider,
    API Service Provider, API Provider, Databases, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/terms/master/_listings/aws-elastic-mapreduce/actionterminatejobflows-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/terms/master/_listings/aws-elastic-mapreduce/actionterminatejobflows-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.elastic.load.balancing.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.elastic.mapreduce.stack.network
- type: x-article
  url: http://aws.amazon.com/articles/Elastic-MapReduce
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/ElasticMapReduce/latest/DeveloperGuide/emr-cli-reference.html
- type: x-faq
  url: https://aws.amazon.com/emr/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/emr/getting-started/
- type: x-partners
  url: https://aws.amazon.com/emr/partners/
- type: x-pricing
  url: https://aws.amazon.com/emr/pricing/
- type: x-documentation
  url: http://docs.aws.amazon.com/ElasticMapReduce/latest/API/
- type: x-website
  url: https://aws.amazon.com/emr/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---