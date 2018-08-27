---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Create Association Batch
  version: 1.0.0
  description: Associates the specified SSM document with the specified instances
    or targets.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEffectiveInstanceAssociations:
    get:
      summary: Describe Effective Instance Associations
      description: All associations for the instance(s).
      operationId: describeEffectiveInstanceAssociations
      x-api-path-slug: actiondescribeeffectiveinstanceassociations-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID for which you want to view all associations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Effective
      - Instance
      - Associations
  /?Action=DescribeInstanceAssociationsStatus:
    get:
      summary: Describe Instance Associations Status
      description: The status of the associations for the instance(s).
      operationId: describeInstanceAssociationsStatus
      x-api-path-slug: actiondescribeinstanceassociationsstatus-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance IDs for which you want association status information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Associations
      - Status
  /?Action=ListAssociations:
    get:
      summary: List Associations
      description: Lists the associations for the specified SSM document or instance.
      operationId: listAssociations
      x-api-path-slug: actionlistassociations-get
      parameters:
      - in: query
        name: AssociationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Associations
  /?Action=CreateAssociation:
    get:
      summary: Create Association
      description: Associates the specified SSM document with the specified instances
        or targets.
      operationId: createAssociation
      x-api-path-slug: actioncreateassociation-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version you want to associate with the target(s)
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      - in: query
        name: OutputLocation
        description: An Amazon S3 bucket where you want to store the output details
          of the request
        type: string
      - in: query
        name: Parameters
        description: The parameters for the documents runtime configuration
        type: string
      - in: query
        name: ScheduleExpression
        description: A cron expression when the association will be applied to the
          target(s)
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags) for the association
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=CreateAssociationBatch:
    get:
      summary: Create Association Batch
      description: Associates the specified SSM document with the specified instances
        or targets.
      operationId: createAssociationBatch
      x-api-path-slug: actioncreateassociationbatch-get
      parameters:
      - in: query
        name: Entries
        description: One or more associations
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
      - Batch
  /?Action=DeleteAssociation:
    get:
      summary: Delete Association
      description: Disassociates the specified SSM document from the specified instance.
      operationId: deleteAssociation
      x-api-path-slug: actiondeleteassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The association ID that you want to delete
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=DescribeAssociation:
    get:
      summary: Describe Association
      description: Describes the associations for the specified SSM document or instance.
      operationId: describeAssociation
      x-api-path-slug: actiondescribeassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The association ID for which you want information
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=UpdateAssociation:
    get:
      summary: Update Association
      description: Updates an association.
      operationId: updateAssociation
      x-api-path-slug: actionupdateassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The ID of the association you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The document version you want update for the association
        type: string
      - in: query
        name: OutputLocation
        description: An Amazon S3 bucket where you want to store the results of this
          request
        type: string
      - in: query
        name: Parameters
        description: The parameters you want to update for the association
        type: string
      - in: query
        name: ScheduleExpression
        description: The cron expression used to schedule the association that you
          want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=UpdateAssociationStatus:
    get:
      summary: Update Association Status
      description: |-
        Updates the status of the SSM document associated with the specified
           instance.
      operationId: updateAssociationStatus
      x-api-path-slug: actionupdateassociationstatus-get
      parameters:
      - in: query
        name: AssociationStatus
        description: The association status
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
      - Status
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