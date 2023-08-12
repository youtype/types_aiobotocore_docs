# Type definitions

> [Index](../README.md) > [IoTThingsGraph](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
    type annotations stubs module [types-aiobotocore-iotthingsgraph](https://pypi.org/project/types-aiobotocore-iotthingsgraph/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AssociateEntityToThingRequestRequestTypeDef

```python
# AssociateEntityToThingRequestRequestTypeDef definition

class AssociateEntityToThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    entityId: str,
    namespaceVersion: NotRequired[int],
```

## DefinitionDocumentTypeDef

```python
# DefinitionDocumentTypeDef definition

class DefinitionDocumentTypeDef(TypedDict):
    language: DefinitionLanguageType,  # (1)
    text: str,
```

1. See [:material-code-brackets: DefinitionLanguageType](./literals.md#definitionlanguagetype) 
## FlowTemplateSummaryTypeDef

```python
# FlowTemplateSummaryTypeDef definition

class FlowTemplateSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    revisionNumber: NotRequired[int],
    createdAt: NotRequired[datetime],
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

## MetricsConfigurationTypeDef

```python
# MetricsConfigurationTypeDef definition

class MetricsConfigurationTypeDef(TypedDict):
    cloudMetricEnabled: NotRequired[bool],
    metricRuleRoleArn: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## SystemInstanceSummaryTypeDef

```python
# SystemInstanceSummaryTypeDef definition

class SystemInstanceSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    status: NotRequired[SystemInstanceDeploymentStatusType],  # (1)
    target: NotRequired[DeploymentTargetType],  # (2)
    greengrassGroupName: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    greengrassGroupId: NotRequired[str],
    greengrassGroupVersionId: NotRequired[str],
```

1. See [:material-code-brackets: SystemInstanceDeploymentStatusType](./literals.md#systeminstancedeploymentstatustype) 
2. See [:material-code-brackets: DeploymentTargetType](./literals.md#deploymenttargettype) 
## SystemTemplateSummaryTypeDef

```python
# SystemTemplateSummaryTypeDef definition

class SystemTemplateSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    revisionNumber: NotRequired[int],
    createdAt: NotRequired[datetime],
```

## DeleteFlowTemplateRequestRequestTypeDef

```python
# DeleteFlowTemplateRequestRequestTypeDef definition

class DeleteFlowTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteSystemInstanceRequestRequestTypeDef

```python
# DeleteSystemInstanceRequestRequestTypeDef definition

class DeleteSystemInstanceRequestRequestTypeDef(TypedDict):
    id: NotRequired[str],
```

## DeleteSystemTemplateRequestRequestTypeDef

```python
# DeleteSystemTemplateRequestRequestTypeDef definition

class DeleteSystemTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DependencyRevisionTypeDef

```python
# DependencyRevisionTypeDef definition

class DependencyRevisionTypeDef(TypedDict):
    id: NotRequired[str],
    revisionNumber: NotRequired[int],
```

## DeploySystemInstanceRequestRequestTypeDef

```python
# DeploySystemInstanceRequestRequestTypeDef definition

class DeploySystemInstanceRequestRequestTypeDef(TypedDict):
    id: NotRequired[str],
```

## DeprecateFlowTemplateRequestRequestTypeDef

```python
# DeprecateFlowTemplateRequestRequestTypeDef definition

class DeprecateFlowTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeprecateSystemTemplateRequestRequestTypeDef

```python
# DeprecateSystemTemplateRequestRequestTypeDef definition

class DeprecateSystemTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DescribeNamespaceRequestRequestTypeDef

```python
# DescribeNamespaceRequestRequestTypeDef definition

class DescribeNamespaceRequestRequestTypeDef(TypedDict):
    namespaceName: NotRequired[str],
```

## DissociateEntityFromThingRequestRequestTypeDef

```python
# DissociateEntityFromThingRequestRequestTypeDef definition

class DissociateEntityFromThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    entityType: EntityTypeType,  # (1)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## EntityFilterTypeDef

```python
# EntityFilterTypeDef definition

class EntityFilterTypeDef(TypedDict):
    name: NotRequired[EntityFilterNameType],  # (1)
    value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EntityFilterNameType](./literals.md#entityfilternametype) 
## FlowExecutionMessageTypeDef

```python
# FlowExecutionMessageTypeDef definition

class FlowExecutionMessageTypeDef(TypedDict):
    messageId: NotRequired[str],
    eventType: NotRequired[FlowExecutionEventTypeType],  # (1)
    timestamp: NotRequired[datetime],
    payload: NotRequired[str],
```

1. See [:material-code-brackets: FlowExecutionEventTypeType](./literals.md#flowexecutioneventtypetype) 
## FlowExecutionSummaryTypeDef

```python
# FlowExecutionSummaryTypeDef definition

class FlowExecutionSummaryTypeDef(TypedDict):
    flowExecutionId: NotRequired[str],
    status: NotRequired[FlowExecutionStatusType],  # (1)
    systemInstanceId: NotRequired[str],
    flowTemplateId: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: FlowExecutionStatusType](./literals.md#flowexecutionstatustype) 
## FlowTemplateFilterTypeDef

```python
# FlowTemplateFilterTypeDef definition

class FlowTemplateFilterTypeDef(TypedDict):
    name: FlowTemplateFilterNameType,  # (1)
    value: Sequence[str],
```

1. See [:material-code-brackets: FlowTemplateFilterNameType](./literals.md#flowtemplatefilternametype) 
## GetEntitiesRequestRequestTypeDef

```python
# GetEntitiesRequestRequestTypeDef definition

class GetEntitiesRequestRequestTypeDef(TypedDict):
    ids: Sequence[str],
    namespaceVersion: NotRequired[int],
```

## GetFlowTemplateRequestRequestTypeDef

```python
# GetFlowTemplateRequestRequestTypeDef definition

class GetFlowTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    revisionNumber: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetFlowTemplateRevisionsRequestRequestTypeDef

```python
# GetFlowTemplateRevisionsRequestRequestTypeDef definition

class GetFlowTemplateRevisionsRequestRequestTypeDef(TypedDict):
    id: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetSystemInstanceRequestRequestTypeDef

```python
# GetSystemInstanceRequestRequestTypeDef definition

class GetSystemInstanceRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSystemTemplateRequestRequestTypeDef

```python
# GetSystemTemplateRequestRequestTypeDef definition

class GetSystemTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    revisionNumber: NotRequired[int],
```

## GetSystemTemplateRevisionsRequestRequestTypeDef

```python
# GetSystemTemplateRevisionsRequestRequestTypeDef definition

class GetSystemTemplateRevisionsRequestRequestTypeDef(TypedDict):
    id: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetUploadStatusRequestRequestTypeDef

```python
# GetUploadStatusRequestRequestTypeDef definition

class GetUploadStatusRequestRequestTypeDef(TypedDict):
    uploadId: str,
```

## ListFlowExecutionMessagesRequestRequestTypeDef

```python
# ListFlowExecutionMessagesRequestRequestTypeDef definition

class ListFlowExecutionMessagesRequestRequestTypeDef(TypedDict):
    flowExecutionId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SystemInstanceFilterTypeDef

```python
# SystemInstanceFilterTypeDef definition

class SystemInstanceFilterTypeDef(TypedDict):
    name: NotRequired[SystemInstanceFilterNameType],  # (1)
    value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SystemInstanceFilterNameType](./literals.md#systeminstancefilternametype) 
## SystemTemplateFilterTypeDef

```python
# SystemTemplateFilterTypeDef definition

class SystemTemplateFilterTypeDef(TypedDict):
    name: SystemTemplateFilterNameType,  # (1)
    value: Sequence[str],
```

1. See [:material-code-brackets: SystemTemplateFilterNameType](./literals.md#systemtemplatefilternametype) 
## SearchThingsRequestRequestTypeDef

```python
# SearchThingsRequestRequestTypeDef definition

class SearchThingsRequestRequestTypeDef(TypedDict):
    entityId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    namespaceVersion: NotRequired[int],
```

## ThingTypeDef

```python
# ThingTypeDef definition

class ThingTypeDef(TypedDict):
    thingArn: NotRequired[str],
    thingName: NotRequired[str],
```

## UndeploySystemInstanceRequestRequestTypeDef

```python
# UndeploySystemInstanceRequestRequestTypeDef definition

class UndeploySystemInstanceRequestRequestTypeDef(TypedDict):
    id: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateFlowTemplateRequestRequestTypeDef

```python
# CreateFlowTemplateRequestRequestTypeDef definition

class CreateFlowTemplateRequestRequestTypeDef(TypedDict):
    definition: DefinitionDocumentTypeDef,  # (1)
    compatibleNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## CreateSystemTemplateRequestRequestTypeDef

```python
# CreateSystemTemplateRequestRequestTypeDef definition

class CreateSystemTemplateRequestRequestTypeDef(TypedDict):
    definition: DefinitionDocumentTypeDef,  # (1)
    compatibleNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## EntityDescriptionTypeDef

```python
# EntityDescriptionTypeDef definition

class EntityDescriptionTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    type: NotRequired[EntityTypeType],  # (1)
    createdAt: NotRequired[datetime],
    definition: NotRequired[DefinitionDocumentTypeDef],  # (2)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## UpdateFlowTemplateRequestRequestTypeDef

```python
# UpdateFlowTemplateRequestRequestTypeDef definition

class UpdateFlowTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    definition: DefinitionDocumentTypeDef,  # (1)
    compatibleNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## UpdateSystemTemplateRequestRequestTypeDef

```python
# UpdateSystemTemplateRequestRequestTypeDef definition

class UpdateSystemTemplateRequestRequestTypeDef(TypedDict):
    id: str,
    definition: DefinitionDocumentTypeDef,  # (1)
    compatibleNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## UploadEntityDefinitionsRequestRequestTypeDef

```python
# UploadEntityDefinitionsRequestRequestTypeDef definition

class UploadEntityDefinitionsRequestRequestTypeDef(TypedDict):
    document: NotRequired[DefinitionDocumentTypeDef],  # (1)
    syncWithPublicNamespace: NotRequired[bool],
    deprecateExistingEntities: NotRequired[bool],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## FlowTemplateDescriptionTypeDef

```python
# FlowTemplateDescriptionTypeDef definition

class FlowTemplateDescriptionTypeDef(TypedDict):
    summary: NotRequired[FlowTemplateSummaryTypeDef],  # (1)
    definition: NotRequired[DefinitionDocumentTypeDef],  # (2)
    validatedNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: FlowTemplateSummaryTypeDef](./type_defs.md#flowtemplatesummarytypedef) 
2. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## CreateFlowTemplateResponseTypeDef

```python
# CreateFlowTemplateResponseTypeDef definition

class CreateFlowTemplateResponseTypeDef(TypedDict):
    summary: FlowTemplateSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTemplateSummaryTypeDef](./type_defs.md#flowtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNamespaceResponseTypeDef

```python
# DeleteNamespaceResponseTypeDef definition

class DeleteNamespaceResponseTypeDef(TypedDict):
    namespaceArn: str,
    namespaceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNamespaceResponseTypeDef

```python
# DescribeNamespaceResponseTypeDef definition

class DescribeNamespaceResponseTypeDef(TypedDict):
    namespaceArn: str,
    namespaceName: str,
    trackingNamespaceName: str,
    trackingNamespaceVersion: int,
    namespaceVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowTemplateRevisionsResponseTypeDef

```python
# GetFlowTemplateRevisionsResponseTypeDef definition

class GetFlowTemplateRevisionsResponseTypeDef(TypedDict):
    summaries: List[FlowTemplateSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTemplateSummaryTypeDef](./type_defs.md#flowtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamespaceDeletionStatusResponseTypeDef

```python
# GetNamespaceDeletionStatusResponseTypeDef definition

class GetNamespaceDeletionStatusResponseTypeDef(TypedDict):
    namespaceArn: str,
    namespaceName: str,
    status: NamespaceDeletionStatusType,  # (1)
    errorCode: NamespaceDeletionStatusErrorCodesType,  # (2)
    errorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NamespaceDeletionStatusType](./literals.md#namespacedeletionstatustype) 
2. See [:material-code-brackets: NamespaceDeletionStatusErrorCodesType](./literals.md#namespacedeletionstatuserrorcodestype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUploadStatusResponseTypeDef

```python
# GetUploadStatusResponseTypeDef definition

class GetUploadStatusResponseTypeDef(TypedDict):
    uploadId: str,
    uploadStatus: UploadStatusType,  # (1)
    namespaceArn: str,
    namespaceName: str,
    namespaceVersion: int,
    failureReason: List[str],
    createdDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: UploadStatusType](./literals.md#uploadstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFlowTemplatesResponseTypeDef

```python
# SearchFlowTemplatesResponseTypeDef definition

class SearchFlowTemplatesResponseTypeDef(TypedDict):
    summaries: List[FlowTemplateSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTemplateSummaryTypeDef](./type_defs.md#flowtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowTemplateResponseTypeDef

```python
# UpdateFlowTemplateResponseTypeDef definition

class UpdateFlowTemplateResponseTypeDef(TypedDict):
    summary: FlowTemplateSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTemplateSummaryTypeDef](./type_defs.md#flowtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadEntityDefinitionsResponseTypeDef

```python
# UploadEntityDefinitionsResponseTypeDef definition

class UploadEntityDefinitionsResponseTypeDef(TypedDict):
    uploadId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSystemInstanceRequestRequestTypeDef

```python
# CreateSystemInstanceRequestRequestTypeDef definition

class CreateSystemInstanceRequestRequestTypeDef(TypedDict):
    definition: DefinitionDocumentTypeDef,  # (1)
    target: DeploymentTargetType,  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    greengrassGroupName: NotRequired[str],
    s3BucketName: NotRequired[str],
    metricsConfiguration: NotRequired[MetricsConfigurationTypeDef],  # (4)
    flowActionsRoleArn: NotRequired[str],
```

1. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
2. See [:material-code-brackets: DeploymentTargetType](./literals.md#deploymenttargettype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSystemInstanceResponseTypeDef

```python
# CreateSystemInstanceResponseTypeDef definition

class CreateSystemInstanceResponseTypeDef(TypedDict):
    summary: SystemInstanceSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemInstanceSummaryTypeDef](./type_defs.md#systeminstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploySystemInstanceResponseTypeDef

```python
# DeploySystemInstanceResponseTypeDef definition

class DeploySystemInstanceResponseTypeDef(TypedDict):
    summary: SystemInstanceSummaryTypeDef,  # (1)
    greengrassDeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemInstanceSummaryTypeDef](./type_defs.md#systeminstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchSystemInstancesResponseTypeDef

```python
# SearchSystemInstancesResponseTypeDef definition

class SearchSystemInstancesResponseTypeDef(TypedDict):
    summaries: List[SystemInstanceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemInstanceSummaryTypeDef](./type_defs.md#systeminstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UndeploySystemInstanceResponseTypeDef

```python
# UndeploySystemInstanceResponseTypeDef definition

class UndeploySystemInstanceResponseTypeDef(TypedDict):
    summary: SystemInstanceSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemInstanceSummaryTypeDef](./type_defs.md#systeminstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSystemTemplateResponseTypeDef

```python
# CreateSystemTemplateResponseTypeDef definition

class CreateSystemTemplateResponseTypeDef(TypedDict):
    summary: SystemTemplateSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemTemplateSummaryTypeDef](./type_defs.md#systemtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSystemTemplateRevisionsResponseTypeDef

```python
# GetSystemTemplateRevisionsResponseTypeDef definition

class GetSystemTemplateRevisionsResponseTypeDef(TypedDict):
    summaries: List[SystemTemplateSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemTemplateSummaryTypeDef](./type_defs.md#systemtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchSystemTemplatesResponseTypeDef

```python
# SearchSystemTemplatesResponseTypeDef definition

class SearchSystemTemplatesResponseTypeDef(TypedDict):
    summaries: List[SystemTemplateSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemTemplateSummaryTypeDef](./type_defs.md#systemtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SystemTemplateDescriptionTypeDef

```python
# SystemTemplateDescriptionTypeDef definition

class SystemTemplateDescriptionTypeDef(TypedDict):
    summary: NotRequired[SystemTemplateSummaryTypeDef],  # (1)
    definition: NotRequired[DefinitionDocumentTypeDef],  # (2)
    validatedNamespaceVersion: NotRequired[int],
```

1. See [:material-code-braces: SystemTemplateSummaryTypeDef](./type_defs.md#systemtemplatesummarytypedef) 
2. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
## UpdateSystemTemplateResponseTypeDef

```python
# UpdateSystemTemplateResponseTypeDef definition

class UpdateSystemTemplateResponseTypeDef(TypedDict):
    summary: SystemTemplateSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemTemplateSummaryTypeDef](./type_defs.md#systemtemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SystemInstanceDescriptionTypeDef

```python
# SystemInstanceDescriptionTypeDef definition

class SystemInstanceDescriptionTypeDef(TypedDict):
    summary: NotRequired[SystemInstanceSummaryTypeDef],  # (1)
    definition: NotRequired[DefinitionDocumentTypeDef],  # (2)
    s3BucketName: NotRequired[str],
    metricsConfiguration: NotRequired[MetricsConfigurationTypeDef],  # (3)
    validatedNamespaceVersion: NotRequired[int],
    validatedDependencyRevisions: NotRequired[List[DependencyRevisionTypeDef]],  # (4)
    flowActionsRoleArn: NotRequired[str],
```

1. See [:material-code-braces: SystemInstanceSummaryTypeDef](./type_defs.md#systeminstancesummarytypedef) 
2. See [:material-code-braces: DefinitionDocumentTypeDef](./type_defs.md#definitiondocumenttypedef) 
3. See [:material-code-braces: MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef) 
4. See [:material-code-braces: DependencyRevisionTypeDef](./type_defs.md#dependencyrevisiontypedef) 
## SearchEntitiesRequestRequestTypeDef

```python
# SearchEntitiesRequestRequestTypeDef definition

class SearchEntitiesRequestRequestTypeDef(TypedDict):
    entityTypes: Sequence[EntityTypeType],  # (1)
    filters: NotRequired[Sequence[EntityFilterTypeDef]],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    namespaceVersion: NotRequired[int],
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
## ListFlowExecutionMessagesResponseTypeDef

```python
# ListFlowExecutionMessagesResponseTypeDef definition

class ListFlowExecutionMessagesResponseTypeDef(TypedDict):
    messages: List[FlowExecutionMessageTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowExecutionMessageTypeDef](./type_defs.md#flowexecutionmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFlowExecutionsResponseTypeDef

```python
# SearchFlowExecutionsResponseTypeDef definition

class SearchFlowExecutionsResponseTypeDef(TypedDict):
    summaries: List[FlowExecutionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowExecutionSummaryTypeDef](./type_defs.md#flowexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFlowTemplatesRequestRequestTypeDef

```python
# SearchFlowTemplatesRequestRequestTypeDef definition

class SearchFlowTemplatesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FlowTemplateFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FlowTemplateFilterTypeDef](./type_defs.md#flowtemplatefiltertypedef) 
## GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef

```python
# GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef definition

class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(TypedDict):
    id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef

```python
# GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef definition

class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(TypedDict):
    id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef

```python
# ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef definition

class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(TypedDict):
    flowExecutionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchEntitiesRequestSearchEntitiesPaginateTypeDef

```python
# SearchEntitiesRequestSearchEntitiesPaginateTypeDef definition

class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(TypedDict):
    entityTypes: Sequence[EntityTypeType],  # (1)
    filters: NotRequired[Sequence[EntityFilterTypeDef]],  # (2)
    namespaceVersion: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef

```python
# SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef definition

class SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FlowTemplateFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FlowTemplateFilterTypeDef](./type_defs.md#flowtemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchThingsRequestSearchThingsPaginateTypeDef

```python
# SearchThingsRequestSearchThingsPaginateTypeDef definition

class SearchThingsRequestSearchThingsPaginateTypeDef(TypedDict):
    entityId: str,
    namespaceVersion: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchFlowExecutionsRequestRequestTypeDef

```python
# SearchFlowExecutionsRequestRequestTypeDef definition

class SearchFlowExecutionsRequestRequestTypeDef(TypedDict):
    systemInstanceId: str,
    flowExecutionId: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    endTime: NotRequired[Union[datetime, str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef

```python
# SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef definition

class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(TypedDict):
    systemInstanceId: str,
    flowExecutionId: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    endTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSystemInstancesRequestRequestTypeDef

```python
# SearchSystemInstancesRequestRequestTypeDef definition

class SearchSystemInstancesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[SystemInstanceFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: SystemInstanceFilterTypeDef](./type_defs.md#systeminstancefiltertypedef) 
## SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef

```python
# SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef definition

class SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[SystemInstanceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SystemInstanceFilterTypeDef](./type_defs.md#systeminstancefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSystemTemplatesRequestRequestTypeDef

```python
# SearchSystemTemplatesRequestRequestTypeDef definition

class SearchSystemTemplatesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[SystemTemplateFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: SystemTemplateFilterTypeDef](./type_defs.md#systemtemplatefiltertypedef) 
## SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef

```python
# SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef definition

class SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[SystemTemplateFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SystemTemplateFilterTypeDef](./type_defs.md#systemtemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchThingsResponseTypeDef

```python
# SearchThingsResponseTypeDef definition

class SearchThingsResponseTypeDef(TypedDict):
    things: List[ThingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThingTypeDef](./type_defs.md#thingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEntitiesResponseTypeDef

```python
# GetEntitiesResponseTypeDef definition

class GetEntitiesResponseTypeDef(TypedDict):
    descriptions: List[EntityDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityDescriptionTypeDef](./type_defs.md#entitydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchEntitiesResponseTypeDef

```python
# SearchEntitiesResponseTypeDef definition

class SearchEntitiesResponseTypeDef(TypedDict):
    descriptions: List[EntityDescriptionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityDescriptionTypeDef](./type_defs.md#entitydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowTemplateResponseTypeDef

```python
# GetFlowTemplateResponseTypeDef definition

class GetFlowTemplateResponseTypeDef(TypedDict):
    description: FlowTemplateDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowTemplateDescriptionTypeDef](./type_defs.md#flowtemplatedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSystemTemplateResponseTypeDef

```python
# GetSystemTemplateResponseTypeDef definition

class GetSystemTemplateResponseTypeDef(TypedDict):
    description: SystemTemplateDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemTemplateDescriptionTypeDef](./type_defs.md#systemtemplatedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSystemInstanceResponseTypeDef

```python
# GetSystemInstanceResponseTypeDef definition

class GetSystemInstanceResponseTypeDef(TypedDict):
    description: SystemInstanceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SystemInstanceDescriptionTypeDef](./type_defs.md#systeminstancedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
