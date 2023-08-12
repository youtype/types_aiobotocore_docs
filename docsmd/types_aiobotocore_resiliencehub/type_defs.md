# Type definitions

> [Index](../README.md) > [ResilienceHub](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## RecommendationItemTypeDef

```python
# RecommendationItemTypeDef definition

class RecommendationItemTypeDef(TypedDict):
    alreadyImplemented: NotRequired[bool],
    excludeReason: NotRequired[ExcludeRecommendationReasonType],  # (1)
    excluded: NotRequired[bool],
    resourceId: NotRequired[str],
    targetAccountId: NotRequired[str],
    targetRegion: NotRequired[str],
```

1. See [:material-code-brackets: ExcludeRecommendationReasonType](./literals.md#excluderecommendationreasontype) 
## CostTypeDef

```python
# CostTypeDef definition

class CostTypeDef(TypedDict):
    amount: float,
    currency: str,
    frequency: CostFrequencyType,  # (1)
```

1. See [:material-code-brackets: CostFrequencyType](./literals.md#costfrequencytype) 
## DisruptionComplianceTypeDef

```python
# DisruptionComplianceTypeDef definition

class DisruptionComplianceTypeDef(TypedDict):
    complianceStatus: ComplianceStatusType,  # (1)
    achievableRpoInSecs: NotRequired[int],
    achievableRtoInSecs: NotRequired[int],
    currentRpoInSecs: NotRequired[int],
    currentRtoInSecs: NotRequired[int],
    message: NotRequired[str],
    rpoDescription: NotRequired[str],
    rpoReferenceId: NotRequired[str],
    rtoDescription: NotRequired[str],
    rtoReferenceId: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
## ResiliencyScoreTypeDef

```python
# ResiliencyScoreTypeDef definition

class ResiliencyScoreTypeDef(TypedDict):
    disruptionScore: Dict[DisruptionTypeType, float],  # (1)
    score: float,
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) 
## AppComponentTypeDef

```python
# AppComponentTypeDef definition

class AppComponentTypeDef(TypedDict):
    name: str,
    type: str,
    additionalInfo: NotRequired[Dict[str, List[str]]],
    id: NotRequired[str],
```

## EksSourceClusterNamespaceTypeDef

```python
# EksSourceClusterNamespaceTypeDef definition

class EksSourceClusterNamespaceTypeDef(TypedDict):
    eksClusterArn: str,
    namespace: str,
```

## TerraformSourceTypeDef

```python
# TerraformSourceTypeDef definition

class TerraformSourceTypeDef(TypedDict):
    s3StateFileUrl: str,
```

## AppSummaryTypeDef

```python
# AppSummaryTypeDef definition

class AppSummaryTypeDef(TypedDict):
    appArn: str,
    creationTime: datetime,
    name: str,
    assessmentSchedule: NotRequired[AppAssessmentScheduleTypeType],  # (1)
    complianceStatus: NotRequired[AppComplianceStatusTypeType],  # (2)
    description: NotRequired[str],
    driftStatus: NotRequired[AppDriftStatusTypeType],  # (3)
    resiliencyScore: NotRequired[float],
    status: NotRequired[AppStatusTypeType],  # (4)
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-brackets: AppComplianceStatusTypeType](./literals.md#appcompliancestatustypetype) 
3. See [:material-code-brackets: AppDriftStatusTypeType](./literals.md#appdriftstatustypetype) 
4. See [:material-code-brackets: AppStatusTypeType](./literals.md#appstatustypetype) 
## EventSubscriptionTypeDef

```python
# EventSubscriptionTypeDef definition

class EventSubscriptionTypeDef(TypedDict):
    eventType: EventTypeType,  # (1)
    name: str,
    snsTopicArn: NotRequired[str],
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## PermissionModelTypeDef

```python
# PermissionModelTypeDef definition

class PermissionModelTypeDef(TypedDict):
    type: PermissionModelTypeType,  # (1)
    crossAccountRoleArns: NotRequired[Sequence[str]],
    invokerRoleName: NotRequired[str],
```

1. See [:material-code-brackets: PermissionModelTypeType](./literals.md#permissionmodeltypetype) 
## AppVersionSummaryTypeDef

```python
# AppVersionSummaryTypeDef definition

class AppVersionSummaryTypeDef(TypedDict):
    appVersion: str,
    creationTime: NotRequired[datetime],
    identifier: NotRequired[int],
    versionName: NotRequired[str],
```

## BatchUpdateRecommendationStatusFailedEntryTypeDef

```python
# BatchUpdateRecommendationStatusFailedEntryTypeDef definition

class BatchUpdateRecommendationStatusFailedEntryTypeDef(TypedDict):
    entryId: str,
    errorMessage: str,
```

## UpdateRecommendationStatusItemTypeDef

```python
# UpdateRecommendationStatusItemTypeDef definition

class UpdateRecommendationStatusItemTypeDef(TypedDict):
    resourceId: NotRequired[str],
    targetAccountId: NotRequired[str],
    targetRegion: NotRequired[str],
```

## RecommendationDisruptionComplianceTypeDef

```python
# RecommendationDisruptionComplianceTypeDef definition

class RecommendationDisruptionComplianceTypeDef(TypedDict):
    expectedComplianceStatus: ComplianceStatusType,  # (1)
    expectedRpoDescription: NotRequired[str],
    expectedRpoInSecs: NotRequired[int],
    expectedRtoDescription: NotRequired[str],
    expectedRtoInSecs: NotRequired[int],
```

1. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
## CreateAppVersionAppComponentRequestRequestTypeDef

```python
# CreateAppVersionAppComponentRequestRequestTypeDef definition

class CreateAppVersionAppComponentRequestRequestTypeDef(TypedDict):
    appArn: str,
    name: str,
    type: str,
    additionalInfo: NotRequired[Mapping[str, Sequence[str]]],
    clientToken: NotRequired[str],
    id: NotRequired[str],
```

## LogicalResourceIdTypeDef

```python
# LogicalResourceIdTypeDef definition

class LogicalResourceIdTypeDef(TypedDict):
    identifier: str,
    eksSourceName: NotRequired[str],
    logicalStackName: NotRequired[str],
    resourceGroupName: NotRequired[str],
    terraformSourceName: NotRequired[str],
```

## CreateRecommendationTemplateRequestRequestTypeDef

```python
# CreateRecommendationTemplateRequestRequestTypeDef definition

class CreateRecommendationTemplateRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    name: str,
    bucketName: NotRequired[str],
    clientToken: NotRequired[str],
    format: NotRequired[TemplateFormatType],  # (1)
    recommendationIds: NotRequired[Sequence[str]],
    recommendationTypes: NotRequired[Sequence[RenderRecommendationTypeType]],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: TemplateFormatType](./literals.md#templateformattype) 
2. See [:material-code-brackets: RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype) 
## FailurePolicyTypeDef

```python
# FailurePolicyTypeDef definition

class FailurePolicyTypeDef(TypedDict):
    rpoInSecs: int,
    rtoInSecs: int,
```

## DeleteAppAssessmentRequestRequestTypeDef

```python
# DeleteAppAssessmentRequestRequestTypeDef definition

class DeleteAppAssessmentRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    clientToken: NotRequired[str],
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    appArn: str,
    clientToken: NotRequired[str],
    forceDelete: NotRequired[bool],
```

## DeleteAppVersionAppComponentRequestRequestTypeDef

```python
# DeleteAppVersionAppComponentRequestRequestTypeDef definition

class DeleteAppVersionAppComponentRequestRequestTypeDef(TypedDict):
    appArn: str,
    id: str,
    clientToken: NotRequired[str],
```

## DeleteRecommendationTemplateRequestRequestTypeDef

```python
# DeleteRecommendationTemplateRequestRequestTypeDef definition

class DeleteRecommendationTemplateRequestRequestTypeDef(TypedDict):
    recommendationTemplateArn: str,
    clientToken: NotRequired[str],
```

## DeleteResiliencyPolicyRequestRequestTypeDef

```python
# DeleteResiliencyPolicyRequestRequestTypeDef definition

class DeleteResiliencyPolicyRequestRequestTypeDef(TypedDict):
    policyArn: str,
    clientToken: NotRequired[str],
```

## DescribeAppAssessmentRequestRequestTypeDef

```python
# DescribeAppAssessmentRequestRequestTypeDef definition

class DescribeAppAssessmentRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
```

## DescribeAppRequestRequestTypeDef

```python
# DescribeAppRequestRequestTypeDef definition

class DescribeAppRequestRequestTypeDef(TypedDict):
    appArn: str,
```

## DescribeAppVersionAppComponentRequestRequestTypeDef

```python
# DescribeAppVersionAppComponentRequestRequestTypeDef definition

class DescribeAppVersionAppComponentRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    id: str,
```

## DescribeAppVersionRequestRequestTypeDef

```python
# DescribeAppVersionRequestRequestTypeDef definition

class DescribeAppVersionRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
```

## DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef

```python
# DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef definition

class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    resolutionId: NotRequired[str],
```

## DescribeAppVersionTemplateRequestRequestTypeDef

```python
# DescribeAppVersionTemplateRequestRequestTypeDef definition

class DescribeAppVersionTemplateRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
```

## DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef

```python
# DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef definition

class DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef(TypedDict):
    appArn: str,
```

## DescribeResiliencyPolicyRequestRequestTypeDef

```python
# DescribeResiliencyPolicyRequestRequestTypeDef definition

class DescribeResiliencyPolicyRequestRequestTypeDef(TypedDict):
    policyArn: str,
```

## EksSourceTypeDef

```python
# EksSourceTypeDef definition

class EksSourceTypeDef(TypedDict):
    eksClusterArn: str,
    namespaces: Sequence[str],
```

## ListAlarmRecommendationsRequestRequestTypeDef

```python
# ListAlarmRecommendationsRequestRequestTypeDef definition

class ListAlarmRecommendationsRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppAssessmentComplianceDriftsRequestRequestTypeDef

```python
# ListAppAssessmentComplianceDriftsRequestRequestTypeDef definition

class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppAssessmentsRequestRequestTypeDef

```python
# ListAppAssessmentsRequestRequestTypeDef definition

class ListAppAssessmentsRequestRequestTypeDef(TypedDict):
    appArn: NotRequired[str],
    assessmentName: NotRequired[str],
    assessmentStatus: NotRequired[Sequence[AssessmentStatusType]],  # (1)
    complianceStatus: NotRequired[ComplianceStatusType],  # (2)
    invoker: NotRequired[AssessmentInvokerType],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    reverseOrder: NotRequired[bool],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
3. See [:material-code-brackets: AssessmentInvokerType](./literals.md#assessmentinvokertype) 
## ListAppComponentCompliancesRequestRequestTypeDef

```python
# ListAppComponentCompliancesRequestRequestTypeDef definition

class ListAppComponentCompliancesRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppComponentRecommendationsRequestRequestTypeDef

```python
# ListAppComponentRecommendationsRequestRequestTypeDef definition

class ListAppComponentRecommendationsRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppInputSourcesRequestRequestTypeDef

```python
# ListAppInputSourcesRequestRequestTypeDef definition

class ListAppInputSourcesRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppVersionAppComponentsRequestRequestTypeDef

```python
# ListAppVersionAppComponentsRequestRequestTypeDef definition

class ListAppVersionAppComponentsRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppVersionResourceMappingsRequestRequestTypeDef

```python
# ListAppVersionResourceMappingsRequestRequestTypeDef definition

class ListAppVersionResourceMappingsRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppVersionResourcesRequestRequestTypeDef

```python
# ListAppVersionResourcesRequestRequestTypeDef definition

class ListAppVersionResourcesRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resolutionId: NotRequired[str],
```

## ListAppsRequestRequestTypeDef

```python
# ListAppsRequestRequestTypeDef definition

class ListAppsRequestRequestTypeDef(TypedDict):
    appArn: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListRecommendationTemplatesRequestRequestTypeDef

```python
# ListRecommendationTemplatesRequestRequestTypeDef definition

class ListRecommendationTemplatesRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    recommendationTemplateArn: NotRequired[str],
    reverseOrder: NotRequired[bool],
    status: NotRequired[Sequence[RecommendationTemplateStatusType]],  # (1)
```

1. See [:material-code-brackets: RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype) 
## ListResiliencyPoliciesRequestRequestTypeDef

```python
# ListResiliencyPoliciesRequestRequestTypeDef definition

class ListResiliencyPoliciesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    policyName: NotRequired[str],
```

## ListSopRecommendationsRequestRequestTypeDef

```python
# ListSopRecommendationsRequestRequestTypeDef definition

class ListSopRecommendationsRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListSuggestedResiliencyPoliciesRequestRequestTypeDef

```python
# ListSuggestedResiliencyPoliciesRequestRequestTypeDef definition

class ListSuggestedResiliencyPoliciesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTestRecommendationsRequestRequestTypeDef

```python
# ListTestRecommendationsRequestRequestTypeDef definition

class ListTestRecommendationsRequestRequestTypeDef(TypedDict):
    assessmentArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListUnsupportedAppVersionResourcesRequestRequestTypeDef

```python
# ListUnsupportedAppVersionResourcesRequestRequestTypeDef definition

class ListUnsupportedAppVersionResourcesRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resolutionId: NotRequired[str],
```

## PhysicalResourceIdTypeDef

```python
# PhysicalResourceIdTypeDef definition

class PhysicalResourceIdTypeDef(TypedDict):
    identifier: str,
    type: PhysicalIdentifierTypeType,  # (1)
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
```

1. See [:material-code-brackets: PhysicalIdentifierTypeType](./literals.md#physicalidentifiertypetype) 
## PublishAppVersionRequestRequestTypeDef

```python
# PublishAppVersionRequestRequestTypeDef definition

class PublishAppVersionRequestRequestTypeDef(TypedDict):
    appArn: str,
    versionName: NotRequired[str],
```

## PutDraftAppVersionTemplateRequestRequestTypeDef

```python
# PutDraftAppVersionTemplateRequestRequestTypeDef definition

class PutDraftAppVersionTemplateRequestRequestTypeDef(TypedDict):
    appArn: str,
    appTemplateBody: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef

```python
# RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef definition

class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(TypedDict):
    appArn: str,
    appRegistryAppNames: NotRequired[Sequence[str]],
    eksSourceNames: NotRequired[Sequence[str]],
    logicalStackNames: NotRequired[Sequence[str]],
    resourceGroupNames: NotRequired[Sequence[str]],
    resourceNames: NotRequired[Sequence[str]],
    terraformSourceNames: NotRequired[Sequence[str]],
```

## ResolveAppVersionResourcesRequestRequestTypeDef

```python
# ResolveAppVersionResourcesRequestRequestTypeDef definition

class ResolveAppVersionResourcesRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
```

## ResourceErrorTypeDef

```python
# ResourceErrorTypeDef definition

class ResourceErrorTypeDef(TypedDict):
    logicalResourceId: NotRequired[str],
    physicalResourceId: NotRequired[str],
    reason: NotRequired[str],
```

## StartAppAssessmentRequestRequestTypeDef

```python
# StartAppAssessmentRequestRequestTypeDef definition

class StartAppAssessmentRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    assessmentName: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

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

## UpdateAppVersionAppComponentRequestRequestTypeDef

```python
# UpdateAppVersionAppComponentRequestRequestTypeDef definition

class UpdateAppVersionAppComponentRequestRequestTypeDef(TypedDict):
    appArn: str,
    id: str,
    additionalInfo: NotRequired[Mapping[str, Sequence[str]]],
    name: NotRequired[str],
    type: NotRequired[str],
```

## UpdateAppVersionRequestRequestTypeDef

```python
# UpdateAppVersionRequestRequestTypeDef definition

class UpdateAppVersionRequestRequestTypeDef(TypedDict):
    appArn: str,
    additionalInfo: NotRequired[Mapping[str, Sequence[str]]],
```

## DeleteAppAssessmentResponseTypeDef

```python
# DeleteAppAssessmentResponseTypeDef definition

class DeleteAppAssessmentResponseTypeDef(TypedDict):
    assessmentArn: str,
    assessmentStatus: AssessmentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppResponseTypeDef

```python
# DeleteAppResponseTypeDef definition

class DeleteAppResponseTypeDef(TypedDict):
    appArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRecommendationTemplateResponseTypeDef

```python
# DeleteRecommendationTemplateResponseTypeDef definition

class DeleteRecommendationTemplateResponseTypeDef(TypedDict):
    recommendationTemplateArn: str,
    status: RecommendationTemplateStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResiliencyPolicyResponseTypeDef

```python
# DeleteResiliencyPolicyResponseTypeDef definition

class DeleteResiliencyPolicyResponseTypeDef(TypedDict):
    policyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppVersionResourcesResolutionStatusResponseTypeDef

```python
# DescribeAppVersionResourcesResolutionStatusResponseTypeDef definition

class DescribeAppVersionResourcesResolutionStatusResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    errorMessage: str,
    resolutionId: str,
    status: ResourceResolutionStatusTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceResolutionStatusTypeType](./literals.md#resourceresolutionstatustypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppVersionResponseTypeDef

```python
# DescribeAppVersionResponseTypeDef definition

class DescribeAppVersionResponseTypeDef(TypedDict):
    additionalInfo: Dict[str, List[str]],
    appArn: str,
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppVersionTemplateResponseTypeDef

```python
# DescribeAppVersionTemplateResponseTypeDef definition

class DescribeAppVersionTemplateResponseTypeDef(TypedDict):
    appArn: str,
    appTemplateBody: str,
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDraftAppVersionResourcesImportStatusResponseTypeDef

```python
# DescribeDraftAppVersionResourcesImportStatusResponseTypeDef definition

class DescribeDraftAppVersionResourcesImportStatusResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    errorMessage: str,
    status: ResourceImportStatusTypeType,  # (1)
    statusChangeTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceImportStatusTypeType](./literals.md#resourceimportstatustypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishAppVersionResponseTypeDef

```python
# PublishAppVersionResponseTypeDef definition

class PublishAppVersionResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    identifier: int,
    versionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDraftAppVersionTemplateResponseTypeDef

```python
# PutDraftAppVersionTemplateResponseTypeDef definition

class PutDraftAppVersionTemplateResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveDraftAppVersionResourceMappingsResponseTypeDef

```python
# RemoveDraftAppVersionResourceMappingsResponseTypeDef definition

class RemoveDraftAppVersionResourceMappingsResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResolveAppVersionResourcesResponseTypeDef

```python
# ResolveAppVersionResourcesResponseTypeDef definition

class ResolveAppVersionResourcesResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    resolutionId: str,
    status: ResourceResolutionStatusTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceResolutionStatusTypeType](./literals.md#resourceresolutionstatustypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppVersionResponseTypeDef

```python
# UpdateAppVersionResponseTypeDef definition

class UpdateAppVersionResponseTypeDef(TypedDict):
    additionalInfo: Dict[str, List[str]],
    appArn: str,
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AlarmRecommendationTypeDef

```python
# AlarmRecommendationTypeDef definition

class AlarmRecommendationTypeDef(TypedDict):
    name: str,
    recommendationId: str,
    referenceId: str,
    type: AlarmTypeType,  # (2)
    appComponentName: NotRequired[str],
    appComponentNames: NotRequired[List[str]],
    description: NotRequired[str],
    items: NotRequired[List[RecommendationItemTypeDef]],  # (1)
    prerequisite: NotRequired[str],
```

1. See [:material-code-braces: RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef) 
2. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
## SopRecommendationTypeDef

```python
# SopRecommendationTypeDef definition

class SopRecommendationTypeDef(TypedDict):
    recommendationId: str,
    referenceId: str,
    serviceType: SopServiceTypeType,  # (2)
    appComponentName: NotRequired[str],
    description: NotRequired[str],
    items: NotRequired[List[RecommendationItemTypeDef]],  # (1)
    name: NotRequired[str],
    prerequisite: NotRequired[str],
```

1. See [:material-code-braces: RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef) 
2. See [:material-code-brackets: SopServiceTypeType](./literals.md#sopservicetypetype) 
## TestRecommendationTypeDef

```python
# TestRecommendationTypeDef definition

class TestRecommendationTypeDef(TypedDict):
    referenceId: str,
    appComponentName: NotRequired[str],
    dependsOnAlarms: NotRequired[List[str]],
    description: NotRequired[str],
    intent: NotRequired[str],
    items: NotRequired[List[RecommendationItemTypeDef]],  # (1)
    name: NotRequired[str],
    prerequisite: NotRequired[str],
    recommendationId: NotRequired[str],
    risk: NotRequired[TestRiskType],  # (2)
    type: NotRequired[TestTypeType],  # (3)
```

1. See [:material-code-braces: RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef) 
2. See [:material-code-brackets: TestRiskType](./literals.md#testrisktype) 
3. See [:material-code-brackets: TestTypeType](./literals.md#testtypetype) 
## AppAssessmentSummaryTypeDef

```python
# AppAssessmentSummaryTypeDef definition

class AppAssessmentSummaryTypeDef(TypedDict):
    assessmentArn: str,
    assessmentStatus: AssessmentStatusType,  # (1)
    appArn: NotRequired[str],
    appVersion: NotRequired[str],
    assessmentName: NotRequired[str],
    complianceStatus: NotRequired[ComplianceStatusType],  # (2)
    cost: NotRequired[CostTypeDef],  # (3)
    driftStatus: NotRequired[DriftStatusType],  # (4)
    endTime: NotRequired[datetime],
    invoker: NotRequired[AssessmentInvokerType],  # (5)
    message: NotRequired[str],
    resiliencyScore: NotRequired[float],
    startTime: NotRequired[datetime],
    versionName: NotRequired[str],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
3. See [:material-code-braces: CostTypeDef](./type_defs.md#costtypedef) 
4. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
5. See [:material-code-brackets: AssessmentInvokerType](./literals.md#assessmentinvokertype) 
## ComplianceDriftTypeDef

```python
# ComplianceDriftTypeDef definition

class ComplianceDriftTypeDef(TypedDict):
    actualReferenceId: NotRequired[str],
    actualValue: NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],  # (1)
    appId: NotRequired[str],
    appVersion: NotRequired[str],
    diffType: NotRequired[DifferenceTypeType],  # (2)
    driftType: NotRequired[DriftTypeType],  # (3)
    entityId: NotRequired[str],
    entityType: NotRequired[str],
    expectedReferenceId: NotRequired[str],
    expectedValue: NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],  # (1)
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef) 
2. See [:material-code-brackets: DifferenceTypeType](./literals.md#differencetypetype) 
3. See [:material-code-brackets: DriftTypeType](./literals.md#drifttypetype) 
4. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef) 
## AppComponentComplianceTypeDef

```python
# AppComponentComplianceTypeDef definition

class AppComponentComplianceTypeDef(TypedDict):
    appComponentName: NotRequired[str],
    compliance: NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],  # (1)
    cost: NotRequired[CostTypeDef],  # (2)
    message: NotRequired[str],
    resiliencyScore: NotRequired[ResiliencyScoreTypeDef],  # (3)
    status: NotRequired[ComplianceStatusType],  # (4)
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef) 
2. See [:material-code-braces: CostTypeDef](./type_defs.md#costtypedef) 
3. See [:material-code-braces: ResiliencyScoreTypeDef](./type_defs.md#resiliencyscoretypedef) 
4. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
## CreateAppVersionAppComponentResponseTypeDef

```python
# CreateAppVersionAppComponentResponseTypeDef definition

class CreateAppVersionAppComponentResponseTypeDef(TypedDict):
    appArn: str,
    appComponent: AppComponentTypeDef,  # (1)
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppVersionAppComponentResponseTypeDef

```python
# DeleteAppVersionAppComponentResponseTypeDef definition

class DeleteAppVersionAppComponentResponseTypeDef(TypedDict):
    appArn: str,
    appComponent: AppComponentTypeDef,  # (1)
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppVersionAppComponentResponseTypeDef

```python
# DescribeAppVersionAppComponentResponseTypeDef definition

class DescribeAppVersionAppComponentResponseTypeDef(TypedDict):
    appArn: str,
    appComponent: AppComponentTypeDef,  # (1)
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppVersionAppComponentsResponseTypeDef

```python
# ListAppVersionAppComponentsResponseTypeDef definition

class ListAppVersionAppComponentsResponseTypeDef(TypedDict):
    appArn: str,
    appComponents: List[AppComponentTypeDef],  # (1)
    appVersion: str,
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppVersionAppComponentResponseTypeDef

```python
# UpdateAppVersionAppComponentResponseTypeDef definition

class UpdateAppVersionAppComponentResponseTypeDef(TypedDict):
    appArn: str,
    appComponent: AppComponentTypeDef,  # (1)
    appVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppInputSourceTypeDef

```python
# AppInputSourceTypeDef definition

class AppInputSourceTypeDef(TypedDict):
    importType: ResourceMappingTypeType,  # (2)
    eksSourceClusterNamespace: NotRequired[EksSourceClusterNamespaceTypeDef],  # (1)
    resourceCount: NotRequired[int],
    sourceArn: NotRequired[str],
    sourceName: NotRequired[str],
    terraformSource: NotRequired[TerraformSourceTypeDef],  # (3)
```

1. See [:material-code-braces: EksSourceClusterNamespaceTypeDef](./type_defs.md#ekssourceclusternamespacetypedef) 
2. See [:material-code-brackets: ResourceMappingTypeType](./literals.md#resourcemappingtypetype) 
3. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
## DeleteAppInputSourceRequestRequestTypeDef

```python
# DeleteAppInputSourceRequestRequestTypeDef definition

class DeleteAppInputSourceRequestRequestTypeDef(TypedDict):
    appArn: str,
    clientToken: NotRequired[str],
    eksSourceClusterNamespace: NotRequired[EksSourceClusterNamespaceTypeDef],  # (1)
    sourceArn: NotRequired[str],
    terraformSource: NotRequired[TerraformSourceTypeDef],  # (2)
```

1. See [:material-code-braces: EksSourceClusterNamespaceTypeDef](./type_defs.md#ekssourceclusternamespacetypedef) 
2. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
## ListAppsResponseTypeDef

```python
# ListAppsResponseTypeDef definition

class ListAppsResponseTypeDef(TypedDict):
    appSummaries: List[AppSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppSummaryTypeDef](./type_defs.md#appsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppTypeDef

```python
# AppTypeDef definition

class AppTypeDef(TypedDict):
    appArn: str,
    creationTime: datetime,
    name: str,
    assessmentSchedule: NotRequired[AppAssessmentScheduleTypeType],  # (1)
    complianceStatus: NotRequired[AppComplianceStatusTypeType],  # (2)
    description: NotRequired[str],
    driftStatus: NotRequired[AppDriftStatusTypeType],  # (3)
    eventSubscriptions: NotRequired[List[EventSubscriptionTypeDef]],  # (4)
    lastAppComplianceEvaluationTime: NotRequired[datetime],
    lastDriftEvaluationTime: NotRequired[datetime],
    lastResiliencyScoreEvaluationTime: NotRequired[datetime],
    permissionModel: NotRequired[PermissionModelTypeDef],  # (5)
    policyArn: NotRequired[str],
    resiliencyScore: NotRequired[float],
    status: NotRequired[AppStatusTypeType],  # (6)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-brackets: AppComplianceStatusTypeType](./literals.md#appcompliancestatustypetype) 
3. See [:material-code-brackets: AppDriftStatusTypeType](./literals.md#appdriftstatustypetype) 
4. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
5. See [:material-code-braces: PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef) 
6. See [:material-code-brackets: AppStatusTypeType](./literals.md#appstatustypetype) 
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
    name: str,
    assessmentSchedule: NotRequired[AppAssessmentScheduleTypeType],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    eventSubscriptions: NotRequired[Sequence[EventSubscriptionTypeDef]],  # (2)
    permissionModel: NotRequired[PermissionModelTypeDef],  # (3)
    policyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
3. See [:material-code-braces: PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef) 
## UpdateAppRequestRequestTypeDef

```python
# UpdateAppRequestRequestTypeDef definition

class UpdateAppRequestRequestTypeDef(TypedDict):
    appArn: str,
    assessmentSchedule: NotRequired[AppAssessmentScheduleTypeType],  # (1)
    clearResiliencyPolicyArn: NotRequired[bool],
    description: NotRequired[str],
    eventSubscriptions: NotRequired[Sequence[EventSubscriptionTypeDef]],  # (2)
    permissionModel: NotRequired[PermissionModelTypeDef],  # (3)
    policyArn: NotRequired[str],
```

1. See [:material-code-brackets: AppAssessmentScheduleTypeType](./literals.md#appassessmentscheduletypetype) 
2. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
3. See [:material-code-braces: PermissionModelTypeDef](./type_defs.md#permissionmodeltypedef) 
## ListAppVersionsResponseTypeDef

```python
# ListAppVersionsResponseTypeDef definition

class ListAppVersionsResponseTypeDef(TypedDict):
    appVersions: List[AppVersionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppVersionSummaryTypeDef](./type_defs.md#appversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateRecommendationStatusSuccessfulEntryTypeDef

```python
# BatchUpdateRecommendationStatusSuccessfulEntryTypeDef definition

class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(TypedDict):
    entryId: str,
    excluded: bool,
    item: UpdateRecommendationStatusItemTypeDef,  # (2)
    referenceId: str,
    excludeReason: NotRequired[ExcludeRecommendationReasonType],  # (1)
```

1. See [:material-code-brackets: ExcludeRecommendationReasonType](./literals.md#excluderecommendationreasontype) 
2. See [:material-code-braces: UpdateRecommendationStatusItemTypeDef](./type_defs.md#updaterecommendationstatusitemtypedef) 
## UpdateRecommendationStatusRequestEntryTypeDef

```python
# UpdateRecommendationStatusRequestEntryTypeDef definition

class UpdateRecommendationStatusRequestEntryTypeDef(TypedDict):
    entryId: str,
    excluded: bool,
    item: UpdateRecommendationStatusItemTypeDef,  # (2)
    referenceId: str,
    excludeReason: NotRequired[ExcludeRecommendationReasonType],  # (1)
```

1. See [:material-code-brackets: ExcludeRecommendationReasonType](./literals.md#excluderecommendationreasontype) 
2. See [:material-code-braces: UpdateRecommendationStatusItemTypeDef](./type_defs.md#updaterecommendationstatusitemtypedef) 
## ConfigRecommendationTypeDef

```python
# ConfigRecommendationTypeDef definition

class ConfigRecommendationTypeDef(TypedDict):
    name: str,
    optimizationType: ConfigRecommendationOptimizationTypeType,  # (4)
    referenceId: str,
    appComponentName: NotRequired[str],
    compliance: NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],  # (1)
    cost: NotRequired[CostTypeDef],  # (2)
    description: NotRequired[str],
    haArchitecture: NotRequired[HaArchitectureType],  # (3)
    recommendationCompliance: NotRequired[Dict[DisruptionTypeType, RecommendationDisruptionComplianceTypeDef]],  # (5)
    suggestedChanges: NotRequired[List[str]],
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef) 
2. See [:material-code-braces: CostTypeDef](./type_defs.md#costtypedef) 
3. See [:material-code-brackets: HaArchitectureType](./literals.md#haarchitecturetype) 
4. See [:material-code-brackets: ConfigRecommendationOptimizationTypeType](./literals.md#configrecommendationoptimizationtypetype) 
5. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: RecommendationDisruptionComplianceTypeDef](./type_defs.md#recommendationdisruptioncompliancetypedef) 
## CreateAppVersionResourceRequestRequestTypeDef

```python
# CreateAppVersionResourceRequestRequestTypeDef definition

class CreateAppVersionResourceRequestRequestTypeDef(TypedDict):
    appArn: str,
    appComponents: Sequence[str],
    logicalResourceId: LogicalResourceIdTypeDef,  # (1)
    physicalResourceId: str,
    resourceType: str,
    additionalInfo: NotRequired[Mapping[str, Sequence[str]]],
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
    clientToken: NotRequired[str],
    resourceName: NotRequired[str],
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
## DeleteAppVersionResourceRequestRequestTypeDef

```python
# DeleteAppVersionResourceRequestRequestTypeDef definition

class DeleteAppVersionResourceRequestRequestTypeDef(TypedDict):
    appArn: str,
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
    clientToken: NotRequired[str],
    logicalResourceId: NotRequired[LogicalResourceIdTypeDef],  # (1)
    physicalResourceId: NotRequired[str],
    resourceName: NotRequired[str],
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
## DescribeAppVersionResourceRequestRequestTypeDef

```python
# DescribeAppVersionResourceRequestRequestTypeDef definition

class DescribeAppVersionResourceRequestRequestTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
    logicalResourceId: NotRequired[LogicalResourceIdTypeDef],  # (1)
    physicalResourceId: NotRequired[str],
    resourceName: NotRequired[str],
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
## UpdateAppVersionResourceRequestRequestTypeDef

```python
# UpdateAppVersionResourceRequestRequestTypeDef definition

class UpdateAppVersionResourceRequestRequestTypeDef(TypedDict):
    appArn: str,
    additionalInfo: NotRequired[Mapping[str, Sequence[str]]],
    appComponents: NotRequired[Sequence[str]],
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
    excluded: NotRequired[bool],
    logicalResourceId: NotRequired[LogicalResourceIdTypeDef],  # (1)
    physicalResourceId: NotRequired[str],
    resourceName: NotRequired[str],
    resourceType: NotRequired[str],
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
## CreateResiliencyPolicyRequestRequestTypeDef

```python
# CreateResiliencyPolicyRequestRequestTypeDef definition

class CreateResiliencyPolicyRequestRequestTypeDef(TypedDict):
    policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],  # (1)
    policyName: str,
    tier: ResiliencyPolicyTierType,  # (2)
    clientToken: NotRequired[str],
    dataLocationConstraint: NotRequired[DataLocationConstraintType],  # (3)
    policyDescription: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef) 
2. See [:material-code-brackets: ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype) 
3. See [:material-code-brackets: DataLocationConstraintType](./literals.md#datalocationconstrainttype) 
## ResiliencyPolicyTypeDef

```python
# ResiliencyPolicyTypeDef definition

class ResiliencyPolicyTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    dataLocationConstraint: NotRequired[DataLocationConstraintType],  # (1)
    estimatedCostTier: NotRequired[EstimatedCostTierType],  # (2)
    policy: NotRequired[Dict[DisruptionTypeType, FailurePolicyTypeDef]],  # (3)
    policyArn: NotRequired[str],
    policyDescription: NotRequired[str],
    policyName: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    tier: NotRequired[ResiliencyPolicyTierType],  # (4)
```

1. See [:material-code-brackets: DataLocationConstraintType](./literals.md#datalocationconstrainttype) 
2. See [:material-code-brackets: EstimatedCostTierType](./literals.md#estimatedcosttiertype) 
3. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef) 
4. See [:material-code-brackets: ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype) 
## UpdateResiliencyPolicyRequestRequestTypeDef

```python
# UpdateResiliencyPolicyRequestRequestTypeDef definition

class UpdateResiliencyPolicyRequestRequestTypeDef(TypedDict):
    policyArn: str,
    dataLocationConstraint: NotRequired[DataLocationConstraintType],  # (1)
    policy: NotRequired[Mapping[DisruptionTypeType, FailurePolicyTypeDef]],  # (2)
    policyDescription: NotRequired[str],
    policyName: NotRequired[str],
    tier: NotRequired[ResiliencyPolicyTierType],  # (3)
```

1. See [:material-code-brackets: DataLocationConstraintType](./literals.md#datalocationconstrainttype) 
2. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef) 
3. See [:material-code-brackets: ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype) 
## ImportResourcesToDraftAppVersionRequestRequestTypeDef

```python
# ImportResourcesToDraftAppVersionRequestRequestTypeDef definition

class ImportResourcesToDraftAppVersionRequestRequestTypeDef(TypedDict):
    appArn: str,
    eksSources: NotRequired[Sequence[EksSourceTypeDef]],  # (1)
    importStrategy: NotRequired[ResourceImportStrategyTypeType],  # (2)
    sourceArns: NotRequired[Sequence[str]],
    terraformSources: NotRequired[Sequence[TerraformSourceTypeDef]],  # (3)
```

1. See [:material-code-braces: EksSourceTypeDef](./type_defs.md#ekssourcetypedef) 
2. See [:material-code-brackets: ResourceImportStrategyTypeType](./literals.md#resourceimportstrategytypetype) 
3. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
## ImportResourcesToDraftAppVersionResponseTypeDef

```python
# ImportResourcesToDraftAppVersionResponseTypeDef definition

class ImportResourcesToDraftAppVersionResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    eksSources: List[EksSourceTypeDef],  # (1)
    sourceArns: List[str],
    status: ResourceImportStatusTypeType,  # (2)
    terraformSources: List[TerraformSourceTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EksSourceTypeDef](./type_defs.md#ekssourcetypedef) 
2. See [:material-code-brackets: ResourceImportStatusTypeType](./literals.md#resourceimportstatustypetype) 
3. See [:material-code-braces: TerraformSourceTypeDef](./type_defs.md#terraformsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppVersionsRequestRequestTypeDef

```python
# ListAppVersionsRequestRequestTypeDef definition

class ListAppVersionsRequestRequestTypeDef(TypedDict):
    appArn: str,
    endTime: NotRequired[Union[datetime, str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
```

## PhysicalResourceTypeDef

```python
# PhysicalResourceTypeDef definition

class PhysicalResourceTypeDef(TypedDict):
    logicalResourceId: LogicalResourceIdTypeDef,  # (2)
    physicalResourceId: PhysicalResourceIdTypeDef,  # (3)
    resourceType: str,
    additionalInfo: NotRequired[Dict[str, List[str]]],
    appComponents: NotRequired[List[AppComponentTypeDef]],  # (1)
    excluded: NotRequired[bool],
    parentResourceName: NotRequired[str],
    resourceName: NotRequired[str],
    sourceType: NotRequired[ResourceSourceTypeType],  # (4)
```

1. See [:material-code-braces: AppComponentTypeDef](./type_defs.md#appcomponenttypedef) 
2. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
3. See [:material-code-braces: PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef) 
4. See [:material-code-brackets: ResourceSourceTypeType](./literals.md#resourcesourcetypetype) 
## ResourceMappingTypeDef

```python
# ResourceMappingTypeDef definition

class ResourceMappingTypeDef(TypedDict):
    mappingType: ResourceMappingTypeType,  # (1)
    physicalResourceId: PhysicalResourceIdTypeDef,  # (2)
    appRegistryAppName: NotRequired[str],
    eksSourceName: NotRequired[str],
    logicalStackName: NotRequired[str],
    resourceGroupName: NotRequired[str],
    resourceName: NotRequired[str],
    terraformSourceName: NotRequired[str],
```

1. See [:material-code-brackets: ResourceMappingTypeType](./literals.md#resourcemappingtypetype) 
2. See [:material-code-braces: PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef) 
## UnsupportedResourceTypeDef

```python
# UnsupportedResourceTypeDef definition

class UnsupportedResourceTypeDef(TypedDict):
    logicalResourceId: LogicalResourceIdTypeDef,  # (1)
    physicalResourceId: PhysicalResourceIdTypeDef,  # (2)
    resourceType: str,
    unsupportedResourceStatus: NotRequired[str],
```

1. See [:material-code-braces: LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef) 
2. See [:material-code-braces: PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef) 
## RecommendationTemplateTypeDef

```python
# RecommendationTemplateTypeDef definition

class RecommendationTemplateTypeDef(TypedDict):
    assessmentArn: str,
    format: TemplateFormatType,  # (1)
    name: str,
    recommendationTemplateArn: str,
    recommendationTypes: List[RenderRecommendationTypeType],  # (2)
    status: RecommendationTemplateStatusType,  # (3)
    appArn: NotRequired[str],
    endTime: NotRequired[datetime],
    message: NotRequired[str],
    needsReplacements: NotRequired[bool],
    recommendationIds: NotRequired[List[str]],
    startTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    templatesLocation: NotRequired[S3LocationTypeDef],  # (4)
```

1. See [:material-code-brackets: TemplateFormatType](./literals.md#templateformattype) 
2. See [:material-code-brackets: RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype) 
3. See [:material-code-brackets: RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype) 
4. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ResourceErrorsDetailsTypeDef

```python
# ResourceErrorsDetailsTypeDef definition

class ResourceErrorsDetailsTypeDef(TypedDict):
    hasMoreErrors: NotRequired[bool],
    resourceErrors: NotRequired[List[ResourceErrorTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef) 
## ListAlarmRecommendationsResponseTypeDef

```python
# ListAlarmRecommendationsResponseTypeDef definition

class ListAlarmRecommendationsResponseTypeDef(TypedDict):
    alarmRecommendations: List[AlarmRecommendationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmRecommendationTypeDef](./type_defs.md#alarmrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSopRecommendationsResponseTypeDef

```python
# ListSopRecommendationsResponseTypeDef definition

class ListSopRecommendationsResponseTypeDef(TypedDict):
    nextToken: str,
    sopRecommendations: List[SopRecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SopRecommendationTypeDef](./type_defs.md#soprecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTestRecommendationsResponseTypeDef

```python
# ListTestRecommendationsResponseTypeDef definition

class ListTestRecommendationsResponseTypeDef(TypedDict):
    nextToken: str,
    testRecommendations: List[TestRecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TestRecommendationTypeDef](./type_defs.md#testrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppAssessmentsResponseTypeDef

```python
# ListAppAssessmentsResponseTypeDef definition

class ListAppAssessmentsResponseTypeDef(TypedDict):
    assessmentSummaries: List[AppAssessmentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAssessmentSummaryTypeDef](./type_defs.md#appassessmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppAssessmentComplianceDriftsResponseTypeDef

```python
# ListAppAssessmentComplianceDriftsResponseTypeDef definition

class ListAppAssessmentComplianceDriftsResponseTypeDef(TypedDict):
    complianceDrifts: List[ComplianceDriftTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComplianceDriftTypeDef](./type_defs.md#compliancedrifttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppComponentCompliancesResponseTypeDef

```python
# ListAppComponentCompliancesResponseTypeDef definition

class ListAppComponentCompliancesResponseTypeDef(TypedDict):
    componentCompliances: List[AppComponentComplianceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppComponentComplianceTypeDef](./type_defs.md#appcomponentcompliancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppInputSourceResponseTypeDef

```python
# DeleteAppInputSourceResponseTypeDef definition

class DeleteAppInputSourceResponseTypeDef(TypedDict):
    appArn: str,
    appInputSource: AppInputSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInputSourceTypeDef](./type_defs.md#appinputsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppInputSourcesResponseTypeDef

```python
# ListAppInputSourcesResponseTypeDef definition

class ListAppInputSourcesResponseTypeDef(TypedDict):
    appInputSources: List[AppInputSourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppInputSourceTypeDef](./type_defs.md#appinputsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppResponseTypeDef

```python
# CreateAppResponseTypeDef definition

class CreateAppResponseTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppResponseTypeDef

```python
# DescribeAppResponseTypeDef definition

class DescribeAppResponseTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppResponseTypeDef

```python
# UpdateAppResponseTypeDef definition

class UpdateAppResponseTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateRecommendationStatusResponseTypeDef

```python
# BatchUpdateRecommendationStatusResponseTypeDef definition

class BatchUpdateRecommendationStatusResponseTypeDef(TypedDict):
    appArn: str,
    failedEntries: List[BatchUpdateRecommendationStatusFailedEntryTypeDef],  # (1)
    successfulEntries: List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchUpdateRecommendationStatusFailedEntryTypeDef](./type_defs.md#batchupdaterecommendationstatusfailedentrytypedef) 
2. See [:material-code-braces: BatchUpdateRecommendationStatusSuccessfulEntryTypeDef](./type_defs.md#batchupdaterecommendationstatussuccessfulentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateRecommendationStatusRequestRequestTypeDef

```python
# BatchUpdateRecommendationStatusRequestRequestTypeDef definition

class BatchUpdateRecommendationStatusRequestRequestTypeDef(TypedDict):
    appArn: str,
    requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateRecommendationStatusRequestEntryTypeDef](./type_defs.md#updaterecommendationstatusrequestentrytypedef) 
## ComponentRecommendationTypeDef

```python
# ComponentRecommendationTypeDef definition

class ComponentRecommendationTypeDef(TypedDict):
    appComponentName: str,
    configRecommendations: List[ConfigRecommendationTypeDef],  # (1)
    recommendationStatus: RecommendationComplianceStatusType,  # (2)
```

1. See [:material-code-braces: ConfigRecommendationTypeDef](./type_defs.md#configrecommendationtypedef) 
2. See [:material-code-brackets: RecommendationComplianceStatusType](./literals.md#recommendationcompliancestatustype) 
## CreateResiliencyPolicyResponseTypeDef

```python
# CreateResiliencyPolicyResponseTypeDef definition

class CreateResiliencyPolicyResponseTypeDef(TypedDict):
    policy: ResiliencyPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResiliencyPolicyResponseTypeDef

```python
# DescribeResiliencyPolicyResponseTypeDef definition

class DescribeResiliencyPolicyResponseTypeDef(TypedDict):
    policy: ResiliencyPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResiliencyPoliciesResponseTypeDef

```python
# ListResiliencyPoliciesResponseTypeDef definition

class ListResiliencyPoliciesResponseTypeDef(TypedDict):
    nextToken: str,
    resiliencyPolicies: List[ResiliencyPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSuggestedResiliencyPoliciesResponseTypeDef

```python
# ListSuggestedResiliencyPoliciesResponseTypeDef definition

class ListSuggestedResiliencyPoliciesResponseTypeDef(TypedDict):
    nextToken: str,
    resiliencyPolicies: List[ResiliencyPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResiliencyPolicyResponseTypeDef

```python
# UpdateResiliencyPolicyResponseTypeDef definition

class UpdateResiliencyPolicyResponseTypeDef(TypedDict):
    policy: ResiliencyPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppVersionResourceResponseTypeDef

```python
# CreateAppVersionResourceResponseTypeDef definition

class CreateAppVersionResourceResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    physicalResource: PhysicalResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppVersionResourceResponseTypeDef

```python
# DeleteAppVersionResourceResponseTypeDef definition

class DeleteAppVersionResourceResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    physicalResource: PhysicalResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppVersionResourceResponseTypeDef

```python
# DescribeAppVersionResourceResponseTypeDef definition

class DescribeAppVersionResourceResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    physicalResource: PhysicalResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppVersionResourcesResponseTypeDef

```python
# ListAppVersionResourcesResponseTypeDef definition

class ListAppVersionResourcesResponseTypeDef(TypedDict):
    nextToken: str,
    physicalResources: List[PhysicalResourceTypeDef],  # (1)
    resolutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppVersionResourceResponseTypeDef

```python
# UpdateAppVersionResourceResponseTypeDef definition

class UpdateAppVersionResourceResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    physicalResource: PhysicalResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddDraftAppVersionResourceMappingsRequestRequestTypeDef

```python
# AddDraftAppVersionResourceMappingsRequestRequestTypeDef definition

class AddDraftAppVersionResourceMappingsRequestRequestTypeDef(TypedDict):
    appArn: str,
    resourceMappings: Sequence[ResourceMappingTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef) 
## AddDraftAppVersionResourceMappingsResponseTypeDef

```python
# AddDraftAppVersionResourceMappingsResponseTypeDef definition

class AddDraftAppVersionResourceMappingsResponseTypeDef(TypedDict):
    appArn: str,
    appVersion: str,
    resourceMappings: List[ResourceMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppVersionResourceMappingsResponseTypeDef

```python
# ListAppVersionResourceMappingsResponseTypeDef definition

class ListAppVersionResourceMappingsResponseTypeDef(TypedDict):
    nextToken: str,
    resourceMappings: List[ResourceMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUnsupportedAppVersionResourcesResponseTypeDef

```python
# ListUnsupportedAppVersionResourcesResponseTypeDef definition

class ListUnsupportedAppVersionResourcesResponseTypeDef(TypedDict):
    nextToken: str,
    resolutionId: str,
    unsupportedResources: List[UnsupportedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnsupportedResourceTypeDef](./type_defs.md#unsupportedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecommendationTemplateResponseTypeDef

```python
# CreateRecommendationTemplateResponseTypeDef definition

class CreateRecommendationTemplateResponseTypeDef(TypedDict):
    recommendationTemplate: RecommendationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTemplateTypeDef](./type_defs.md#recommendationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecommendationTemplatesResponseTypeDef

```python
# ListRecommendationTemplatesResponseTypeDef definition

class ListRecommendationTemplatesResponseTypeDef(TypedDict):
    nextToken: str,
    recommendationTemplates: List[RecommendationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTemplateTypeDef](./type_defs.md#recommendationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppAssessmentTypeDef

```python
# AppAssessmentTypeDef definition

class AppAssessmentTypeDef(TypedDict):
    assessmentArn: str,
    assessmentStatus: AssessmentStatusType,  # (1)
    invoker: AssessmentInvokerType,  # (6)
    appArn: NotRequired[str],
    appVersion: NotRequired[str],
    assessmentName: NotRequired[str],
    compliance: NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],  # (2)
    complianceStatus: NotRequired[ComplianceStatusType],  # (3)
    cost: NotRequired[CostTypeDef],  # (4)
    driftStatus: NotRequired[DriftStatusType],  # (5)
    endTime: NotRequired[datetime],
    message: NotRequired[str],
    policy: NotRequired[ResiliencyPolicyTypeDef],  # (7)
    resiliencyScore: NotRequired[ResiliencyScoreTypeDef],  # (8)
    resourceErrorsDetails: NotRequired[ResourceErrorsDetailsTypeDef],  # (9)
    startTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    versionName: NotRequired[str],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-brackets: DisruptionTypeType](./literals.md#disruptiontypetype) [:material-code-braces: DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef) 
3. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
4. See [:material-code-braces: CostTypeDef](./type_defs.md#costtypedef) 
5. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
6. See [:material-code-brackets: AssessmentInvokerType](./literals.md#assessmentinvokertype) 
7. See [:material-code-braces: ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef) 
8. See [:material-code-braces: ResiliencyScoreTypeDef](./type_defs.md#resiliencyscoretypedef) 
9. See [:material-code-braces: ResourceErrorsDetailsTypeDef](./type_defs.md#resourceerrorsdetailstypedef) 
## ListAppComponentRecommendationsResponseTypeDef

```python
# ListAppComponentRecommendationsResponseTypeDef definition

class ListAppComponentRecommendationsResponseTypeDef(TypedDict):
    componentRecommendations: List[ComponentRecommendationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentRecommendationTypeDef](./type_defs.md#componentrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppAssessmentResponseTypeDef

```python
# DescribeAppAssessmentResponseTypeDef definition

class DescribeAppAssessmentResponseTypeDef(TypedDict):
    assessment: AppAssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAssessmentTypeDef](./type_defs.md#appassessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAppAssessmentResponseTypeDef

```python
# StartAppAssessmentResponseTypeDef definition

class StartAppAssessmentResponseTypeDef(TypedDict):
    assessment: AppAssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAssessmentTypeDef](./type_defs.md#appassessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
