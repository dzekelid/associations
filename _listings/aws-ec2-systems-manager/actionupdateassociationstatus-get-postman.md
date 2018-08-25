{
  "info": {
    "name": "Amazon EC2 Systems Manager API Update Association Status",
    "_postman_id": "0f7a435d-9ab1-4280-a5e4-db04c0ece64f",
    "description": "Updates the status of the SSM document associated with the specified\n   instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "6d11421e-e6f8-41d9-82cc-64107d3116c2",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45fde9e0-eb13-49cb-b002-77113341d826"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "4ec429b4-f5b3-4142-9332-7bee4cb527f6",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3670de06-42aa-4f76-b9a8-b14b1d773b76"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "59f4282a-d2ed-4312-a63a-2e75cb1f01ee",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c03196-6db9-42cd-acab-3023d9d237c4"
            }
          ]
        },
        {
          "id": "70018e1e-5c43-4146-9f94-a2616c6b0ead",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0195208-820d-49f7-b91a-5ccdffba174c"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "512c016d-c38b-4cab-a911-ff93613588c9",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcac0ae0-4ea0-4127-b6a9-7cdba0fafc44"
            }
          ]
        },
        {
          "id": "76fcd114-a446-43cf-b7be-110fc42574f5",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc31d9d2-f83b-4479-8779-2ccf106ac87a"
            }
          ]
        },
        {
          "id": "bc0685c0-8a21-4462-b045-477cdd172070",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23262a6e-f304-4435-8f75-517e40cb853e"
            }
          ]
        },
        {
          "id": "890f1b46-0fdf-4ed0-ae70-77bdc1e7477e",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc244f5-3e18-48a2-afd2-0325f00a4e3f"
            }
          ]
        },
        {
          "id": "dc596d25-ae6a-46e5-afd6-caea0578496f",
          "name": "updateAssociation",
          "request": {
            "url": "http://example.com/api/?Action=UpdateAssociation?AssociationId=AssociationId&DocumentVersion=DocumentVersion&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an association."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1505a74-807c-4b24-821d-b12ddbd37487"
            }
          ]
        },
        {
          "id": "4fda054a-4792-443a-a835-8a0afc0fbd4b",
          "name": "updateAssociationStatus",
          "request": {
            "url": "http://example.com/api/?Action=UpdateAssociationStatus?AssociationStatus=AssociationStatus&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the status of the SSM document associated with the specified\n   instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "907cc5a6-7ea4-4dc4-908f-d42fcd8a29ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "2eaea0ae-3b83-4575-83f3-994142dda783",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f49e64b5-3252-4d17-89cb-12277759ac2f"
            }
          ]
        },
        {
          "id": "2c34c8d9-d52b-42af-9cb0-6b46759f4fca",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17d5d3c0-2b92-4425-a0aa-5b0925209c99"
            }
          ]
        },
        {
          "id": "00b3c1c6-4e5c-403e-8c53-83d584385631",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4aa43d56-10e0-454c-a631-e7a67a94306a"
            }
          ]
        },
        {
          "id": "5332437e-a336-40ad-9439-52aecd8cf302",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24447f20-5d47-4c88-a326-57ff2dbbc574"
            }
          ]
        },
        {
          "id": "8f575f80-3c1d-4d4b-9278-3f44e8dcb586",
          "name": "getDocument",
          "request": {
            "url": "http://example.com/api/?Action=GetDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the contents of the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d846a202-0fdd-4b01-ba93-1301b4baf226"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "5118e447-6095-4577-9604-382033564b2d",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "587f3142-9d68-4ab0-aa83-295b7eb2124a"
            }
          ]
        },
        {
          "id": "a1f825c5-c93e-4edf-a8d7-483dde0b86b8",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0946af8-692e-4ef1-b969-b4df60452bba"
            }
          ]
        },
        {
          "id": "92b012c1-235f-4e8a-9ad8-104476b6ec82",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "787f44d6-d117-4a01-8252-36a9871d6632"
            }
          ]
        },
        {
          "id": "0aaac2c9-4d8b-44e3-8665-58f6ac156d46",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fe35393-8bde-4b78-8be5-ac975afacdca"
            }
          ]
        },
        {
          "id": "2967be19-3a1b-4116-8302-af80466c8197",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcefa2e5-49ac-4b6e-96f7-516864bc84a3"
            }
          ]
        },
        {
          "id": "fe79884e-dd47-4ef9-8cd2-a0f314c80fe3",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1c6cb8f-3a3a-4c76-b17e-366502abb5f3"
            }
          ]
        },
        {
          "id": "89fc7db2-b36b-4ae4-9e10-ea90139c6604",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3385a7bb-1f13-47b5-a3a1-7f293639c89d"
            }
          ]
        },
        {
          "id": "058ff308-0857-4ed4-bf9f-b4d617fdfe37",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ea45295-24f5-47c7-b1ac-0f917162e366"
            }
          ]
        },
        {
          "id": "7e9091f4-76b7-4dc2-95c0-ed5159c7334a",
          "name": "getMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d737ff24-259c-4d94-b1bb-90107000cbc7"
            }
          ]
        },
        {
          "id": "fc039197-b9c2-4c58-b1d0-9443fc0bc45c",
          "name": "getMaintenanceWindowExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecution?WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8627cc37-1481-4a32-8d42-fe548adac17c"
            }
          ]
        },
        {
          "id": "1ac97d41-efbd-4e20-9247-1a6978cca6cb",
          "name": "getMaintenanceWindowExecutionTask",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecutionTask?TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d359880-fc77-4ea7-811b-542752cd663a"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "09c8b9c9-445d-42bf-be04-76dfdbd870ef",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe851dc9-d472-4aeb-91ef-a63e55828c49"
            }
          ]
        },
        {
          "id": "c67b8f3c-e21d-4bcd-b339-58ac15015b72",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0be181c-3862-4903-bc1d-a7954dc75058"
            }
          ]
        },
        {
          "id": "ac9cdd43-22f1-42e8-973b-33bb47ab152d",
          "name": "getPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70c4ac8a-1f75-41f5-85fb-ac15e06041cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "619c7058-d2a1-4756-8c9d-72a907a7034f",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c178dec-ed66-4214-909a-cbfc77688678"
            }
          ]
        },
        {
          "id": "08fd12c4-e858-4976-996d-4dd4b28efaf6",
          "name": "getParameterHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetParameterHistory?MaxResults=MaxResults&Name=Name&NextToken=NextToken&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query a list of all parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b98c67d4-0d65-4f10-9570-83eaf1bd9403"
            }
          ]
        },
        {
          "id": "de238496-66d0-4546-9938-26759eb419bd",
          "name": "putParameter",
          "request": {
            "url": "http://example.com/api/?Action=PutParameter?Description=Description&KeyId=KeyId&Name=Name&Overwrite=Overwrite&Type=Type&Value=Value",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add one or more paramaters to the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85aa3894-7e41-468c-9493-1c333c8a3e04"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "2262bde1-8b28-47cd-afc3-02349f082bcc",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ad3c3aa-6b00-4f60-aa6e-1e626ecb3e6a"
            }
          ]
        },
        {
          "id": "d3023c8f-62c1-4362-a552-0b02a20359d5",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "587c823e-1579-4fb2-9706-6440ae778918"
            }
          ]
        },
        {
          "id": "1e4e6368-2ac4-4d11-92d6-75fd47f99831",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b69a7b79-ff5e-4703-990f-5c1fb61ba285"
            }
          ]
        },
        {
          "id": "2f5a40f2-5a52-4dd8-bd10-89a8ba3225fc",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "405cc566-250a-4a10-9200-4187b87549bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "5662232e-014c-42da-8941-25099cd993f5",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ba2c16f-2e26-4313-b8f5-1c1375e06781"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "6a3acb17-3b4f-4bc6-b98b-cc3dc58c19c8",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91be120f-2d14-4153-a877-051c19395637"
            }
          ]
        },
        {
          "id": "d0e559e3-caa4-4758-8810-f07f137ba3ca",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5078cc5-9c86-483d-a95a-f1faec95a8f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "a4ab247b-2168-4186-9f64-c07617ef316b",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04140b63-7f9c-47cb-9e3e-171c4ada5d61"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "53cd6b03-3ecc-40b6-8bc3-2a03cf2ea02d",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "059880f4-dfc9-4e70-9201-c34e9c596716"
            }
          ]
        },
        {
          "id": "9d25cd7b-d68a-45ec-8c69-f0e3173d5228",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "829d703a-5ea7-42f8-8759-d53639403581"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "b9987e3f-a511-4168-a5e1-f9ef6a1a16f3",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20c9cff7-110e-4b81-b57e-fe6147785920"
            }
          ]
        },
        {
          "id": "79c4abc1-e3ae-4f58-8273-c5a3ad9b303f",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "752b970b-6c2e-4a31-ad42-6782cbb48f0f"
            }
          ]
        },
        {
          "id": "b4e41e73-24ec-4b7a-a25d-198d15080b95",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a2d6e28-d976-4a16-9e39-50ff835312f0"
            }
          ]
        },
        {
          "id": "c50b2ca5-4bbd-4820-a753-60f598353d7c",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe7711c4-4595-43b7-bf0e-eefb42faf172"
            }
          ]
        },
        {
          "id": "0387d936-b95c-441b-9c94-75a260fd243e",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0194dcfd-742e-4d7d-b6f1-1abfe7e492a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "fc67aaa4-3446-41de-8b73-db8f63c05e87",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7845cb70-2d2b-4766-ac96-adcc4c734856"
            }
          ]
        },
        {
          "id": "dcdf2c3b-61f5-481b-b672-8b83f5de7016",
          "name": "getParameters",
          "request": {
            "url": "http://example.com/api/?Action=GetParameters?Names=Names&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1acf1ebf-4dea-4bd6-a505-1c85a3eb7dda"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "7eea50ed-422f-4068-9ab5-04c97f836b20",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5555270-1879-40c2-bf4d-9b1dc5180772"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "59540d8e-7522-40f0-8041-dde786fb7fb1",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca0b5b29-2a72-4ab1-92e7-1e3689d1168a"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "34cf5c47-a867-4922-9dff-1679155ee11b",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d808911-d668-4a16-a0c7-6bb91ca13e4e"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "b669c355-f158-4cb7-82c2-e6232b5e0b48",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87299ad0-4f99-4f1e-b363-739602d8a576"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "54579f03-472a-48de-b368-aa267e1ea13d",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4559dbf6-3f49-4492-895e-94daabe61f96"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "f13396a6-28c1-45a8-a6ce-c49e126ef159",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f047c14-4678-4a9b-9f06-33e516e5ba43"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "c22da4fc-4d59-4f52-af43-4aba5cc87419",
          "name": "getInventory",
          "request": {
            "url": "http://example.com/api/?Action=GetInventory?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&ResultAttributes=ResultAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query inventory information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78900241-ebfd-4075-a9ef-c137a76cd07a"
            }
          ]
        },
        {
          "id": "1984db58-e547-4026-ad22-ea12db890a4f",
          "name": "getInventorySchema",
          "request": {
            "url": "http://example.com/api/?Action=GetInventorySchema?MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of inventory type names for the account, or return a list of attribute\n   names for a specific Inventory item type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3af4d97e-1924-4a7c-b182-acee9b47fdbd"
            }
          ]
        },
        {
          "id": "caa5de03-b1bc-450c-9903-c8b5ec46f7ce",
          "name": "putInventory",
          "request": {
            "url": "http://example.com/api/?Action=PutInventory?InstanceId=InstanceId&Items=Items",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk update custom inventory items on one more instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c5c4b73-538f-49e4-80cd-80945bb80742"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "376362ce-4f61-4517-b444-273fd1deab14",
          "name": "getPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetPatchBaselineForPatchGroup?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the patch baseline that should be used for the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d83bc775-6bd6-4acc-b334-1d7a8fa384c3"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "e7113edf-e87c-40c2-8037-7166e0c11d53",
          "name": "listAssociations",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociations?AssociationFilterList=AssociationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac88c03f-8222-4cd9-897e-628fcfc6713e"
            }
          ]
        },
        {
          "id": "7be9cdb2-322d-43a1-ba4c-20f01ac52d0d",
          "name": "listCommandInvocations",
          "request": {
            "url": "http://example.com/api/?Action=ListCommandInvocations?CommandId=CommandId&Details=Details&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An invocation is copy of a command sent to a specific instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f824d3b-dd67-48ce-9010-abda16eae0e5"
            }
          ]
        },
        {
          "id": "a084f789-0ba5-4854-a16b-23c16c6b11f2",
          "name": "listCommands",
          "request": {
            "url": "http://example.com/api/?Action=ListCommands?CommandId=CommandId&Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the commands requested by users of the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98ec9fe2-2359-4a4e-928e-a4a9d89139a6"
            }
          ]
        },
        {
          "id": "a7fa9a29-4e02-418c-92ef-0e7cc653d3fe",
          "name": "listDocuments",
          "request": {
            "url": "http://example.com/api/?Action=ListDocuments?DocumentFilterList=DocumentFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your SSM documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d88da37-67b9-413b-81bc-44ce95e5bcad"
            }
          ]
        },
        {
          "id": "021bad77-9a2e-40ae-83bc-d6023577422e",
          "name": "listDocumentVersions",
          "request": {
            "url": "http://example.com/api/?Action=ListDocumentVersions?MaxResults=MaxResults&Name=Name&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all versions for a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4165b494-b288-4a3a-a8af-8aa7186bc9a9"
            }
          ]
        },
        {
          "id": "fb4b264e-a149-4afc-a46c-bf1b998016ae",
          "name": "listInventoryEntries",
          "request": {
            "url": "http://example.com/api/?Action=ListInventoryEntries?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of inventory items returned by the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "deefe922-5e9b-43f9-9b42-cef7ba2bb553"
            }
          ]
        },
        {
          "id": "7f05ba66-704d-4b8a-ac4c-3fa7372d0cd5",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?ResourceId=ResourceId&ResourceType=ResourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the tags assigned to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0510e9aa-4070-4305-b974-7d994da65a75"
            }
          ]
        }
      ]
    },
    {
      "name": "Modify",
      "item": [
        {
          "id": "78065267-f4eb-4f2c-aa44-4020add35d1b",
          "name": "modifyDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDocumentPermission?AccountIdsToAdd=AccountIdsToAdd&AccountIdsToRemove=AccountIdsToRemove&Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Share a document publicly or privately."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66af5b1d-c0cc-454b-b5bc-aa8541a32c8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Register",
      "item": [
        {
          "id": "6a89536b-5b03-424e-9dfc-cda5544a07f9",
          "name": "registerDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=RegisterDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Defines the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49a6f652-1b94-406c-afc2-4c8e39eee0c0"
            }
          ]
        },
        {
          "id": "5b6dfc2f-1a01-418d-8f5f-458ef324397c",
          "name": "registerPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=RegisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a patch baseline for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9964c92-e644-446a-8612-68cc7e247234"
            }
          ]
        },
        {
          "id": "467ea76b-246f-47f3-b906-bcd20ee3b16f",
          "name": "registerTargetWithMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTargetWithMaintenanceWindow?ClientToken=ClientToken&OwnerInformation=OwnerInformation&ResourceType=ResourceType&Targets=Targets&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a target with a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01fa5d4c-55bc-42f6-afc2-4629766eb6fb"
            }
          ]
        },
        {
          "id": "c220a8a1-3cab-4e1d-9127-1ec2d8080b0c",
          "name": "registerTaskWithMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTaskWithMaintenanceWindow?ClientToken=ClientToken&LoggingInfo=LoggingInfo&MaxConcurrency=MaxConcurrency&MaxErrors=MaxErrors&Priority=Priority&ServiceRoleArn=ServiceRoleArn&Targets=Targets&TaskArn=TaskArn&TaskParameters=TaskParameters&TaskType=TaskType&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new task to a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78ed1e55-1f9c-44f2-9bca-cc5099f22ad5"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "111c7c3c-5895-44f7-9ddb-299287dce9a3",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceId=ResourceId&ResourceType=ResourceType&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes all tags from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed19d84f-4089-45b3-9d0d-f3918c14904f"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "41f9e9b8-03a7-4061-8d0f-e77e765d3131",
          "name": "sendCommand",
          "request": {
            "url": "http://example.com/api/?Action=SendCommand?Comment=Comment&DocumentHash=DocumentHash&DocumentHashType=DocumentHashType&DocumentName=DocumentName&InstanceIds=InstanceIds&MaxConcurrency=MaxConcurrency&MaxErrors=MaxErrors&NotificationConfig=NotificationConfig&OutputS3BucketName=OutputS3BucketName&OutputS3KeyPrefix=OutputS3KeyPrefix&OutputS3Region=OutputS3Region&Parameters=Parameters&ServiceRoleArn=ServiceRoleArn&Targets=Targets&TimeoutSeconds=TimeoutSeconds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes commands on one or more remote instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc3586a3-3f2c-4e32-bc67-fae712652fe2"
            }
          ]
        }
      ]
    },
    {
      "name": "Start",
      "item": [
        {
          "id": "e74de4ae-1037-4795-aaa5-3fd6c5627e4c",
          "name": "startAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=StartAutomationExecution?DocumentName=DocumentName&DocumentVersion=DocumentVersion&Parameters=Parameters",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates execution of an Automation document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "216e6b11-d85a-426b-abb8-a0cc5bd3d52c"
            }
          ]
        }
      ]
    },
    {
      "name": "Stop",
      "item": [
        {
          "id": "693dee45-6620-4251-8198-307fc6604235",
          "name": "stopAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=StopAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stop an Automation that is currently executing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c94d63f-3aa9-488e-8222-eaa0bf1e18c2"
            }
          ]
        }
      ]
    }
  ]
}