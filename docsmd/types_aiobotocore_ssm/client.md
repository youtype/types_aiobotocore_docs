# SSMClient

> [Index](../README.md) > [SSM](./README.md) > SSMClient

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#ssm)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## SSMClient

Type annotations and code completion for `#!python session.create_client("ssm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)

```python
# SSMClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ssm.client import SSMClient

session = get_session()
async with session.create_client("ssm") as client:
    client: SSMClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ssm").exceptions` structure.

```python
# SSMClient.exceptions usage example

async with session.create_client("ssm") as client:
    try:
        do_something(client)
    except (
            client.AlreadyExistsException,
        client.AssociatedInstances,
        client.AssociationAlreadyExists,
        client.AssociationDoesNotExist,
        client.AssociationExecutionDoesNotExist,
        client.AssociationLimitExceeded,
        client.AssociationVersionLimitExceeded,
        client.AutomationDefinitionNotApprovedException,
        client.AutomationDefinitionNotFoundException,
        client.AutomationDefinitionVersionNotFoundException,
        client.AutomationExecutionLimitExceededException,
        client.AutomationExecutionNotFoundException,
        client.AutomationStepNotFoundException,
        client.ClientError,
        client.ComplianceTypeCountLimitExceededException,
        client.CustomSchemaCountLimitExceededException,
        client.DocumentAlreadyExists,
        client.DocumentLimitExceeded,
        client.DocumentPermissionLimit,
        client.DocumentVersionLimitExceeded,
        client.DoesNotExistException,
        client.DuplicateDocumentContent,
        client.DuplicateDocumentVersionName,
        client.DuplicateInstanceId,
        client.FeatureNotAvailableException,
        client.HierarchyLevelLimitExceededException,
        client.HierarchyTypeMismatchException,
        client.IdempotentParameterMismatch,
        client.IncompatiblePolicyException,
        client.InternalServerError,
        client.InvalidActivation,
        client.InvalidActivationId,
        client.InvalidAggregatorException,
        client.InvalidAllowedPatternException,
        client.InvalidAssociation,
        client.InvalidAssociationVersion,
        client.InvalidAutomationExecutionParametersException,
        client.InvalidAutomationSignalException,
        client.InvalidAutomationStatusUpdateException,
        client.InvalidCommandId,
        client.InvalidDeleteInventoryParametersException,
        client.InvalidDeletionIdException,
        client.InvalidDocument,
        client.InvalidDocumentContent,
        client.InvalidDocumentOperation,
        client.InvalidDocumentSchemaVersion,
        client.InvalidDocumentType,
        client.InvalidDocumentVersion,
        client.InvalidFilter,
        client.InvalidFilterKey,
        client.InvalidFilterOption,
        client.InvalidFilterValue,
        client.InvalidInstanceId,
        client.InvalidInstanceInformationFilterValue,
        client.InvalidInstancePropertyFilterValue,
        client.InvalidInventoryGroupException,
        client.InvalidInventoryItemContextException,
        client.InvalidInventoryRequestException,
        client.InvalidItemContentException,
        client.InvalidKeyId,
        client.InvalidNextToken,
        client.InvalidNotificationConfig,
        client.InvalidOptionException,
        client.InvalidOutputFolder,
        client.InvalidOutputLocation,
        client.InvalidParameters,
        client.InvalidPermissionType,
        client.InvalidPluginName,
        client.InvalidPolicyAttributeException,
        client.InvalidPolicyTypeException,
        client.InvalidResourceId,
        client.InvalidResourceType,
        client.InvalidResultAttributeException,
        client.InvalidRole,
        client.InvalidSchedule,
        client.InvalidTag,
        client.InvalidTarget,
        client.InvalidTargetMaps,
        client.InvalidTypeNameException,
        client.InvalidUpdate,
        client.InvocationDoesNotExist,
        client.ItemContentMismatchException,
        client.ItemSizeLimitExceededException,
        client.MalformedResourcePolicyDocumentException,
        client.MaxDocumentSizeExceeded,
        client.OpsItemAccessDeniedException,
        client.OpsItemAlreadyExistsException,
        client.OpsItemConflictException,
        client.OpsItemInvalidParameterException,
        client.OpsItemLimitExceededException,
        client.OpsItemNotFoundException,
        client.OpsItemRelatedItemAlreadyExistsException,
        client.OpsItemRelatedItemAssociationNotFoundException,
        client.OpsMetadataAlreadyExistsException,
        client.OpsMetadataInvalidArgumentException,
        client.OpsMetadataKeyLimitExceededException,
        client.OpsMetadataLimitExceededException,
        client.OpsMetadataNotFoundException,
        client.OpsMetadataTooManyUpdatesException,
        client.ParameterAlreadyExists,
        client.ParameterLimitExceeded,
        client.ParameterMaxVersionLimitExceeded,
        client.ParameterNotFound,
        client.ParameterPatternMismatchException,
        client.ParameterVersionLabelLimitExceeded,
        client.ParameterVersionNotFound,
        client.PoliciesLimitExceededException,
        client.ResourceDataSyncAlreadyExistsException,
        client.ResourceDataSyncConflictException,
        client.ResourceDataSyncCountExceededException,
        client.ResourceDataSyncInvalidConfigurationException,
        client.ResourceDataSyncNotFoundException,
        client.ResourceInUseException,
        client.ResourceLimitExceededException,
        client.ResourceNotFoundException,
        client.ResourcePolicyConflictException,
        client.ResourcePolicyInvalidParameterException,
        client.ResourcePolicyLimitExceededException,
        client.ResourcePolicyNotFoundException,
        client.ServiceSettingNotFound,
        client.StatusUnchanged,
        client.SubTypeCountLimitExceededException,
        client.TargetInUseException,
        client.TargetNotConnected,
        client.TooManyTagsError,
        client.TooManyUpdates,
        client.TotalSizeLimitExceededException,
        client.UnsupportedCalendarException,
        client.UnsupportedFeatureRequiredException,
        client.UnsupportedInventoryItemContextException,
        client.UnsupportedInventorySchemaVersionException,
        client.UnsupportedOperatingSystem,
        client.UnsupportedOperationException,
        client.UnsupportedParameterType,
        client.UnsupportedPlatformType,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SSMClient usage type checking example

from types_aiobotocore_ssm.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ssm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ssm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### add\_tags\_to\_resource

Adds or overwrites one or more tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("ssm").add_tags_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/add_tags_to_resource.html)

```python
# add_tags_to_resource method definition

