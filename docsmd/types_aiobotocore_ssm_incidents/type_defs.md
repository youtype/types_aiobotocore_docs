# Type definitions

> [Index](../README.md) > [SSMIncidents](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
    type annotations stubs module [types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SsmAutomationUnionTypeDef

```python
# SsmAutomationUnionTypeDef definition

SsmAutomationUnionTypeDef = Union[
    SsmAutomationTypeDef,  # (1)
    SsmAutomationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SsmAutomationTypeDef](./type_defs.md#ssmautomationtypedef) 
2. See [:material-code-braces: SsmAutomationOutputTypeDef](./type_defs.md#ssmautomationoutputtypedef) 

## ActionUnionTypeDef

```python
# ActionUnionTypeDef definition

ActionUnionTypeDef = Union[
    ActionTypeDef,  # (1)
    ActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 



## AddRegionActionTypeDef

```python
# AddRegionActionTypeDef definition

class AddRegionActionTypeDef(TypedDict):
    regionName: str,
    sseKmsKeyId: NotRequired[str],
```

## AttributeValueListTypeDef

```python
# AttributeValueListTypeDef definition

class AttributeValueListTypeDef(TypedDict):
    integerValues: NotRequired[Sequence[int]],
    stringValues: NotRequired[Sequence[str]],
```

## AutomationExecutionTypeDef

```python
# AutomationExecutionTypeDef definition

class AutomationExecutionTypeDef(TypedDict):
    ssmExecutionArn: NotRequired[str],
```

## BatchGetIncidentFindingsErrorTypeDef

```python
# BatchGetIncidentFindingsErrorTypeDef definition

class BatchGetIncidentFindingsErrorTypeDef(TypedDict):
    code: str,
    findingId: str,
    message: str,
```

## BatchGetIncidentFindingsInputRequestTypeDef

```python
# BatchGetIncidentFindingsInputRequestTypeDef definition

class BatchGetIncidentFindingsInputRequestTypeDef(TypedDict):
    findingIds: Sequence[str],
    incidentRecordArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ChatChannelOutputTypeDef

```python
# ChatChannelOutputTypeDef definition

class ChatChannelOutputTypeDef(TypedDict):
    chatbotSns: NotRequired[List[str]],
    empty: NotRequired[Dict[str, Any]],
```

## ChatChannelTypeDef

```python
# ChatChannelTypeDef definition

class ChatChannelTypeDef(TypedDict):
    chatbotSns: NotRequired[Sequence[str]],
    empty: NotRequired[Mapping[str, Any]],
```

## CloudFormationStackUpdateTypeDef

```python
# CloudFormationStackUpdateTypeDef definition

class CloudFormationStackUpdateTypeDef(TypedDict):
    stackArn: str,
    startTime: datetime,
    endTime: NotRequired[datetime],
```

## CodeDeployDeploymentTypeDef

```python
# CodeDeployDeploymentTypeDef definition

class CodeDeployDeploymentTypeDef(TypedDict):
    deploymentGroupArn: str,
    deploymentId: str,
    startTime: datetime,
    endTime: NotRequired[datetime],
```

## RegionMapInputValueTypeDef

```python
# RegionMapInputValueTypeDef definition

class RegionMapInputValueTypeDef(TypedDict):
    sseKmsKeyId: NotRequired[str],
```

## EventReferenceTypeDef

```python
# EventReferenceTypeDef definition

class EventReferenceTypeDef(TypedDict):
    relatedItemId: NotRequired[str],
    resource: NotRequired[str],
```

## DeleteIncidentRecordInputRequestTypeDef

```python
# DeleteIncidentRecordInputRequestTypeDef definition

class DeleteIncidentRecordInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteRegionActionTypeDef

```python
# DeleteRegionActionTypeDef definition

class DeleteRegionActionTypeDef(TypedDict):
    regionName: str,
```

## DeleteReplicationSetInputRequestTypeDef

```python
# DeleteReplicationSetInputRequestTypeDef definition

class DeleteReplicationSetInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteResourcePolicyInputRequestTypeDef

```python
# DeleteResourcePolicyInputRequestTypeDef definition

class DeleteResourcePolicyInputRequestTypeDef(TypedDict):
    policyId: str,
    resourceArn: str,
```

## DeleteResponsePlanInputRequestTypeDef

```python
# DeleteResponsePlanInputRequestTypeDef definition

class DeleteResponsePlanInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteTimelineEventInputRequestTypeDef

```python
# DeleteTimelineEventInputRequestTypeDef definition

class DeleteTimelineEventInputRequestTypeDef(TypedDict):
    eventId: str,
    incidentRecordArn: str,
```

## DynamicSsmParameterValueTypeDef

```python
# DynamicSsmParameterValueTypeDef definition

class DynamicSsmParameterValueTypeDef(TypedDict):
    variable: NotRequired[VariableTypeType],  # (1)
```

1. See [:material-code-brackets: VariableTypeType](./literals.md#variabletypetype) 
## FindingSummaryTypeDef

```python
# FindingSummaryTypeDef definition

class FindingSummaryTypeDef(TypedDict):
    id: str,
    lastModifiedTime: datetime,
```

## GetIncidentRecordInputRequestTypeDef

```python
# GetIncidentRecordInputRequestTypeDef definition

class GetIncidentRecordInputRequestTypeDef(TypedDict):
    arn: str,
```

## GetReplicationSetInputRequestTypeDef

```python
# GetReplicationSetInputRequestTypeDef definition

class GetReplicationSetInputRequestTypeDef(TypedDict):
    arn: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetResourcePoliciesInputRequestTypeDef

```python
# GetResourcePoliciesInputRequestTypeDef definition

class GetResourcePoliciesInputRequestTypeDef(TypedDict):
    resourceArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    policyDocument: str,
    policyId: str,
    ramResourceShareRegion: str,
```

## GetResponsePlanInputRequestTypeDef

```python
# GetResponsePlanInputRequestTypeDef definition

class GetResponsePlanInputRequestTypeDef(TypedDict):
    arn: str,
```

## GetTimelineEventInputRequestTypeDef

```python
# GetTimelineEventInputRequestTypeDef definition

class GetTimelineEventInputRequestTypeDef(TypedDict):
    eventId: str,
    incidentRecordArn: str,
```

## IncidentRecordSourceTypeDef

```python
# IncidentRecordSourceTypeDef definition

class IncidentRecordSourceTypeDef(TypedDict):
    createdBy: str,
    source: str,
    invokedBy: NotRequired[str],
    resourceArn: NotRequired[str],
```

## NotificationTargetItemTypeDef

```python
# NotificationTargetItemTypeDef definition

class NotificationTargetItemTypeDef(TypedDict):
    snsTopicArn: NotRequired[str],
```

## PagerDutyIncidentDetailTypeDef

```python
# PagerDutyIncidentDetailTypeDef definition

class PagerDutyIncidentDetailTypeDef(TypedDict):
    id: str,
    autoResolve: NotRequired[bool],
    secretId: NotRequired[str],
```

## ListIncidentFindingsInputRequestTypeDef

```python
# ListIncidentFindingsInputRequestTypeDef definition

class ListIncidentFindingsInputRequestTypeDef(TypedDict):
    incidentRecordArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListRelatedItemsInputRequestTypeDef

```python
# ListRelatedItemsInputRequestTypeDef definition

class ListRelatedItemsInputRequestTypeDef(TypedDict):
    incidentRecordArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListReplicationSetsInputRequestTypeDef

```python
# ListReplicationSetsInputRequestTypeDef definition

class ListReplicationSetsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListResponsePlansInputRequestTypeDef

```python
# ListResponsePlansInputRequestTypeDef definition

class ListResponsePlansInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ResponsePlanSummaryTypeDef

```python
# ResponsePlanSummaryTypeDef definition

class ResponsePlanSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    displayName: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PagerDutyIncidentConfigurationTypeDef

```python
# PagerDutyIncidentConfigurationTypeDef definition

class PagerDutyIncidentConfigurationTypeDef(TypedDict):
    serviceId: str,
```

## PutResourcePolicyInputRequestTypeDef

```python
# PutResourcePolicyInputRequestTypeDef definition

class PutResourcePolicyInputRequestTypeDef(TypedDict):
    policy: str,
    resourceArn: str,
```

## RegionInfoTypeDef

```python
# RegionInfoTypeDef definition

class RegionInfoTypeDef(TypedDict):
    status: RegionStatusType,  # (1)
    statusUpdateDateTime: datetime,
    sseKmsKeyId: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RegionStatusType](./literals.md#regionstatustype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDeletionProtectionInputRequestTypeDef

```python
# UpdateDeletionProtectionInputRequestTypeDef definition

class UpdateDeletionProtectionInputRequestTypeDef(TypedDict):
    arn: str,
    deletionProtected: bool,
    clientToken: NotRequired[str],
```

## CreateReplicationSetOutputTypeDef

```python
# CreateReplicationSetOutputTypeDef definition

class CreateReplicationSetOutputTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResponsePlanOutputTypeDef

```python
# CreateResponsePlanOutputTypeDef definition

class CreateResponsePlanOutputTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTimelineEventOutputTypeDef

```python
# CreateTimelineEventOutputTypeDef definition

class CreateTimelineEventOutputTypeDef(TypedDict):
    eventId: str,
    incidentRecordArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReplicationSetsOutputTypeDef

```python
# ListReplicationSetsOutputTypeDef definition

class ListReplicationSetsOutputTypeDef(TypedDict):
    replicationSetArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyOutputTypeDef

```python
# PutResourcePolicyOutputTypeDef definition

class PutResourcePolicyOutputTypeDef(TypedDict):
    policyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartIncidentOutputTypeDef

```python
# StartIncidentOutputTypeDef definition

class StartIncidentOutputTypeDef(TypedDict):
    incidentRecordArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingDetailsTypeDef

```python
# FindingDetailsTypeDef definition

class FindingDetailsTypeDef(TypedDict):
    cloudFormationStackUpdate: NotRequired[CloudFormationStackUpdateTypeDef],  # (1)
    codeDeployDeployment: NotRequired[CodeDeployDeploymentTypeDef],  # (2)
```

1. See [:material-code-braces: CloudFormationStackUpdateTypeDef](./type_defs.md#cloudformationstackupdatetypedef) 
2. See [:material-code-braces: CodeDeployDeploymentTypeDef](./type_defs.md#codedeploydeploymenttypedef) 
## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    after: NotRequired[TimestampTypeDef],
    before: NotRequired[TimestampTypeDef],
    equals: NotRequired[AttributeValueListTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueListTypeDef](./type_defs.md#attributevaluelisttypedef) 
## TriggerDetailsTypeDef

```python
# TriggerDetailsTypeDef definition

class TriggerDetailsTypeDef(TypedDict):
    source: str,
    timestamp: TimestampTypeDef,
    rawData: NotRequired[str],
    triggerArn: NotRequired[str],
```

## CreateReplicationSetInputRequestTypeDef

```python
# CreateReplicationSetInputRequestTypeDef definition

class CreateReplicationSetInputRequestTypeDef(TypedDict):
    regions: Mapping[str, RegionMapInputValueTypeDef],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RegionMapInputValueTypeDef](./type_defs.md#regionmapinputvaluetypedef) 
## CreateTimelineEventInputRequestTypeDef

```python
# CreateTimelineEventInputRequestTypeDef definition

class CreateTimelineEventInputRequestTypeDef(TypedDict):
    eventData: str,
    eventTime: TimestampTypeDef,
    eventType: str,
    incidentRecordArn: str,
    clientToken: NotRequired[str],
    eventReferences: NotRequired[Sequence[EventReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: EventReferenceTypeDef](./type_defs.md#eventreferencetypedef) 
## EventSummaryTypeDef

```python
# EventSummaryTypeDef definition

class EventSummaryTypeDef(TypedDict):
    eventId: str,
    eventTime: datetime,
    eventType: str,
    eventUpdatedTime: datetime,
    incidentRecordArn: str,
    eventReferences: NotRequired[List[EventReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: EventReferenceTypeDef](./type_defs.md#eventreferencetypedef) 
## TimelineEventTypeDef

```python
# TimelineEventTypeDef definition

class TimelineEventTypeDef(TypedDict):
    eventData: str,
    eventId: str,
    eventTime: datetime,
    eventType: str,
    eventUpdatedTime: datetime,
    incidentRecordArn: str,
    eventReferences: NotRequired[List[EventReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: EventReferenceTypeDef](./type_defs.md#eventreferencetypedef) 
## UpdateTimelineEventInputRequestTypeDef

```python
# UpdateTimelineEventInputRequestTypeDef definition

class UpdateTimelineEventInputRequestTypeDef(TypedDict):
    eventId: str,
    incidentRecordArn: str,
    clientToken: NotRequired[str],
    eventData: NotRequired[str],
    eventReferences: NotRequired[Sequence[EventReferenceTypeDef]],  # (1)
    eventTime: NotRequired[TimestampTypeDef],
    eventType: NotRequired[str],
```

1. See [:material-code-braces: EventReferenceTypeDef](./type_defs.md#eventreferencetypedef) 
## UpdateReplicationSetActionTypeDef

```python
# UpdateReplicationSetActionTypeDef definition

class UpdateReplicationSetActionTypeDef(TypedDict):
    addRegionAction: NotRequired[AddRegionActionTypeDef],  # (1)
    deleteRegionAction: NotRequired[DeleteRegionActionTypeDef],  # (2)
```

1. See [:material-code-braces: AddRegionActionTypeDef](./type_defs.md#addregionactiontypedef) 
2. See [:material-code-braces: DeleteRegionActionTypeDef](./type_defs.md#deleteregionactiontypedef) 
## SsmAutomationOutputTypeDef

```python
# SsmAutomationOutputTypeDef definition

class SsmAutomationOutputTypeDef(TypedDict):
    documentName: str,
    roleArn: str,
    documentVersion: NotRequired[str],
    dynamicParameters: NotRequired[Dict[str, DynamicSsmParameterValueTypeDef]],  # (1)
    parameters: NotRequired[Dict[str, List[str]]],
    targetAccount: NotRequired[SsmTargetAccountType],  # (2)
```

1. See [:material-code-braces: DynamicSsmParameterValueTypeDef](./type_defs.md#dynamicssmparametervaluetypedef) 
2. See [:material-code-brackets: SsmTargetAccountType](./literals.md#ssmtargetaccounttype) 
## SsmAutomationTypeDef

```python
# SsmAutomationTypeDef definition

class SsmAutomationTypeDef(TypedDict):
    documentName: str,
    roleArn: str,
    documentVersion: NotRequired[str],
    dynamicParameters: NotRequired[Mapping[str, DynamicSsmParameterValueTypeDef]],  # (1)
    parameters: NotRequired[Mapping[str, Sequence[str]]],
    targetAccount: NotRequired[SsmTargetAccountType],  # (2)
```

1. See [:material-code-braces: DynamicSsmParameterValueTypeDef](./type_defs.md#dynamicssmparametervaluetypedef) 
2. See [:material-code-brackets: SsmTargetAccountType](./literals.md#ssmtargetaccounttype) 
## ListIncidentFindingsOutputTypeDef

```python
# ListIncidentFindingsOutputTypeDef definition

class ListIncidentFindingsOutputTypeDef(TypedDict):
    findings: List[FindingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FindingSummaryTypeDef](./type_defs.md#findingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef

```python
# GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef definition

class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(TypedDict):
    arn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef

```python
# GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef definition

class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(TypedDict):
    arn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef

```python
# GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef definition

class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIncidentFindingsInputListIncidentFindingsPaginateTypeDef

```python
# ListIncidentFindingsInputListIncidentFindingsPaginateTypeDef definition

class ListIncidentFindingsInputListIncidentFindingsPaginateTypeDef(TypedDict):
    incidentRecordArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRelatedItemsInputListRelatedItemsPaginateTypeDef

```python
# ListRelatedItemsInputListRelatedItemsPaginateTypeDef definition

class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(TypedDict):
    incidentRecordArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReplicationSetsInputListReplicationSetsPaginateTypeDef

```python
# ListReplicationSetsInputListReplicationSetsPaginateTypeDef definition

class ListReplicationSetsInputListReplicationSetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResponsePlansInputListResponsePlansPaginateTypeDef

```python
# ListResponsePlansInputListResponsePlansPaginateTypeDef definition

class ListResponsePlansInputListResponsePlansPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcePoliciesOutputTypeDef

```python
# GetResourcePoliciesOutputTypeDef definition

class GetResourcePoliciesOutputTypeDef(TypedDict):
    resourcePolicies: List[ResourcePolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncidentRecordSummaryTypeDef

```python
# IncidentRecordSummaryTypeDef definition

class IncidentRecordSummaryTypeDef(TypedDict):
    arn: str,
    creationTime: datetime,
    impact: int,
    incidentRecordSource: IncidentRecordSourceTypeDef,  # (1)
    status: IncidentRecordStatusType,  # (2)
    title: str,
    resolvedTime: NotRequired[datetime],
```

1. See [:material-code-braces: IncidentRecordSourceTypeDef](./type_defs.md#incidentrecordsourcetypedef) 
2. See [:material-code-brackets: IncidentRecordStatusType](./literals.md#incidentrecordstatustype) 
## IncidentRecordTypeDef

```python
# IncidentRecordTypeDef definition

class IncidentRecordTypeDef(TypedDict):
    arn: str,
    creationTime: datetime,
    dedupeString: str,
    impact: int,
    incidentRecordSource: IncidentRecordSourceTypeDef,  # (3)
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    status: IncidentRecordStatusType,  # (5)
    title: str,
    automationExecutions: NotRequired[List[AutomationExecutionTypeDef]],  # (1)
    chatChannel: NotRequired[ChatChannelOutputTypeDef],  # (2)
    notificationTargets: NotRequired[List[NotificationTargetItemTypeDef]],  # (4)
    resolvedTime: NotRequired[datetime],
    summary: NotRequired[str],
```

1. See [:material-code-braces: AutomationExecutionTypeDef](./type_defs.md#automationexecutiontypedef) 
2. See [:material-code-braces: ChatChannelOutputTypeDef](./type_defs.md#chatchanneloutputtypedef) 
3. See [:material-code-braces: IncidentRecordSourceTypeDef](./type_defs.md#incidentrecordsourcetypedef) 
4. See [:material-code-braces: NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef) 
5. See [:material-code-brackets: IncidentRecordStatusType](./literals.md#incidentrecordstatustype) 
## IncidentTemplateOutputTypeDef

```python
# IncidentTemplateOutputTypeDef definition

class IncidentTemplateOutputTypeDef(TypedDict):
    impact: int,
    title: str,
    dedupeString: NotRequired[str],
    incidentTags: NotRequired[Dict[str, str]],
    notificationTargets: NotRequired[List[NotificationTargetItemTypeDef]],  # (1)
    summary: NotRequired[str],
```

1. See [:material-code-braces: NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef) 
## IncidentTemplateTypeDef

```python
# IncidentTemplateTypeDef definition

class IncidentTemplateTypeDef(TypedDict):
    impact: int,
    title: str,
    dedupeString: NotRequired[str],
    incidentTags: NotRequired[Mapping[str, str]],
    notificationTargets: NotRequired[Sequence[NotificationTargetItemTypeDef]],  # (1)
    summary: NotRequired[str],
```

1. See [:material-code-braces: NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef) 
## UpdateIncidentRecordInputRequestTypeDef

```python
# UpdateIncidentRecordInputRequestTypeDef definition

class UpdateIncidentRecordInputRequestTypeDef(TypedDict):
    arn: str,
    chatChannel: NotRequired[ChatChannelTypeDef],  # (1)
    clientToken: NotRequired[str],
    impact: NotRequired[int],
    notificationTargets: NotRequired[Sequence[NotificationTargetItemTypeDef]],  # (2)
    status: NotRequired[IncidentRecordStatusType],  # (3)
    summary: NotRequired[str],
    title: NotRequired[str],
```

1. See [:material-code-braces: ChatChannelTypeDef](./type_defs.md#chatchanneltypedef) 
2. See [:material-code-braces: NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef) 
3. See [:material-code-brackets: IncidentRecordStatusType](./literals.md#incidentrecordstatustype) 
## ItemValueTypeDef

```python
# ItemValueTypeDef definition

class ItemValueTypeDef(TypedDict):
    arn: NotRequired[str],
    metricDefinition: NotRequired[str],
    pagerDutyIncidentDetail: NotRequired[PagerDutyIncidentDetailTypeDef],  # (1)
    url: NotRequired[str],
```

1. See [:material-code-braces: PagerDutyIncidentDetailTypeDef](./type_defs.md#pagerdutyincidentdetailtypedef) 
## ListResponsePlansOutputTypeDef

```python
# ListResponsePlansOutputTypeDef definition

class ListResponsePlansOutputTypeDef(TypedDict):
    responsePlanSummaries: List[ResponsePlanSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponsePlanSummaryTypeDef](./type_defs.md#responseplansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PagerDutyConfigurationTypeDef

```python
# PagerDutyConfigurationTypeDef definition

class PagerDutyConfigurationTypeDef(TypedDict):
    name: str,
    pagerDutyIncidentConfiguration: PagerDutyIncidentConfigurationTypeDef,  # (1)
    secretId: str,
```

1. See [:material-code-braces: PagerDutyIncidentConfigurationTypeDef](./type_defs.md#pagerdutyincidentconfigurationtypedef) 
## ReplicationSetTypeDef

```python
# ReplicationSetTypeDef definition

class ReplicationSetTypeDef(TypedDict):
    createdBy: str,
    createdTime: datetime,
    deletionProtected: bool,
    lastModifiedBy: str,
    lastModifiedTime: datetime,
    regionMap: Dict[str, RegionInfoTypeDef],  # (1)
    status: ReplicationSetStatusType,  # (2)
    arn: NotRequired[str],
```

1. See [:material-code-braces: RegionInfoTypeDef](./type_defs.md#regioninfotypedef) 
2. See [:material-code-brackets: ReplicationSetStatusType](./literals.md#replicationsetstatustype) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    creationTime: datetime,
    id: str,
    lastModifiedTime: datetime,
    details: NotRequired[FindingDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: FindingDetailsTypeDef](./type_defs.md#findingdetailstypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    condition: ConditionTypeDef,  # (1)
    key: str,
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## ListTimelineEventsOutputTypeDef

```python
# ListTimelineEventsOutputTypeDef definition

class ListTimelineEventsOutputTypeDef(TypedDict):
    eventSummaries: List[EventSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventSummaryTypeDef](./type_defs.md#eventsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTimelineEventOutputTypeDef

```python
# GetTimelineEventOutputTypeDef definition

class GetTimelineEventOutputTypeDef(TypedDict):
    event: TimelineEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimelineEventTypeDef](./type_defs.md#timelineeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationSetInputRequestTypeDef

```python
# UpdateReplicationSetInputRequestTypeDef definition

class UpdateReplicationSetInputRequestTypeDef(TypedDict):
    actions: Sequence[UpdateReplicationSetActionTypeDef],  # (1)
    arn: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateReplicationSetActionTypeDef](./type_defs.md#updatereplicationsetactiontypedef) 
## ActionOutputTypeDef

```python
# ActionOutputTypeDef definition

class ActionOutputTypeDef(TypedDict):
    ssmAutomation: NotRequired[SsmAutomationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SsmAutomationOutputTypeDef](./type_defs.md#ssmautomationoutputtypedef) 
## ListIncidentRecordsOutputTypeDef

```python
# ListIncidentRecordsOutputTypeDef definition

class ListIncidentRecordsOutputTypeDef(TypedDict):
    incidentRecordSummaries: List[IncidentRecordSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IncidentRecordSummaryTypeDef](./type_defs.md#incidentrecordsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIncidentRecordOutputTypeDef

```python
# GetIncidentRecordOutputTypeDef definition

class GetIncidentRecordOutputTypeDef(TypedDict):
    incidentRecord: IncidentRecordTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IncidentRecordTypeDef](./type_defs.md#incidentrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ItemIdentifierTypeDef

```python
# ItemIdentifierTypeDef definition

class ItemIdentifierTypeDef(TypedDict):
    type: ItemTypeType,  # (1)
    value: ItemValueTypeDef,  # (2)
```

1. See [:material-code-brackets: ItemTypeType](./literals.md#itemtypetype) 
2. See [:material-code-braces: ItemValueTypeDef](./type_defs.md#itemvaluetypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    pagerDutyConfiguration: NotRequired[PagerDutyConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PagerDutyConfigurationTypeDef](./type_defs.md#pagerdutyconfigurationtypedef) 
## GetReplicationSetOutputTypeDef

```python
# GetReplicationSetOutputTypeDef definition

class GetReplicationSetOutputTypeDef(TypedDict):
    replicationSet: ReplicationSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationSetTypeDef](./type_defs.md#replicationsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetIncidentFindingsOutputTypeDef

```python
# BatchGetIncidentFindingsOutputTypeDef definition

class BatchGetIncidentFindingsOutputTypeDef(TypedDict):
    errors: List[BatchGetIncidentFindingsErrorTypeDef],  # (1)
    findings: List[FindingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetIncidentFindingsErrorTypeDef](./type_defs.md#batchgetincidentfindingserrortypedef) 
2. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef

```python
# ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef definition

class ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIncidentRecordsInputRequestTypeDef

```python
# ListIncidentRecordsInputRequestTypeDef definition

class ListIncidentRecordsInputRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListTimelineEventsInputListTimelineEventsPaginateTypeDef

```python
# ListTimelineEventsInputListTimelineEventsPaginateTypeDef definition

class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(TypedDict):
    incidentRecordArn: str,
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    sortBy: NotRequired[TimelineEventSortType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: TimelineEventSortType](./literals.md#timelineeventsorttype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTimelineEventsInputRequestTypeDef

```python
# ListTimelineEventsInputRequestTypeDef definition

class ListTimelineEventsInputRequestTypeDef(TypedDict):
    incidentRecordArn: str,
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[TimelineEventSortType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: TimelineEventSortType](./literals.md#timelineeventsorttype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    ssmAutomation: NotRequired[SsmAutomationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SsmAutomationTypeDef](./type_defs.md#ssmautomationtypedef) [:material-code-braces: SsmAutomationOutputTypeDef](./type_defs.md#ssmautomationoutputtypedef) 
## RelatedItemTypeDef

```python
# RelatedItemTypeDef definition

class RelatedItemTypeDef(TypedDict):
    identifier: ItemIdentifierTypeDef,  # (1)
    generatedId: NotRequired[str],
    title: NotRequired[str],
```

1. See [:material-code-braces: ItemIdentifierTypeDef](./type_defs.md#itemidentifiertypedef) 
## GetResponsePlanOutputTypeDef

```python
# GetResponsePlanOutputTypeDef definition

class GetResponsePlanOutputTypeDef(TypedDict):
    actions: List[ActionOutputTypeDef],  # (1)
    arn: str,
    chatChannel: ChatChannelOutputTypeDef,  # (2)
    displayName: str,
    engagements: List[str],
    incidentTemplate: IncidentTemplateOutputTypeDef,  # (3)
    integrations: List[IntegrationTypeDef],  # (4)
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-braces: ChatChannelOutputTypeDef](./type_defs.md#chatchanneloutputtypedef) 
3. See [:material-code-braces: IncidentTemplateOutputTypeDef](./type_defs.md#incidenttemplateoutputtypedef) 
4. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResponsePlanInputRequestTypeDef

```python
# UpdateResponsePlanInputRequestTypeDef definition

class UpdateResponsePlanInputRequestTypeDef(TypedDict):
    arn: str,
    actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
    chatChannel: NotRequired[ChatChannelTypeDef],  # (2)
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    engagements: NotRequired[Sequence[str]],
    incidentTemplateDedupeString: NotRequired[str],
    incidentTemplateImpact: NotRequired[int],
    incidentTemplateNotificationTargets: NotRequired[Sequence[NotificationTargetItemTypeDef]],  # (3)
    incidentTemplateSummary: NotRequired[str],
    incidentTemplateTags: NotRequired[Mapping[str, str]],
    incidentTemplateTitle: NotRequired[str],
    integrations: NotRequired[Sequence[IntegrationTypeDef]],  # (4)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ChatChannelTypeDef](./type_defs.md#chatchanneltypedef) 
3. See [:material-code-braces: NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef) 
4. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
## ListRelatedItemsOutputTypeDef

```python
# ListRelatedItemsOutputTypeDef definition

class ListRelatedItemsOutputTypeDef(TypedDict):
    relatedItems: List[RelatedItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RelatedItemTypeDef](./type_defs.md#relateditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RelatedItemsUpdateTypeDef

```python
# RelatedItemsUpdateTypeDef definition

class RelatedItemsUpdateTypeDef(TypedDict):
    itemToAdd: NotRequired[RelatedItemTypeDef],  # (1)
    itemToRemove: NotRequired[ItemIdentifierTypeDef],  # (2)
```

1. See [:material-code-braces: RelatedItemTypeDef](./type_defs.md#relateditemtypedef) 
2. See [:material-code-braces: ItemIdentifierTypeDef](./type_defs.md#itemidentifiertypedef) 
## StartIncidentInputRequestTypeDef

```python
# StartIncidentInputRequestTypeDef definition

class StartIncidentInputRequestTypeDef(TypedDict):
    responsePlanArn: str,
    clientToken: NotRequired[str],
    impact: NotRequired[int],
    relatedItems: NotRequired[Sequence[RelatedItemTypeDef]],  # (1)
    title: NotRequired[str],
    triggerDetails: NotRequired[TriggerDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: RelatedItemTypeDef](./type_defs.md#relateditemtypedef) 
2. See [:material-code-braces: TriggerDetailsTypeDef](./type_defs.md#triggerdetailstypedef) 
## CreateResponsePlanInputRequestTypeDef

```python
# CreateResponsePlanInputRequestTypeDef definition

class CreateResponsePlanInputRequestTypeDef(TypedDict):
    incidentTemplate: IncidentTemplateTypeDef,  # (1)
    name: str,
    actions: NotRequired[Sequence[ActionUnionTypeDef]],  # (2)
    chatChannel: NotRequired[ChatChannelTypeDef],  # (3)
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    engagements: NotRequired[Sequence[str]],
    integrations: NotRequired[Sequence[IntegrationTypeDef]],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IncidentTemplateTypeDef](./type_defs.md#incidenttemplatetypedef) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
3. See [:material-code-braces: ChatChannelTypeDef](./type_defs.md#chatchanneltypedef) 
4. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
## UpdateRelatedItemsInputRequestTypeDef

```python
# UpdateRelatedItemsInputRequestTypeDef definition

class UpdateRelatedItemsInputRequestTypeDef(TypedDict):
    incidentRecordArn: str,
    relatedItemsUpdate: RelatedItemsUpdateTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: RelatedItemsUpdateTypeDef](./type_defs.md#relateditemsupdatetypedef) 
