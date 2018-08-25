{
  "info": {
    "name": "Amazon EC2 Systems Manager API Update Association",
    "_postman_id": "214d2233-8cd0-4320-8606-b1dd53d2be6f",
    "description": "Updates an association.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "583ac4af-5385-47be-8f55-42693fa73e7d",
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
              "id": "b7716409-0787-4465-86f7-f28742bc6137"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "7b62cfab-899c-4f64-823b-00923a0827bf",
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
              "id": "bf0edf2a-4bd4-411e-8eeb-7af74839a9c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "4ee3bfd0-5664-407a-9227-d11d82ac521b",
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
              "id": "751d0d42-6f61-436e-9e5e-0fee9a4c3f02"
            }
          ]
        },
        {
          "id": "f5c60660-f860-48c5-a172-2448dfa79869",
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
              "id": "7c814207-c70b-4094-9a0d-c1ee61f949b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "04e1ba62-10ea-4081-a82a-2ce1932b62f5",
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
              "id": "5bc83433-f8f1-4532-b9f9-7d1e74658c15"
            }
          ]
        },
        {
          "id": "7b1976f9-59bd-436f-b3f5-e6a6bbe105b5",
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
              "id": "7cae8e3b-386c-4fbb-a6c2-547d4dc39b8b"
            }
          ]
        },
        {
          "id": "1c916f49-a93b-453f-b8b4-cc42c6b73f44",
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
              "id": "af4e9c38-7267-4a1f-97af-ab05b913871e"
            }
          ]
        },
        {
          "id": "aeae5fa5-4758-4114-a6de-56d94129d754",
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
              "id": "96bfeddc-5190-4cc8-aab5-ddf388993256"
            }
          ]
        },
        {
          "id": "aebc0842-230a-40db-986d-ea464c00b265",
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
              "id": "55c5aa56-fec2-40a8-90ad-643ec1fca3cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "acc5ba79-d482-4cee-92df-a4f108bb50c6",
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
              "id": "a5a03e07-7bf7-448e-a746-973b5f86dc52"
            }
          ]
        },
        {
          "id": "bbc4c3b5-fcb0-43d4-9a54-85c641b8d7b2",
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
              "id": "9532abcc-c34b-4571-afb6-a8b1dbcdbda6"
            }
          ]
        },
        {
          "id": "33cb5b7a-9778-4554-aeb5-19b0d80f6f8e",
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
              "id": "27361878-3b2b-471a-a9bf-66e7e7aaa659"
            }
          ]
        },
        {
          "id": "ea998354-2b02-4937-9ba0-6eacc74728b3",
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
              "id": "24c929e9-564e-409e-8857-78d56f075db9"
            }
          ]
        },
        {
          "id": "347743b8-cc68-475d-b5d0-77586c7227d2",
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
              "id": "2745ba0b-326d-420f-8ef2-fa8cbdbd8ee4"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "890328ee-a3bb-40ec-8f71-4c3863a9f67a",
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
              "id": "d44775f2-f776-4ec5-a08a-00a7cbd7fa19"
            }
          ]
        },
        {
          "id": "9aa624cf-5601-4324-a9cc-941b4b24b3a9",
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
              "id": "34867579-37cb-4cd2-8438-44e5e7387f4d"
            }
          ]
        },
        {
          "id": "2e3f0dc7-ad15-4338-803a-bf61185d964c",
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
              "id": "f532ff42-6b59-477f-ae15-c40ae1afca2f"
            }
          ]
        },
        {
          "id": "9902abf1-c7ce-40a0-bc86-fcbbd77668ef",
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
              "id": "f0d5252d-1040-46cb-87fe-e417f650927f"
            }
          ]
        },
        {
          "id": "79b85a0d-9e2a-4be1-b6fd-b3ab7f0bddef",
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
              "id": "8e618fa0-408d-40e0-9177-3abf99d4e0bf"
            }
          ]
        },
        {
          "id": "3b2c0dbc-451c-4965-9a07-eb05b906f3db",
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
              "id": "5a098eaa-cbdb-4a54-8fa0-c3cb07c3bf8b"
            }
          ]
        },
        {
          "id": "084afc8d-e3d1-475b-9ebe-a3f0019f5ac3",
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
              "id": "78bd6d5b-dfd2-4796-be25-b75a6e526c01"
            }
          ]
        },
        {
          "id": "fd345bc2-8556-4181-a5e2-3085a37c444f",
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
              "id": "dad0c51a-fff3-412b-822e-f656dcb3b6fd"
            }
          ]
        },
        {
          "id": "6db602cd-472f-4917-829b-8551681f7d7f",
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
              "id": "d28b1379-1e80-4dc0-84a6-fbc39b5fc42b"
            }
          ]
        },
        {
          "id": "47e3bb4f-0f93-46a7-966b-b4e18ad9ab95",
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
              "id": "dca4c3cb-d65f-41ee-8ab8-678515084cae"
            }
          ]
        },
        {
          "id": "995cd79a-24ab-44cf-88d1-61f789dab5ec",
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
              "id": "dc978566-068a-4bf9-9e8f-53f59ab84c73"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "abae1633-906c-4393-a135-4007c8611051",
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
              "id": "66a89a5a-79c1-43a4-9bba-a67d57096a3c"
            }
          ]
        },
        {
          "id": "6c6ae65d-2ea9-4cba-be1c-0556393035ff",
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
              "id": "856af82e-9832-4fa6-96d1-67286d11a467"
            }
          ]
        },
        {
          "id": "c46744c1-5355-44a6-960f-742d78dc531a",
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
              "id": "febfcbc6-c521-4260-b2a8-3848636d600d"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "5bcb3eb6-6de7-4968-9465-6ad556eb1c04",
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
              "id": "e1946cbd-4513-42cc-ab76-ddef0e6470d6"
            }
          ]
        },
        {
          "id": "26364816-fbb4-471d-8b48-9fdbbb6c7a9c",
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
              "id": "a10022f8-dfa9-4a2e-89df-68b8efe45848"
            }
          ]
        },
        {
          "id": "a94a75d3-7248-4269-a0ef-4f78eb35d6f1",
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
              "id": "f186d2f4-1c66-4e80-9062-c0071bbddab3"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "e112ba81-5290-40d6-928a-d2cf355e6214",
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
              "id": "6602a2f6-4ed6-4964-968c-7687db1dd1a9"
            }
          ]
        },
        {
          "id": "af6ebdc1-6624-4b33-80e8-ecf6c2a3136f",
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
              "id": "6e413b12-eab2-4c18-99ae-02c256704995"
            }
          ]
        },
        {
          "id": "c7f89dec-7916-4ac8-bcac-7db68a7a1ba9",
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
              "id": "05f7ab24-a0fd-4242-8e2a-827568020add"
            }
          ]
        },
        {
          "id": "de4f8a19-b691-452e-b2a9-74502243db76",
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
              "id": "e455f379-8a09-4f92-8559-ee48d0f13510"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "322ecd0d-dcc1-4985-9d08-f4462c2616f8",
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
              "id": "f6003aab-8e1e-458b-9ae2-e0af798dc64c"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "3d728ec5-4b24-4694-90ea-3ae5de463dec",
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
              "id": "48becbb5-35ab-45f7-af6e-4247753edd5b"
            }
          ]
        },
        {
          "id": "09346fda-bae5-4967-b14e-83bc3c1c8fa8",
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
              "id": "ecdcf33f-f174-4d13-aca5-4b8a166488e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "eab86c93-e71f-4cd3-98b5-4585cb6cc67f",
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
              "id": "c8b02cba-da69-45bc-9fac-71731d278e7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "a73918e3-5ec3-45aa-8f28-ae70872dee45",
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
              "id": "a410ec28-b630-4ae6-92ed-0eff04e320ac"
            }
          ]
        },
        {
          "id": "575909a9-6836-4ba6-b8f0-188db0fd18f4",
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
              "id": "422c5af4-11eb-40ce-86b4-9ea09b9552df"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "255855c6-42a3-4956-b0d4-aad2dfc07559",
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
              "id": "de8a5473-332c-4aea-b9d9-c44a89141793"
            }
          ]
        },
        {
          "id": "f47c2aff-8fc4-4d0d-a756-5f81f4ca9e66",
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
              "id": "fb5199b2-bc83-46c3-afcd-b5b558af0dd3"
            }
          ]
        },
        {
          "id": "338036d6-8ca7-4352-91d7-55853cee68f9",
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
              "id": "38d41674-98a9-4270-b113-668727fcc589"
            }
          ]
        },
        {
          "id": "5172b322-cee8-41f0-a20c-bd0e177952a1",
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
              "id": "c4bf781c-e62a-41f6-b5dd-6e0a20bf671d"
            }
          ]
        },
        {
          "id": "1a2bbf28-c6d5-4cf3-bc1e-55e5fe79eb42",
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
              "id": "93e15f76-b809-4c83-aabe-6d6e1fa8d72a"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "41c9a029-c852-407e-8c94-12f95946e0e0",
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
              "id": "65b35b89-2081-47a0-b270-422475162e95"
            }
          ]
        },
        {
          "id": "ed66b2b6-32cc-4db1-9db4-4bdf3776b138",
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
              "id": "2af47952-588a-4002-81c5-b6ec11ce5007"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "1646ae7f-7f22-4415-9bd3-434bb48a6d6e",
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
              "id": "32fbfea8-dd5b-478f-b972-4c1083348592"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "8fd5a441-749b-4ea8-bc2a-91ff9e78ae71",
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
              "id": "f0193934-6ffa-43c1-8b1b-cd7f15a6da16"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "64b9c3e9-3de0-4fcc-bbb6-b71d69795671",
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
              "id": "3d702151-1e92-491f-8ec5-769ae6f3924a"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "fb437a0c-a596-459e-a661-bf4f493b296d",
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
              "id": "f9dd3ad9-b84e-41d8-abd0-c69117bbe7d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "4cef76ed-26f1-463a-96cd-f399ee6dc189",
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
              "id": "355ded98-c301-483f-bfd7-52ba336ca1c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "6610fc51-ef63-49b0-937f-f698e03ce43d",
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
              "id": "f16c10f2-7622-4ab1-bb47-9b0acf34faa1"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "2cf61122-7d21-4d20-9eea-4b826717ce3c",
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
              "id": "d34c560c-8bf6-4c59-a439-e4ca0fd15ad3"
            }
          ]
        },
        {
          "id": "8e1f2608-a2ba-4e60-944b-6bb6efd0a218",
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
              "id": "94ca4d9e-e40d-4d76-a72d-674ee0c2b053"
            }
          ]
        },
        {
          "id": "780fd8bc-3178-459e-9ea7-485bf35c6035",
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
              "id": "8b92c4cd-244b-4789-95e7-b07a643fd105"
            }
          ]
        }
      ]
    },
    {
      "name": "BaselineGroup",
      "item": [
        {
          "id": "63944223-5ab5-411a-8d3a-86e91559403a",
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
              "id": "bdf775e8-7abb-4795-a547-558de1977863"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b0e325d5-e0d9-41b3-bbc1-90dd0942b27c",
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
              "id": "699e588f-6d87-43e9-8595-997b89a64ea1"
            }
          ]
        },
        {
          "id": "c1b230e1-d859-4a4b-97c8-7fab047cb093",
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
              "id": "83c18a3e-6df6-4cdc-927c-61aa85dec47a"
            }
          ]
        },
        {
          "id": "98e57226-2227-4613-9b6a-b6a5adfe43ad",
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
              "id": "dc4db337-cc49-44e7-841c-e1d3dcf109b9"
            }
          ]
        },
        {
          "id": "31b77be0-ac6b-4159-b43d-13c93ee96973",
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
              "id": "cf5b9645-93db-4232-9a5b-ad142401450e"
            }
          ]
        },
        {
          "id": "30d9c2d9-d450-46f8-b284-f03525842f5d",
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
              "id": "4943b306-96b0-427e-9218-ad160002777f"
            }
          ]
        },
        {
          "id": "7d4e2fc5-e72b-4cf6-a30e-a0072dd406b8",
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
              "id": "bf9ce8a4-b7fb-4a05-8b21-aed50d9d2ed6"
            }
          ]
        },
        {
          "id": "c5e323d5-d769-486e-9d1c-e9b79e36ad3a",
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
              "id": "e40ffdd5-747b-4148-9b34-be4aa1d92046"
            }
          ]
        }
      ]
    },
    {
      "name": "Modify",
      "item": [
        {
          "id": "8a4822ac-10c5-4f94-96b7-cefd39a5298a",
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
              "id": "3465ad32-87d5-4238-b2a6-a8cb2321fdc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Register",
      "item": [
        {
          "id": "4c96cda8-272f-4a42-9489-13a43d0b82f1",
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
              "id": "2ae7dc33-c53d-4746-95ca-f528ed67635b"
            }
          ]
        },
        {
          "id": "4cb7f78d-b952-460c-b7bd-49b276bce062",
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
              "id": "be27af5f-80c8-4c5b-8f58-931fc2f52dd2"
            }
          ]
        },
        {
          "id": "2c79d171-9269-4aaf-b34f-81537894667c",
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
              "id": "6be66577-c36f-4294-b516-1718e8d66c03"
            }
          ]
        },
        {
          "id": "9db4f4af-2edd-46f9-89eb-6a498cf949a5",
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
              "id": "8067c8ec-ec53-4b48-8097-9eba85477475"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "f10ed9b8-57e8-4e96-86d6-8122e37c0a48",
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
              "id": "6b70e646-cba5-4abc-94e4-08c142624c4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "af18eecd-651a-49da-8d84-94755d6ae092",
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
              "id": "23160627-95ed-41ef-93d3-4a950d977c37"
            }
          ]
        }
      ]
    },
    {
      "name": "Start",
      "item": [
        {
          "id": "a1215b8f-fdac-4a72-a361-acd04baea3a3",
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
              "id": "f260695d-92cd-47c1-8e63-7b91ba665e3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Stop",
      "item": [
        {
          "id": "59f27766-dc78-4894-bc66-694d5d4f64e8",
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
              "id": "d51d8d31-ecbd-4139-ab43-84eac4cf5c0b"
            }
          ]
        }
      ]
    }
  ]
}