await def add_tags_to_resource(
    self,
    *,
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags_to_resource method usage example with argument unpacking

kwargs: AddTagsToResourceRequestTypeDef = {  # (1)
    "ResourceType": ...,
    "ResourceId": ...,
    "Tags": ...,
}

parent.add_tags_to_resource(**kwargs)
```

1. See [:material-code-braces: AddTagsToResourceRequestTypeDef](./type_defs.md#addtagstoresourcerequesttypedef) 

### associate\_ops\_item\_related\_item

Associates a related item to a Systems Manager OpsCenter OpsItem.

Type annotations and code completion for `#!python session.create_client("ssm").associate_ops_item_related_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/associate_ops_item_related_item.html)

```python
# associate_ops_item_related_item method definition

await def associate_ops_item_related_item(
    self,
    *,
    OpsItemId: str,
    AssociationType: str,
    ResourceType: str,
    ResourceUri: str,
) -> AssociateOpsItemRelatedItemResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateOpsItemRelatedItemResponseTypeDef](./type_defs.md#associateopsitemrelateditemresponsetypedef) 


```python
# associate_ops_item_related_item method usage example with argument unpacking

kwargs: AssociateOpsItemRelatedItemRequestTypeDef = {  # (1)
    "OpsItemId": ...,
    "AssociationType": ...,
    "ResourceType": ...,
    "ResourceUri": ...,
}

parent.associate_ops_item_related_item(**kwargs)
```

1. See [:material-code-braces: AssociateOpsItemRelatedItemRequestTypeDef](./type_defs.md#associateopsitemrelateditemrequesttypedef) 

### cancel\_command

Attempts to cancel the command specified by the Command ID.

Type annotations and code completion for `#!python session.create_client("ssm").cancel_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/cancel_command.html)

```python
# cancel_command method definition

await def cancel_command(
    self,
    *,
    CommandId: str,
    InstanceIds: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_command method usage example with argument unpacking

kwargs: CancelCommandRequestTypeDef = {  # (1)
    "CommandId": ...,
}

parent.cancel_command(**kwargs)
```

1. See [:material-code-braces: CancelCommandRequestTypeDef](./type_defs.md#cancelcommandrequesttypedef) 

### cancel\_maintenance\_window\_execution

Stops a maintenance window execution that is already in progress and cancels
any tasks in the window that haven't already starting running.

Type annotations and code completion for `#!python session.create_client("ssm").cancel_maintenance_window_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/cancel_maintenance_window_execution.html)

```python
# cancel_maintenance_window_execution method definition

await def cancel_maintenance_window_execution(
    self,
    *,
    WindowExecutionId: str,
) -> CancelMaintenanceWindowExecutionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelMaintenanceWindowExecutionResultTypeDef](./type_defs.md#cancelmaintenancewindowexecutionresulttypedef) 


```python
# cancel_maintenance_window_execution method usage example with argument unpacking

kwargs: CancelMaintenanceWindowExecutionRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
}

parent.cancel_maintenance_window_execution(**kwargs)
```

1. See [:material-code-braces: CancelMaintenanceWindowExecutionRequestTypeDef](./type_defs.md#cancelmaintenancewindowexecutionrequesttypedef) 

### create\_activation

Generates an activation code and activation ID you can use to register your
on-premises servers, edge devices, or virtual machine (VM) with Amazon Web
Services Systems Manager.

Type annotations and code completion for `#!python session.create_client("ssm").create_activation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_activation.html)

```python
# create_activation method definition

await def create_activation(
    self,
    *,
    IamRole: str,
    Description: str = ...,
    DefaultInstanceName: str = ...,
    RegistrationLimit: int = ...,
    ExpirationDate: TimestampTypeDef = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...,  # (2)
) -> CreateActivationResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: RegistrationMetadataItemTypeDef](./type_defs.md#registrationmetadataitemtypedef) 
3. See [:material-code-braces: CreateActivationResultTypeDef](./type_defs.md#createactivationresulttypedef) 


```python
# create_activation method usage example with argument unpacking

kwargs: CreateActivationRequestTypeDef = {  # (1)
    "IamRole": ...,
}

parent.create_activation(**kwargs)
```

1. See [:material-code-braces: CreateActivationRequestTypeDef](./type_defs.md#createactivationrequesttypedef) 

### create\_association

A State Manager association defines the state that you want to maintain on your
managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").create_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_association.html)

```python
# create_association method definition

await def create_association(
    self,
    *,
    Name: str,
    DocumentVersion: str = ...,
    InstanceId: str = ...,
    Parameters: Mapping[str, Sequence[str]] = ...,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (1)
    ScheduleExpression: str = ...,
    OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,  # (2)
    AssociationName: str = ...,
    AutomationTargetParameterName: str = ...,
    MaxErrors: str = ...,
    MaxConcurrency: str = ...,
    ComplianceSeverity: AssociationComplianceSeverityType = ...,  # (3)
    SyncCompliance: AssociationSyncComplianceType = ...,  # (4)
    ApplyOnlyAtCronInterval: bool = ...,
    CalendarNames: Sequence[str] = ...,
    TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,  # (5)
    ScheduleOffset: int = ...,
    Duration: int = ...,
    TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (7)
) -> CreateAssociationResultTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
8. See [:material-code-braces: CreateAssociationResultTypeDef](./type_defs.md#createassociationresulttypedef) 


```python
# create_association method usage example with argument unpacking

kwargs: CreateAssociationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_association(**kwargs)
```

1. See [:material-code-braces: CreateAssociationRequestTypeDef](./type_defs.md#createassociationrequesttypedef) 

### create\_association\_batch

Associates the specified Amazon Web Services Systems Manager document (SSM
document) with the specified managed nodes or targets.

Type annotations and code completion for `#!python session.create_client("ssm").create_association_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_association_batch.html)

```python
# create_association_batch method definition

await def create_association_batch(
    self,
    *,
    Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],  # (1)
) -> CreateAssociationBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateAssociationBatchRequestEntryTypeDef](./type_defs.md#createassociationbatchrequestentrytypedef) [:material-code-braces: CreateAssociationBatchRequestEntryOutputTypeDef](./type_defs.md#createassociationbatchrequestentryoutputtypedef) 
2. See [:material-code-braces: CreateAssociationBatchResultTypeDef](./type_defs.md#createassociationbatchresulttypedef) 


```python
# create_association_batch method usage example with argument unpacking

kwargs: CreateAssociationBatchRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.create_association_batch(**kwargs)
```

1. See [:material-code-braces: CreateAssociationBatchRequestTypeDef](./type_defs.md#createassociationbatchrequesttypedef) 

### create\_document

Creates a Amazon Web Services Systems Manager (SSM document).

Type annotations and code completion for `#!python session.create_client("ssm").create_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_document.html)

```python
# create_document method definition

await def create_document(
    self,
    *,
    Content: str,
    Name: str,
    Requires: Sequence[DocumentRequiresTypeDef] = ...,  # (1)
    Attachments: Sequence[AttachmentsSourceTypeDef] = ...,  # (2)
    DisplayName: str = ...,
    VersionName: str = ...,
    DocumentType: DocumentTypeType = ...,  # (3)
    DocumentFormat: DocumentFormatType = ...,  # (4)
    TargetType: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateDocumentResultTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DocumentRequiresTypeDef](./type_defs.md#documentrequirestypedef) 
2. See [:material-code-braces: AttachmentsSourceTypeDef](./type_defs.md#attachmentssourcetypedef) 
3. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
4. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateDocumentResultTypeDef](./type_defs.md#createdocumentresulttypedef) 


```python
# create_document method usage example with argument unpacking

kwargs: CreateDocumentRequestTypeDef = {  # (1)
    "Content": ...,
    "Name": ...,
}

parent.create_document(**kwargs)
```

1. See [:material-code-braces: CreateDocumentRequestTypeDef](./type_defs.md#createdocumentrequesttypedef) 

### create\_maintenance\_window

Creates a new maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").create_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_maintenance_window.html)

```python
# create_maintenance_window method definition

await def create_maintenance_window(
    self,
    *,
    Name: str,
    Schedule: str,
    Duration: int,
    Cutoff: int,
    AllowUnassociatedTargets: bool,
    Description: str = ...,
    StartDate: str = ...,
    EndDate: str = ...,
    ScheduleTimezone: str = ...,
    ScheduleOffset: int = ...,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateMaintenanceWindowResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateMaintenanceWindowResultTypeDef](./type_defs.md#createmaintenancewindowresulttypedef) 


```python
# create_maintenance_window method usage example with argument unpacking

kwargs: CreateMaintenanceWindowRequestTypeDef = {  # (1)
    "Name": ...,
    "Schedule": ...,
    "Duration": ...,
    "Cutoff": ...,
    "AllowUnassociatedTargets": ...,
}

parent.create_maintenance_window(**kwargs)
```

1. See [:material-code-braces: CreateMaintenanceWindowRequestTypeDef](./type_defs.md#createmaintenancewindowrequesttypedef) 

### create\_ops\_item

Creates a new OpsItem.

Type annotations and code completion for `#!python session.create_client("ssm").create_ops_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_ops_item.html)

```python
# create_ops_item method definition

await def create_ops_item(
    self,
    *,
    Description: str,
    Source: str,
    Title: str,
    OpsItemType: str = ...,
    OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,  # (1)
    Notifications: Sequence[OpsItemNotificationTypeDef] = ...,  # (2)
    Priority: int = ...,
    RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    Category: str = ...,
    Severity: str = ...,
    ActualStartTime: TimestampTypeDef = ...,
    ActualEndTime: TimestampTypeDef = ...,
    PlannedStartTime: TimestampTypeDef = ...,
    PlannedEndTime: TimestampTypeDef = ...,
    AccountId: str = ...,
) -> CreateOpsItemResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
2. See [:material-code-braces: OpsItemNotificationTypeDef](./type_defs.md#opsitemnotificationtypedef) 
3. See [:material-code-braces: RelatedOpsItemTypeDef](./type_defs.md#relatedopsitemtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateOpsItemResponseTypeDef](./type_defs.md#createopsitemresponsetypedef) 


```python
# create_ops_item method usage example with argument unpacking

kwargs: CreateOpsItemRequestTypeDef = {  # (1)
    "Description": ...,
    "Source": ...,
    "Title": ...,
}

parent.create_ops_item(**kwargs)
```

1. See [:material-code-braces: CreateOpsItemRequestTypeDef](./type_defs.md#createopsitemrequesttypedef) 

### create\_ops\_metadata

If you create a new application in Application Manager, Amazon Web Services
Systems Manager calls this API operation to specify information about the new
application, including the application type.

Type annotations and code completion for `#!python session.create_client("ssm").create_ops_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_ops_metadata.html)

```python
# create_ops_metadata method definition

await def create_ops_metadata(
    self,
    *,
    ResourceId: str,
    Metadata: Mapping[str, MetadataValueTypeDef] = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateOpsMetadataResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateOpsMetadataResultTypeDef](./type_defs.md#createopsmetadataresulttypedef) 


```python
# create_ops_metadata method usage example with argument unpacking

kwargs: CreateOpsMetadataRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.create_ops_metadata(**kwargs)
```

1. See [:material-code-braces: CreateOpsMetadataRequestTypeDef](./type_defs.md#createopsmetadatarequesttypedef) 

### create\_patch\_baseline

Creates a patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").create_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_patch_baseline.html)

```python
# create_patch_baseline method definition

await def create_patch_baseline(
    self,
    *,
    Name: str,
    OperatingSystem: OperatingSystemType = ...,  # (1)
    GlobalFilters: PatchFilterGroupUnionTypeDef = ...,  # (2)
    ApprovalRules: PatchRuleGroupUnionTypeDef = ...,  # (3)
    ApprovedPatches: Sequence[str] = ...,
    ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,  # (4)
    ApprovedPatchesEnableNonSecurity: bool = ...,
    RejectedPatches: Sequence[str] = ...,
    RejectedPatchesAction: PatchActionType = ...,  # (5)
    Description: str = ...,
    Sources: Sequence[PatchSourceUnionTypeDef] = ...,  # (6)
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (7)
) -> CreatePatchBaselineResultTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
3. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
4. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
5. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
6. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CreatePatchBaselineResultTypeDef](./type_defs.md#createpatchbaselineresulttypedef) 


```python
# create_patch_baseline method usage example with argument unpacking

kwargs: CreatePatchBaselineRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_patch_baseline(**kwargs)
```

1. See [:material-code-braces: CreatePatchBaselineRequestTypeDef](./type_defs.md#createpatchbaselinerequesttypedef) 

### create\_resource\_data\_sync

A resource data sync helps you view data from multiple sources in a single
location.

Type annotations and code completion for `#!python session.create_client("ssm").create_resource_data_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/create_resource_data_sync.html)

```python
# create_resource_data_sync method definition

await def create_resource_data_sync(
    self,
    *,
    SyncName: str,
    S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,  # (1)
    SyncType: str = ...,
    SyncSource: ResourceDataSyncSourceTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceDataSyncS3DestinationTypeDef](./type_defs.md#resourcedatasyncs3destinationtypedef) 
2. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 


```python
# create_resource_data_sync method usage example with argument unpacking

kwargs: CreateResourceDataSyncRequestTypeDef = {  # (1)
    "SyncName": ...,
}

parent.create_resource_data_sync(**kwargs)
```

1. See [:material-code-braces: CreateResourceDataSyncRequestTypeDef](./type_defs.md#createresourcedatasyncrequesttypedef) 

### delete\_activation

Deletes an activation.

Type annotations and code completion for `#!python session.create_client("ssm").delete_activation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_activation.html)

```python
# delete_activation method definition

await def delete_activation(
    self,
    *,
    ActivationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_activation method usage example with argument unpacking

kwargs: DeleteActivationRequestTypeDef = {  # (1)
    "ActivationId": ...,
}

parent.delete_activation(**kwargs)
```

1. See [:material-code-braces: DeleteActivationRequestTypeDef](./type_defs.md#deleteactivationrequesttypedef) 

### delete\_association

Disassociates the specified Amazon Web Services Systems Manager document (SSM
document) from the specified managed node.

Type annotations and code completion for `#!python session.create_client("ssm").delete_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_association.html)

```python
# delete_association method definition

await def delete_association(
    self,
    *,
    Name: str = ...,
    InstanceId: str = ...,
    AssociationId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_association method usage example with argument unpacking

kwargs: DeleteAssociationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_association(**kwargs)
```

1. See [:material-code-braces: DeleteAssociationRequestTypeDef](./type_defs.md#deleteassociationrequesttypedef) 

### delete\_document

Deletes the Amazon Web Services Systems Manager document (SSM document) and all
managed node associations to the document.

Type annotations and code completion for `#!python session.create_client("ssm").delete_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_document.html)

```python
# delete_document method definition

await def delete_document(
    self,
    *,
    Name: str,
    DocumentVersion: str = ...,
    VersionName: str = ...,
    Force: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_document method usage example with argument unpacking

kwargs: DeleteDocumentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_document(**kwargs)
```

1. See [:material-code-braces: DeleteDocumentRequestTypeDef](./type_defs.md#deletedocumentrequesttypedef) 

### delete\_inventory

Delete a custom inventory type or the data associated with a custom Inventory
type.

Type annotations and code completion for `#!python session.create_client("ssm").delete_inventory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_inventory.html)

```python
# delete_inventory method definition

await def delete_inventory(
    self,
    *,
    TypeName: str,
    SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,  # (1)
    DryRun: bool = ...,
    ClientToken: str = ...,
) -> DeleteInventoryResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InventorySchemaDeleteOptionType](./literals.md#inventoryschemadeleteoptiontype) 
2. See [:material-code-braces: DeleteInventoryResultTypeDef](./type_defs.md#deleteinventoryresulttypedef) 


```python
# delete_inventory method usage example with argument unpacking

kwargs: DeleteInventoryRequestTypeDef = {  # (1)
    "TypeName": ...,
}

parent.delete_inventory(**kwargs)
```

1. See [:material-code-braces: DeleteInventoryRequestTypeDef](./type_defs.md#deleteinventoryrequesttypedef) 

### delete\_maintenance\_window

Deletes a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").delete_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_maintenance_window.html)

```python
# delete_maintenance_window method definition

await def delete_maintenance_window(
    self,
    *,
    WindowId: str,
) -> DeleteMaintenanceWindowResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMaintenanceWindowResultTypeDef](./type_defs.md#deletemaintenancewindowresulttypedef) 


```python
# delete_maintenance_window method usage example with argument unpacking

kwargs: DeleteMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.delete_maintenance_window(**kwargs)
```

1. See [:material-code-braces: DeleteMaintenanceWindowRequestTypeDef](./type_defs.md#deletemaintenancewindowrequesttypedef) 

### delete\_ops\_item

Delete an OpsItem.

Type annotations and code completion for `#!python session.create_client("ssm").delete_ops_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_ops_item.html)

```python
# delete_ops_item method definition

await def delete_ops_item(
    self,
    *,
    OpsItemId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ops_item method usage example with argument unpacking

kwargs: DeleteOpsItemRequestTypeDef = {  # (1)
    "OpsItemId": ...,
}

parent.delete_ops_item(**kwargs)
```

1. See [:material-code-braces: DeleteOpsItemRequestTypeDef](./type_defs.md#deleteopsitemrequesttypedef) 

### delete\_ops\_metadata

Delete OpsMetadata related to an application.

Type annotations and code completion for `#!python session.create_client("ssm").delete_ops_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_ops_metadata.html)

```python
# delete_ops_metadata method definition

await def delete_ops_metadata(
    self,
    *,
    OpsMetadataArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ops_metadata method usage example with argument unpacking

kwargs: DeleteOpsMetadataRequestTypeDef = {  # (1)
    "OpsMetadataArn": ...,
}

parent.delete_ops_metadata(**kwargs)
```

1. See [:material-code-braces: DeleteOpsMetadataRequestTypeDef](./type_defs.md#deleteopsmetadatarequesttypedef) 

### delete\_parameter

Delete a parameter from the system.

Type annotations and code completion for `#!python session.create_client("ssm").delete_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_parameter.html)

```python
# delete_parameter method definition

await def delete_parameter(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_parameter method usage example with argument unpacking

kwargs: DeleteParameterRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_parameter(**kwargs)
```

1. See [:material-code-braces: DeleteParameterRequestTypeDef](./type_defs.md#deleteparameterrequesttypedef) 

### delete\_parameters

Delete a list of parameters.

Type annotations and code completion for `#!python session.create_client("ssm").delete_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_parameters.html)

```python
# delete_parameters method definition

await def delete_parameters(
    self,
    *,
    Names: Sequence[str],
) -> DeleteParametersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteParametersResultTypeDef](./type_defs.md#deleteparametersresulttypedef) 


```python
# delete_parameters method usage example with argument unpacking

kwargs: DeleteParametersRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.delete_parameters(**kwargs)
```

1. See [:material-code-braces: DeleteParametersRequestTypeDef](./type_defs.md#deleteparametersrequesttypedef) 

### delete\_patch\_baseline

Deletes a patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").delete_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_patch_baseline.html)

```python
# delete_patch_baseline method definition

await def delete_patch_baseline(
    self,
    *,
    BaselineId: str,
) -> DeletePatchBaselineResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePatchBaselineResultTypeDef](./type_defs.md#deletepatchbaselineresulttypedef) 


```python
# delete_patch_baseline method usage example with argument unpacking

kwargs: DeletePatchBaselineRequestTypeDef = {  # (1)
    "BaselineId": ...,
}

parent.delete_patch_baseline(**kwargs)
```

1. See [:material-code-braces: DeletePatchBaselineRequestTypeDef](./type_defs.md#deletepatchbaselinerequesttypedef) 

### delete\_resource\_data\_sync

Deletes a resource data sync configuration.

Type annotations and code completion for `#!python session.create_client("ssm").delete_resource_data_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_resource_data_sync.html)

```python
# delete_resource_data_sync method definition

await def delete_resource_data_sync(
    self,
    *,
    SyncName: str,
    SyncType: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource_data_sync method usage example with argument unpacking

kwargs: DeleteResourceDataSyncRequestTypeDef = {  # (1)
    "SyncName": ...,
}

parent.delete_resource_data_sync(**kwargs)
```

1. See [:material-code-braces: DeleteResourceDataSyncRequestTypeDef](./type_defs.md#deleteresourcedatasyncrequesttypedef) 

### delete\_resource\_policy

Deletes a Systems Manager resource policy.

Type annotations and code completion for `#!python session.create_client("ssm").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/delete_resource_policy.html)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
    PolicyId: str,
    PolicyHash: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "PolicyId": ...,
    "PolicyHash": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestTypeDef](./type_defs.md#deleteresourcepolicyrequesttypedef) 

### deregister\_managed\_instance

Removes the server or virtual machine from the list of registered servers.

Type annotations and code completion for `#!python session.create_client("ssm").deregister_managed_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/deregister_managed_instance.html)

```python
# deregister_managed_instance method definition

await def deregister_managed_instance(
    self,
    *,
    InstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_managed_instance method usage example with argument unpacking

kwargs: DeregisterManagedInstanceRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.deregister_managed_instance(**kwargs)
```

1. See [:material-code-braces: DeregisterManagedInstanceRequestTypeDef](./type_defs.md#deregistermanagedinstancerequesttypedef) 

### deregister\_patch\_baseline\_for\_patch\_group

Removes a patch group from a patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").deregister_patch_baseline_for_patch_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/deregister_patch_baseline_for_patch_group.html)

```python
# deregister_patch_baseline_for_patch_group method definition

await def deregister_patch_baseline_for_patch_group(
    self,
    *,
    BaselineId: str,
    PatchGroup: str,
) -> DeregisterPatchBaselineForPatchGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterPatchBaselineForPatchGroupResultTypeDef](./type_defs.md#deregisterpatchbaselineforpatchgroupresulttypedef) 


```python
# deregister_patch_baseline_for_patch_group method usage example with argument unpacking

kwargs: DeregisterPatchBaselineForPatchGroupRequestTypeDef = {  # (1)
    "BaselineId": ...,
    "PatchGroup": ...,
}

parent.deregister_patch_baseline_for_patch_group(**kwargs)
```

1. See [:material-code-braces: DeregisterPatchBaselineForPatchGroupRequestTypeDef](./type_defs.md#deregisterpatchbaselineforpatchgrouprequesttypedef) 

### deregister\_target\_from\_maintenance\_window

Removes a target from a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").deregister_target_from_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/deregister_target_from_maintenance_window.html)

```python
# deregister_target_from_maintenance_window method definition

await def deregister_target_from_maintenance_window(
    self,
    *,
    WindowId: str,
    WindowTargetId: str,
    Safe: bool = ...,
) -> DeregisterTargetFromMaintenanceWindowResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterTargetFromMaintenanceWindowResultTypeDef](./type_defs.md#deregistertargetfrommaintenancewindowresulttypedef) 


```python
# deregister_target_from_maintenance_window method usage example with argument unpacking

kwargs: DeregisterTargetFromMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
    "WindowTargetId": ...,
}

parent.deregister_target_from_maintenance_window(**kwargs)
```

1. See [:material-code-braces: DeregisterTargetFromMaintenanceWindowRequestTypeDef](./type_defs.md#deregistertargetfrommaintenancewindowrequesttypedef) 

### deregister\_task\_from\_maintenance\_window

Removes a task from a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").deregister_task_from_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/deregister_task_from_maintenance_window.html)

```python
# deregister_task_from_maintenance_window method definition

await def deregister_task_from_maintenance_window(
    self,
    *,
    WindowId: str,
    WindowTaskId: str,
) -> DeregisterTaskFromMaintenanceWindowResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterTaskFromMaintenanceWindowResultTypeDef](./type_defs.md#deregistertaskfrommaintenancewindowresulttypedef) 


```python
# deregister_task_from_maintenance_window method usage example with argument unpacking

kwargs: DeregisterTaskFromMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
    "WindowTaskId": ...,
}

parent.deregister_task_from_maintenance_window(**kwargs)
```

1. See [:material-code-braces: DeregisterTaskFromMaintenanceWindowRequestTypeDef](./type_defs.md#deregistertaskfrommaintenancewindowrequesttypedef) 

### describe\_activations

Describes details about the activation, such as the date and time the
activation was created, its expiration date, the Identity and Access Management
(IAM) role assigned to the managed nodes in the activation, and the number of
nodes registered by using this activation.

Type annotations and code completion for `#!python session.create_client("ssm").describe_activations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_activations.html)

```python
# describe_activations method definition

await def describe_activations(
    self,
    *,
    Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeActivationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeActivationsFilterTypeDef](./type_defs.md#describeactivationsfiltertypedef) 
2. See [:material-code-braces: DescribeActivationsResultTypeDef](./type_defs.md#describeactivationsresulttypedef) 


```python
# describe_activations method usage example with argument unpacking

kwargs: DescribeActivationsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_activations(**kwargs)
```

1. See [:material-code-braces: DescribeActivationsRequestTypeDef](./type_defs.md#describeactivationsrequesttypedef) 

### describe\_association

Describes the association for the specified target or managed node.

Type annotations and code completion for `#!python session.create_client("ssm").describe_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_association.html)

```python
# describe_association method definition

await def describe_association(
    self,
    *,
    Name: str = ...,
    InstanceId: str = ...,
    AssociationId: str = ...,
    AssociationVersion: str = ...,
) -> DescribeAssociationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssociationResultTypeDef](./type_defs.md#describeassociationresulttypedef) 


```python
# describe_association method usage example with argument unpacking

kwargs: DescribeAssociationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_association(**kwargs)
```

1. See [:material-code-braces: DescribeAssociationRequestTypeDef](./type_defs.md#describeassociationrequesttypedef) 

### describe\_association\_execution\_targets

Views information about a specific execution of a specific association.

Type annotations and code completion for `#!python session.create_client("ssm").describe_association_execution_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_association_execution_targets.html)

```python
# describe_association_execution_targets method definition

await def describe_association_execution_targets(
    self,
    *,
    AssociationId: str,
    ExecutionId: str,
    Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeAssociationExecutionTargetsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociationExecutionTargetsFilterTypeDef](./type_defs.md#associationexecutiontargetsfiltertypedef) 
2. See [:material-code-braces: DescribeAssociationExecutionTargetsResultTypeDef](./type_defs.md#describeassociationexecutiontargetsresulttypedef) 


```python
# describe_association_execution_targets method usage example with argument unpacking

kwargs: DescribeAssociationExecutionTargetsRequestTypeDef = {  # (1)
    "AssociationId": ...,
    "ExecutionId": ...,
}

parent.describe_association_execution_targets(**kwargs)
```

1. See [:material-code-braces: DescribeAssociationExecutionTargetsRequestTypeDef](./type_defs.md#describeassociationexecutiontargetsrequesttypedef) 

### describe\_association\_executions

Views all executions for a specific association ID.

Type annotations and code completion for `#!python session.create_client("ssm").describe_association_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_association_executions.html)

```python
# describe_association_executions method definition

await def describe_association_executions(
    self,
    *,
    AssociationId: str,
    Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeAssociationExecutionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociationExecutionFilterTypeDef](./type_defs.md#associationexecutionfiltertypedef) 
2. See [:material-code-braces: DescribeAssociationExecutionsResultTypeDef](./type_defs.md#describeassociationexecutionsresulttypedef) 


```python
# describe_association_executions method usage example with argument unpacking

kwargs: DescribeAssociationExecutionsRequestTypeDef = {  # (1)
    "AssociationId": ...,
}

parent.describe_association_executions(**kwargs)
```

1. See [:material-code-braces: DescribeAssociationExecutionsRequestTypeDef](./type_defs.md#describeassociationexecutionsrequesttypedef) 

### describe\_automation\_executions

Provides details about all active and terminated Automation executions.

Type annotations and code completion for `#!python session.create_client("ssm").describe_automation_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_automation_executions.html)

```python
# describe_automation_executions method definition

await def describe_automation_executions(
    self,
    *,
    Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeAutomationExecutionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AutomationExecutionFilterTypeDef](./type_defs.md#automationexecutionfiltertypedef) 
2. See [:material-code-braces: DescribeAutomationExecutionsResultTypeDef](./type_defs.md#describeautomationexecutionsresulttypedef) 


```python
# describe_automation_executions method usage example with argument unpacking

kwargs: DescribeAutomationExecutionsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_automation_executions(**kwargs)
```

1. See [:material-code-braces: DescribeAutomationExecutionsRequestTypeDef](./type_defs.md#describeautomationexecutionsrequesttypedef) 

### describe\_automation\_step\_executions

Information about all active and terminated step executions in an Automation
workflow.

Type annotations and code completion for `#!python session.create_client("ssm").describe_automation_step_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_automation_step_executions.html)

```python
# describe_automation_step_executions method definition

await def describe_automation_step_executions(
    self,
    *,
    AutomationExecutionId: str,
    Filters: Sequence[StepExecutionFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    ReverseOrder: bool = ...,
) -> DescribeAutomationStepExecutionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StepExecutionFilterTypeDef](./type_defs.md#stepexecutionfiltertypedef) 
2. See [:material-code-braces: DescribeAutomationStepExecutionsResultTypeDef](./type_defs.md#describeautomationstepexecutionsresulttypedef) 


```python
# describe_automation_step_executions method usage example with argument unpacking

kwargs: DescribeAutomationStepExecutionsRequestTypeDef = {  # (1)
    "AutomationExecutionId": ...,
}

parent.describe_automation_step_executions(**kwargs)
```

1. See [:material-code-braces: DescribeAutomationStepExecutionsRequestTypeDef](./type_defs.md#describeautomationstepexecutionsrequesttypedef) 

### describe\_available\_patches

Lists all patches eligible to be included in a patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").describe_available_patches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_available_patches.html)

```python
# describe_available_patches method definition

await def describe_available_patches(
    self,
    *,
    Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeAvailablePatchesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: DescribeAvailablePatchesResultTypeDef](./type_defs.md#describeavailablepatchesresulttypedef) 


```python
# describe_available_patches method usage example with argument unpacking

kwargs: DescribeAvailablePatchesRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_available_patches(**kwargs)
```

1. See [:material-code-braces: DescribeAvailablePatchesRequestTypeDef](./type_defs.md#describeavailablepatchesrequesttypedef) 

### describe\_document

Describes the specified Amazon Web Services Systems Manager document (SSM
document).

Type annotations and code completion for `#!python session.create_client("ssm").describe_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_document.html)

```python
# describe_document method definition

await def describe_document(
    self,
    *,
    Name: str,
    DocumentVersion: str = ...,
    VersionName: str = ...,
) -> DescribeDocumentResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDocumentResultTypeDef](./type_defs.md#describedocumentresulttypedef) 


```python
# describe_document method usage example with argument unpacking

kwargs: DescribeDocumentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_document(**kwargs)
```

1. See [:material-code-braces: DescribeDocumentRequestTypeDef](./type_defs.md#describedocumentrequesttypedef) 

### describe\_document\_permission

Describes the permissions for a Amazon Web Services Systems Manager document
(SSM document).

Type annotations and code completion for `#!python session.create_client("ssm").describe_document_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_document_permission.html)

```python
# describe_document_permission method definition

await def describe_document_permission(
    self,
    *,
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeDocumentPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 
2. See [:material-code-braces: DescribeDocumentPermissionResponseTypeDef](./type_defs.md#describedocumentpermissionresponsetypedef) 


```python
# describe_document_permission method usage example with argument unpacking

kwargs: DescribeDocumentPermissionRequestTypeDef = {  # (1)
    "Name": ...,
    "PermissionType": ...,
}

parent.describe_document_permission(**kwargs)
```

1. See [:material-code-braces: DescribeDocumentPermissionRequestTypeDef](./type_defs.md#describedocumentpermissionrequesttypedef) 

### describe\_effective\_instance\_associations

All associations for the managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").describe_effective_instance_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_effective_instance_associations.html)

```python
# describe_effective_instance_associations method definition

await def describe_effective_instance_associations(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeEffectiveInstanceAssociationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEffectiveInstanceAssociationsResultTypeDef](./type_defs.md#describeeffectiveinstanceassociationsresulttypedef) 


```python
# describe_effective_instance_associations method usage example with argument unpacking

kwargs: DescribeEffectiveInstanceAssociationsRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_effective_instance_associations(**kwargs)
```

1. See [:material-code-braces: DescribeEffectiveInstanceAssociationsRequestTypeDef](./type_defs.md#describeeffectiveinstanceassociationsrequesttypedef) 

### describe\_effective\_patches\_for\_patch\_baseline

Retrieves the current effective patches (the patch and the approval state) for
the specified patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").describe_effective_patches_for_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_effective_patches_for_patch_baseline.html)

```python
# describe_effective_patches_for_patch_baseline method definition

await def describe_effective_patches_for_patch_baseline(
    self,
    *,
    BaselineId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEffectivePatchesForPatchBaselineResultTypeDef](./type_defs.md#describeeffectivepatchesforpatchbaselineresulttypedef) 


```python
# describe_effective_patches_for_patch_baseline method usage example with argument unpacking

kwargs: DescribeEffectivePatchesForPatchBaselineRequestTypeDef = {  # (1)
    "BaselineId": ...,
}

parent.describe_effective_patches_for_patch_baseline(**kwargs)
```

1. See [:material-code-braces: DescribeEffectivePatchesForPatchBaselineRequestTypeDef](./type_defs.md#describeeffectivepatchesforpatchbaselinerequesttypedef) 

### describe\_instance\_associations\_status

The status of the associations for the managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_associations_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_associations_status.html)

```python
# describe_instance_associations_status method definition

await def describe_instance_associations_status(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeInstanceAssociationsStatusResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstanceAssociationsStatusResultTypeDef](./type_defs.md#describeinstanceassociationsstatusresulttypedef) 


```python
# describe_instance_associations_status method usage example with argument unpacking

kwargs: DescribeInstanceAssociationsStatusRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_instance_associations_status(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceAssociationsStatusRequestTypeDef](./type_defs.md#describeinstanceassociationsstatusrequesttypedef) 

### describe\_instance\_information

Provides information about one or more of your managed nodes, including the
operating system platform, SSM Agent version, association status, and IP
address.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_information` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_information.html)

```python
# describe_instance_information method definition

await def describe_instance_information(
    self,
    *,
    InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,  # (1)
    Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeInstanceInformationResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InstanceInformationFilterTypeDef](./type_defs.md#instanceinformationfiltertypedef) 
2. See [:material-code-braces: InstanceInformationStringFilterTypeDef](./type_defs.md#instanceinformationstringfiltertypedef) 
3. See [:material-code-braces: DescribeInstanceInformationResultTypeDef](./type_defs.md#describeinstanceinformationresulttypedef) 


```python
# describe_instance_information method usage example with argument unpacking

kwargs: DescribeInstanceInformationRequestTypeDef = {  # (1)
    "InstanceInformationFilterList": ...,
}

parent.describe_instance_information(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceInformationRequestTypeDef](./type_defs.md#describeinstanceinformationrequesttypedef) 

### describe\_instance\_patch\_states

Retrieves the high-level patch state of one or more managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_patch_states` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_patch_states.html)

```python
# describe_instance_patch_states method definition

await def describe_instance_patch_states(
    self,
    *,
    InstanceIds: Sequence[str],
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeInstancePatchStatesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstancePatchStatesResultTypeDef](./type_defs.md#describeinstancepatchstatesresulttypedef) 


```python
# describe_instance_patch_states method usage example with argument unpacking

kwargs: DescribeInstancePatchStatesRequestTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.describe_instance_patch_states(**kwargs)
```

1. See [:material-code-braces: DescribeInstancePatchStatesRequestTypeDef](./type_defs.md#describeinstancepatchstatesrequesttypedef) 

### describe\_instance\_patch\_states\_for\_patch\_group

Retrieves the high-level patch state for the managed nodes in the specified
patch group.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_patch_states_for_patch_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_patch_states_for_patch_group.html)

```python
# describe_instance_patch_states_for_patch_group method definition

await def describe_instance_patch_states_for_patch_group(
    self,
    *,
    PatchGroup: str,
    Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeInstancePatchStatesForPatchGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstancePatchStateFilterTypeDef](./type_defs.md#instancepatchstatefiltertypedef) 
2. See [:material-code-braces: DescribeInstancePatchStatesForPatchGroupResultTypeDef](./type_defs.md#describeinstancepatchstatesforpatchgroupresulttypedef) 


```python
# describe_instance_patch_states_for_patch_group method usage example with argument unpacking

kwargs: DescribeInstancePatchStatesForPatchGroupRequestTypeDef = {  # (1)
    "PatchGroup": ...,
}

parent.describe_instance_patch_states_for_patch_group(**kwargs)
```

1. See [:material-code-braces: DescribeInstancePatchStatesForPatchGroupRequestTypeDef](./type_defs.md#describeinstancepatchstatesforpatchgrouprequesttypedef) 

### describe\_instance\_patches

Retrieves information about the patches on the specified managed node and their
state relative to the patch baseline being used for the node.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_patches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_patches.html)

```python
# describe_instance_patches method definition

await def describe_instance_patches(
    self,
    *,
    InstanceId: str,
    Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeInstancePatchesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: DescribeInstancePatchesResultTypeDef](./type_defs.md#describeinstancepatchesresulttypedef) 


```python
# describe_instance_patches method usage example with argument unpacking

kwargs: DescribeInstancePatchesRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_instance_patches(**kwargs)
```

1. See [:material-code-braces: DescribeInstancePatchesRequestTypeDef](./type_defs.md#describeinstancepatchesrequesttypedef) 

### describe\_instance\_properties

An API operation used by the Systems Manager console to display information
about Systems Manager managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").describe_instance_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_instance_properties.html)

```python
# describe_instance_properties method definition

await def describe_instance_properties(
    self,
    *,
    InstancePropertyFilterList: Sequence[InstancePropertyFilterTypeDef] = ...,  # (1)
    FiltersWithOperator: Sequence[InstancePropertyStringFilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeInstancePropertiesResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InstancePropertyFilterTypeDef](./type_defs.md#instancepropertyfiltertypedef) 
2. See [:material-code-braces: InstancePropertyStringFilterTypeDef](./type_defs.md#instancepropertystringfiltertypedef) 
3. See [:material-code-braces: DescribeInstancePropertiesResultTypeDef](./type_defs.md#describeinstancepropertiesresulttypedef) 


```python
# describe_instance_properties method usage example with argument unpacking

kwargs: DescribeInstancePropertiesRequestTypeDef = {  # (1)
    "InstancePropertyFilterList": ...,
}

parent.describe_instance_properties(**kwargs)
```

1. See [:material-code-braces: DescribeInstancePropertiesRequestTypeDef](./type_defs.md#describeinstancepropertiesrequesttypedef) 

### describe\_inventory\_deletions

Describes a specific delete inventory operation.

Type annotations and code completion for `#!python session.create_client("ssm").describe_inventory_deletions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_inventory_deletions.html)

```python
# describe_inventory_deletions method definition

await def describe_inventory_deletions(
    self,
    *,
    DeletionId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeInventoryDeletionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInventoryDeletionsResultTypeDef](./type_defs.md#describeinventorydeletionsresulttypedef) 


```python
# describe_inventory_deletions method usage example with argument unpacking

kwargs: DescribeInventoryDeletionsRequestTypeDef = {  # (1)
    "DeletionId": ...,
}

parent.describe_inventory_deletions(**kwargs)
```

1. See [:material-code-braces: DescribeInventoryDeletionsRequestTypeDef](./type_defs.md#describeinventorydeletionsrequesttypedef) 

### describe\_maintenance\_window\_execution\_task\_invocations

Retrieves the individual task executions (one per target) for a particular task
run as part of a maintenance window execution.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_execution_task_invocations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_execution_task_invocations.html)

```python
# describe_maintenance_window_execution_task_invocations method definition

await def describe_maintenance_window_execution_task_invocations(
    self,
    *,
    WindowExecutionId: str,
    TaskId: str,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef](./type_defs.md#describemaintenancewindowexecutiontaskinvocationsresulttypedef) 


```python
# describe_maintenance_window_execution_task_invocations method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
    "TaskId": ...,
}

parent.describe_maintenance_window_execution_task_invocations(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowExecutionTaskInvocationsRequestTypeDef](./type_defs.md#describemaintenancewindowexecutiontaskinvocationsrequesttypedef) 

### describe\_maintenance\_window\_execution\_tasks

For a given maintenance window execution, lists the tasks that were run.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_execution_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_execution_tasks.html)

```python
# describe_maintenance_window_execution_tasks method definition

await def describe_maintenance_window_execution_tasks(
    self,
    *,
    WindowExecutionId: str,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowExecutionTasksResultTypeDef](./type_defs.md#describemaintenancewindowexecutiontasksresulttypedef) 


```python
# describe_maintenance_window_execution_tasks method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowExecutionTasksRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
}

parent.describe_maintenance_window_execution_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowExecutionTasksRequestTypeDef](./type_defs.md#describemaintenancewindowexecutiontasksrequesttypedef) 

### describe\_maintenance\_window\_executions

Lists the executions of a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_executions.html)

```python
# describe_maintenance_window_executions method definition

await def describe_maintenance_window_executions(
    self,
    *,
    WindowId: str,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowExecutionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowExecutionsResultTypeDef](./type_defs.md#describemaintenancewindowexecutionsresulttypedef) 


```python
# describe_maintenance_window_executions method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowExecutionsRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.describe_maintenance_window_executions(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowExecutionsRequestTypeDef](./type_defs.md#describemaintenancewindowexecutionsrequesttypedef) 

### describe\_maintenance\_window\_schedule

Retrieves information about upcoming executions of a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_schedule.html)

```python
# describe_maintenance_window_schedule method definition

await def describe_maintenance_window_schedule(
    self,
    *,
    WindowId: str = ...,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (1)
    ResourceType: MaintenanceWindowResourceTypeType = ...,  # (2)
    Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowScheduleResultTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
4. See [:material-code-braces: DescribeMaintenanceWindowScheduleResultTypeDef](./type_defs.md#describemaintenancewindowscheduleresulttypedef) 


```python
# describe_maintenance_window_schedule method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowScheduleRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.describe_maintenance_window_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowScheduleRequestTypeDef](./type_defs.md#describemaintenancewindowschedulerequesttypedef) 

### describe\_maintenance\_window\_targets

Lists the targets registered with the maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_targets.html)

```python
# describe_maintenance_window_targets method definition

await def describe_maintenance_window_targets(
    self,
    *,
    WindowId: str,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowTargetsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowTargetsResultTypeDef](./type_defs.md#describemaintenancewindowtargetsresulttypedef) 


```python
# describe_maintenance_window_targets method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowTargetsRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.describe_maintenance_window_targets(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowTargetsRequestTypeDef](./type_defs.md#describemaintenancewindowtargetsrequesttypedef) 

### describe\_maintenance\_window\_tasks

Lists the tasks in a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_window_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_window_tasks.html)

```python
# describe_maintenance_window_tasks method definition

await def describe_maintenance_window_tasks(
    self,
    *,
    WindowId: str,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowTasksResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowTasksResultTypeDef](./type_defs.md#describemaintenancewindowtasksresulttypedef) 


```python
# describe_maintenance_window_tasks method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowTasksRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.describe_maintenance_window_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowTasksRequestTypeDef](./type_defs.md#describemaintenancewindowtasksrequesttypedef) 

### describe\_maintenance\_windows

Retrieves the maintenance windows in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_windows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_windows.html)

```python
# describe_maintenance_windows method definition

await def describe_maintenance_windows(
    self,
    *,
    Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MaintenanceWindowFilterTypeDef](./type_defs.md#maintenancewindowfiltertypedef) 
2. See [:material-code-braces: DescribeMaintenanceWindowsResultTypeDef](./type_defs.md#describemaintenancewindowsresulttypedef) 


```python
# describe_maintenance_windows method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_maintenance_windows(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowsRequestTypeDef](./type_defs.md#describemaintenancewindowsrequesttypedef) 

### describe\_maintenance\_windows\_for\_target

Retrieves information about the maintenance window targets or tasks that a
managed node is associated with.

Type annotations and code completion for `#!python session.create_client("ssm").describe_maintenance_windows_for_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_maintenance_windows_for_target.html)

```python
# describe_maintenance_windows_for_target method definition

await def describe_maintenance_windows_for_target(
    self,
    *,
    Targets: Sequence[TargetUnionTypeDef],  # (1)
    ResourceType: MaintenanceWindowResourceTypeType,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMaintenanceWindowsForTargetResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
3. See [:material-code-braces: DescribeMaintenanceWindowsForTargetResultTypeDef](./type_defs.md#describemaintenancewindowsfortargetresulttypedef) 


```python
# describe_maintenance_windows_for_target method usage example with argument unpacking

kwargs: DescribeMaintenanceWindowsForTargetRequestTypeDef = {  # (1)
    "Targets": ...,
    "ResourceType": ...,
}

parent.describe_maintenance_windows_for_target(**kwargs)
```

1. See [:material-code-braces: DescribeMaintenanceWindowsForTargetRequestTypeDef](./type_defs.md#describemaintenancewindowsfortargetrequesttypedef) 

### describe\_ops\_items

Query a set of OpsItems.

Type annotations and code completion for `#!python session.create_client("ssm").describe_ops_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_ops_items.html)

```python
# describe_ops_items method definition

await def describe_ops_items(
    self,
    *,
    OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeOpsItemsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OpsItemFilterTypeDef](./type_defs.md#opsitemfiltertypedef) 
2. See [:material-code-braces: DescribeOpsItemsResponseTypeDef](./type_defs.md#describeopsitemsresponsetypedef) 


```python
# describe_ops_items method usage example with argument unpacking

kwargs: DescribeOpsItemsRequestTypeDef = {  # (1)
    "OpsItemFilters": ...,
}

parent.describe_ops_items(**kwargs)
```

1. See [:material-code-braces: DescribeOpsItemsRequestTypeDef](./type_defs.md#describeopsitemsrequesttypedef) 

### describe\_parameters

Lists the parameters in your Amazon Web Services account or the parameters
shared with you when you enable the <a
href="https://docs.aws.amazon.com/systems-manager/latest/APIReference/API_DescribeParameters.html#systemsmanager-DescribeParameters-request-Shared">Shared</a>
option.

Type annotations and code completion for `#!python session.create_client("ssm").describe_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_parameters.html)

```python
# describe_parameters method definition

await def describe_parameters(
    self,
    *,
    Filters: Sequence[ParametersFilterTypeDef] = ...,  # (1)
    ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
    Shared: bool = ...,
) -> DescribeParametersResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ParametersFilterTypeDef](./type_defs.md#parametersfiltertypedef) 
2. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
3. See [:material-code-braces: DescribeParametersResultTypeDef](./type_defs.md#describeparametersresulttypedef) 


```python
# describe_parameters method usage example with argument unpacking

kwargs: DescribeParametersRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_parameters(**kwargs)
```

1. See [:material-code-braces: DescribeParametersRequestTypeDef](./type_defs.md#describeparametersrequesttypedef) 

### describe\_patch\_baselines

Lists the patch baselines in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("ssm").describe_patch_baselines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_patch_baselines.html)

```python
# describe_patch_baselines method definition

await def describe_patch_baselines(
    self,
    *,
    Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribePatchBaselinesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: DescribePatchBaselinesResultTypeDef](./type_defs.md#describepatchbaselinesresulttypedef) 


```python
# describe_patch_baselines method usage example with argument unpacking

kwargs: DescribePatchBaselinesRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_patch_baselines(**kwargs)
```

1. See [:material-code-braces: DescribePatchBaselinesRequestTypeDef](./type_defs.md#describepatchbaselinesrequesttypedef) 

### describe\_patch\_group\_state

Returns high-level aggregated patch compliance state information for a patch
group.

Type annotations and code completion for `#!python session.create_client("ssm").describe_patch_group_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_patch_group_state.html)

```python
# describe_patch_group_state method definition

await def describe_patch_group_state(
    self,
    *,
    PatchGroup: str,
) -> DescribePatchGroupStateResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePatchGroupStateResultTypeDef](./type_defs.md#describepatchgroupstateresulttypedef) 


```python
# describe_patch_group_state method usage example with argument unpacking

kwargs: DescribePatchGroupStateRequestTypeDef = {  # (1)
    "PatchGroup": ...,
}

parent.describe_patch_group_state(**kwargs)
```

1. See [:material-code-braces: DescribePatchGroupStateRequestTypeDef](./type_defs.md#describepatchgroupstaterequesttypedef) 

### describe\_patch\_groups

Lists all patch groups that have been registered with patch baselines.

Type annotations and code completion for `#!python session.create_client("ssm").describe_patch_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_patch_groups.html)

```python
# describe_patch_groups method definition

await def describe_patch_groups(
    self,
    *,
    MaxResults: int = ...,
    Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
) -> DescribePatchGroupsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOrchestratorFilterTypeDef](./type_defs.md#patchorchestratorfiltertypedef) 
2. See [:material-code-braces: DescribePatchGroupsResultTypeDef](./type_defs.md#describepatchgroupsresulttypedef) 


```python
# describe_patch_groups method usage example with argument unpacking

kwargs: DescribePatchGroupsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_patch_groups(**kwargs)
```

1. See [:material-code-braces: DescribePatchGroupsRequestTypeDef](./type_defs.md#describepatchgroupsrequesttypedef) 

### describe\_patch\_properties

Lists the properties of available patches organized by product, product family,
classification, severity, and other properties of available patches.

Type annotations and code completion for `#!python session.create_client("ssm").describe_patch_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_patch_properties.html)

```python
# describe_patch_properties method definition

await def describe_patch_properties(
    self,
    *,
    OperatingSystem: OperatingSystemType,  # (1)
    Property: PatchPropertyType,  # (2)
    PatchSet: PatchSetType = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribePatchPropertiesResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-brackets: PatchPropertyType](./literals.md#patchpropertytype) 
3. See [:material-code-brackets: PatchSetType](./literals.md#patchsettype) 
4. See [:material-code-braces: DescribePatchPropertiesResultTypeDef](./type_defs.md#describepatchpropertiesresulttypedef) 


```python
# describe_patch_properties method usage example with argument unpacking

kwargs: DescribePatchPropertiesRequestTypeDef = {  # (1)
    "OperatingSystem": ...,
    "Property": ...,
}

parent.describe_patch_properties(**kwargs)
```

1. See [:material-code-braces: DescribePatchPropertiesRequestTypeDef](./type_defs.md#describepatchpropertiesrequesttypedef) 

### describe\_sessions

Retrieves a list of all active sessions (both connected and disconnected) or
terminated sessions from the past 30 days.

Type annotations and code completion for `#!python session.create_client("ssm").describe_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/describe_sessions.html)

```python
# describe_sessions method definition

await def describe_sessions(
    self,
    *,
    State: SessionStateType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[SessionFilterTypeDef] = ...,  # (2)
) -> DescribeSessionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef) 
3. See [:material-code-braces: DescribeSessionsResponseTypeDef](./type_defs.md#describesessionsresponsetypedef) 


```python
# describe_sessions method usage example with argument unpacking

kwargs: DescribeSessionsRequestTypeDef = {  # (1)
    "State": ...,
}

parent.describe_sessions(**kwargs)
```

1. See [:material-code-braces: DescribeSessionsRequestTypeDef](./type_defs.md#describesessionsrequesttypedef) 

### disassociate\_ops\_item\_related\_item

Deletes the association between an OpsItem and a related item.

Type annotations and code completion for `#!python session.create_client("ssm").disassociate_ops_item_related_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/disassociate_ops_item_related_item.html)

```python
# disassociate_ops_item_related_item method definition

await def disassociate_ops_item_related_item(
    self,
    *,
    OpsItemId: str,
    AssociationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_ops_item_related_item method usage example with argument unpacking

kwargs: DisassociateOpsItemRelatedItemRequestTypeDef = {  # (1)
    "OpsItemId": ...,
    "AssociationId": ...,
}

parent.disassociate_ops_item_related_item(**kwargs)
```

1. See [:material-code-braces: DisassociateOpsItemRelatedItemRequestTypeDef](./type_defs.md#disassociateopsitemrelateditemrequesttypedef) 

### get\_automation\_execution

Get detailed information about a particular Automation execution.

Type annotations and code completion for `#!python session.create_client("ssm").get_automation_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_automation_execution.html)

```python
# get_automation_execution method definition

await def get_automation_execution(
    self,
    *,
    AutomationExecutionId: str,
) -> GetAutomationExecutionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAutomationExecutionResultTypeDef](./type_defs.md#getautomationexecutionresulttypedef) 


```python
# get_automation_execution method usage example with argument unpacking

kwargs: GetAutomationExecutionRequestTypeDef = {  # (1)
    "AutomationExecutionId": ...,
}

parent.get_automation_execution(**kwargs)
```

1. See [:material-code-braces: GetAutomationExecutionRequestTypeDef](./type_defs.md#getautomationexecutionrequesttypedef) 

### get\_calendar\_state

Gets the state of a Amazon Web Services Systems Manager change calendar at the
current time or a specified time.

Type annotations and code completion for `#!python session.create_client("ssm").get_calendar_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_calendar_state.html)

```python
# get_calendar_state method definition

await def get_calendar_state(
    self,
    *,
    CalendarNames: Sequence[str],
    AtTime: str = ...,
) -> GetCalendarStateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCalendarStateResponseTypeDef](./type_defs.md#getcalendarstateresponsetypedef) 


```python
# get_calendar_state method usage example with argument unpacking

kwargs: GetCalendarStateRequestTypeDef = {  # (1)
    "CalendarNames": ...,
}

parent.get_calendar_state(**kwargs)
```

1. See [:material-code-braces: GetCalendarStateRequestTypeDef](./type_defs.md#getcalendarstaterequesttypedef) 

### get\_command\_invocation

Returns detailed information about command execution for an invocation or
plugin.

Type annotations and code completion for `#!python session.create_client("ssm").get_command_invocation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_command_invocation.html)

```python
# get_command_invocation method definition

await def get_command_invocation(
    self,
    *,
    CommandId: str,
    InstanceId: str,
    PluginName: str = ...,
) -> GetCommandInvocationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCommandInvocationResultTypeDef](./type_defs.md#getcommandinvocationresulttypedef) 


```python
# get_command_invocation method usage example with argument unpacking

kwargs: GetCommandInvocationRequestTypeDef = {  # (1)
    "CommandId": ...,
    "InstanceId": ...,
}

parent.get_command_invocation(**kwargs)
```

1. See [:material-code-braces: GetCommandInvocationRequestTypeDef](./type_defs.md#getcommandinvocationrequesttypedef) 

### get\_connection\_status

Retrieves the Session Manager connection status for a managed node to determine
whether it is running and ready to receive Session Manager connections.

Type annotations and code completion for `#!python session.create_client("ssm").get_connection_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_connection_status.html)

```python
# get_connection_status method definition

await def get_connection_status(
    self,
    *,
    Target: str,
) -> GetConnectionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectionStatusResponseTypeDef](./type_defs.md#getconnectionstatusresponsetypedef) 


```python
# get_connection_status method usage example with argument unpacking

kwargs: GetConnectionStatusRequestTypeDef = {  # (1)
    "Target": ...,
}

parent.get_connection_status(**kwargs)
```

1. See [:material-code-braces: GetConnectionStatusRequestTypeDef](./type_defs.md#getconnectionstatusrequesttypedef) 

### get\_default\_patch\_baseline

Retrieves the default patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").get_default_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_default_patch_baseline.html)

```python
# get_default_patch_baseline method definition

await def get_default_patch_baseline(
    self,
    *,
    OperatingSystem: OperatingSystemType = ...,  # (1)
) -> GetDefaultPatchBaselineResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: GetDefaultPatchBaselineResultTypeDef](./type_defs.md#getdefaultpatchbaselineresulttypedef) 


```python
# get_default_patch_baseline method usage example with argument unpacking

kwargs: GetDefaultPatchBaselineRequestTypeDef = {  # (1)
    "OperatingSystem": ...,
}

parent.get_default_patch_baseline(**kwargs)
```

1. See [:material-code-braces: GetDefaultPatchBaselineRequestTypeDef](./type_defs.md#getdefaultpatchbaselinerequesttypedef) 

### get\_deployable\_patch\_snapshot\_for\_instance

Retrieves the current snapshot for the patch baseline the managed node uses.

Type annotations and code completion for `#!python session.create_client("ssm").get_deployable_patch_snapshot_for_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_deployable_patch_snapshot_for_instance.html)

```python
# get_deployable_patch_snapshot_for_instance method definition

await def get_deployable_patch_snapshot_for_instance(
    self,
    *,
    InstanceId: str,
    SnapshotId: str,
    BaselineOverride: BaselineOverrideTypeDef = ...,  # (1)
) -> GetDeployablePatchSnapshotForInstanceResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BaselineOverrideTypeDef](./type_defs.md#baselineoverridetypedef) 
2. See [:material-code-braces: GetDeployablePatchSnapshotForInstanceResultTypeDef](./type_defs.md#getdeployablepatchsnapshotforinstanceresulttypedef) 


```python
# get_deployable_patch_snapshot_for_instance method usage example with argument unpacking

kwargs: GetDeployablePatchSnapshotForInstanceRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "SnapshotId": ...,
}

parent.get_deployable_patch_snapshot_for_instance(**kwargs)
```

1. See [:material-code-braces: GetDeployablePatchSnapshotForInstanceRequestTypeDef](./type_defs.md#getdeployablepatchsnapshotforinstancerequesttypedef) 

### get\_document

Gets the contents of the specified Amazon Web Services Systems Manager document
(SSM document).

Type annotations and code completion for `#!python session.create_client("ssm").get_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_document.html)

```python
# get_document method definition

await def get_document(
    self,
    *,
    Name: str,
    VersionName: str = ...,
    DocumentVersion: str = ...,
    DocumentFormat: DocumentFormatType = ...,  # (1)
) -> GetDocumentResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
2. See [:material-code-braces: GetDocumentResultTypeDef](./type_defs.md#getdocumentresulttypedef) 


```python
# get_document method usage example with argument unpacking

kwargs: GetDocumentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_document(**kwargs)
```

1. See [:material-code-braces: GetDocumentRequestTypeDef](./type_defs.md#getdocumentrequesttypedef) 

### get\_execution\_preview

Initiates the process of retrieving an existing preview that shows the effects
that running a specified Automation runbook would have on the targeted
resources.

Type annotations and code completion for `#!python session.create_client("ssm").get_execution_preview` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_execution_preview.html)

```python
# get_execution_preview method definition

await def get_execution_preview(
    self,
    *,
    ExecutionPreviewId: str,
) -> GetExecutionPreviewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExecutionPreviewResponseTypeDef](./type_defs.md#getexecutionpreviewresponsetypedef) 


```python
# get_execution_preview method usage example with argument unpacking

kwargs: GetExecutionPreviewRequestTypeDef = {  # (1)
    "ExecutionPreviewId": ...,
}

parent.get_execution_preview(**kwargs)
```

1. See [:material-code-braces: GetExecutionPreviewRequestTypeDef](./type_defs.md#getexecutionpreviewrequesttypedef) 

### get\_inventory

Query inventory information.

Type annotations and code completion for `#!python session.create_client("ssm").get_inventory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_inventory.html)

```python
# get_inventory method definition

await def get_inventory(
    self,
    *,
    Filters: Sequence[InventoryFilterTypeDef] = ...,  # (1)
    Aggregators: Sequence[InventoryAggregatorTypeDef] = ...,  # (2)
    ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetInventoryResultTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: InventoryAggregatorTypeDef](./type_defs.md#inventoryaggregatortypedef) 
3. See [:material-code-braces: ResultAttributeTypeDef](./type_defs.md#resultattributetypedef) 
4. See [:material-code-braces: GetInventoryResultTypeDef](./type_defs.md#getinventoryresulttypedef) 


```python
# get_inventory method usage example with argument unpacking

kwargs: GetInventoryRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.get_inventory(**kwargs)
```

1. See [:material-code-braces: GetInventoryRequestTypeDef](./type_defs.md#getinventoryrequesttypedef) 

### get\_inventory\_schema

Return a list of inventory type names for the account, or return a list of
attribute names for a specific Inventory item type.

Type annotations and code completion for `#!python session.create_client("ssm").get_inventory_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_inventory_schema.html)

```python
# get_inventory_schema method definition

await def get_inventory_schema(
    self,
    *,
    TypeName: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Aggregator: bool = ...,
    SubType: bool = ...,
) -> GetInventorySchemaResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInventorySchemaResultTypeDef](./type_defs.md#getinventoryschemaresulttypedef) 


```python
# get_inventory_schema method usage example with argument unpacking

kwargs: GetInventorySchemaRequestTypeDef = {  # (1)
    "TypeName": ...,
}

parent.get_inventory_schema(**kwargs)
```

1. See [:material-code-braces: GetInventorySchemaRequestTypeDef](./type_defs.md#getinventoryschemarequesttypedef) 

### get\_maintenance\_window

Retrieves a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").get_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_maintenance_window.html)

```python
# get_maintenance_window method definition

await def get_maintenance_window(
    self,
    *,
    WindowId: str,
) -> GetMaintenanceWindowResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMaintenanceWindowResultTypeDef](./type_defs.md#getmaintenancewindowresulttypedef) 


```python
# get_maintenance_window method usage example with argument unpacking

kwargs: GetMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.get_maintenance_window(**kwargs)
```

1. See [:material-code-braces: GetMaintenanceWindowRequestTypeDef](./type_defs.md#getmaintenancewindowrequesttypedef) 

### get\_maintenance\_window\_execution

Retrieves details about a specific a maintenance window execution.

Type annotations and code completion for `#!python session.create_client("ssm").get_maintenance_window_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_maintenance_window_execution.html)

```python
# get_maintenance_window_execution method definition

await def get_maintenance_window_execution(
    self,
    *,
    WindowExecutionId: str,
) -> GetMaintenanceWindowExecutionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionResultTypeDef](./type_defs.md#getmaintenancewindowexecutionresulttypedef) 


```python
# get_maintenance_window_execution method usage example with argument unpacking

kwargs: GetMaintenanceWindowExecutionRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
}

parent.get_maintenance_window_execution(**kwargs)
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionRequestTypeDef](./type_defs.md#getmaintenancewindowexecutionrequesttypedef) 

### get\_maintenance\_window\_execution\_task

Retrieves the details about a specific task run as part of a maintenance window
execution.

Type annotations and code completion for `#!python session.create_client("ssm").get_maintenance_window_execution_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_maintenance_window_execution_task.html)

```python
# get_maintenance_window_execution_task method definition

await def get_maintenance_window_execution_task(
    self,
    *,
    WindowExecutionId: str,
    TaskId: str,
) -> GetMaintenanceWindowExecutionTaskResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionTaskResultTypeDef](./type_defs.md#getmaintenancewindowexecutiontaskresulttypedef) 


```python
# get_maintenance_window_execution_task method usage example with argument unpacking

kwargs: GetMaintenanceWindowExecutionTaskRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
    "TaskId": ...,
}

parent.get_maintenance_window_execution_task(**kwargs)
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionTaskRequestTypeDef](./type_defs.md#getmaintenancewindowexecutiontaskrequesttypedef) 

### get\_maintenance\_window\_execution\_task\_invocation

Retrieves information about a specific task running on a specific target.

Type annotations and code completion for `#!python session.create_client("ssm").get_maintenance_window_execution_task_invocation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_maintenance_window_execution_task_invocation.html)

```python
# get_maintenance_window_execution_task_invocation method definition

await def get_maintenance_window_execution_task_invocation(
    self,
    *,
    WindowExecutionId: str,
    TaskId: str,
    InvocationId: str,
) -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionTaskInvocationResultTypeDef](./type_defs.md#getmaintenancewindowexecutiontaskinvocationresulttypedef) 


```python
# get_maintenance_window_execution_task_invocation method usage example with argument unpacking

kwargs: GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef = {  # (1)
    "WindowExecutionId": ...,
    "TaskId": ...,
    "InvocationId": ...,
}

parent.get_maintenance_window_execution_task_invocation(**kwargs)
```

1. See [:material-code-braces: GetMaintenanceWindowExecutionTaskInvocationRequestTypeDef](./type_defs.md#getmaintenancewindowexecutiontaskinvocationrequesttypedef) 

### get\_maintenance\_window\_task

Retrieves the details of a maintenance window task.

Type annotations and code completion for `#!python session.create_client("ssm").get_maintenance_window_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_maintenance_window_task.html)

```python
# get_maintenance_window_task method definition

await def get_maintenance_window_task(
    self,
    *,
    WindowId: str,
    WindowTaskId: str,
) -> GetMaintenanceWindowTaskResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMaintenanceWindowTaskResultTypeDef](./type_defs.md#getmaintenancewindowtaskresulttypedef) 


```python
# get_maintenance_window_task method usage example with argument unpacking

kwargs: GetMaintenanceWindowTaskRequestTypeDef = {  # (1)
    "WindowId": ...,
    "WindowTaskId": ...,
}

parent.get_maintenance_window_task(**kwargs)
```

1. See [:material-code-braces: GetMaintenanceWindowTaskRequestTypeDef](./type_defs.md#getmaintenancewindowtaskrequesttypedef) 

### get\_ops\_item

Get information about an OpsItem by using the ID.

Type annotations and code completion for `#!python session.create_client("ssm").get_ops_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_ops_item.html)

```python
# get_ops_item method definition

await def get_ops_item(
    self,
    *,
    OpsItemId: str,
    OpsItemArn: str = ...,
) -> GetOpsItemResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpsItemResponseTypeDef](./type_defs.md#getopsitemresponsetypedef) 


```python
# get_ops_item method usage example with argument unpacking

kwargs: GetOpsItemRequestTypeDef = {  # (1)
    "OpsItemId": ...,
}

parent.get_ops_item(**kwargs)
```

1. See [:material-code-braces: GetOpsItemRequestTypeDef](./type_defs.md#getopsitemrequesttypedef) 

### get\_ops\_metadata

View operational metadata related to an application in Application Manager.

Type annotations and code completion for `#!python session.create_client("ssm").get_ops_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_ops_metadata.html)

```python
# get_ops_metadata method definition

await def get_ops_metadata(
    self,
    *,
    OpsMetadataArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetOpsMetadataResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpsMetadataResultTypeDef](./type_defs.md#getopsmetadataresulttypedef) 


```python
# get_ops_metadata method usage example with argument unpacking

kwargs: GetOpsMetadataRequestTypeDef = {  # (1)
    "OpsMetadataArn": ...,
}

parent.get_ops_metadata(**kwargs)
```

1. See [:material-code-braces: GetOpsMetadataRequestTypeDef](./type_defs.md#getopsmetadatarequesttypedef) 

### get\_ops\_summary

View a summary of operations metadata (OpsData) based on specified filters and
aggregators.

Type annotations and code completion for `#!python session.create_client("ssm").get_ops_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_ops_summary.html)

```python
# get_ops_summary method definition

await def get_ops_summary(
    self,
    *,
    SyncName: str = ...,
    Filters: Sequence[OpsFilterTypeDef] = ...,  # (1)
    Aggregators: Sequence[OpsAggregatorTypeDef] = ...,  # (2)
    ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetOpsSummaryResultTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: OpsFilterTypeDef](./type_defs.md#opsfiltertypedef) 
2. See [:material-code-braces: OpsAggregatorTypeDef](./type_defs.md#opsaggregatortypedef) 
3. See [:material-code-braces: OpsResultAttributeTypeDef](./type_defs.md#opsresultattributetypedef) 
4. See [:material-code-braces: GetOpsSummaryResultTypeDef](./type_defs.md#getopssummaryresulttypedef) 


```python
# get_ops_summary method usage example with argument unpacking

kwargs: GetOpsSummaryRequestTypeDef = {  # (1)
    "SyncName": ...,
}

parent.get_ops_summary(**kwargs)
```

1. See [:material-code-braces: GetOpsSummaryRequestTypeDef](./type_defs.md#getopssummaryrequesttypedef) 

### get\_parameter

Get information about a single parameter by specifying the parameter name.

Type annotations and code completion for `#!python session.create_client("ssm").get_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_parameter.html)

```python
# get_parameter method definition

await def get_parameter(
    self,
    *,
    Name: str,
    WithDecryption: bool = ...,
) -> GetParameterResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParameterResultTypeDef](./type_defs.md#getparameterresulttypedef) 


```python
# get_parameter method usage example with argument unpacking

kwargs: GetParameterRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_parameter(**kwargs)
```

1. See [:material-code-braces: GetParameterRequestTypeDef](./type_defs.md#getparameterrequesttypedef) 

### get\_parameter\_history

Retrieves the history of all changes to a parameter.

Type annotations and code completion for `#!python session.create_client("ssm").get_parameter_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_parameter_history.html)

```python
# get_parameter_history method definition

await def get_parameter_history(
    self,
    *,
    Name: str,
    WithDecryption: bool = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetParameterHistoryResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParameterHistoryResultTypeDef](./type_defs.md#getparameterhistoryresulttypedef) 


```python
# get_parameter_history method usage example with argument unpacking

kwargs: GetParameterHistoryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_parameter_history(**kwargs)
```

1. See [:material-code-braces: GetParameterHistoryRequestTypeDef](./type_defs.md#getparameterhistoryrequesttypedef) 

### get\_parameters

Get information about one or more parameters by specifying multiple parameter
names.

Type annotations and code completion for `#!python session.create_client("ssm").get_parameters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_parameters.html)

```python
# get_parameters method definition

await def get_parameters(
    self,
    *,
    Names: Sequence[str],
    WithDecryption: bool = ...,
) -> GetParametersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParametersResultTypeDef](./type_defs.md#getparametersresulttypedef) 


```python
# get_parameters method usage example with argument unpacking

kwargs: GetParametersRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.get_parameters(**kwargs)
```

1. See [:material-code-braces: GetParametersRequestTypeDef](./type_defs.md#getparametersrequesttypedef) 

### get\_parameters\_by\_path

Retrieve information about one or more parameters under a specified level in a
hierarchy.

Type annotations and code completion for `#!python session.create_client("ssm").get_parameters_by_path` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_parameters_by_path.html)

```python
# get_parameters_by_path method definition

await def get_parameters_by_path(
    self,
    *,
    Path: str,
    Recursive: bool = ...,
    ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,  # (1)
    WithDecryption: bool = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetParametersByPathResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParameterStringFilterTypeDef](./type_defs.md#parameterstringfiltertypedef) 
2. See [:material-code-braces: GetParametersByPathResultTypeDef](./type_defs.md#getparametersbypathresulttypedef) 


```python
# get_parameters_by_path method usage example with argument unpacking

kwargs: GetParametersByPathRequestTypeDef = {  # (1)
    "Path": ...,
}

parent.get_parameters_by_path(**kwargs)
```

1. See [:material-code-braces: GetParametersByPathRequestTypeDef](./type_defs.md#getparametersbypathrequesttypedef) 

### get\_patch\_baseline

Retrieves information about a patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").get_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_patch_baseline.html)

```python
# get_patch_baseline method definition

await def get_patch_baseline(
    self,
    *,
    BaselineId: str,
) -> GetPatchBaselineResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPatchBaselineResultTypeDef](./type_defs.md#getpatchbaselineresulttypedef) 


```python
# get_patch_baseline method usage example with argument unpacking

kwargs: GetPatchBaselineRequestTypeDef = {  # (1)
    "BaselineId": ...,
}

parent.get_patch_baseline(**kwargs)
```

1. See [:material-code-braces: GetPatchBaselineRequestTypeDef](./type_defs.md#getpatchbaselinerequesttypedef) 

### get\_patch\_baseline\_for\_patch\_group

Retrieves the patch baseline that should be used for the specified patch group.

Type annotations and code completion for `#!python session.create_client("ssm").get_patch_baseline_for_patch_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_patch_baseline_for_patch_group.html)

```python
# get_patch_baseline_for_patch_group method definition

await def get_patch_baseline_for_patch_group(
    self,
    *,
    PatchGroup: str,
    OperatingSystem: OperatingSystemType = ...,  # (1)
) -> GetPatchBaselineForPatchGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: GetPatchBaselineForPatchGroupResultTypeDef](./type_defs.md#getpatchbaselineforpatchgroupresulttypedef) 


```python
# get_patch_baseline_for_patch_group method usage example with argument unpacking

kwargs: GetPatchBaselineForPatchGroupRequestTypeDef = {  # (1)
    "PatchGroup": ...,
}

parent.get_patch_baseline_for_patch_group(**kwargs)
```

1. See [:material-code-braces: GetPatchBaselineForPatchGroupRequestTypeDef](./type_defs.md#getpatchbaselineforpatchgrouprequesttypedef) 

### get\_resource\_policies

Returns an array of the <code>Policy</code> object.

Type annotations and code completion for `#!python session.create_client("ssm").get_resource_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_resource_policies.html)

```python
# get_resource_policies method definition

await def get_resource_policies(
    self,
    *,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetResourcePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


```python
# get_resource_policies method usage example with argument unpacking

kwargs: GetResourcePoliciesRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policies(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesRequestTypeDef](./type_defs.md#getresourcepoliciesrequesttypedef) 

### get\_service\_setting

<code>ServiceSetting</code> is an account-level setting for an Amazon Web
Services service.

Type annotations and code completion for `#!python session.create_client("ssm").get_service_setting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/get_service_setting.html)

```python
# get_service_setting method definition

await def get_service_setting(
    self,
    *,
    SettingId: str,
) -> GetServiceSettingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSettingResultTypeDef](./type_defs.md#getservicesettingresulttypedef) 


```python
# get_service_setting method usage example with argument unpacking

kwargs: GetServiceSettingRequestTypeDef = {  # (1)
    "SettingId": ...,
}

parent.get_service_setting(**kwargs)
```

1. See [:material-code-braces: GetServiceSettingRequestTypeDef](./type_defs.md#getservicesettingrequesttypedef) 

### label\_parameter\_version

A parameter label is a user-defined alias to help you manage different versions
of a parameter.

Type annotations and code completion for `#!python session.create_client("ssm").label_parameter_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/label_parameter_version.html)

```python
# label_parameter_version method definition

await def label_parameter_version(
    self,
    *,
    Name: str,
    Labels: Sequence[str],
    ParameterVersion: int = ...,
) -> LabelParameterVersionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LabelParameterVersionResultTypeDef](./type_defs.md#labelparameterversionresulttypedef) 


```python
# label_parameter_version method usage example with argument unpacking

kwargs: LabelParameterVersionRequestTypeDef = {  # (1)
    "Name": ...,
    "Labels": ...,
}

parent.label_parameter_version(**kwargs)
```

1. See [:material-code-braces: LabelParameterVersionRequestTypeDef](./type_defs.md#labelparameterversionrequesttypedef) 

### list\_association\_versions

Retrieves all versions of an association for a specific association ID.

Type annotations and code completion for `#!python session.create_client("ssm").list_association_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_association_versions.html)

```python
# list_association_versions method definition

await def list_association_versions(
    self,
    *,
    AssociationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAssociationVersionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssociationVersionsResultTypeDef](./type_defs.md#listassociationversionsresulttypedef) 


```python
# list_association_versions method usage example with argument unpacking

kwargs: ListAssociationVersionsRequestTypeDef = {  # (1)
    "AssociationId": ...,
}

parent.list_association_versions(**kwargs)
```

1. See [:material-code-braces: ListAssociationVersionsRequestTypeDef](./type_defs.md#listassociationversionsrequesttypedef) 

### list\_associations

Returns all State Manager associations in the current Amazon Web Services
account and Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("ssm").list_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_associations.html)

```python
# list_associations method definition

await def list_associations(
    self,
    *,
    AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAssociationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociationFilterTypeDef](./type_defs.md#associationfiltertypedef) 
2. See [:material-code-braces: ListAssociationsResultTypeDef](./type_defs.md#listassociationsresulttypedef) 


```python
# list_associations method usage example with argument unpacking

kwargs: ListAssociationsRequestTypeDef = {  # (1)
    "AssociationFilterList": ...,
}

parent.list_associations(**kwargs)
```

1. See [:material-code-braces: ListAssociationsRequestTypeDef](./type_defs.md#listassociationsrequesttypedef) 

### list\_command\_invocations

An invocation is copy of a command sent to a specific managed node.

Type annotations and code completion for `#!python session.create_client("ssm").list_command_invocations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_command_invocations.html)

```python
# list_command_invocations method definition

await def list_command_invocations(
    self,
    *,
    CommandId: str = ...,
    InstanceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[CommandFilterTypeDef] = ...,  # (1)
    Details: bool = ...,
) -> ListCommandInvocationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: ListCommandInvocationsResultTypeDef](./type_defs.md#listcommandinvocationsresulttypedef) 


```python
# list_command_invocations method usage example with argument unpacking

kwargs: ListCommandInvocationsRequestTypeDef = {  # (1)
    "CommandId": ...,
}

parent.list_command_invocations(**kwargs)
```

1. See [:material-code-braces: ListCommandInvocationsRequestTypeDef](./type_defs.md#listcommandinvocationsrequesttypedef) 

### list\_commands

Lists the commands requested by users of the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("ssm").list_commands` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_commands.html)

```python
# list_commands method definition

await def list_commands(
    self,
    *,
    CommandId: str = ...,
    InstanceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[CommandFilterTypeDef] = ...,  # (1)
) -> ListCommandsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CommandFilterTypeDef](./type_defs.md#commandfiltertypedef) 
2. See [:material-code-braces: ListCommandsResultTypeDef](./type_defs.md#listcommandsresulttypedef) 


```python
# list_commands method usage example with argument unpacking

kwargs: ListCommandsRequestTypeDef = {  # (1)
    "CommandId": ...,
}

parent.list_commands(**kwargs)
```

1. See [:material-code-braces: ListCommandsRequestTypeDef](./type_defs.md#listcommandsrequesttypedef) 

### list\_compliance\_items

For a specified resource ID, this API operation returns a list of compliance
statuses for different resource types.

Type annotations and code completion for `#!python session.create_client("ssm").list_compliance_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_compliance_items.html)

```python
# list_compliance_items method definition

await def list_compliance_items(
    self,
    *,
    Filters: Sequence[ComplianceStringFilterTypeDef] = ...,  # (1)
    ResourceIds: Sequence[str] = ...,
    ResourceTypes: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListComplianceItemsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: ListComplianceItemsResultTypeDef](./type_defs.md#listcomplianceitemsresulttypedef) 


```python
# list_compliance_items method usage example with argument unpacking

kwargs: ListComplianceItemsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_compliance_items(**kwargs)
```

1. See [:material-code-braces: ListComplianceItemsRequestTypeDef](./type_defs.md#listcomplianceitemsrequesttypedef) 

### list\_compliance\_summaries

Returns a summary count of compliant and non-compliant resources for a
compliance type.

Type annotations and code completion for `#!python session.create_client("ssm").list_compliance_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_compliance_summaries.html)

```python
# list_compliance_summaries method definition

await def list_compliance_summaries(
    self,
    *,
    Filters: Sequence[ComplianceStringFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListComplianceSummariesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: ListComplianceSummariesResultTypeDef](./type_defs.md#listcompliancesummariesresulttypedef) 


```python
# list_compliance_summaries method usage example with argument unpacking

kwargs: ListComplianceSummariesRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_compliance_summaries(**kwargs)
```

1. See [:material-code-braces: ListComplianceSummariesRequestTypeDef](./type_defs.md#listcompliancesummariesrequesttypedef) 

### list\_document\_metadata\_history

Information about approval reviews for a version of a change template in Change
Manager.

Type annotations and code completion for `#!python session.create_client("ssm").list_document_metadata_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_document_metadata_history.html)

```python
# list_document_metadata_history method definition

await def list_document_metadata_history(
    self,
    *,
    Name: str,
    Metadata: DocumentMetadataEnumType,  # (1)
    DocumentVersion: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDocumentMetadataHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DocumentMetadataEnumType](./literals.md#documentmetadataenumtype) 
2. See [:material-code-braces: ListDocumentMetadataHistoryResponseTypeDef](./type_defs.md#listdocumentmetadatahistoryresponsetypedef) 


```python
# list_document_metadata_history method usage example with argument unpacking

kwargs: ListDocumentMetadataHistoryRequestTypeDef = {  # (1)
    "Name": ...,
    "Metadata": ...,
}

parent.list_document_metadata_history(**kwargs)
```

1. See [:material-code-braces: ListDocumentMetadataHistoryRequestTypeDef](./type_defs.md#listdocumentmetadatahistoryrequesttypedef) 

### list\_document\_versions

List all versions for a document.

Type annotations and code completion for `#!python session.create_client("ssm").list_document_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_document_versions.html)

```python
# list_document_versions method definition

await def list_document_versions(
    self,
    *,
    Name: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDocumentVersionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDocumentVersionsResultTypeDef](./type_defs.md#listdocumentversionsresulttypedef) 


```python
# list_document_versions method usage example with argument unpacking

kwargs: ListDocumentVersionsRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.list_document_versions(**kwargs)
```

1. See [:material-code-braces: ListDocumentVersionsRequestTypeDef](./type_defs.md#listdocumentversionsrequesttypedef) 

### list\_documents

Returns all Systems Manager (SSM) documents in the current Amazon Web Services
account and Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("ssm").list_documents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_documents.html)

```python
# list_documents method definition

await def list_documents(
    self,
    *,
    DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,  # (1)
    Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDocumentsResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DocumentFilterTypeDef](./type_defs.md#documentfiltertypedef) 
2. See [:material-code-braces: DocumentKeyValuesFilterTypeDef](./type_defs.md#documentkeyvaluesfiltertypedef) 
3. See [:material-code-braces: ListDocumentsResultTypeDef](./type_defs.md#listdocumentsresulttypedef) 


```python
# list_documents method usage example with argument unpacking

kwargs: ListDocumentsRequestTypeDef = {  # (1)
    "DocumentFilterList": ...,
}

parent.list_documents(**kwargs)
```

1. See [:material-code-braces: ListDocumentsRequestTypeDef](./type_defs.md#listdocumentsrequesttypedef) 

### list\_inventory\_entries

A list of inventory items returned by the request.

Type annotations and code completion for `#!python session.create_client("ssm").list_inventory_entries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_inventory_entries.html)

```python
# list_inventory_entries method definition

await def list_inventory_entries(
    self,
    *,
    InstanceId: str,
    TypeName: str,
    Filters: Sequence[InventoryFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInventoryEntriesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: ListInventoryEntriesResultTypeDef](./type_defs.md#listinventoryentriesresulttypedef) 


```python
# list_inventory_entries method usage example with argument unpacking

kwargs: ListInventoryEntriesRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "TypeName": ...,
}

parent.list_inventory_entries(**kwargs)
```

1. See [:material-code-braces: ListInventoryEntriesRequestTypeDef](./type_defs.md#listinventoryentriesrequesttypedef) 

### list\_nodes

Takes in filters and returns a list of managed nodes matching the filter
criteria.

Type annotations and code completion for `#!python session.create_client("ssm").list_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_nodes.html)

```python
# list_nodes method definition

await def list_nodes(
    self,
    *,
    SyncName: str = ...,
    Filters: Sequence[NodeFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListNodesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
2. See [:material-code-braces: ListNodesResultTypeDef](./type_defs.md#listnodesresulttypedef) 


```python
# list_nodes method usage example with argument unpacking

kwargs: ListNodesRequestTypeDef = {  # (1)
    "SyncName": ...,
}

parent.list_nodes(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestTypeDef](./type_defs.md#listnodesrequesttypedef) 

### list\_nodes\_summary

Generates a summary of managed instance/node metadata based on the filters and
aggregators you specify.

Type annotations and code completion for `#!python session.create_client("ssm").list_nodes_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_nodes_summary.html)

```python
# list_nodes_summary method definition

await def list_nodes_summary(
    self,
    *,
    Aggregators: Sequence[NodeAggregatorTypeDef],  # (1)
    SyncName: str = ...,
    Filters: Sequence[NodeFilterTypeDef] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListNodesSummaryResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: NodeAggregatorTypeDef](./type_defs.md#nodeaggregatortypedef) 
2. See [:material-code-braces: NodeFilterTypeDef](./type_defs.md#nodefiltertypedef) 
3. See [:material-code-braces: ListNodesSummaryResultTypeDef](./type_defs.md#listnodessummaryresulttypedef) 


```python
# list_nodes_summary method usage example with argument unpacking

kwargs: ListNodesSummaryRequestTypeDef = {  # (1)
    "Aggregators": ...,
}

parent.list_nodes_summary(**kwargs)
```

1. See [:material-code-braces: ListNodesSummaryRequestTypeDef](./type_defs.md#listnodessummaryrequesttypedef) 

### list\_ops\_item\_events

Returns a list of all OpsItem events in the current Amazon Web Services Region
and Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("ssm").list_ops_item_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_ops_item_events.html)

```python
# list_ops_item_events method definition

await def list_ops_item_events(
    self,
    *,
    Filters: Sequence[OpsItemEventFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOpsItemEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OpsItemEventFilterTypeDef](./type_defs.md#opsitemeventfiltertypedef) 
2. See [:material-code-braces: ListOpsItemEventsResponseTypeDef](./type_defs.md#listopsitemeventsresponsetypedef) 


```python
# list_ops_item_events method usage example with argument unpacking

kwargs: ListOpsItemEventsRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_ops_item_events(**kwargs)
```

1. See [:material-code-braces: ListOpsItemEventsRequestTypeDef](./type_defs.md#listopsitemeventsrequesttypedef) 

### list\_ops\_item\_related\_items

Lists all related-item resources associated with a Systems Manager OpsCenter
OpsItem.

Type annotations and code completion for `#!python session.create_client("ssm").list_ops_item_related_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_ops_item_related_items.html)

```python
# list_ops_item_related_items method definition

await def list_ops_item_related_items(
    self,
    *,
    OpsItemId: str = ...,
    Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOpsItemRelatedItemsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OpsItemRelatedItemsFilterTypeDef](./type_defs.md#opsitemrelateditemsfiltertypedef) 
2. See [:material-code-braces: ListOpsItemRelatedItemsResponseTypeDef](./type_defs.md#listopsitemrelateditemsresponsetypedef) 


```python
# list_ops_item_related_items method usage example with argument unpacking

kwargs: ListOpsItemRelatedItemsRequestTypeDef = {  # (1)
    "OpsItemId": ...,
}

parent.list_ops_item_related_items(**kwargs)
```

1. See [:material-code-braces: ListOpsItemRelatedItemsRequestTypeDef](./type_defs.md#listopsitemrelateditemsrequesttypedef) 

### list\_ops\_metadata

Amazon Web Services Systems Manager calls this API operation when displaying
all Application Manager OpsMetadata objects or blobs.

Type annotations and code completion for `#!python session.create_client("ssm").list_ops_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_ops_metadata.html)

```python
# list_ops_metadata method definition

await def list_ops_metadata(
    self,
    *,
    Filters: Sequence[OpsMetadataFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOpsMetadataResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OpsMetadataFilterTypeDef](./type_defs.md#opsmetadatafiltertypedef) 
2. See [:material-code-braces: ListOpsMetadataResultTypeDef](./type_defs.md#listopsmetadataresulttypedef) 


```python
# list_ops_metadata method usage example with argument unpacking

kwargs: ListOpsMetadataRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_ops_metadata(**kwargs)
```

1. See [:material-code-braces: ListOpsMetadataRequestTypeDef](./type_defs.md#listopsmetadatarequesttypedef) 

### list\_resource\_compliance\_summaries

Returns a resource-level summary count.

Type annotations and code completion for `#!python session.create_client("ssm").list_resource_compliance_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_resource_compliance_summaries.html)

```python
# list_resource_compliance_summaries method definition

await def list_resource_compliance_summaries(
    self,
    *,
    Filters: Sequence[ComplianceStringFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListResourceComplianceSummariesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ComplianceStringFilterTypeDef](./type_defs.md#compliancestringfiltertypedef) 
2. See [:material-code-braces: ListResourceComplianceSummariesResultTypeDef](./type_defs.md#listresourcecompliancesummariesresulttypedef) 


```python
# list_resource_compliance_summaries method usage example with argument unpacking

kwargs: ListResourceComplianceSummariesRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_resource_compliance_summaries(**kwargs)
```

1. See [:material-code-braces: ListResourceComplianceSummariesRequestTypeDef](./type_defs.md#listresourcecompliancesummariesrequesttypedef) 

### list\_resource\_data\_sync

Lists your resource data sync configurations.

Type annotations and code completion for `#!python session.create_client("ssm").list_resource_data_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_resource_data_sync.html)

```python
# list_resource_data_sync method definition

await def list_resource_data_sync(
    self,
    *,
    SyncType: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListResourceDataSyncResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourceDataSyncResultTypeDef](./type_defs.md#listresourcedatasyncresulttypedef) 


```python
# list_resource_data_sync method usage example with argument unpacking

kwargs: ListResourceDataSyncRequestTypeDef = {  # (1)
    "SyncType": ...,
}

parent.list_resource_data_sync(**kwargs)
```

1. See [:material-code-braces: ListResourceDataSyncRequestTypeDef](./type_defs.md#listresourcedatasyncrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags assigned to the specified resource.

Type annotations and code completion for `#!python session.create_client("ssm").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
) -> ListTagsForResourceResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 
2. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### modify\_document\_permission

Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
privately.

Type annotations and code completion for `#!python session.create_client("ssm").modify_document_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/modify_document_permission.html)

```python
# modify_document_permission method definition

await def modify_document_permission(
    self,
    *,
    Name: str,
    PermissionType: DocumentPermissionTypeType,  # (1)
    AccountIdsToAdd: Sequence[str] = ...,
    AccountIdsToRemove: Sequence[str] = ...,
    SharedDocumentVersion: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DocumentPermissionTypeType](./literals.md#documentpermissiontypetype) 


```python
# modify_document_permission method usage example with argument unpacking

kwargs: ModifyDocumentPermissionRequestTypeDef = {  # (1)
    "Name": ...,
    "PermissionType": ...,
}

parent.modify_document_permission(**kwargs)
```

1. See [:material-code-braces: ModifyDocumentPermissionRequestTypeDef](./type_defs.md#modifydocumentpermissionrequesttypedef) 

### put\_compliance\_items

Registers a compliance type and other compliance details on a designated
resource.

Type annotations and code completion for `#!python session.create_client("ssm").put_compliance_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/put_compliance_items.html)

```python
# put_compliance_items method definition

await def put_compliance_items(
    self,
    *,
    ResourceId: str,
    ResourceType: str,
    ComplianceType: str,
    ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,  # (1)
    Items: Sequence[ComplianceItemEntryTypeDef],  # (2)
    ItemContentHash: str = ...,
    UploadType: ComplianceUploadTypeType = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ComplianceExecutionSummaryTypeDef](./type_defs.md#complianceexecutionsummarytypedef) [:material-code-braces: ComplianceExecutionSummaryOutputTypeDef](./type_defs.md#complianceexecutionsummaryoutputtypedef) 
2. See [:material-code-braces: ComplianceItemEntryTypeDef](./type_defs.md#complianceitementrytypedef) 
3. See [:material-code-brackets: ComplianceUploadTypeType](./literals.md#complianceuploadtypetype) 


```python
# put_compliance_items method usage example with argument unpacking

kwargs: PutComplianceItemsRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "ResourceType": ...,
    "ComplianceType": ...,
    "ExecutionSummary": ...,
    "Items": ...,
}

parent.put_compliance_items(**kwargs)
```

1. See [:material-code-braces: PutComplianceItemsRequestTypeDef](./type_defs.md#putcomplianceitemsrequesttypedef) 

### put\_inventory

Bulk update custom inventory items on one or more managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").put_inventory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/put_inventory.html)

```python
# put_inventory method definition

await def put_inventory(
    self,
    *,
    InstanceId: str,
    Items: Sequence[InventoryItemTypeDef],  # (1)
) -> PutInventoryResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InventoryItemTypeDef](./type_defs.md#inventoryitemtypedef) 
2. See [:material-code-braces: PutInventoryResultTypeDef](./type_defs.md#putinventoryresulttypedef) 


```python
# put_inventory method usage example with argument unpacking

kwargs: PutInventoryRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Items": ...,
}

parent.put_inventory(**kwargs)
```

1. See [:material-code-braces: PutInventoryRequestTypeDef](./type_defs.md#putinventoryrequesttypedef) 

### put\_parameter

Add a parameter to the system.

Type annotations and code completion for `#!python session.create_client("ssm").put_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/put_parameter.html)

```python
# put_parameter method definition

await def put_parameter(
    self,
    *,
    Name: str,
    Value: str,
    Description: str = ...,
    Type: ParameterTypeType = ...,  # (1)
    KeyId: str = ...,
    Overwrite: bool = ...,
    AllowedPattern: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    Tier: ParameterTierType = ...,  # (3)
    Policies: str = ...,
    DataType: str = ...,
) -> PutParameterResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ParameterTierType](./literals.md#parametertiertype) 
4. See [:material-code-braces: PutParameterResultTypeDef](./type_defs.md#putparameterresulttypedef) 


```python
# put_parameter method usage example with argument unpacking

kwargs: PutParameterRequestTypeDef = {  # (1)
    "Name": ...,
    "Value": ...,
}

parent.put_parameter(**kwargs)
```

1. See [:material-code-braces: PutParameterRequestTypeDef](./type_defs.md#putparameterrequesttypedef) 

### put\_resource\_policy

Creates or updates a Systems Manager resource policy.

Type annotations and code completion for `#!python session.create_client("ssm").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/put_resource_policy.html)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    Policy: str,
    PolicyId: str = ...,
    PolicyHash: str = ...,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestTypeDef](./type_defs.md#putresourcepolicyrequesttypedef) 

### register\_default\_patch\_baseline

Defines the default patch baseline for the relevant operating system.

Type annotations and code completion for `#!python session.create_client("ssm").register_default_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/register_default_patch_baseline.html)

```python
# register_default_patch_baseline method definition

await def register_default_patch_baseline(
    self,
    *,
    BaselineId: str,
) -> RegisterDefaultPatchBaselineResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterDefaultPatchBaselineResultTypeDef](./type_defs.md#registerdefaultpatchbaselineresulttypedef) 


```python
# register_default_patch_baseline method usage example with argument unpacking

kwargs: RegisterDefaultPatchBaselineRequestTypeDef = {  # (1)
    "BaselineId": ...,
}

parent.register_default_patch_baseline(**kwargs)
```

1. See [:material-code-braces: RegisterDefaultPatchBaselineRequestTypeDef](./type_defs.md#registerdefaultpatchbaselinerequesttypedef) 

### register\_patch\_baseline\_for\_patch\_group

Registers a patch baseline for a patch group.

Type annotations and code completion for `#!python session.create_client("ssm").register_patch_baseline_for_patch_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/register_patch_baseline_for_patch_group.html)

```python
# register_patch_baseline_for_patch_group method definition

await def register_patch_baseline_for_patch_group(
    self,
    *,
    BaselineId: str,
    PatchGroup: str,
) -> RegisterPatchBaselineForPatchGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterPatchBaselineForPatchGroupResultTypeDef](./type_defs.md#registerpatchbaselineforpatchgroupresulttypedef) 


```python
# register_patch_baseline_for_patch_group method usage example with argument unpacking

kwargs: RegisterPatchBaselineForPatchGroupRequestTypeDef = {  # (1)
    "BaselineId": ...,
    "PatchGroup": ...,
}

parent.register_patch_baseline_for_patch_group(**kwargs)
```

1. See [:material-code-braces: RegisterPatchBaselineForPatchGroupRequestTypeDef](./type_defs.md#registerpatchbaselineforpatchgrouprequesttypedef) 

### register\_target\_with\_maintenance\_window

Registers a target with a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").register_target_with_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/register_target_with_maintenance_window.html)

```python
# register_target_with_maintenance_window method definition

await def register_target_with_maintenance_window(
    self,
    *,
    WindowId: str,
    ResourceType: MaintenanceWindowResourceTypeType,  # (1)
    Targets: Sequence[TargetUnionTypeDef],  # (2)
    OwnerInformation: str = ...,
    Name: str = ...,
    Description: str = ...,
    ClientToken: str = ...,
) -> RegisterTargetWithMaintenanceWindowResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MaintenanceWindowResourceTypeType](./literals.md#maintenancewindowresourcetypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: RegisterTargetWithMaintenanceWindowResultTypeDef](./type_defs.md#registertargetwithmaintenancewindowresulttypedef) 


```python
# register_target_with_maintenance_window method usage example with argument unpacking

kwargs: RegisterTargetWithMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
    "ResourceType": ...,
    "Targets": ...,
}

parent.register_target_with_maintenance_window(**kwargs)
```

1. See [:material-code-braces: RegisterTargetWithMaintenanceWindowRequestTypeDef](./type_defs.md#registertargetwithmaintenancewindowrequesttypedef) 

### register\_task\_with\_maintenance\_window

Adds a new task to a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").register_task_with_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/register_task_with_maintenance_window.html)

```python
# register_task_with_maintenance_window method definition

await def register_task_with_maintenance_window(
    self,
    *,
    WindowId: str,
    TaskArn: str,
    TaskType: MaintenanceWindowTaskTypeType,  # (1)
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (2)
    ServiceRoleArn: str = ...,
    TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef] = ...,  # (3)
    TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,  # (4)
    Priority: int = ...,
    MaxConcurrency: str = ...,
    MaxErrors: str = ...,
    LoggingInfo: LoggingInfoTypeDef = ...,  # (5)
    Name: str = ...,
    Description: str = ...,
    ClientToken: str = ...,
    CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,  # (6)
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (7)
) -> RegisterTaskWithMaintenanceWindowResultTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: MaintenanceWindowTaskTypeType](./literals.md#maintenancewindowtasktypetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
4. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
5. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
6. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
7. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
8. See [:material-code-braces: RegisterTaskWithMaintenanceWindowResultTypeDef](./type_defs.md#registertaskwithmaintenancewindowresulttypedef) 


```python
# register_task_with_maintenance_window method usage example with argument unpacking

kwargs: RegisterTaskWithMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
    "TaskArn": ...,
    "TaskType": ...,
}

parent.register_task_with_maintenance_window(**kwargs)
```

1. See [:material-code-braces: RegisterTaskWithMaintenanceWindowRequestTypeDef](./type_defs.md#registertaskwithmaintenancewindowrequesttypedef) 

### remove\_tags\_from\_resource

Removes tag keys from the specified resource.

Type annotations and code completion for `#!python session.create_client("ssm").remove_tags_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/remove_tags_from_resource.html)

```python
# remove_tags_from_resource method definition

await def remove_tags_from_resource(
    self,
    *,
    ResourceType: ResourceTypeForTaggingType,  # (1)
    ResourceId: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeForTaggingType](./literals.md#resourcetypefortaggingtype) 


```python
# remove_tags_from_resource method usage example with argument unpacking

kwargs: RemoveTagsFromResourceRequestTypeDef = {  # (1)
    "ResourceType": ...,
    "ResourceId": ...,
    "TagKeys": ...,
}

parent.remove_tags_from_resource(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromResourceRequestTypeDef](./type_defs.md#removetagsfromresourcerequesttypedef) 

### reset\_service\_setting

<code>ServiceSetting</code> is an account-level setting for an Amazon Web
Services service.

Type annotations and code completion for `#!python session.create_client("ssm").reset_service_setting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/reset_service_setting.html)

```python
# reset_service_setting method definition

await def reset_service_setting(
    self,
    *,
    SettingId: str,
) -> ResetServiceSettingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetServiceSettingResultTypeDef](./type_defs.md#resetservicesettingresulttypedef) 


```python
# reset_service_setting method usage example with argument unpacking

kwargs: ResetServiceSettingRequestTypeDef = {  # (1)
    "SettingId": ...,
}

parent.reset_service_setting(**kwargs)
```

1. See [:material-code-braces: ResetServiceSettingRequestTypeDef](./type_defs.md#resetservicesettingrequesttypedef) 

### resume\_session

Reconnects a session to a managed node after it has been disconnected.

Type annotations and code completion for `#!python session.create_client("ssm").resume_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/resume_session.html)

```python
# resume_session method definition

await def resume_session(
    self,
    *,
    SessionId: str,
) -> ResumeSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResumeSessionResponseTypeDef](./type_defs.md#resumesessionresponsetypedef) 


```python
# resume_session method usage example with argument unpacking

kwargs: ResumeSessionRequestTypeDef = {  # (1)
    "SessionId": ...,
}

parent.resume_session(**kwargs)
```

1. See [:material-code-braces: ResumeSessionRequestTypeDef](./type_defs.md#resumesessionrequesttypedef) 

### send\_automation\_signal

Sends a signal to an Automation execution to change the current behavior or
status of the execution.

Type annotations and code completion for `#!python session.create_client("ssm").send_automation_signal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/send_automation_signal.html)

```python
# send_automation_signal method definition

await def send_automation_signal(
    self,
    *,
    AutomationExecutionId: str,
    SignalType: SignalTypeType,  # (1)
    Payload: Mapping[str, Sequence[str]] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SignalTypeType](./literals.md#signaltypetype) 


```python
# send_automation_signal method usage example with argument unpacking

kwargs: SendAutomationSignalRequestTypeDef = {  # (1)
    "AutomationExecutionId": ...,
    "SignalType": ...,
}

parent.send_automation_signal(**kwargs)
```

1. See [:material-code-braces: SendAutomationSignalRequestTypeDef](./type_defs.md#sendautomationsignalrequesttypedef) 

### send\_command

Runs commands on one or more managed nodes.

Type annotations and code completion for `#!python session.create_client("ssm").send_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/send_command.html)

```python
# send_command method definition

await def send_command(
    self,
    *,
    DocumentName: str,
    InstanceIds: Sequence[str] = ...,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (1)
    DocumentVersion: str = ...,
    DocumentHash: str = ...,
    DocumentHashType: DocumentHashTypeType = ...,  # (2)
    TimeoutSeconds: int = ...,
    Comment: str = ...,
    Parameters: Mapping[str, Sequence[str]] = ...,
    OutputS3Region: str = ...,
    OutputS3BucketName: str = ...,
    OutputS3KeyPrefix: str = ...,
    MaxConcurrency: str = ...,
    MaxErrors: str = ...,
    ServiceRoleArn: str = ...,
    NotificationConfig: NotificationConfigUnionTypeDef = ...,  # (3)
    CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,  # (4)
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (5)
) -> SendCommandResultTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-brackets: DocumentHashTypeType](./literals.md#documenthashtypetype) 
3. See [:material-code-braces: NotificationConfigTypeDef](./type_defs.md#notificationconfigtypedef) [:material-code-braces: NotificationConfigOutputTypeDef](./type_defs.md#notificationconfigoutputtypedef) 
4. See [:material-code-braces: CloudWatchOutputConfigTypeDef](./type_defs.md#cloudwatchoutputconfigtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
6. See [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 


```python
# send_command method usage example with argument unpacking

kwargs: SendCommandRequestTypeDef = {  # (1)
    "DocumentName": ...,
}

parent.send_command(**kwargs)
```

1. See [:material-code-braces: SendCommandRequestTypeDef](./type_defs.md#sendcommandrequesttypedef) 

### start\_associations\_once

Runs an association immediately and only one time.

Type annotations and code completion for `#!python session.create_client("ssm").start_associations_once` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/start_associations_once.html)

```python
# start_associations_once method definition

await def start_associations_once(
    self,
    *,
    AssociationIds: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# start_associations_once method usage example with argument unpacking

kwargs: StartAssociationsOnceRequestTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.start_associations_once(**kwargs)
```

1. See [:material-code-braces: StartAssociationsOnceRequestTypeDef](./type_defs.md#startassociationsoncerequesttypedef) 

### start\_automation\_execution

Initiates execution of an Automation runbook.

Type annotations and code completion for `#!python session.create_client("ssm").start_automation_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/start_automation_execution.html)

```python
# start_automation_execution method definition

await def start_automation_execution(
    self,
    *,
    DocumentName: str,
    DocumentVersion: str = ...,
    Parameters: Mapping[str, Sequence[str]] = ...,
    ClientToken: str = ...,
    Mode: ExecutionModeType = ...,  # (1)
    TargetParameterName: str = ...,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (2)
    TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
    MaxConcurrency: str = ...,
    MaxErrors: str = ...,
    TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (5)
    TargetLocationsURL: str = ...,
) -> StartAutomationExecutionResultTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
6. See [:material-code-braces: StartAutomationExecutionResultTypeDef](./type_defs.md#startautomationexecutionresulttypedef) 


```python
# start_automation_execution method usage example with argument unpacking

kwargs: StartAutomationExecutionRequestTypeDef = {  # (1)
    "DocumentName": ...,
}

parent.start_automation_execution(**kwargs)
```

1. See [:material-code-braces: StartAutomationExecutionRequestTypeDef](./type_defs.md#startautomationexecutionrequesttypedef) 

### start\_change\_request\_execution

Creates a change request for Change Manager.

Type annotations and code completion for `#!python session.create_client("ssm").start_change_request_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/start_change_request_execution.html)

```python
# start_change_request_execution method definition

await def start_change_request_execution(
    self,
    *,
    DocumentName: str,
    Runbooks: Sequence[RunbookUnionTypeDef],  # (1)
    ScheduledTime: TimestampTypeDef = ...,
    DocumentVersion: str = ...,
    Parameters: Mapping[str, Sequence[str]] = ...,
    ChangeRequestName: str = ...,
    ClientToken: str = ...,
    AutoApprove: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ScheduledEndTime: TimestampTypeDef = ...,
    ChangeDetails: str = ...,
) -> StartChangeRequestExecutionResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RunbookTypeDef](./type_defs.md#runbooktypedef) [:material-code-braces: RunbookOutputTypeDef](./type_defs.md#runbookoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: StartChangeRequestExecutionResultTypeDef](./type_defs.md#startchangerequestexecutionresulttypedef) 


```python
# start_change_request_execution method usage example with argument unpacking

kwargs: StartChangeRequestExecutionRequestTypeDef = {  # (1)
    "DocumentName": ...,
    "Runbooks": ...,
}

parent.start_change_request_execution(**kwargs)
```

1. See [:material-code-braces: StartChangeRequestExecutionRequestTypeDef](./type_defs.md#startchangerequestexecutionrequesttypedef) 

### start\_execution\_preview

Initiates the process of creating a preview showing the effects that running a
specified Automation runbook would have on the targeted resources.

Type annotations and code completion for `#!python session.create_client("ssm").start_execution_preview` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/start_execution_preview.html)

```python
# start_execution_preview method definition

await def start_execution_preview(
    self,
    *,
    DocumentName: str,
    DocumentVersion: str = ...,
    ExecutionInputs: ExecutionInputsTypeDef = ...,  # (1)
) -> StartExecutionPreviewResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExecutionInputsTypeDef](./type_defs.md#executioninputstypedef) 
2. See [:material-code-braces: StartExecutionPreviewResponseTypeDef](./type_defs.md#startexecutionpreviewresponsetypedef) 


```python
# start_execution_preview method usage example with argument unpacking

kwargs: StartExecutionPreviewRequestTypeDef = {  # (1)
    "DocumentName": ...,
}

parent.start_execution_preview(**kwargs)
```

1. See [:material-code-braces: StartExecutionPreviewRequestTypeDef](./type_defs.md#startexecutionpreviewrequesttypedef) 

### start\_session

Initiates a connection to a target (for example, a managed node) for a Session
Manager session.

Type annotations and code completion for `#!python session.create_client("ssm").start_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/start_session.html)

```python
# start_session method definition

await def start_session(
    self,
    *,
    Target: str,
    DocumentName: str = ...,
    Reason: str = ...,
    Parameters: Mapping[str, Sequence[str]] = ...,
) -> StartSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartSessionResponseTypeDef](./type_defs.md#startsessionresponsetypedef) 


```python
# start_session method usage example with argument unpacking

kwargs: StartSessionRequestTypeDef = {  # (1)
    "Target": ...,
}

parent.start_session(**kwargs)
```

1. See [:material-code-braces: StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef) 

### stop\_automation\_execution

Stop an Automation that is currently running.

Type annotations and code completion for `#!python session.create_client("ssm").stop_automation_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/stop_automation_execution.html)

```python
# stop_automation_execution method definition

await def stop_automation_execution(
    self,
    *,
    AutomationExecutionId: str,
    Type: StopTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: StopTypeType](./literals.md#stoptypetype) 


```python
# stop_automation_execution method usage example with argument unpacking

kwargs: StopAutomationExecutionRequestTypeDef = {  # (1)
    "AutomationExecutionId": ...,
}

parent.stop_automation_execution(**kwargs)
```

1. See [:material-code-braces: StopAutomationExecutionRequestTypeDef](./type_defs.md#stopautomationexecutionrequesttypedef) 

### terminate\_session

Permanently ends a session and closes the data connection between the Session
Manager client and SSM Agent on the managed node.

Type annotations and code completion for `#!python session.create_client("ssm").terminate_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/terminate_session.html)

```python
# terminate_session method definition

await def terminate_session(
    self,
    *,
    SessionId: str,
) -> TerminateSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TerminateSessionResponseTypeDef](./type_defs.md#terminatesessionresponsetypedef) 


```python
# terminate_session method usage example with argument unpacking

kwargs: TerminateSessionRequestTypeDef = {  # (1)
    "SessionId": ...,
}

parent.terminate_session(**kwargs)
```

1. See [:material-code-braces: TerminateSessionRequestTypeDef](./type_defs.md#terminatesessionrequesttypedef) 

### unlabel\_parameter\_version

Remove a label or labels from a parameter.

Type annotations and code completion for `#!python session.create_client("ssm").unlabel_parameter_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/unlabel_parameter_version.html)

```python
# unlabel_parameter_version method definition

await def unlabel_parameter_version(
    self,
    *,
    Name: str,
    ParameterVersion: int,
    Labels: Sequence[str],
) -> UnlabelParameterVersionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UnlabelParameterVersionResultTypeDef](./type_defs.md#unlabelparameterversionresulttypedef) 


```python
# unlabel_parameter_version method usage example with argument unpacking

kwargs: UnlabelParameterVersionRequestTypeDef = {  # (1)
    "Name": ...,
    "ParameterVersion": ...,
    "Labels": ...,
}

parent.unlabel_parameter_version(**kwargs)
```

1. See [:material-code-braces: UnlabelParameterVersionRequestTypeDef](./type_defs.md#unlabelparameterversionrequesttypedef) 

### update\_association

Updates an association.

Type annotations and code completion for `#!python session.create_client("ssm").update_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_association.html)

```python
# update_association method definition

await def update_association(
    self,
    *,
    AssociationId: str,
    Parameters: Mapping[str, Sequence[str]] = ...,
    DocumentVersion: str = ...,
    ScheduleExpression: str = ...,
    OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,  # (1)
    Name: str = ...,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (2)
    AssociationName: str = ...,
    AssociationVersion: str = ...,
    AutomationTargetParameterName: str = ...,
    MaxErrors: str = ...,
    MaxConcurrency: str = ...,
    ComplianceSeverity: AssociationComplianceSeverityType = ...,  # (3)
    SyncCompliance: AssociationSyncComplianceType = ...,  # (4)
    ApplyOnlyAtCronInterval: bool = ...,
    CalendarNames: Sequence[str] = ...,
    TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,  # (5)
    ScheduleOffset: int = ...,
    Duration: int = ...,
    TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (6)
) -> UpdateAssociationResultTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: InstanceAssociationOutputLocationTypeDef](./type_defs.md#instanceassociationoutputlocationtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
3. See [:material-code-brackets: AssociationComplianceSeverityType](./literals.md#associationcomplianceseveritytype) 
4. See [:material-code-brackets: AssociationSyncComplianceType](./literals.md#associationsynccompliancetype) 
5. See [:material-code-braces: TargetLocationTypeDef](./type_defs.md#targetlocationtypedef) [:material-code-braces: TargetLocationOutputTypeDef](./type_defs.md#targetlocationoutputtypedef) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
7. See [:material-code-braces: UpdateAssociationResultTypeDef](./type_defs.md#updateassociationresulttypedef) 


```python
# update_association method usage example with argument unpacking

kwargs: UpdateAssociationRequestTypeDef = {  # (1)
    "AssociationId": ...,
}

parent.update_association(**kwargs)
```

1. See [:material-code-braces: UpdateAssociationRequestTypeDef](./type_defs.md#updateassociationrequesttypedef) 

### update\_association\_status

Updates the status of the Amazon Web Services Systems Manager document (SSM
document) associated with the specified managed node.

Type annotations and code completion for `#!python session.create_client("ssm").update_association_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_association_status.html)

```python
# update_association_status method definition

await def update_association_status(
    self,
    *,
    Name: str,
    InstanceId: str,
    AssociationStatus: AssociationStatusUnionTypeDef,  # (1)
) -> UpdateAssociationStatusResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociationStatusTypeDef](./type_defs.md#associationstatustypedef) [:material-code-braces: AssociationStatusOutputTypeDef](./type_defs.md#associationstatusoutputtypedef) 
2. See [:material-code-braces: UpdateAssociationStatusResultTypeDef](./type_defs.md#updateassociationstatusresulttypedef) 


```python
# update_association_status method usage example with argument unpacking

kwargs: UpdateAssociationStatusRequestTypeDef = {  # (1)
    "Name": ...,
    "InstanceId": ...,
    "AssociationStatus": ...,
}

parent.update_association_status(**kwargs)
```

1. See [:material-code-braces: UpdateAssociationStatusRequestTypeDef](./type_defs.md#updateassociationstatusrequesttypedef) 

### update\_document

Updates one or more values for an SSM document.

Type annotations and code completion for `#!python session.create_client("ssm").update_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_document.html)

```python
# update_document method definition

await def update_document(
    self,
    *,
    Content: str,
    Name: str,
    Attachments: Sequence[AttachmentsSourceTypeDef] = ...,  # (1)
    DisplayName: str = ...,
    VersionName: str = ...,
    DocumentVersion: str = ...,
    DocumentFormat: DocumentFormatType = ...,  # (2)
    TargetType: str = ...,
) -> UpdateDocumentResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AttachmentsSourceTypeDef](./type_defs.md#attachmentssourcetypedef) 
2. See [:material-code-brackets: DocumentFormatType](./literals.md#documentformattype) 
3. See [:material-code-braces: UpdateDocumentResultTypeDef](./type_defs.md#updatedocumentresulttypedef) 


```python
# update_document method usage example with argument unpacking

kwargs: UpdateDocumentRequestTypeDef = {  # (1)
    "Content": ...,
    "Name": ...,
}

parent.update_document(**kwargs)
```

1. See [:material-code-braces: UpdateDocumentRequestTypeDef](./type_defs.md#updatedocumentrequesttypedef) 

### update\_document\_default\_version

Set the default version of a document.

Type annotations and code completion for `#!python session.create_client("ssm").update_document_default_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_document_default_version.html)

```python
# update_document_default_version method definition

await def update_document_default_version(
    self,
    *,
    Name: str,
    DocumentVersion: str,
) -> UpdateDocumentDefaultVersionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDocumentDefaultVersionResultTypeDef](./type_defs.md#updatedocumentdefaultversionresulttypedef) 


```python
# update_document_default_version method usage example with argument unpacking

kwargs: UpdateDocumentDefaultVersionRequestTypeDef = {  # (1)
    "Name": ...,
    "DocumentVersion": ...,
}

parent.update_document_default_version(**kwargs)
```

1. See [:material-code-braces: UpdateDocumentDefaultVersionRequestTypeDef](./type_defs.md#updatedocumentdefaultversionrequesttypedef) 

### update\_document\_metadata

Updates information related to approval reviews for a specific version of a
change template in Change Manager.

Type annotations and code completion for `#!python session.create_client("ssm").update_document_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_document_metadata.html)

```python
# update_document_metadata method definition

await def update_document_metadata(
    self,
    *,
    Name: str,
    DocumentReviews: DocumentReviewsTypeDef,  # (1)
    DocumentVersion: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DocumentReviewsTypeDef](./type_defs.md#documentreviewstypedef) 


```python
# update_document_metadata method usage example with argument unpacking

kwargs: UpdateDocumentMetadataRequestTypeDef = {  # (1)
    "Name": ...,
    "DocumentReviews": ...,
}

parent.update_document_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateDocumentMetadataRequestTypeDef](./type_defs.md#updatedocumentmetadatarequesttypedef) 

### update\_maintenance\_window

Updates an existing maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").update_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_maintenance_window.html)

```python
# update_maintenance_window method definition

await def update_maintenance_window(
    self,
    *,
    WindowId: str,
    Name: str = ...,
    Description: str = ...,
    StartDate: str = ...,
    EndDate: str = ...,
    Schedule: str = ...,
    ScheduleTimezone: str = ...,
    ScheduleOffset: int = ...,
    Duration: int = ...,
    Cutoff: int = ...,
    AllowUnassociatedTargets: bool = ...,
    Enabled: bool = ...,
    Replace: bool = ...,
) -> UpdateMaintenanceWindowResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateMaintenanceWindowResultTypeDef](./type_defs.md#updatemaintenancewindowresulttypedef) 


```python
# update_maintenance_window method usage example with argument unpacking

kwargs: UpdateMaintenanceWindowRequestTypeDef = {  # (1)
    "WindowId": ...,
}

parent.update_maintenance_window(**kwargs)
```

1. See [:material-code-braces: UpdateMaintenanceWindowRequestTypeDef](./type_defs.md#updatemaintenancewindowrequesttypedef) 

### update\_maintenance\_window\_target

Modifies the target of an existing maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").update_maintenance_window_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_maintenance_window_target.html)

```python
# update_maintenance_window_target method definition

await def update_maintenance_window_target(
    self,
    *,
    WindowId: str,
    WindowTargetId: str,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (1)
    OwnerInformation: str = ...,
    Name: str = ...,
    Description: str = ...,
    Replace: bool = ...,
) -> UpdateMaintenanceWindowTargetResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: UpdateMaintenanceWindowTargetResultTypeDef](./type_defs.md#updatemaintenancewindowtargetresulttypedef) 


```python
# update_maintenance_window_target method usage example with argument unpacking

kwargs: UpdateMaintenanceWindowTargetRequestTypeDef = {  # (1)
    "WindowId": ...,
    "WindowTargetId": ...,
}

parent.update_maintenance_window_target(**kwargs)
```

1. See [:material-code-braces: UpdateMaintenanceWindowTargetRequestTypeDef](./type_defs.md#updatemaintenancewindowtargetrequesttypedef) 

### update\_maintenance\_window\_task

Modifies a task assigned to a maintenance window.

Type annotations and code completion for `#!python session.create_client("ssm").update_maintenance_window_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_maintenance_window_task.html)

```python
# update_maintenance_window_task method definition

await def update_maintenance_window_task(
    self,
    *,
    WindowId: str,
    WindowTaskId: str,
    Targets: Sequence[TargetUnionTypeDef] = ...,  # (1)
    TaskArn: str = ...,
    ServiceRoleArn: str = ...,
    TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef] = ...,  # (2)
    TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,  # (3)
    Priority: int = ...,
    MaxConcurrency: str = ...,
    MaxErrors: str = ...,
    LoggingInfo: LoggingInfoTypeDef = ...,  # (4)
    Name: str = ...,
    Description: str = ...,
    Replace: bool = ...,
    CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,  # (5)
    AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...,  # (6)
) -> UpdateMaintenanceWindowTaskResultTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
2. See [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressiontypedef) [:material-code-braces: MaintenanceWindowTaskParameterValueExpressionOutputTypeDef](./type_defs.md#maintenancewindowtaskparametervalueexpressionoutputtypedef) 
3. See [:material-code-braces: MaintenanceWindowTaskInvocationParametersTypeDef](./type_defs.md#maintenancewindowtaskinvocationparameterstypedef) [:material-code-braces: MaintenanceWindowTaskInvocationParametersOutputTypeDef](./type_defs.md#maintenancewindowtaskinvocationparametersoutputtypedef) 
4. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
5. See [:material-code-brackets: MaintenanceWindowTaskCutoffBehaviorType](./literals.md#maintenancewindowtaskcutoffbehaviortype) 
6. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
7. See [:material-code-braces: UpdateMaintenanceWindowTaskResultTypeDef](./type_defs.md#updatemaintenancewindowtaskresulttypedef) 


```python
# update_maintenance_window_task method usage example with argument unpacking

kwargs: UpdateMaintenanceWindowTaskRequestTypeDef = {  # (1)
    "WindowId": ...,
    "WindowTaskId": ...,
}

parent.update_maintenance_window_task(**kwargs)
```

1. See [:material-code-braces: UpdateMaintenanceWindowTaskRequestTypeDef](./type_defs.md#updatemaintenancewindowtaskrequesttypedef) 

### update\_managed\_instance\_role

Changes the Identity and Access Management (IAM) role that is assigned to the
on-premises server, edge device, or virtual machines (VM).

Type annotations and code completion for `#!python session.create_client("ssm").update_managed_instance_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_managed_instance_role.html)

```python
# update_managed_instance_role method definition

await def update_managed_instance_role(
    self,
    *,
    InstanceId: str,
    IamRole: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_managed_instance_role method usage example with argument unpacking

kwargs: UpdateManagedInstanceRoleRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IamRole": ...,
}

parent.update_managed_instance_role(**kwargs)
```

1. See [:material-code-braces: UpdateManagedInstanceRoleRequestTypeDef](./type_defs.md#updatemanagedinstancerolerequesttypedef) 

### update\_ops\_item

Edit or change an OpsItem.

Type annotations and code completion for `#!python session.create_client("ssm").update_ops_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_ops_item.html)

```python
# update_ops_item method definition

await def update_ops_item(
    self,
    *,
    OpsItemId: str,
    Description: str = ...,
    OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,  # (1)
    OperationalDataToDelete: Sequence[str] = ...,
    Notifications: Sequence[OpsItemNotificationTypeDef] = ...,  # (2)
    Priority: int = ...,
    RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,  # (3)
    Status: OpsItemStatusType = ...,  # (4)
    Title: str = ...,
    Category: str = ...,
    Severity: str = ...,
    ActualStartTime: TimestampTypeDef = ...,
    ActualEndTime: TimestampTypeDef = ...,
    PlannedStartTime: TimestampTypeDef = ...,
    PlannedEndTime: TimestampTypeDef = ...,
    OpsItemArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OpsItemDataValueTypeDef](./type_defs.md#opsitemdatavaluetypedef) 
2. See [:material-code-braces: OpsItemNotificationTypeDef](./type_defs.md#opsitemnotificationtypedef) 
3. See [:material-code-braces: RelatedOpsItemTypeDef](./type_defs.md#relatedopsitemtypedef) 
4. See [:material-code-brackets: OpsItemStatusType](./literals.md#opsitemstatustype) 


```python
# update_ops_item method usage example with argument unpacking

kwargs: UpdateOpsItemRequestTypeDef = {  # (1)
    "OpsItemId": ...,
}

parent.update_ops_item(**kwargs)
```

1. See [:material-code-braces: UpdateOpsItemRequestTypeDef](./type_defs.md#updateopsitemrequesttypedef) 

### update\_ops\_metadata

Amazon Web Services Systems Manager calls this API operation when you edit
OpsMetadata in Application Manager.

Type annotations and code completion for `#!python session.create_client("ssm").update_ops_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_ops_metadata.html)

```python
# update_ops_metadata method definition

await def update_ops_metadata(
    self,
    *,
    OpsMetadataArn: str,
    MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,  # (1)
    KeysToDelete: Sequence[str] = ...,
) -> UpdateOpsMetadataResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MetadataValueTypeDef](./type_defs.md#metadatavaluetypedef) 
2. See [:material-code-braces: UpdateOpsMetadataResultTypeDef](./type_defs.md#updateopsmetadataresulttypedef) 


```python
# update_ops_metadata method usage example with argument unpacking

kwargs: UpdateOpsMetadataRequestTypeDef = {  # (1)
    "OpsMetadataArn": ...,
}

parent.update_ops_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateOpsMetadataRequestTypeDef](./type_defs.md#updateopsmetadatarequesttypedef) 

### update\_patch\_baseline

Modifies an existing patch baseline.

Type annotations and code completion for `#!python session.create_client("ssm").update_patch_baseline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_patch_baseline.html)

```python
# update_patch_baseline method definition

await def update_patch_baseline(
    self,
    *,
    BaselineId: str,
    Name: str = ...,
    GlobalFilters: PatchFilterGroupUnionTypeDef = ...,  # (1)
    ApprovalRules: PatchRuleGroupUnionTypeDef = ...,  # (2)
    ApprovedPatches: Sequence[str] = ...,
    ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,  # (3)
    ApprovedPatchesEnableNonSecurity: bool = ...,
    RejectedPatches: Sequence[str] = ...,
    RejectedPatchesAction: PatchActionType = ...,  # (4)
    Description: str = ...,
    Sources: Sequence[PatchSourceUnionTypeDef] = ...,  # (5)
    Replace: bool = ...,
) -> UpdatePatchBaselineResultTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: PatchFilterGroupTypeDef](./type_defs.md#patchfiltergrouptypedef) [:material-code-braces: PatchFilterGroupOutputTypeDef](./type_defs.md#patchfiltergroupoutputtypedef) 
2. See [:material-code-braces: PatchRuleGroupTypeDef](./type_defs.md#patchrulegrouptypedef) [:material-code-braces: PatchRuleGroupOutputTypeDef](./type_defs.md#patchrulegroupoutputtypedef) 
3. See [:material-code-brackets: PatchComplianceLevelType](./literals.md#patchcomplianceleveltype) 
4. See [:material-code-brackets: PatchActionType](./literals.md#patchactiontype) 
5. See [:material-code-braces: PatchSourceTypeDef](./type_defs.md#patchsourcetypedef) [:material-code-braces: PatchSourceOutputTypeDef](./type_defs.md#patchsourceoutputtypedef) 
6. See [:material-code-braces: UpdatePatchBaselineResultTypeDef](./type_defs.md#updatepatchbaselineresulttypedef) 


```python
# update_patch_baseline method usage example with argument unpacking

kwargs: UpdatePatchBaselineRequestTypeDef = {  # (1)
    "BaselineId": ...,
}

parent.update_patch_baseline(**kwargs)
```

1. See [:material-code-braces: UpdatePatchBaselineRequestTypeDef](./type_defs.md#updatepatchbaselinerequesttypedef) 

### update\_resource\_data\_sync

Update a resource data sync.

Type annotations and code completion for `#!python session.create_client("ssm").update_resource_data_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_resource_data_sync.html)

```python
# update_resource_data_sync method definition

await def update_resource_data_sync(
    self,
    *,
    SyncName: str,
    SyncType: str,
    SyncSource: ResourceDataSyncSourceTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceDataSyncSourceTypeDef](./type_defs.md#resourcedatasyncsourcetypedef) 


```python
# update_resource_data_sync method usage example with argument unpacking

kwargs: UpdateResourceDataSyncRequestTypeDef = {  # (1)
    "SyncName": ...,
    "SyncType": ...,
    "SyncSource": ...,
}

parent.update_resource_data_sync(**kwargs)
```

1. See [:material-code-braces: UpdateResourceDataSyncRequestTypeDef](./type_defs.md#updateresourcedatasyncrequesttypedef) 

### update\_service\_setting

<code>ServiceSetting</code> is an account-level setting for an Amazon Web
Services service.

Type annotations and code completion for `#!python session.create_client("ssm").update_service_setting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm/client/update_service_setting.html)

```python
# update_service_setting method definition

await def update_service_setting(
    self,
    *,
    SettingId: str,
    SettingValue: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_service_setting method usage example with argument unpacking

kwargs: UpdateServiceSettingRequestTypeDef = {  # (1)
    "SettingId": ...,
    "SettingValue": ...,
}

parent.update_service_setting(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSettingRequestTypeDef](./type_defs.md#updateservicesettingrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ssm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ssm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("ssm").get_paginator` method with overloads.

- `client.get_paginator("describe_activations")` -> [DescribeActivationsPaginator](./paginators.md#describeactivationspaginator)
- `client.get_paginator("describe_association_execution_targets")` -> [DescribeAssociationExecutionTargetsPaginator](./paginators.md#describeassociationexecutiontargetspaginator)
- `client.get_paginator("describe_association_executions")` -> [DescribeAssociationExecutionsPaginator](./paginators.md#describeassociationexecutionspaginator)
- `client.get_paginator("describe_automation_executions")` -> [DescribeAutomationExecutionsPaginator](./paginators.md#describeautomationexecutionspaginator)
- `client.get_paginator("describe_automation_step_executions")` -> [DescribeAutomationStepExecutionsPaginator](./paginators.md#describeautomationstepexecutionspaginator)
- `client.get_paginator("describe_available_patches")` -> [DescribeAvailablePatchesPaginator](./paginators.md#describeavailablepatchespaginator)
- `client.get_paginator("describe_effective_instance_associations")` -> [DescribeEffectiveInstanceAssociationsPaginator](./paginators.md#describeeffectiveinstanceassociationspaginator)
- `client.get_paginator("describe_effective_patches_for_patch_baseline")` -> [DescribeEffectivePatchesForPatchBaselinePaginator](./paginators.md#describeeffectivepatchesforpatchbaselinepaginator)
- `client.get_paginator("describe_instance_associations_status")` -> [DescribeInstanceAssociationsStatusPaginator](./paginators.md#describeinstanceassociationsstatuspaginator)
- `client.get_paginator("describe_instance_information")` -> [DescribeInstanceInformationPaginator](./paginators.md#describeinstanceinformationpaginator)
- `client.get_paginator("describe_instance_patch_states_for_patch_group")` -> [DescribeInstancePatchStatesForPatchGroupPaginator](./paginators.md#describeinstancepatchstatesforpatchgrouppaginator)
- `client.get_paginator("describe_instance_patch_states")` -> [DescribeInstancePatchStatesPaginator](./paginators.md#describeinstancepatchstatespaginator)
- `client.get_paginator("describe_instance_patches")` -> [DescribeInstancePatchesPaginator](./paginators.md#describeinstancepatchespaginator)
- `client.get_paginator("describe_instance_properties")` -> [DescribeInstancePropertiesPaginator](./paginators.md#describeinstancepropertiespaginator)
- `client.get_paginator("describe_inventory_deletions")` -> [DescribeInventoryDeletionsPaginator](./paginators.md#describeinventorydeletionspaginator)
- `client.get_paginator("describe_maintenance_window_execution_task_invocations")` -> [DescribeMaintenanceWindowExecutionTaskInvocationsPaginator](./paginators.md#describemaintenancewindowexecutiontaskinvocationspaginator)
- `client.get_paginator("describe_maintenance_window_execution_tasks")` -> [DescribeMaintenanceWindowExecutionTasksPaginator](./paginators.md#describemaintenancewindowexecutiontaskspaginator)
- `client.get_paginator("describe_maintenance_window_executions")` -> [DescribeMaintenanceWindowExecutionsPaginator](./paginators.md#describemaintenancewindowexecutionspaginator)
- `client.get_paginator("describe_maintenance_window_schedule")` -> [DescribeMaintenanceWindowSchedulePaginator](./paginators.md#describemaintenancewindowschedulepaginator)
- `client.get_paginator("describe_maintenance_window_targets")` -> [DescribeMaintenanceWindowTargetsPaginator](./paginators.md#describemaintenancewindowtargetspaginator)
- `client.get_paginator("describe_maintenance_window_tasks")` -> [DescribeMaintenanceWindowTasksPaginator](./paginators.md#describemaintenancewindowtaskspaginator)
- `client.get_paginator("describe_maintenance_windows_for_target")` -> [DescribeMaintenanceWindowsForTargetPaginator](./paginators.md#describemaintenancewindowsfortargetpaginator)
- `client.get_paginator("describe_maintenance_windows")` -> [DescribeMaintenanceWindowsPaginator](./paginators.md#describemaintenancewindowspaginator)
- `client.get_paginator("describe_ops_items")` -> [DescribeOpsItemsPaginator](./paginators.md#describeopsitemspaginator)
- `client.get_paginator("describe_parameters")` -> [DescribeParametersPaginator](./paginators.md#describeparameterspaginator)
- `client.get_paginator("describe_patch_baselines")` -> [DescribePatchBaselinesPaginator](./paginators.md#describepatchbaselinespaginator)
- `client.get_paginator("describe_patch_groups")` -> [DescribePatchGroupsPaginator](./paginators.md#describepatchgroupspaginator)
- `client.get_paginator("describe_patch_properties")` -> [DescribePatchPropertiesPaginator](./paginators.md#describepatchpropertiespaginator)
- `client.get_paginator("describe_sessions")` -> [DescribeSessionsPaginator](./paginators.md#describesessionspaginator)
- `client.get_paginator("get_inventory")` -> [GetInventoryPaginator](./paginators.md#getinventorypaginator)
- `client.get_paginator("get_inventory_schema")` -> [GetInventorySchemaPaginator](./paginators.md#getinventoryschemapaginator)
- `client.get_paginator("get_ops_summary")` -> [GetOpsSummaryPaginator](./paginators.md#getopssummarypaginator)
- `client.get_paginator("get_parameter_history")` -> [GetParameterHistoryPaginator](./paginators.md#getparameterhistorypaginator)
- `client.get_paginator("get_parameters_by_path")` -> [GetParametersByPathPaginator](./paginators.md#getparametersbypathpaginator)
- `client.get_paginator("get_resource_policies")` -> [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
- `client.get_paginator("list_association_versions")` -> [ListAssociationVersionsPaginator](./paginators.md#listassociationversionspaginator)
- `client.get_paginator("list_associations")` -> [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
- `client.get_paginator("list_command_invocations")` -> [ListCommandInvocationsPaginator](./paginators.md#listcommandinvocationspaginator)
- `client.get_paginator("list_commands")` -> [ListCommandsPaginator](./paginators.md#listcommandspaginator)
- `client.get_paginator("list_compliance_items")` -> [ListComplianceItemsPaginator](./paginators.md#listcomplianceitemspaginator)
- `client.get_paginator("list_compliance_summaries")` -> [ListComplianceSummariesPaginator](./paginators.md#listcompliancesummariespaginator)
- `client.get_paginator("list_document_versions")` -> [ListDocumentVersionsPaginator](./paginators.md#listdocumentversionspaginator)
- `client.get_paginator("list_documents")` -> [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
- `client.get_paginator("list_nodes")` -> [ListNodesPaginator](./paginators.md#listnodespaginator)
- `client.get_paginator("list_nodes_summary")` -> [ListNodesSummaryPaginator](./paginators.md#listnodessummarypaginator)
- `client.get_paginator("list_ops_item_events")` -> [ListOpsItemEventsPaginator](./paginators.md#listopsitemeventspaginator)
- `client.get_paginator("list_ops_item_related_items")` -> [ListOpsItemRelatedItemsPaginator](./paginators.md#listopsitemrelateditemspaginator)
- `client.get_paginator("list_ops_metadata")` -> [ListOpsMetadataPaginator](./paginators.md#listopsmetadatapaginator)
- `client.get_paginator("list_resource_compliance_summaries")` -> [ListResourceComplianceSummariesPaginator](./paginators.md#listresourcecompliancesummariespaginator)
- `client.get_paginator("list_resource_data_sync")` -> [ListResourceDataSyncPaginator](./paginators.md#listresourcedatasyncpaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("ssm").get_waiter` method with overloads.

- `client.get_waiter("command_executed")` -> [CommandExecutedWaiter](./waiters.md#commandexecutedwaiter)

