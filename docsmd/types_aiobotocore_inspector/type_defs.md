# Type definitions

> [Index](../README.md) > [Inspector](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
    type annotations stubs module [types-aiobotocore-inspector](https://pypi.org/project/types-aiobotocore-inspector/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## FailedItemDetailsTypeDef

```python
# FailedItemDetailsTypeDef definition

class FailedItemDetailsTypeDef(TypedDict):
    failureCode: FailedItemErrorCodeType,  # (1)
    retryable: bool,
```

1. See [:material-code-brackets: FailedItemErrorCodeType](./literals.md#faileditemerrorcodetype) 
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

## AgentFilterTypeDef

```python
# AgentFilterTypeDef definition

class AgentFilterTypeDef(TypedDict):
    agentHealths: Sequence[AgentHealthType],  # (1)
    agentHealthCodes: Sequence[AgentHealthCodeType],  # (2)
```

1. See [:material-code-brackets: AgentHealthType](./literals.md#agenthealthtype) 
2. See [:material-code-brackets: AgentHealthCodeType](./literals.md#agenthealthcodetype) 
## AgentPreviewTypeDef

```python
# AgentPreviewTypeDef definition

class AgentPreviewTypeDef(TypedDict):
    agentId: str,
    hostname: NotRequired[str],
    autoScalingGroup: NotRequired[str],
    agentHealth: NotRequired[AgentHealthType],  # (1)
    agentVersion: NotRequired[str],
    operatingSystem: NotRequired[str],
    kernelVersion: NotRequired[str],
    ipv4Address: NotRequired[str],
```

1. See [:material-code-brackets: AgentHealthType](./literals.md#agenthealthtype) 
## TelemetryMetadataTypeDef

```python
# TelemetryMetadataTypeDef definition

class TelemetryMetadataTypeDef(TypedDict):
    messageType: str,
    count: int,
    dataSize: NotRequired[int],
```

## DurationRangeTypeDef

```python
# DurationRangeTypeDef definition

class DurationRangeTypeDef(TypedDict):
    minSeconds: NotRequired[int],
    maxSeconds: NotRequired[int],
```

## AssessmentRunNotificationTypeDef

```python
# AssessmentRunNotificationTypeDef definition

class AssessmentRunNotificationTypeDef(TypedDict):
    date: datetime,
    event: InspectorEventType,  # (1)
    error: bool,
    message: NotRequired[str],
    snsTopicArn: NotRequired[str],
    snsPublishStatusCode: NotRequired[AssessmentRunNotificationSnsStatusCodeType],  # (2)
```

1. See [:material-code-brackets: InspectorEventType](./literals.md#inspectoreventtype) 
2. See [:material-code-brackets: AssessmentRunNotificationSnsStatusCodeType](./literals.md#assessmentrunnotificationsnsstatuscodetype) 
## AssessmentRunStateChangeTypeDef

```python
# AssessmentRunStateChangeTypeDef definition

class AssessmentRunStateChangeTypeDef(TypedDict):
    stateChangedAt: datetime,
    state: AssessmentRunStateType,  # (1)
```

1. See [:material-code-brackets: AssessmentRunStateType](./literals.md#assessmentrunstatetype) 
## AssessmentTargetFilterTypeDef

```python
# AssessmentTargetFilterTypeDef definition

class AssessmentTargetFilterTypeDef(TypedDict):
    assessmentTargetNamePattern: NotRequired[str],
```

## AssessmentTargetTypeDef

```python
# AssessmentTargetTypeDef definition

class AssessmentTargetTypeDef(TypedDict):
    arn: str,
    name: str,
    createdAt: datetime,
    updatedAt: datetime,
    resourceGroupArn: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## CreateAssessmentTargetRequestRequestTypeDef

```python
# CreateAssessmentTargetRequestRequestTypeDef definition

class CreateAssessmentTargetRequestRequestTypeDef(TypedDict):
    assessmentTargetName: str,
    resourceGroupArn: NotRequired[str],
```

## CreateExclusionsPreviewRequestRequestTypeDef

```python
# CreateExclusionsPreviewRequestRequestTypeDef definition

class CreateExclusionsPreviewRequestRequestTypeDef(TypedDict):
    assessmentTemplateArn: str,
```

## ResourceGroupTagTypeDef

```python
# ResourceGroupTagTypeDef definition

class ResourceGroupTagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## DeleteAssessmentRunRequestRequestTypeDef

```python
# DeleteAssessmentRunRequestRequestTypeDef definition

class DeleteAssessmentRunRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
```

## DeleteAssessmentTargetRequestRequestTypeDef

```python
# DeleteAssessmentTargetRequestRequestTypeDef definition

class DeleteAssessmentTargetRequestRequestTypeDef(TypedDict):
    assessmentTargetArn: str,
```

## DeleteAssessmentTemplateRequestRequestTypeDef

```python
# DeleteAssessmentTemplateRequestRequestTypeDef definition

class DeleteAssessmentTemplateRequestRequestTypeDef(TypedDict):
    assessmentTemplateArn: str,
```

## DescribeAssessmentRunsRequestRequestTypeDef

```python
# DescribeAssessmentRunsRequestRequestTypeDef definition

class DescribeAssessmentRunsRequestRequestTypeDef(TypedDict):
    assessmentRunArns: Sequence[str],
```

## DescribeAssessmentTargetsRequestRequestTypeDef

```python
# DescribeAssessmentTargetsRequestRequestTypeDef definition

class DescribeAssessmentTargetsRequestRequestTypeDef(TypedDict):
    assessmentTargetArns: Sequence[str],
```

## DescribeAssessmentTemplatesRequestRequestTypeDef

```python
# DescribeAssessmentTemplatesRequestRequestTypeDef definition

class DescribeAssessmentTemplatesRequestRequestTypeDef(TypedDict):
    assessmentTemplateArns: Sequence[str],
```

## DescribeExclusionsRequestRequestTypeDef

```python
# DescribeExclusionsRequestRequestTypeDef definition

class DescribeExclusionsRequestRequestTypeDef(TypedDict):
    exclusionArns: Sequence[str],
    locale: NotRequired[LocaleType],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## DescribeFindingsRequestRequestTypeDef

```python
# DescribeFindingsRequestRequestTypeDef definition

class DescribeFindingsRequestRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
    locale: NotRequired[LocaleType],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## DescribeResourceGroupsRequestRequestTypeDef

```python
# DescribeResourceGroupsRequestRequestTypeDef definition

class DescribeResourceGroupsRequestRequestTypeDef(TypedDict):
    resourceGroupArns: Sequence[str],
```

## DescribeRulesPackagesRequestRequestTypeDef

```python
# DescribeRulesPackagesRequestRequestTypeDef definition

class DescribeRulesPackagesRequestRequestTypeDef(TypedDict):
    rulesPackageArns: Sequence[str],
    locale: NotRequired[LocaleType],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## RulesPackageTypeDef

```python
# RulesPackageTypeDef definition

class RulesPackageTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    provider: str,
    description: NotRequired[str],
```

## EventSubscriptionTypeDef

```python
# EventSubscriptionTypeDef definition

class EventSubscriptionTypeDef(TypedDict):
    event: InspectorEventType,  # (1)
    subscribedAt: datetime,
```

1. See [:material-code-brackets: InspectorEventType](./literals.md#inspectoreventtype) 
## ScopeTypeDef

```python
# ScopeTypeDef definition

class ScopeTypeDef(TypedDict):
    key: NotRequired[ScopeTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ScopeTypeType](./literals.md#scopetypetype) 
## InspectorServiceAttributesTypeDef

```python
# InspectorServiceAttributesTypeDef definition

class InspectorServiceAttributesTypeDef(TypedDict):
    schemaVersion: int,
    assessmentRunArn: NotRequired[str],
    rulesPackageArn: NotRequired[str],
```

## GetAssessmentReportRequestRequestTypeDef

```python
# GetAssessmentReportRequestRequestTypeDef definition

class GetAssessmentReportRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
    reportFileFormat: ReportFileFormatType,  # (1)
    reportType: ReportTypeType,  # (2)
```

1. See [:material-code-brackets: ReportFileFormatType](./literals.md#reportfileformattype) 
2. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
## GetExclusionsPreviewRequestRequestTypeDef

```python
# GetExclusionsPreviewRequestRequestTypeDef definition

class GetExclusionsPreviewRequestRequestTypeDef(TypedDict):
    assessmentTemplateArn: str,
    previewToken: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    locale: NotRequired[LocaleType],  # (1)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## GetTelemetryMetadataRequestRequestTypeDef

```python
# GetTelemetryMetadataRequestRequestTypeDef definition

class GetTelemetryMetadataRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEventSubscriptionsRequestRequestTypeDef

```python
# ListEventSubscriptionsRequestRequestTypeDef definition

class ListEventSubscriptionsRequestRequestTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListExclusionsRequestRequestTypeDef

```python
# ListExclusionsRequestRequestTypeDef definition

class ListExclusionsRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListRulesPackagesRequestRequestTypeDef

```python
# ListRulesPackagesRequestRequestTypeDef definition

class ListRulesPackagesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PrivateIpTypeDef

```python
# PrivateIpTypeDef definition

class PrivateIpTypeDef(TypedDict):
    privateDnsName: NotRequired[str],
    privateIpAddress: NotRequired[str],
```

## SecurityGroupTypeDef

```python
# SecurityGroupTypeDef definition

class SecurityGroupTypeDef(TypedDict):
    groupName: NotRequired[str],
    groupId: NotRequired[str],
```

## PreviewAgentsRequestRequestTypeDef

```python
# PreviewAgentsRequestRequestTypeDef definition

class PreviewAgentsRequestRequestTypeDef(TypedDict):
    previewAgentsArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RegisterCrossAccountAccessRoleRequestRequestTypeDef

```python
# RegisterCrossAccountAccessRoleRequestRequestTypeDef definition

class RegisterCrossAccountAccessRoleRequestRequestTypeDef(TypedDict):
    roleArn: str,
```

## RemoveAttributesFromFindingsRequestRequestTypeDef

```python
# RemoveAttributesFromFindingsRequestRequestTypeDef definition

class RemoveAttributesFromFindingsRequestRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
    attributeKeys: Sequence[str],
```

## StartAssessmentRunRequestRequestTypeDef

```python
# StartAssessmentRunRequestRequestTypeDef definition

class StartAssessmentRunRequestRequestTypeDef(TypedDict):
    assessmentTemplateArn: str,
    assessmentRunName: NotRequired[str],
```

## StopAssessmentRunRequestRequestTypeDef

```python
# StopAssessmentRunRequestRequestTypeDef definition

class StopAssessmentRunRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
    stopAction: NotRequired[StopActionType],  # (1)
```

1. See [:material-code-brackets: StopActionType](./literals.md#stopactiontype) 
## SubscribeToEventRequestRequestTypeDef

```python
# SubscribeToEventRequestRequestTypeDef definition

class SubscribeToEventRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    event: InspectorEventType,  # (1)
    topicArn: str,
```

1. See [:material-code-brackets: InspectorEventType](./literals.md#inspectoreventtype) 
## UnsubscribeFromEventRequestRequestTypeDef

```python
# UnsubscribeFromEventRequestRequestTypeDef definition

class UnsubscribeFromEventRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    event: InspectorEventType,  # (1)
    topicArn: str,
```

1. See [:material-code-brackets: InspectorEventType](./literals.md#inspectoreventtype) 
## UpdateAssessmentTargetRequestRequestTypeDef

```python
# UpdateAssessmentTargetRequestRequestTypeDef definition

class UpdateAssessmentTargetRequestRequestTypeDef(TypedDict):
    assessmentTargetArn: str,
    assessmentTargetName: str,
    resourceGroupArn: NotRequired[str],
```

## AddAttributesToFindingsRequestRequestTypeDef

```python
# AddAttributesToFindingsRequestRequestTypeDef definition

class AddAttributesToFindingsRequestRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
    attributes: Sequence[AttributeTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## AssessmentTemplateTypeDef

```python
# AssessmentTemplateTypeDef definition

class AssessmentTemplateTypeDef(TypedDict):
    arn: str,
    name: str,
    assessmentTargetArn: str,
    durationInSeconds: int,
    rulesPackageArns: List[str],
    userAttributesForFindings: List[AttributeTypeDef],  # (1)
    assessmentRunCount: int,
    createdAt: datetime,
    lastAssessmentRunArn: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## CreateAssessmentTemplateRequestRequestTypeDef

```python
# CreateAssessmentTemplateRequestRequestTypeDef definition

class CreateAssessmentTemplateRequestRequestTypeDef(TypedDict):
    assessmentTargetArn: str,
    assessmentTemplateName: str,
    durationInSeconds: int,
    rulesPackageArns: Sequence[str],
    userAttributesForFindings: NotRequired[Sequence[AttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## AddAttributesToFindingsResponseTypeDef

```python
# AddAttributesToFindingsResponseTypeDef definition

class AddAttributesToFindingsResponseTypeDef(TypedDict):
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssessmentTargetResponseTypeDef

```python
# CreateAssessmentTargetResponseTypeDef definition

class CreateAssessmentTargetResponseTypeDef(TypedDict):
    assessmentTargetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssessmentTemplateResponseTypeDef

```python
# CreateAssessmentTemplateResponseTypeDef definition

class CreateAssessmentTemplateResponseTypeDef(TypedDict):
    assessmentTemplateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExclusionsPreviewResponseTypeDef

```python
# CreateExclusionsPreviewResponseTypeDef definition

class CreateExclusionsPreviewResponseTypeDef(TypedDict):
    previewToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceGroupResponseTypeDef

```python
# CreateResourceGroupResponseTypeDef definition

class CreateResourceGroupResponseTypeDef(TypedDict):
    resourceGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCrossAccountAccessRoleResponseTypeDef

```python
# DescribeCrossAccountAccessRoleResponseTypeDef definition

class DescribeCrossAccountAccessRoleResponseTypeDef(TypedDict):
    roleArn: str,
    valid: bool,
    registeredAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssessmentReportResponseTypeDef

```python
# GetAssessmentReportResponseTypeDef definition

class GetAssessmentReportResponseTypeDef(TypedDict):
    status: ReportStatusType,  # (1)
    url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReportStatusType](./literals.md#reportstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentRunsResponseTypeDef

```python
# ListAssessmentRunsResponseTypeDef definition

class ListAssessmentRunsResponseTypeDef(TypedDict):
    assessmentRunArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentTargetsResponseTypeDef

```python
# ListAssessmentTargetsResponseTypeDef definition

class ListAssessmentTargetsResponseTypeDef(TypedDict):
    assessmentTargetArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentTemplatesResponseTypeDef

```python
# ListAssessmentTemplatesResponseTypeDef definition

class ListAssessmentTemplatesResponseTypeDef(TypedDict):
    assessmentTemplateArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExclusionsResponseTypeDef

```python
# ListExclusionsResponseTypeDef definition

class ListExclusionsResponseTypeDef(TypedDict):
    exclusionArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsResponseTypeDef

```python
# ListFindingsResponseTypeDef definition

class ListFindingsResponseTypeDef(TypedDict):
    findingArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesPackagesResponseTypeDef

```python
# ListRulesPackagesResponseTypeDef definition

class ListRulesPackagesResponseTypeDef(TypedDict):
    rulesPackageArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveAttributesFromFindingsResponseTypeDef

```python
# RemoveAttributesFromFindingsResponseTypeDef definition

class RemoveAttributesFromFindingsResponseTypeDef(TypedDict):
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssessmentRunResponseTypeDef

```python
# StartAssessmentRunResponseTypeDef definition

class StartAssessmentRunResponseTypeDef(TypedDict):
    assessmentRunArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentRunAgentsRequestRequestTypeDef

```python
# ListAssessmentRunAgentsRequestRequestTypeDef definition

class ListAssessmentRunAgentsRequestRequestTypeDef(TypedDict):
    assessmentRunArn: str,
    filter: NotRequired[AgentFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: AgentFilterTypeDef](./type_defs.md#agentfiltertypedef) 
## PreviewAgentsResponseTypeDef

```python
# PreviewAgentsResponseTypeDef definition

class PreviewAgentsResponseTypeDef(TypedDict):
    agentPreviews: List[AgentPreviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentPreviewTypeDef](./type_defs.md#agentpreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentRunAgentTypeDef

```python
# AssessmentRunAgentTypeDef definition

class AssessmentRunAgentTypeDef(TypedDict):
    agentId: str,
    assessmentRunArn: str,
    agentHealth: AgentHealthType,  # (1)
    agentHealthCode: AgentHealthCodeType,  # (2)
    telemetryMetadata: List[TelemetryMetadataTypeDef],  # (3)
    agentHealthDetails: NotRequired[str],
    autoScalingGroup: NotRequired[str],
```

1. See [:material-code-brackets: AgentHealthType](./literals.md#agenthealthtype) 
2. See [:material-code-brackets: AgentHealthCodeType](./literals.md#agenthealthcodetype) 
3. See [:material-code-braces: TelemetryMetadataTypeDef](./type_defs.md#telemetrymetadatatypedef) 
## GetTelemetryMetadataResponseTypeDef

```python
# GetTelemetryMetadataResponseTypeDef definition

class GetTelemetryMetadataResponseTypeDef(TypedDict):
    telemetryMetadata: List[TelemetryMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TelemetryMetadataTypeDef](./type_defs.md#telemetrymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentTemplateFilterTypeDef

```python
# AssessmentTemplateFilterTypeDef definition

class AssessmentTemplateFilterTypeDef(TypedDict):
    namePattern: NotRequired[str],
    durationRange: NotRequired[DurationRangeTypeDef],  # (1)
    rulesPackageArns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: DurationRangeTypeDef](./type_defs.md#durationrangetypedef) 
## AssessmentRunTypeDef

```python
# AssessmentRunTypeDef definition

class AssessmentRunTypeDef(TypedDict):
    arn: str,
    name: str,
    assessmentTemplateArn: str,
    state: AssessmentRunStateType,  # (1)
    durationInSeconds: int,
    rulesPackageArns: List[str],
    userAttributesForFindings: List[AttributeTypeDef],  # (2)
    createdAt: datetime,
    stateChangedAt: datetime,
    dataCollected: bool,
    stateChanges: List[AssessmentRunStateChangeTypeDef],  # (3)
    notifications: List[AssessmentRunNotificationTypeDef],  # (4)
    findingCounts: Dict[SeverityType, int],  # (5)
    startedAt: NotRequired[datetime],
    completedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: AssessmentRunStateType](./literals.md#assessmentrunstatetype) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
3. See [:material-code-braces: AssessmentRunStateChangeTypeDef](./type_defs.md#assessmentrunstatechangetypedef) 
4. See [:material-code-braces: AssessmentRunNotificationTypeDef](./type_defs.md#assessmentrunnotificationtypedef) 
5. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
## ListAssessmentTargetsRequestRequestTypeDef

```python
# ListAssessmentTargetsRequestRequestTypeDef definition

class ListAssessmentTargetsRequestRequestTypeDef(TypedDict):
    filter: NotRequired[AssessmentTargetFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: AssessmentTargetFilterTypeDef](./type_defs.md#assessmenttargetfiltertypedef) 
## DescribeAssessmentTargetsResponseTypeDef

```python
# DescribeAssessmentTargetsResponseTypeDef definition

class DescribeAssessmentTargetsResponseTypeDef(TypedDict):
    assessmentTargets: List[AssessmentTargetTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssessmentTargetTypeDef](./type_defs.md#assessmenttargettypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetTagsForResourceRequestRequestTypeDef

```python
# SetTagsForResourceRequestRequestTypeDef definition

class SetTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateResourceGroupRequestRequestTypeDef

```python
# CreateResourceGroupRequestRequestTypeDef definition

class CreateResourceGroupRequestRequestTypeDef(TypedDict):
    resourceGroupTags: Sequence[ResourceGroupTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceGroupTagTypeDef](./type_defs.md#resourcegrouptagtypedef) 
## ResourceGroupTypeDef

```python
# ResourceGroupTypeDef definition

class ResourceGroupTypeDef(TypedDict):
    arn: str,
    tags: List[ResourceGroupTagTypeDef],  # (1)
    createdAt: datetime,
```

1. See [:material-code-braces: ResourceGroupTagTypeDef](./type_defs.md#resourcegrouptagtypedef) 
## DescribeRulesPackagesResponseTypeDef

```python
# DescribeRulesPackagesResponseTypeDef definition

class DescribeRulesPackagesResponseTypeDef(TypedDict):
    rulesPackages: List[RulesPackageTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RulesPackageTypeDef](./type_defs.md#rulespackagetypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    resourceArn: str,
    topicArn: str,
    eventSubscriptions: List[EventSubscriptionTypeDef],  # (1)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
## ExclusionPreviewTypeDef

```python
# ExclusionPreviewTypeDef definition

class ExclusionPreviewTypeDef(TypedDict):
    title: str,
    description: str,
    recommendation: str,
    scopes: List[ScopeTypeDef],  # (1)
    attributes: NotRequired[List[AttributeTypeDef]],  # (2)
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ExclusionTypeDef

```python
# ExclusionTypeDef definition

class ExclusionTypeDef(TypedDict):
    arn: str,
    title: str,
    description: str,
    recommendation: str,
    scopes: List[ScopeTypeDef],  # (1)
    attributes: NotRequired[List[AttributeTypeDef]],  # (2)
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef

```python
# ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef definition

class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(TypedDict):
    assessmentRunArn: str,
    filter: NotRequired[AgentFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AgentFilterTypeDef](./type_defs.md#agentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef

```python
# ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef definition

class ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef(TypedDict):
    filter: NotRequired[AssessmentTargetFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssessmentTargetFilterTypeDef](./type_defs.md#assessmenttargetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef

```python
# ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef definition

class ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExclusionsRequestListExclusionsPaginateTypeDef

```python
# ListExclusionsRequestListExclusionsPaginateTypeDef definition

class ListExclusionsRequestListExclusionsPaginateTypeDef(TypedDict):
    assessmentRunArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesPackagesRequestListRulesPackagesPaginateTypeDef

```python
# ListRulesPackagesRequestListRulesPackagesPaginateTypeDef definition

class ListRulesPackagesRequestListRulesPackagesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PreviewAgentsRequestPreviewAgentsPaginateTypeDef

```python
# PreviewAgentsRequestPreviewAgentsPaginateTypeDef definition

class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(TypedDict):
    previewAgentsArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    networkInterfaceId: NotRequired[str],
    subnetId: NotRequired[str],
    vpcId: NotRequired[str],
    privateDnsName: NotRequired[str],
    privateIpAddress: NotRequired[str],
    privateIpAddresses: NotRequired[List[PrivateIpTypeDef]],  # (1)
    publicDnsName: NotRequired[str],
    publicIp: NotRequired[str],
    ipv6Addresses: NotRequired[List[str]],
    securityGroups: NotRequired[List[SecurityGroupTypeDef]],  # (2)
```

1. See [:material-code-braces: PrivateIpTypeDef](./type_defs.md#privateiptypedef) 
2. See [:material-code-braces: SecurityGroupTypeDef](./type_defs.md#securitygrouptypedef) 
## TimestampRangeTypeDef

```python
# TimestampRangeTypeDef definition

class TimestampRangeTypeDef(TypedDict):
    beginDate: NotRequired[TimestampTypeDef],
    endDate: NotRequired[TimestampTypeDef],
```

## DescribeAssessmentTemplatesResponseTypeDef

```python
# DescribeAssessmentTemplatesResponseTypeDef definition

class DescribeAssessmentTemplatesResponseTypeDef(TypedDict):
    assessmentTemplates: List[AssessmentTemplateTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssessmentTemplateTypeDef](./type_defs.md#assessmenttemplatetypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentRunAgentsResponseTypeDef

```python
# ListAssessmentRunAgentsResponseTypeDef definition

class ListAssessmentRunAgentsResponseTypeDef(TypedDict):
    assessmentRunAgents: List[AssessmentRunAgentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentRunAgentTypeDef](./type_defs.md#assessmentrunagenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef

```python
# ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef definition

class ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef(TypedDict):
    assessmentTargetArns: NotRequired[Sequence[str]],
    filter: NotRequired[AssessmentTemplateFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssessmentTemplateFilterTypeDef](./type_defs.md#assessmenttemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssessmentTemplatesRequestRequestTypeDef

```python
# ListAssessmentTemplatesRequestRequestTypeDef definition

class ListAssessmentTemplatesRequestRequestTypeDef(TypedDict):
    assessmentTargetArns: NotRequired[Sequence[str]],
    filter: NotRequired[AssessmentTemplateFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: AssessmentTemplateFilterTypeDef](./type_defs.md#assessmenttemplatefiltertypedef) 
## DescribeAssessmentRunsResponseTypeDef

```python
# DescribeAssessmentRunsResponseTypeDef definition

class DescribeAssessmentRunsResponseTypeDef(TypedDict):
    assessmentRuns: List[AssessmentRunTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssessmentRunTypeDef](./type_defs.md#assessmentruntypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourceGroupsResponseTypeDef

```python
# DescribeResourceGroupsResponseTypeDef definition

class DescribeResourceGroupsResponseTypeDef(TypedDict):
    resourceGroups: List[ResourceGroupTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceGroupTypeDef](./type_defs.md#resourcegrouptypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventSubscriptionsResponseTypeDef

```python
# ListEventSubscriptionsResponseTypeDef definition

class ListEventSubscriptionsResponseTypeDef(TypedDict):
    subscriptions: List[SubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExclusionsPreviewResponseTypeDef

```python
# GetExclusionsPreviewResponseTypeDef definition

class GetExclusionsPreviewResponseTypeDef(TypedDict):
    previewStatus: PreviewStatusType,  # (1)
    exclusionPreviews: List[ExclusionPreviewTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PreviewStatusType](./literals.md#previewstatustype) 
2. See [:material-code-braces: ExclusionPreviewTypeDef](./type_defs.md#exclusionpreviewtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExclusionsResponseTypeDef

```python
# DescribeExclusionsResponseTypeDef definition

class DescribeExclusionsResponseTypeDef(TypedDict):
    exclusions: Dict[str, ExclusionTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExclusionTypeDef](./type_defs.md#exclusiontypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetAttributesTypeDef

```python
# AssetAttributesTypeDef definition

class AssetAttributesTypeDef(TypedDict):
    schemaVersion: int,
    agentId: NotRequired[str],
    autoScalingGroup: NotRequired[str],
    amiId: NotRequired[str],
    hostname: NotRequired[str],
    ipv4Addresses: NotRequired[List[str]],
    tags: NotRequired[List[TagTypeDef]],  # (1)
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## AssessmentRunFilterTypeDef

```python
# AssessmentRunFilterTypeDef definition

class AssessmentRunFilterTypeDef(TypedDict):
    namePattern: NotRequired[str],
    states: NotRequired[Sequence[AssessmentRunStateType]],  # (1)
    durationRange: NotRequired[DurationRangeTypeDef],  # (2)
    rulesPackageArns: NotRequired[Sequence[str]],
    startTimeRange: NotRequired[TimestampRangeTypeDef],  # (3)
    completionTimeRange: NotRequired[TimestampRangeTypeDef],  # (3)
    stateChangeTimeRange: NotRequired[TimestampRangeTypeDef],  # (3)
```

1. See [:material-code-brackets: AssessmentRunStateType](./literals.md#assessmentrunstatetype) 
2. See [:material-code-braces: DurationRangeTypeDef](./type_defs.md#durationrangetypedef) 
3. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef) 
4. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef) 
5. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef) 
## FindingFilterTypeDef

```python
# FindingFilterTypeDef definition

class FindingFilterTypeDef(TypedDict):
    agentIds: NotRequired[Sequence[str]],
    autoScalingGroups: NotRequired[Sequence[str]],
    ruleNames: NotRequired[Sequence[str]],
    severities: NotRequired[Sequence[SeverityType]],  # (1)
    rulesPackageArns: NotRequired[Sequence[str]],
    attributes: NotRequired[Sequence[AttributeTypeDef]],  # (2)
    userAttributes: NotRequired[Sequence[AttributeTypeDef]],  # (2)
    creationTimeRange: NotRequired[TimestampRangeTypeDef],  # (4)
```

1. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
3. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
4. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    arn: str,
    attributes: List[AttributeTypeDef],  # (5)
    userAttributes: List[AttributeTypeDef],  # (5)
    createdAt: datetime,
    updatedAt: datetime,
    schemaVersion: NotRequired[int],
    service: NotRequired[str],
    serviceAttributes: NotRequired[InspectorServiceAttributesTypeDef],  # (1)
    assetType: NotRequired[AssetTypeType],  # (2)
    assetAttributes: NotRequired[AssetAttributesTypeDef],  # (3)
    id: NotRequired[str],
    title: NotRequired[str],
    description: NotRequired[str],
    recommendation: NotRequired[str],
    severity: NotRequired[SeverityType],  # (4)
    numericSeverity: NotRequired[float],
    confidence: NotRequired[int],
    indicatorOfCompromise: NotRequired[bool],
```

1. See [:material-code-braces: InspectorServiceAttributesTypeDef](./type_defs.md#inspectorserviceattributestypedef) 
2. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
3. See [:material-code-braces: AssetAttributesTypeDef](./type_defs.md#assetattributestypedef) 
4. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
5. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
6. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef

```python
# ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef definition

class ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef(TypedDict):
    assessmentTemplateArns: NotRequired[Sequence[str]],
    filter: NotRequired[AssessmentRunFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AssessmentRunFilterTypeDef](./type_defs.md#assessmentrunfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssessmentRunsRequestRequestTypeDef

```python
# ListAssessmentRunsRequestRequestTypeDef definition

class ListAssessmentRunsRequestRequestTypeDef(TypedDict):
    assessmentTemplateArns: NotRequired[Sequence[str]],
    filter: NotRequired[AssessmentRunFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: AssessmentRunFilterTypeDef](./type_defs.md#assessmentrunfiltertypedef) 
## ListFindingsRequestListFindingsPaginateTypeDef

```python
# ListFindingsRequestListFindingsPaginateTypeDef definition

class ListFindingsRequestListFindingsPaginateTypeDef(TypedDict):
    assessmentRunArns: NotRequired[Sequence[str]],
    filter: NotRequired[FindingFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FindingFilterTypeDef](./type_defs.md#findingfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestRequestTypeDef

```python
# ListFindingsRequestRequestTypeDef definition

class ListFindingsRequestRequestTypeDef(TypedDict):
    assessmentRunArns: NotRequired[Sequence[str]],
    filter: NotRequired[FindingFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FindingFilterTypeDef](./type_defs.md#findingfiltertypedef) 
## DescribeFindingsResponseTypeDef

```python
# DescribeFindingsResponseTypeDef definition

class DescribeFindingsResponseTypeDef(TypedDict):
    findings: List[FindingTypeDef],  # (1)
    failedItems: Dict[str, FailedItemDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: FailedItemDetailsTypeDef](./type_defs.md#faileditemdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
