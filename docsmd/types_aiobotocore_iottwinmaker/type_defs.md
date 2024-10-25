# Type definitions

> [Index](../README.md) > [IoTTwinMaker](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## EntityPropertyReferenceUnionTypeDef

```python
# EntityPropertyReferenceUnionTypeDef definition

EntityPropertyReferenceUnionTypeDef = Union[
    EntityPropertyReferenceTypeDef,  # (1)
    EntityPropertyReferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef) 
2. See [:material-code-braces: EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef) 

## DataValueUnionTypeDef

```python
# DataValueUnionTypeDef definition

DataValueUnionTypeDef = Union[
    DataValueTypeDef,  # (1)
    DataValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 

## IotSiteWiseSourceConfigurationUnionTypeDef

```python
# IotSiteWiseSourceConfigurationUnionTypeDef definition

IotSiteWiseSourceConfigurationUnionTypeDef = Union[
    IotSiteWiseSourceConfigurationTypeDef,  # (1)
    IotSiteWiseSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IotSiteWiseSourceConfigurationTypeDef](./type_defs.md#iotsitewisesourceconfigurationtypedef) 
2. See [:material-code-braces: IotSiteWiseSourceConfigurationOutputTypeDef](./type_defs.md#iotsitewisesourceconfigurationoutputtypedef) 

## IotTwinMakerSourceConfigurationUnionTypeDef

```python
# IotTwinMakerSourceConfigurationUnionTypeDef definition

IotTwinMakerSourceConfigurationUnionTypeDef = Union[
    IotTwinMakerSourceConfigurationTypeDef,  # (1)
    IotTwinMakerSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IotTwinMakerSourceConfigurationTypeDef](./type_defs.md#iottwinmakersourceconfigurationtypedef) 
2. See [:material-code-braces: IotTwinMakerSourceConfigurationOutputTypeDef](./type_defs.md#iottwinmakersourceconfigurationoutputtypedef) 

## DataTypeUnionTypeDef

```python
# DataTypeUnionTypeDef definition

DataTypeUnionTypeDef = Union[
    DataTypeTypeDef,  # (1)
    DataTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataTypeTypeDef](./type_defs.md#datatypetypedef) 
2. See [:material-code-braces: DataTypeOutputTypeDef](./type_defs.md#datatypeoutputtypedef) 

## PropertyValueUnionTypeDef

```python
# PropertyValueUnionTypeDef definition

PropertyValueUnionTypeDef = Union[
    PropertyValueTypeDef,  # (1)
    PropertyValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef) 
2. See [:material-code-braces: PropertyValueOutputTypeDef](./type_defs.md#propertyvalueoutputtypedef) 

## SourceConfigurationUnionTypeDef

```python
# SourceConfigurationUnionTypeDef definition

SourceConfigurationUnionTypeDef = Union[
    SourceConfigurationTypeDef,  # (1)
    SourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
2. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 

## PropertyValueEntryUnionTypeDef

```python
# PropertyValueEntryUnionTypeDef definition

PropertyValueEntryUnionTypeDef = Union[
    PropertyValueEntryTypeDef,  # (1)
    PropertyValueEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef) 
2. See [:material-code-braces: PropertyValueEntryOutputTypeDef](./type_defs.md#propertyvalueentryoutputtypedef) 



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

## BundleInformationTypeDef

```python
# BundleInformationTypeDef definition

class BundleInformationTypeDef(TypedDict):
    bundleNames: List[str],
    pricingTier: NotRequired[PricingTierType],  # (1)
```

1. See [:material-code-brackets: PricingTierType](./literals.md#pricingtiertype) 
## CancelMetadataTransferJobRequestRequestTypeDef

```python
# CancelMetadataTransferJobRequestRequestTypeDef definition

class CancelMetadataTransferJobRequestRequestTypeDef(TypedDict):
    metadataTransferJobId: str,
```

## MetadataTransferJobProgressTypeDef

```python
# MetadataTransferJobProgressTypeDef definition

class MetadataTransferJobProgressTypeDef(TypedDict):
    totalCount: NotRequired[int],
    succeededCount: NotRequired[int],
    skippedCount: NotRequired[int],
    failedCount: NotRequired[int],
```

## ColumnDescriptionTypeDef

```python
# ColumnDescriptionTypeDef definition

class ColumnDescriptionTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
## ComponentPropertyGroupRequestTypeDef

```python
# ComponentPropertyGroupRequestTypeDef definition

class ComponentPropertyGroupRequestTypeDef(TypedDict):
    groupType: NotRequired[GroupTypeType],  # (1)
    propertyNames: NotRequired[Sequence[str]],
    updateType: NotRequired[PropertyGroupUpdateTypeType],  # (2)
```

1. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
2. See [:material-code-brackets: PropertyGroupUpdateTypeType](./literals.md#propertygroupupdatetypetype) 
## ComponentPropertyGroupResponseTypeDef

```python
# ComponentPropertyGroupResponseTypeDef definition

class ComponentPropertyGroupResponseTypeDef(TypedDict):
    groupType: GroupTypeType,  # (1)
    propertyNames: List[str],
    isInherited: bool,
```

1. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
## CompositeComponentTypeRequestTypeDef

```python
# CompositeComponentTypeRequestTypeDef definition

class CompositeComponentTypeRequestTypeDef(TypedDict):
    componentTypeId: NotRequired[str],
```

## CompositeComponentTypeResponseTypeDef

```python
# CompositeComponentTypeResponseTypeDef definition

class CompositeComponentTypeResponseTypeDef(TypedDict):
    componentTypeId: NotRequired[str],
    isInherited: NotRequired[bool],
```

## PropertyGroupRequestTypeDef

```python
# PropertyGroupRequestTypeDef definition

class PropertyGroupRequestTypeDef(TypedDict):
    groupType: NotRequired[GroupTypeType],  # (1)
    propertyNames: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
## CreateSceneRequestRequestTypeDef

```python
# CreateSceneRequestRequestTypeDef definition

class CreateSceneRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    sceneId: str,
    contentLocation: str,
    description: NotRequired[str],
    capabilities: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
    sceneMetadata: NotRequired[Mapping[str, str]],
```

## CreateSyncJobRequestRequestTypeDef

```python
# CreateSyncJobRequestRequestTypeDef definition

class CreateSyncJobRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    syncSource: str,
    syncRole: str,
    tags: NotRequired[Mapping[str, str]],
```

## CreateWorkspaceRequestRequestTypeDef

```python
# CreateWorkspaceRequestRequestTypeDef definition

class CreateWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    description: NotRequired[str],
    s3Location: NotRequired[str],
    role: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## LambdaFunctionTypeDef

```python
# LambdaFunctionTypeDef definition

class LambdaFunctionTypeDef(TypedDict):
    arn: str,
```

## RelationshipTypeDef

```python
# RelationshipTypeDef definition

class RelationshipTypeDef(TypedDict):
    targetComponentTypeId: NotRequired[str],
    relationshipType: NotRequired[str],
```

## RelationshipValueTypeDef

```python
# RelationshipValueTypeDef definition

class RelationshipValueTypeDef(TypedDict):
    targetEntityId: NotRequired[str],
    targetComponentName: NotRequired[str],
```

## DeleteComponentTypeRequestRequestTypeDef

```python
# DeleteComponentTypeRequestRequestTypeDef definition

class DeleteComponentTypeRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    componentTypeId: str,
```

## DeleteEntityRequestRequestTypeDef

```python
# DeleteEntityRequestRequestTypeDef definition

class DeleteEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
    isRecursive: NotRequired[bool],
```

## DeleteSceneRequestRequestTypeDef

```python
# DeleteSceneRequestRequestTypeDef definition

class DeleteSceneRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    sceneId: str,
```

## DeleteSyncJobRequestRequestTypeDef

```python
# DeleteSyncJobRequestRequestTypeDef definition

class DeleteSyncJobRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    syncSource: str,
```

## DeleteWorkspaceRequestRequestTypeDef

```python
# DeleteWorkspaceRequestRequestTypeDef definition

class DeleteWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## IotTwinMakerDestinationConfigurationTypeDef

```python
# IotTwinMakerDestinationConfigurationTypeDef definition

class IotTwinMakerDestinationConfigurationTypeDef(TypedDict):
    workspace: str,
```

## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    location: str,
```

## EntityPropertyReferenceOutputTypeDef

```python
# EntityPropertyReferenceOutputTypeDef definition

class EntityPropertyReferenceOutputTypeDef(TypedDict):
    propertyName: str,
    componentName: NotRequired[str],
    componentPath: NotRequired[str],
    externalIdProperty: NotRequired[Dict[str, str]],
    entityId: NotRequired[str],
```

## EntityPropertyReferenceTypeDef

```python
# EntityPropertyReferenceTypeDef definition

class EntityPropertyReferenceTypeDef(TypedDict):
    propertyName: str,
    componentName: NotRequired[str],
    componentPath: NotRequired[str],
    externalIdProperty: NotRequired[Mapping[str, str]],
    entityId: NotRequired[str],
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    code: NotRequired[ErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ExecuteQueryRequestRequestTypeDef

```python
# ExecuteQueryRequestRequestTypeDef definition

class ExecuteQueryRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    queryStatement: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RowTypeDef

```python
# RowTypeDef definition

class RowTypeDef(TypedDict):
    rowData: NotRequired[List[Dict[str, Any]]],
```

## FilterByAssetModelTypeDef

```python
# FilterByAssetModelTypeDef definition

class FilterByAssetModelTypeDef(TypedDict):
    assetModelId: NotRequired[str],
    assetModelExternalId: NotRequired[str],
    includeOffspring: NotRequired[bool],
    includeAssets: NotRequired[bool],
```

## FilterByAssetTypeDef

```python
# FilterByAssetTypeDef definition

class FilterByAssetTypeDef(TypedDict):
    assetId: NotRequired[str],
    assetExternalId: NotRequired[str],
    includeOffspring: NotRequired[bool],
    includeAssetModel: NotRequired[bool],
```

## FilterByComponentTypeTypeDef

```python
# FilterByComponentTypeTypeDef definition

class FilterByComponentTypeTypeDef(TypedDict):
    componentTypeId: str,
```

## FilterByEntityTypeDef

```python
# FilterByEntityTypeDef definition

class FilterByEntityTypeDef(TypedDict):
    entityId: str,
```

## GetComponentTypeRequestRequestTypeDef

```python
# GetComponentTypeRequestRequestTypeDef definition

class GetComponentTypeRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    componentTypeId: str,
```

## PropertyGroupResponseTypeDef

```python
# PropertyGroupResponseTypeDef definition

class PropertyGroupResponseTypeDef(TypedDict):
    groupType: GroupTypeType,  # (1)
    propertyNames: List[str],
    isInherited: bool,
```

1. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
## GetEntityRequestRequestTypeDef

```python
# GetEntityRequestRequestTypeDef definition

class GetEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
```

## GetMetadataTransferJobRequestRequestTypeDef

```python
# GetMetadataTransferJobRequestRequestTypeDef definition

class GetMetadataTransferJobRequestRequestTypeDef(TypedDict):
    metadataTransferJobId: str,
```

## InterpolationParametersTypeDef

```python
# InterpolationParametersTypeDef definition

class InterpolationParametersTypeDef(TypedDict):
    interpolationType: NotRequired[InterpolationTypeType],  # (1)
    intervalInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: InterpolationTypeType](./literals.md#interpolationtypetype) 
## GetSceneRequestRequestTypeDef

```python
# GetSceneRequestRequestTypeDef definition

class GetSceneRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    sceneId: str,
```

## SceneErrorTypeDef

```python
# SceneErrorTypeDef definition

class SceneErrorTypeDef(TypedDict):
    code: NotRequired[SceneErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: SceneErrorCodeType](./literals.md#sceneerrorcodetype) 
## GetSyncJobRequestRequestTypeDef

```python
# GetSyncJobRequestRequestTypeDef definition

class GetSyncJobRequestRequestTypeDef(TypedDict):
    syncSource: str,
    workspaceId: NotRequired[str],
```

## GetWorkspaceRequestRequestTypeDef

```python
# GetWorkspaceRequestRequestTypeDef definition

class GetWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## ListComponentTypesFilterTypeDef

```python
# ListComponentTypesFilterTypeDef definition

class ListComponentTypesFilterTypeDef(TypedDict):
    extendsFrom: NotRequired[str],
    namespace: NotRequired[str],
    isAbstract: NotRequired[bool],
```

## ListComponentsRequestRequestTypeDef

```python
# ListComponentsRequestRequestTypeDef definition

class ListComponentsRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
    componentPath: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEntitiesFilterTypeDef

```python
# ListEntitiesFilterTypeDef definition

class ListEntitiesFilterTypeDef(TypedDict):
    parentEntityId: NotRequired[str],
    componentTypeId: NotRequired[str],
    externalId: NotRequired[str],
```

## ListMetadataTransferJobsFilterTypeDef

```python
# ListMetadataTransferJobsFilterTypeDef definition

class ListMetadataTransferJobsFilterTypeDef(TypedDict):
    workspaceId: NotRequired[str],
    state: NotRequired[MetadataTransferJobStateType],  # (1)
```

1. See [:material-code-brackets: MetadataTransferJobStateType](./literals.md#metadatatransferjobstatetype) 
## ListPropertiesRequestRequestTypeDef

```python
# ListPropertiesRequestRequestTypeDef definition

class ListPropertiesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
    componentName: NotRequired[str],
    componentPath: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListScenesRequestRequestTypeDef

```python
# ListScenesRequestRequestTypeDef definition

class ListScenesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SceneSummaryTypeDef

```python
# SceneSummaryTypeDef definition

class SceneSummaryTypeDef(TypedDict):
    sceneId: str,
    contentLocation: str,
    arn: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    description: NotRequired[str],
```

## ListSyncJobsRequestRequestTypeDef

```python
# ListSyncJobsRequestRequestTypeDef definition

class ListSyncJobsRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SyncResourceFilterTypeDef

```python
# SyncResourceFilterTypeDef definition

class SyncResourceFilterTypeDef(TypedDict):
    state: NotRequired[SyncResourceStateType],  # (1)
    resourceType: NotRequired[SyncResourceTypeType],  # (2)
    resourceId: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-brackets: SyncResourceStateType](./literals.md#syncresourcestatetype) 
2. See [:material-code-brackets: SyncResourceTypeType](./literals.md#syncresourcetypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListWorkspacesRequestRequestTypeDef

```python
# ListWorkspacesRequestRequestTypeDef definition

class ListWorkspacesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkspaceSummaryTypeDef

```python
# WorkspaceSummaryTypeDef definition

class WorkspaceSummaryTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    description: NotRequired[str],
    linkedServices: NotRequired[List[str]],
```

## OrderByTypeDef

```python
# OrderByTypeDef definition

class OrderByTypeDef(TypedDict):
    propertyName: str,
    order: NotRequired[OrderType],  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ParentEntityUpdateRequestTypeDef

```python
# ParentEntityUpdateRequestTypeDef definition

class ParentEntityUpdateRequestTypeDef(TypedDict):
    updateType: ParentEntityUpdateTypeType,  # (1)
    parentEntityId: NotRequired[str],
```

1. See [:material-code-brackets: ParentEntityUpdateTypeType](./literals.md#parententityupdatetypetype) 
## S3SourceConfigurationTypeDef

```python
# S3SourceConfigurationTypeDef definition

class S3SourceConfigurationTypeDef(TypedDict):
    location: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UpdatePricingPlanRequestRequestTypeDef

```python
# UpdatePricingPlanRequestRequestTypeDef definition

class UpdatePricingPlanRequestRequestTypeDef(TypedDict):
    pricingMode: PricingModeType,  # (1)
    bundleNames: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PricingModeType](./literals.md#pricingmodetype) 
## UpdateSceneRequestRequestTypeDef

```python
# UpdateSceneRequestRequestTypeDef definition

class UpdateSceneRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    sceneId: str,
    contentLocation: NotRequired[str],
    description: NotRequired[str],
    capabilities: NotRequired[Sequence[str]],
    sceneMetadata: NotRequired[Mapping[str, str]],
```

## UpdateWorkspaceRequestRequestTypeDef

```python
# UpdateWorkspaceRequestRequestTypeDef definition

class UpdateWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    description: NotRequired[str],
    role: NotRequired[str],
    s3Location: NotRequired[str],
```

## CreateComponentTypeResponseTypeDef

```python
# CreateComponentTypeResponseTypeDef definition

class CreateComponentTypeResponseTypeDef(TypedDict):
    arn: str,
    creationDateTime: datetime,
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEntityResponseTypeDef

```python
# CreateEntityResponseTypeDef definition

class CreateEntityResponseTypeDef(TypedDict):
    entityId: str,
    arn: str,
    creationDateTime: datetime,
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSceneResponseTypeDef

```python
# CreateSceneResponseTypeDef definition

class CreateSceneResponseTypeDef(TypedDict):
    arn: str,
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSyncJobResponseTypeDef

```python
# CreateSyncJobResponseTypeDef definition

class CreateSyncJobResponseTypeDef(TypedDict):
    arn: str,
    creationDateTime: datetime,
    state: SyncJobStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SyncJobStateType](./literals.md#syncjobstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceResponseTypeDef

```python
# CreateWorkspaceResponseTypeDef definition

class CreateWorkspaceResponseTypeDef(TypedDict):
    arn: str,
    creationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteComponentTypeResponseTypeDef

```python
# DeleteComponentTypeResponseTypeDef definition

class DeleteComponentTypeResponseTypeDef(TypedDict):
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEntityResponseTypeDef

```python
# DeleteEntityResponseTypeDef definition

class DeleteEntityResponseTypeDef(TypedDict):
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSyncJobResponseTypeDef

```python
# DeleteSyncJobResponseTypeDef definition

class DeleteSyncJobResponseTypeDef(TypedDict):
    state: SyncJobStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SyncJobStateType](./literals.md#syncjobstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceResponseTypeDef

```python
# DeleteWorkspaceResponseTypeDef definition

class DeleteWorkspaceResponseTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkspaceResponseTypeDef

```python
# GetWorkspaceResponseTypeDef definition

class GetWorkspaceResponseTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    description: str,
    linkedServices: List[str],
    s3Location: str,
    role: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComponentTypeResponseTypeDef

```python
# UpdateComponentTypeResponseTypeDef definition

class UpdateComponentTypeResponseTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    componentTypeId: str,
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEntityResponseTypeDef

```python
# UpdateEntityResponseTypeDef definition

class UpdateEntityResponseTypeDef(TypedDict):
    updateDateTime: datetime,
    state: StateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSceneResponseTypeDef

```python
# UpdateSceneResponseTypeDef definition

class UpdateSceneResponseTypeDef(TypedDict):
    updateDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspaceResponseTypeDef

```python
# UpdateWorkspaceResponseTypeDef definition

class UpdateWorkspaceResponseTypeDef(TypedDict):
    updateDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PricingPlanTypeDef

```python
# PricingPlanTypeDef definition

class PricingPlanTypeDef(TypedDict):
    effectiveDateTime: datetime,
    pricingMode: PricingModeType,  # (2)
    updateDateTime: datetime,
    updateReason: UpdateReasonType,  # (3)
    billableEntityCount: NotRequired[int],
    bundleInformation: NotRequired[BundleInformationTypeDef],  # (1)
```

1. See [:material-code-braces: BundleInformationTypeDef](./type_defs.md#bundleinformationtypedef) 
2. See [:material-code-brackets: PricingModeType](./literals.md#pricingmodetype) 
3. See [:material-code-brackets: UpdateReasonType](./literals.md#updatereasontype) 
## DataConnectorTypeDef

```python
# DataConnectorTypeDef definition

class DataConnectorTypeDef(TypedDict):
    lambda: NotRequired[LambdaFunctionTypeDef],  # (1)
    isNative: NotRequired[bool],
```

1. See [:material-code-braces: LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef) 
## DataValueOutputTypeDef

```python
# DataValueOutputTypeDef definition

class DataValueOutputTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    integerValue: NotRequired[int],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
    listValue: NotRequired[List[Dict[str, Any]]],
    mapValue: NotRequired[Dict[str, Dict[str, Any]]],
    relationshipValue: NotRequired[RelationshipValueTypeDef],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-braces: RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef) 
## DataValueTypeDef

```python
# DataValueTypeDef definition

class DataValueTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    integerValue: NotRequired[int],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
    listValue: NotRequired[Sequence[Mapping[str, Any]]],
    mapValue: NotRequired[Mapping[str, Mapping[str, Any]]],
    relationshipValue: NotRequired[RelationshipValueTypeDef],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-braces: RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    type: DestinationTypeType,  # (1)
    s3Configuration: NotRequired[S3DestinationConfigurationTypeDef],  # (2)
    iotTwinMakerConfiguration: NotRequired[IotTwinMakerDestinationConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
2. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
3. See [:material-code-braces: IotTwinMakerDestinationConfigurationTypeDef](./type_defs.md#iottwinmakerdestinationconfigurationtypedef) 
## MetadataTransferJobStatusTypeDef

```python
# MetadataTransferJobStatusTypeDef definition

class MetadataTransferJobStatusTypeDef(TypedDict):
    state: NotRequired[MetadataTransferJobStateType],  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
    queuedPosition: NotRequired[int],
```

1. See [:material-code-brackets: MetadataTransferJobStateType](./literals.md#metadatatransferjobstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## StatusTypeDef

```python
# StatusTypeDef definition

class StatusTypeDef(TypedDict):
    state: NotRequired[StateType],  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## SyncJobStatusTypeDef

```python
# SyncJobStatusTypeDef definition

class SyncJobStatusTypeDef(TypedDict):
    state: NotRequired[SyncJobStateType],  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: SyncJobStateType](./literals.md#syncjobstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## SyncResourceStatusTypeDef

```python
# SyncResourceStatusTypeDef definition

class SyncResourceStatusTypeDef(TypedDict):
    state: NotRequired[SyncResourceStateType],  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: SyncResourceStateType](./literals.md#syncresourcestatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## ExecuteQueryResponseTypeDef

```python
# ExecuteQueryResponseTypeDef definition

class ExecuteQueryResponseTypeDef(TypedDict):
    columnDescriptions: List[ColumnDescriptionTypeDef],  # (1)
    rows: List[RowTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnDescriptionTypeDef](./type_defs.md#columndescriptiontypedef) 
2. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IotSiteWiseSourceConfigurationFilterTypeDef

```python
# IotSiteWiseSourceConfigurationFilterTypeDef definition

class IotSiteWiseSourceConfigurationFilterTypeDef(TypedDict):
    filterByAssetModel: NotRequired[FilterByAssetModelTypeDef],  # (1)
    filterByAsset: NotRequired[FilterByAssetTypeDef],  # (2)
```

1. See [:material-code-braces: FilterByAssetModelTypeDef](./type_defs.md#filterbyassetmodeltypedef) 
2. See [:material-code-braces: FilterByAssetTypeDef](./type_defs.md#filterbyassettypedef) 
## IotTwinMakerSourceConfigurationFilterTypeDef

```python
# IotTwinMakerSourceConfigurationFilterTypeDef definition

class IotTwinMakerSourceConfigurationFilterTypeDef(TypedDict):
    filterByComponentType: NotRequired[FilterByComponentTypeTypeDef],  # (1)
    filterByEntity: NotRequired[FilterByEntityTypeDef],  # (2)
```

1. See [:material-code-braces: FilterByComponentTypeTypeDef](./type_defs.md#filterbycomponenttypetypedef) 
2. See [:material-code-braces: FilterByEntityTypeDef](./type_defs.md#filterbyentitytypedef) 
## GetSceneResponseTypeDef

```python
# GetSceneResponseTypeDef definition

class GetSceneResponseTypeDef(TypedDict):
    workspaceId: str,
    sceneId: str,
    contentLocation: str,
    arn: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    description: str,
    capabilities: List[str],
    sceneMetadata: Dict[str, str],
    generatedSceneMetadata: Dict[str, str],
    error: SceneErrorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SceneErrorTypeDef](./type_defs.md#sceneerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentTypesRequestRequestTypeDef

```python
# ListComponentTypesRequestRequestTypeDef definition

class ListComponentTypesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    filters: NotRequired[Sequence[ListComponentTypesFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ListComponentTypesFilterTypeDef](./type_defs.md#listcomponenttypesfiltertypedef) 
## ListEntitiesRequestRequestTypeDef

```python
# ListEntitiesRequestRequestTypeDef definition

class ListEntitiesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    filters: NotRequired[Sequence[ListEntitiesFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListEntitiesFilterTypeDef](./type_defs.md#listentitiesfiltertypedef) 
## ListMetadataTransferJobsRequestRequestTypeDef

```python
# ListMetadataTransferJobsRequestRequestTypeDef definition

class ListMetadataTransferJobsRequestRequestTypeDef(TypedDict):
    sourceType: SourceTypeType,  # (1)
    destinationType: DestinationTypeType,  # (2)
    filters: NotRequired[Sequence[ListMetadataTransferJobsFilterTypeDef]],  # (3)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
3. See [:material-code-braces: ListMetadataTransferJobsFilterTypeDef](./type_defs.md#listmetadatatransferjobsfiltertypedef) 
## ListScenesResponseTypeDef

```python
# ListScenesResponseTypeDef definition

class ListScenesResponseTypeDef(TypedDict):
    sceneSummaries: List[SceneSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SceneSummaryTypeDef](./type_defs.md#scenesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSyncResourcesRequestRequestTypeDef

```python
# ListSyncResourcesRequestRequestTypeDef definition

class ListSyncResourcesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    syncSource: str,
    filters: NotRequired[Sequence[SyncResourceFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SyncResourceFilterTypeDef](./type_defs.md#syncresourcefiltertypedef) 
## ListWorkspacesResponseTypeDef

```python
# ListWorkspacesResponseTypeDef definition

class ListWorkspacesResponseTypeDef(TypedDict):
    workspaceSummaries: List[WorkspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPricingPlanResponseTypeDef

```python
# GetPricingPlanResponseTypeDef definition

class GetPricingPlanResponseTypeDef(TypedDict):
    currentPricingPlan: PricingPlanTypeDef,  # (1)
    pendingPricingPlan: PricingPlanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PricingPlanTypeDef](./type_defs.md#pricingplantypedef) 
2. See [:material-code-braces: PricingPlanTypeDef](./type_defs.md#pricingplantypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePricingPlanResponseTypeDef

```python
# UpdatePricingPlanResponseTypeDef definition

class UpdatePricingPlanResponseTypeDef(TypedDict):
    currentPricingPlan: PricingPlanTypeDef,  # (1)
    pendingPricingPlan: PricingPlanTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PricingPlanTypeDef](./type_defs.md#pricingplantypedef) 
2. See [:material-code-braces: PricingPlanTypeDef](./type_defs.md#pricingplantypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionRequestTypeDef

```python
# FunctionRequestTypeDef definition

class FunctionRequestTypeDef(TypedDict):
    requiredProperties: NotRequired[Sequence[str]],
    scope: NotRequired[ScopeType],  # (1)
    implementedBy: NotRequired[DataConnectorTypeDef],  # (2)
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DataConnectorTypeDef](./type_defs.md#dataconnectortypedef) 
## FunctionResponseTypeDef

```python
# FunctionResponseTypeDef definition

class FunctionResponseTypeDef(TypedDict):
    requiredProperties: NotRequired[List[str]],
    scope: NotRequired[ScopeType],  # (1)
    implementedBy: NotRequired[DataConnectorTypeDef],  # (2)
    isInherited: NotRequired[bool],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DataConnectorTypeDef](./type_defs.md#dataconnectortypedef) 
## DataTypeOutputTypeDef

```python
# DataTypeOutputTypeDef definition

class DataTypeOutputTypeDef(TypedDict):
    type: TypeType,  # (1)
    nestedType: NotRequired[Dict[str, Any]],
    allowedValues: NotRequired[List[DataValueOutputTypeDef]],  # (2)
    unitOfMeasure: NotRequired[str],
    relationship: NotRequired[RelationshipTypeDef],  # (3)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
3. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
## PropertyLatestValueTypeDef

```python
# PropertyLatestValueTypeDef definition

class PropertyLatestValueTypeDef(TypedDict):
    propertyReference: EntityPropertyReferenceOutputTypeDef,  # (1)
    propertyValue: NotRequired[DataValueOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## PropertyValueOutputTypeDef

```python
# PropertyValueOutputTypeDef definition

class PropertyValueOutputTypeDef(TypedDict):
    value: DataValueOutputTypeDef,  # (1)
    timestamp: NotRequired[datetime],
    time: NotRequired[str],
```

1. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## CancelMetadataTransferJobResponseTypeDef

```python
# CancelMetadataTransferJobResponseTypeDef definition

class CancelMetadataTransferJobResponseTypeDef(TypedDict):
    metadataTransferJobId: str,
    arn: str,
    updateDateTime: datetime,
    status: MetadataTransferJobStatusTypeDef,  # (1)
    progress: MetadataTransferJobProgressTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef) 
2. See [:material-code-braces: MetadataTransferJobProgressTypeDef](./type_defs.md#metadatatransferjobprogresstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMetadataTransferJobResponseTypeDef

```python
# CreateMetadataTransferJobResponseTypeDef definition

class CreateMetadataTransferJobResponseTypeDef(TypedDict):
    metadataTransferJobId: str,
    arn: str,
    creationDateTime: datetime,
    status: MetadataTransferJobStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetadataTransferJobSummaryTypeDef

```python
# MetadataTransferJobSummaryTypeDef definition

class MetadataTransferJobSummaryTypeDef(TypedDict):
    metadataTransferJobId: str,
    arn: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    status: MetadataTransferJobStatusTypeDef,  # (1)
    progress: NotRequired[MetadataTransferJobProgressTypeDef],  # (2)
```

1. See [:material-code-braces: MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef) 
2. See [:material-code-braces: MetadataTransferJobProgressTypeDef](./type_defs.md#metadatatransferjobprogresstypedef) 
## ComponentSummaryTypeDef

```python
# ComponentSummaryTypeDef definition

class ComponentSummaryTypeDef(TypedDict):
    componentName: str,
    componentTypeId: str,
    status: StatusTypeDef,  # (2)
    definedIn: NotRequired[str],
    description: NotRequired[str],
    propertyGroups: NotRequired[Dict[str, ComponentPropertyGroupResponseTypeDef]],  # (1)
    syncSource: NotRequired[str],
    componentPath: NotRequired[str],
```

1. See [:material-code-braces: ComponentPropertyGroupResponseTypeDef](./type_defs.md#componentpropertygroupresponsetypedef) 
2. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
## ComponentTypeSummaryTypeDef

```python
# ComponentTypeSummaryTypeDef definition

class ComponentTypeSummaryTypeDef(TypedDict):
    arn: str,
    componentTypeId: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    description: NotRequired[str],
    status: NotRequired[StatusTypeDef],  # (1)
    componentTypeName: NotRequired[str],
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
## EntitySummaryTypeDef

```python
# EntitySummaryTypeDef definition

class EntitySummaryTypeDef(TypedDict):
    entityId: str,
    entityName: str,
    arn: str,
    status: StatusTypeDef,  # (1)
    creationDateTime: datetime,
    updateDateTime: datetime,
    parentEntityId: NotRequired[str],
    description: NotRequired[str],
    hasChildEntities: NotRequired[bool],
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
## GetSyncJobResponseTypeDef

```python
# GetSyncJobResponseTypeDef definition

class GetSyncJobResponseTypeDef(TypedDict):
    arn: str,
    workspaceId: str,
    syncSource: str,
    syncRole: str,
    status: SyncJobStatusTypeDef,  # (1)
    creationDateTime: datetime,
    updateDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SyncJobStatusTypeDef](./type_defs.md#syncjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SyncJobSummaryTypeDef

```python
# SyncJobSummaryTypeDef definition

class SyncJobSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    workspaceId: NotRequired[str],
    syncSource: NotRequired[str],
    status: NotRequired[SyncJobStatusTypeDef],  # (1)
    creationDateTime: NotRequired[datetime],
    updateDateTime: NotRequired[datetime],
```

1. See [:material-code-braces: SyncJobStatusTypeDef](./type_defs.md#syncjobstatustypedef) 
## SyncResourceSummaryTypeDef

```python
# SyncResourceSummaryTypeDef definition

class SyncResourceSummaryTypeDef(TypedDict):
    resourceType: NotRequired[SyncResourceTypeType],  # (1)
    externalId: NotRequired[str],
    resourceId: NotRequired[str],
    status: NotRequired[SyncResourceStatusTypeDef],  # (2)
    updateDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SyncResourceTypeType](./literals.md#syncresourcetypetype) 
2. See [:material-code-braces: SyncResourceStatusTypeDef](./type_defs.md#syncresourcestatustypedef) 
## IotSiteWiseSourceConfigurationOutputTypeDef

```python
# IotSiteWiseSourceConfigurationOutputTypeDef definition

class IotSiteWiseSourceConfigurationOutputTypeDef(TypedDict):
    filters: NotRequired[List[IotSiteWiseSourceConfigurationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IotSiteWiseSourceConfigurationFilterTypeDef](./type_defs.md#iotsitewisesourceconfigurationfiltertypedef) 
## IotSiteWiseSourceConfigurationTypeDef

```python
# IotSiteWiseSourceConfigurationTypeDef definition

class IotSiteWiseSourceConfigurationTypeDef(TypedDict):
    filters: NotRequired[Sequence[IotSiteWiseSourceConfigurationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IotSiteWiseSourceConfigurationFilterTypeDef](./type_defs.md#iotsitewisesourceconfigurationfiltertypedef) 
## IotTwinMakerSourceConfigurationOutputTypeDef

```python
# IotTwinMakerSourceConfigurationOutputTypeDef definition

class IotTwinMakerSourceConfigurationOutputTypeDef(TypedDict):
    workspace: str,
    filters: NotRequired[List[IotTwinMakerSourceConfigurationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IotTwinMakerSourceConfigurationFilterTypeDef](./type_defs.md#iottwinmakersourceconfigurationfiltertypedef) 
## IotTwinMakerSourceConfigurationTypeDef

```python
# IotTwinMakerSourceConfigurationTypeDef definition

class IotTwinMakerSourceConfigurationTypeDef(TypedDict):
    workspace: str,
    filters: NotRequired[Sequence[IotTwinMakerSourceConfigurationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IotTwinMakerSourceConfigurationFilterTypeDef](./type_defs.md#iottwinmakersourceconfigurationfiltertypedef) 
## PropertyDefinitionResponseTypeDef

```python
# PropertyDefinitionResponseTypeDef definition

class PropertyDefinitionResponseTypeDef(TypedDict):
    dataType: DataTypeOutputTypeDef,  # (1)
    isTimeSeries: bool,
    isRequiredInEntity: bool,
    isExternalId: bool,
    isStoredExternally: bool,
    isImported: bool,
    isFinal: bool,
    isInherited: bool,
    defaultValue: NotRequired[DataValueOutputTypeDef],  # (2)
    configuration: NotRequired[Dict[str, str]],
    displayName: NotRequired[str],
```

1. See [:material-code-braces: DataTypeOutputTypeDef](./type_defs.md#datatypeoutputtypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## GetPropertyValueResponseTypeDef

```python
# GetPropertyValueResponseTypeDef definition

class GetPropertyValueResponseTypeDef(TypedDict):
    propertyValues: Dict[str, PropertyLatestValueTypeDef],  # (1)
    tabularPropertyValues: List[List[Dict[str, DataValueOutputTypeDef]]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PropertyLatestValueTypeDef](./type_defs.md#propertylatestvaluetypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyValueEntryOutputTypeDef

```python
# PropertyValueEntryOutputTypeDef definition

class PropertyValueEntryOutputTypeDef(TypedDict):
    entityPropertyReference: EntityPropertyReferenceOutputTypeDef,  # (1)
    propertyValues: NotRequired[List[PropertyValueOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef) 
2. See [:material-code-braces: PropertyValueOutputTypeDef](./type_defs.md#propertyvalueoutputtypedef) 
## PropertyValueHistoryTypeDef

```python
# PropertyValueHistoryTypeDef definition

class PropertyValueHistoryTypeDef(TypedDict):
    entityPropertyReference: EntityPropertyReferenceOutputTypeDef,  # (1)
    values: NotRequired[List[PropertyValueOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef) 
2. See [:material-code-braces: PropertyValueOutputTypeDef](./type_defs.md#propertyvalueoutputtypedef) 
## DataTypeTypeDef

```python
# DataTypeTypeDef definition

class DataTypeTypeDef(TypedDict):
    type: TypeType,  # (1)
    nestedType: NotRequired[Mapping[str, Any]],
    allowedValues: NotRequired[Sequence[DataValueUnionTypeDef]],  # (2)
    unitOfMeasure: NotRequired[str],
    relationship: NotRequired[RelationshipTypeDef],  # (3)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
3. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
## PropertyFilterTypeDef

```python
# PropertyFilterTypeDef definition

class PropertyFilterTypeDef(TypedDict):
    propertyName: NotRequired[str],
    operator: NotRequired[str],
    value: NotRequired[DataValueUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## PropertyValueTypeDef

```python
# PropertyValueTypeDef definition

class PropertyValueTypeDef(TypedDict):
    value: DataValueUnionTypeDef,  # (1)
    timestamp: NotRequired[TimestampTypeDef],
    time: NotRequired[str],
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## ListMetadataTransferJobsResponseTypeDef

```python
# ListMetadataTransferJobsResponseTypeDef definition

class ListMetadataTransferJobsResponseTypeDef(TypedDict):
    metadataTransferJobSummaries: List[MetadataTransferJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataTransferJobSummaryTypeDef](./type_defs.md#metadatatransferjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentsResponseTypeDef

```python
# ListComponentsResponseTypeDef definition

class ListComponentsResponseTypeDef(TypedDict):
    componentSummaries: List[ComponentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentTypesResponseTypeDef

```python
# ListComponentTypesResponseTypeDef definition

class ListComponentTypesResponseTypeDef(TypedDict):
    workspaceId: str,
    componentTypeSummaries: List[ComponentTypeSummaryTypeDef],  # (1)
    maxResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ComponentTypeSummaryTypeDef](./type_defs.md#componenttypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitiesResponseTypeDef

```python
# ListEntitiesResponseTypeDef definition

class ListEntitiesResponseTypeDef(TypedDict):
    entitySummaries: List[EntitySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSyncJobsResponseTypeDef

```python
# ListSyncJobsResponseTypeDef definition

class ListSyncJobsResponseTypeDef(TypedDict):
    syncJobSummaries: List[SyncJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SyncJobSummaryTypeDef](./type_defs.md#syncjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSyncResourcesResponseTypeDef

```python
# ListSyncResourcesResponseTypeDef definition

class ListSyncResourcesResponseTypeDef(TypedDict):
    syncResources: List[SyncResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SyncResourceSummaryTypeDef](./type_defs.md#syncresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceConfigurationOutputTypeDef

```python
# SourceConfigurationOutputTypeDef definition

class SourceConfigurationOutputTypeDef(TypedDict):
    type: SourceTypeType,  # (1)
    s3Configuration: NotRequired[S3SourceConfigurationTypeDef],  # (2)
    iotSiteWiseConfiguration: NotRequired[IotSiteWiseSourceConfigurationOutputTypeDef],  # (3)
    iotTwinMakerConfiguration: NotRequired[IotTwinMakerSourceConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: S3SourceConfigurationTypeDef](./type_defs.md#s3sourceconfigurationtypedef) 
3. See [:material-code-braces: IotSiteWiseSourceConfigurationOutputTypeDef](./type_defs.md#iotsitewisesourceconfigurationoutputtypedef) 
4. See [:material-code-braces: IotTwinMakerSourceConfigurationOutputTypeDef](./type_defs.md#iottwinmakersourceconfigurationoutputtypedef) 
## GetComponentTypeResponseTypeDef

```python
# GetComponentTypeResponseTypeDef definition

class GetComponentTypeResponseTypeDef(TypedDict):
    workspaceId: str,
    isSingleton: bool,
    componentTypeId: str,
    description: str,
    propertyDefinitions: Dict[str, PropertyDefinitionResponseTypeDef],  # (1)
    extendsFrom: List[str],
    functions: Dict[str, FunctionResponseTypeDef],  # (2)
    creationDateTime: datetime,
    updateDateTime: datetime,
    arn: str,
    isAbstract: bool,
    isSchemaInitialized: bool,
    status: StatusTypeDef,  # (3)
    propertyGroups: Dict[str, PropertyGroupResponseTypeDef],  # (4)
    syncSource: str,
    componentTypeName: str,
    compositeComponentTypes: Dict[str, CompositeComponentTypeResponseTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef) 
2. See [:material-code-braces: FunctionResponseTypeDef](./type_defs.md#functionresponsetypedef) 
3. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
4. See [:material-code-braces: PropertyGroupResponseTypeDef](./type_defs.md#propertygroupresponsetypedef) 
5. See [:material-code-braces: CompositeComponentTypeResponseTypeDef](./type_defs.md#compositecomponenttyperesponsetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyResponseTypeDef

```python
# PropertyResponseTypeDef definition

class PropertyResponseTypeDef(TypedDict):
    definition: NotRequired[PropertyDefinitionResponseTypeDef],  # (1)
    value: NotRequired[DataValueOutputTypeDef],  # (2)
    areAllPropertyValuesReturned: NotRequired[bool],
```

1. See [:material-code-braces: PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## PropertySummaryTypeDef

```python
# PropertySummaryTypeDef definition

class PropertySummaryTypeDef(TypedDict):
    propertyName: str,
    definition: NotRequired[PropertyDefinitionResponseTypeDef],  # (1)
    value: NotRequired[DataValueOutputTypeDef],  # (2)
    areAllPropertyValuesReturned: NotRequired[bool],
```

1. See [:material-code-braces: PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef) 
2. See [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## BatchPutPropertyErrorTypeDef

```python
# BatchPutPropertyErrorTypeDef definition

class BatchPutPropertyErrorTypeDef(TypedDict):
    errorCode: str,
    errorMessage: str,
    entry: PropertyValueEntryOutputTypeDef,  # (1)
```

1. See [:material-code-braces: PropertyValueEntryOutputTypeDef](./type_defs.md#propertyvalueentryoutputtypedef) 
## GetPropertyValueHistoryResponseTypeDef

```python
# GetPropertyValueHistoryResponseTypeDef definition

class GetPropertyValueHistoryResponseTypeDef(TypedDict):
    propertyValues: List[PropertyValueHistoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PropertyValueHistoryTypeDef](./type_defs.md#propertyvaluehistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPropertyValueHistoryRequestRequestTypeDef

```python
# GetPropertyValueHistoryRequestRequestTypeDef definition

class GetPropertyValueHistoryRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    selectedProperties: Sequence[str],
    entityId: NotRequired[str],
    componentName: NotRequired[str],
    componentPath: NotRequired[str],
    componentTypeId: NotRequired[str],
    propertyFilters: NotRequired[Sequence[PropertyFilterTypeDef]],  # (1)
    startDateTime: NotRequired[TimestampTypeDef],
    endDateTime: NotRequired[TimestampTypeDef],
    interpolation: NotRequired[InterpolationParametersTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    orderByTime: NotRequired[OrderByTimeType],  # (3)
    startTime: NotRequired[str],
    endTime: NotRequired[str],
```

1. See [:material-code-braces: PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef) 
2. See [:material-code-braces: InterpolationParametersTypeDef](./type_defs.md#interpolationparameterstypedef) 
3. See [:material-code-brackets: OrderByTimeType](./literals.md#orderbytimetype) 
## TabularConditionsTypeDef

```python
# TabularConditionsTypeDef definition

class TabularConditionsTypeDef(TypedDict):
    orderBy: NotRequired[Sequence[OrderByTypeDef]],  # (1)
    propertyFilters: NotRequired[Sequence[PropertyFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
2. See [:material-code-braces: PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef) 
## GetMetadataTransferJobResponseTypeDef

```python
# GetMetadataTransferJobResponseTypeDef definition

class GetMetadataTransferJobResponseTypeDef(TypedDict):
    metadataTransferJobId: str,
    arn: str,
    description: str,
    sources: List[SourceConfigurationOutputTypeDef],  # (1)
    destination: DestinationConfigurationTypeDef,  # (2)
    metadataTransferJobRole: str,
    reportUrl: str,
    creationDateTime: datetime,
    updateDateTime: datetime,
    status: MetadataTransferJobStatusTypeDef,  # (3)
    progress: MetadataTransferJobProgressTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
3. See [:material-code-braces: MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef) 
4. See [:material-code-braces: MetadataTransferJobProgressTypeDef](./type_defs.md#metadatatransferjobprogresstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceConfigurationTypeDef

```python
# SourceConfigurationTypeDef definition

class SourceConfigurationTypeDef(TypedDict):
    type: SourceTypeType,  # (1)
    s3Configuration: NotRequired[S3SourceConfigurationTypeDef],  # (2)
    iotSiteWiseConfiguration: NotRequired[IotSiteWiseSourceConfigurationUnionTypeDef],  # (3)
    iotTwinMakerConfiguration: NotRequired[IotTwinMakerSourceConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: S3SourceConfigurationTypeDef](./type_defs.md#s3sourceconfigurationtypedef) 
3. See [:material-code-braces: IotSiteWiseSourceConfigurationTypeDef](./type_defs.md#iotsitewisesourceconfigurationtypedef) [:material-code-braces: IotSiteWiseSourceConfigurationOutputTypeDef](./type_defs.md#iotsitewisesourceconfigurationoutputtypedef) 
4. See [:material-code-braces: IotTwinMakerSourceConfigurationTypeDef](./type_defs.md#iottwinmakersourceconfigurationtypedef) [:material-code-braces: IotTwinMakerSourceConfigurationOutputTypeDef](./type_defs.md#iottwinmakersourceconfigurationoutputtypedef) 
## ComponentResponseTypeDef

```python
# ComponentResponseTypeDef definition

class ComponentResponseTypeDef(TypedDict):
    componentName: NotRequired[str],
    description: NotRequired[str],
    componentTypeId: NotRequired[str],
    status: NotRequired[StatusTypeDef],  # (1)
    definedIn: NotRequired[str],
    properties: NotRequired[Dict[str, PropertyResponseTypeDef]],  # (2)
    propertyGroups: NotRequired[Dict[str, ComponentPropertyGroupResponseTypeDef]],  # (3)
    syncSource: NotRequired[str],
    areAllPropertiesReturned: NotRequired[bool],
    compositeComponents: NotRequired[Dict[str, ComponentSummaryTypeDef]],  # (4)
    areAllCompositeComponentsReturned: NotRequired[bool],
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
2. See [:material-code-braces: PropertyResponseTypeDef](./type_defs.md#propertyresponsetypedef) 
3. See [:material-code-braces: ComponentPropertyGroupResponseTypeDef](./type_defs.md#componentpropertygroupresponsetypedef) 
4. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
## ListPropertiesResponseTypeDef

```python
# ListPropertiesResponseTypeDef definition

class ListPropertiesResponseTypeDef(TypedDict):
    propertySummaries: List[PropertySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PropertySummaryTypeDef](./type_defs.md#propertysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutPropertyErrorEntryTypeDef

```python
# BatchPutPropertyErrorEntryTypeDef definition

class BatchPutPropertyErrorEntryTypeDef(TypedDict):
    errors: List[BatchPutPropertyErrorTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutPropertyErrorTypeDef](./type_defs.md#batchputpropertyerrortypedef) 
## PropertyDefinitionRequestTypeDef

```python
# PropertyDefinitionRequestTypeDef definition

class PropertyDefinitionRequestTypeDef(TypedDict):
    dataType: NotRequired[DataTypeUnionTypeDef],  # (1)
    isRequiredInEntity: NotRequired[bool],
    isExternalId: NotRequired[bool],
    isStoredExternally: NotRequired[bool],
    isTimeSeries: NotRequired[bool],
    defaultValue: NotRequired[DataValueUnionTypeDef],  # (2)
    configuration: NotRequired[Mapping[str, str]],
    displayName: NotRequired[str],
```

1. See [:material-code-braces: DataTypeTypeDef](./type_defs.md#datatypetypedef) [:material-code-braces: DataTypeOutputTypeDef](./type_defs.md#datatypeoutputtypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
## GetPropertyValueRequestRequestTypeDef

```python
# GetPropertyValueRequestRequestTypeDef definition

class GetPropertyValueRequestRequestTypeDef(TypedDict):
    selectedProperties: Sequence[str],
    workspaceId: str,
    componentName: NotRequired[str],
    componentPath: NotRequired[str],
    componentTypeId: NotRequired[str],
    entityId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    propertyGroupName: NotRequired[str],
    tabularConditions: NotRequired[TabularConditionsTypeDef],  # (1)
```

1. See [:material-code-braces: TabularConditionsTypeDef](./type_defs.md#tabularconditionstypedef) 
## PropertyValueEntryTypeDef

```python
# PropertyValueEntryTypeDef definition

class PropertyValueEntryTypeDef(TypedDict):
    entityPropertyReference: EntityPropertyReferenceUnionTypeDef,  # (1)
    propertyValues: NotRequired[Sequence[PropertyValueUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef) [:material-code-braces: EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef) 
2. See [:material-code-braces: PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef) [:material-code-braces: PropertyValueOutputTypeDef](./type_defs.md#propertyvalueoutputtypedef) 
## GetEntityResponseTypeDef

```python
# GetEntityResponseTypeDef definition

class GetEntityResponseTypeDef(TypedDict):
    entityId: str,
    entityName: str,
    arn: str,
    status: StatusTypeDef,  # (1)
    workspaceId: str,
    description: str,
    components: Dict[str, ComponentResponseTypeDef],  # (2)
    parentEntityId: str,
    hasChildEntities: bool,
    creationDateTime: datetime,
    updateDateTime: datetime,
    syncSource: str,
    areAllComponentsReturned: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
2. See [:material-code-braces: ComponentResponseTypeDef](./type_defs.md#componentresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutPropertyValuesResponseTypeDef

```python
# BatchPutPropertyValuesResponseTypeDef definition

class BatchPutPropertyValuesResponseTypeDef(TypedDict):
    errorEntries: List[BatchPutPropertyErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutPropertyErrorEntryTypeDef](./type_defs.md#batchputpropertyerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComponentTypeRequestRequestTypeDef

```python
# CreateComponentTypeRequestRequestTypeDef definition

class CreateComponentTypeRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    componentTypeId: str,
    isSingleton: NotRequired[bool],
    description: NotRequired[str],
    propertyDefinitions: NotRequired[Mapping[str, PropertyDefinitionRequestTypeDef]],  # (1)
    extendsFrom: NotRequired[Sequence[str]],
    functions: NotRequired[Mapping[str, FunctionRequestTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
    propertyGroups: NotRequired[Mapping[str, PropertyGroupRequestTypeDef]],  # (3)
    componentTypeName: NotRequired[str],
    compositeComponentTypes: NotRequired[Mapping[str, CompositeComponentTypeRequestTypeDef]],  # (4)
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
4. See [:material-code-braces: CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef) 
## PropertyRequestTypeDef

```python
# PropertyRequestTypeDef definition

class PropertyRequestTypeDef(TypedDict):
    definition: NotRequired[PropertyDefinitionRequestTypeDef],  # (1)
    value: NotRequired[DataValueUnionTypeDef],  # (2)
    updateType: NotRequired[PropertyUpdateTypeType],  # (3)
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) [:material-code-braces: DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef) 
3. See [:material-code-brackets: PropertyUpdateTypeType](./literals.md#propertyupdatetypetype) 
## UpdateComponentTypeRequestRequestTypeDef

```python
# UpdateComponentTypeRequestRequestTypeDef definition

class UpdateComponentTypeRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    componentTypeId: str,
    isSingleton: NotRequired[bool],
    description: NotRequired[str],
    propertyDefinitions: NotRequired[Mapping[str, PropertyDefinitionRequestTypeDef]],  # (1)
    extendsFrom: NotRequired[Sequence[str]],
    functions: NotRequired[Mapping[str, FunctionRequestTypeDef]],  # (2)
    propertyGroups: NotRequired[Mapping[str, PropertyGroupRequestTypeDef]],  # (3)
    componentTypeName: NotRequired[str],
    compositeComponentTypes: NotRequired[Mapping[str, CompositeComponentTypeRequestTypeDef]],  # (4)
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
4. See [:material-code-braces: CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef) 
## CreateMetadataTransferJobRequestRequestTypeDef

```python
# CreateMetadataTransferJobRequestRequestTypeDef definition

class CreateMetadataTransferJobRequestRequestTypeDef(TypedDict):
    sources: Sequence[SourceConfigurationUnionTypeDef],  # (1)
    destination: DestinationConfigurationTypeDef,  # (2)
    metadataTransferJobId: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) [:material-code-braces: SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
## ComponentRequestTypeDef

```python
# ComponentRequestTypeDef definition

class ComponentRequestTypeDef(TypedDict):
    description: NotRequired[str],
    componentTypeId: NotRequired[str],
    properties: NotRequired[Mapping[str, PropertyRequestTypeDef]],  # (1)
    propertyGroups: NotRequired[Mapping[str, ComponentPropertyGroupRequestTypeDef]],  # (2)
```

1. See [:material-code-braces: PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef) 
2. See [:material-code-braces: ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef) 
## ComponentUpdateRequestTypeDef

```python
# ComponentUpdateRequestTypeDef definition

class ComponentUpdateRequestTypeDef(TypedDict):
    updateType: NotRequired[ComponentUpdateTypeType],  # (1)
    description: NotRequired[str],
    componentTypeId: NotRequired[str],
    propertyUpdates: NotRequired[Mapping[str, PropertyRequestTypeDef]],  # (2)
    propertyGroupUpdates: NotRequired[Mapping[str, ComponentPropertyGroupRequestTypeDef]],  # (3)
```

1. See [:material-code-brackets: ComponentUpdateTypeType](./literals.md#componentupdatetypetype) 
2. See [:material-code-braces: PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef) 
3. See [:material-code-braces: ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef) 
## CompositeComponentRequestTypeDef

```python
# CompositeComponentRequestTypeDef definition

class CompositeComponentRequestTypeDef(TypedDict):
    description: NotRequired[str],
    properties: NotRequired[Mapping[str, PropertyRequestTypeDef]],  # (1)
    propertyGroups: NotRequired[Mapping[str, ComponentPropertyGroupRequestTypeDef]],  # (2)
```

1. See [:material-code-braces: PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef) 
2. See [:material-code-braces: ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef) 
## CompositeComponentUpdateRequestTypeDef

```python
# CompositeComponentUpdateRequestTypeDef definition

class CompositeComponentUpdateRequestTypeDef(TypedDict):
    updateType: NotRequired[ComponentUpdateTypeType],  # (1)
    description: NotRequired[str],
    propertyUpdates: NotRequired[Mapping[str, PropertyRequestTypeDef]],  # (2)
    propertyGroupUpdates: NotRequired[Mapping[str, ComponentPropertyGroupRequestTypeDef]],  # (3)
```

1. See [:material-code-brackets: ComponentUpdateTypeType](./literals.md#componentupdatetypetype) 
2. See [:material-code-braces: PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef) 
3. See [:material-code-braces: ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef) 
## BatchPutPropertyValuesRequestRequestTypeDef

```python
# BatchPutPropertyValuesRequestRequestTypeDef definition

class BatchPutPropertyValuesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entries: Sequence[PropertyValueEntryUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef) [:material-code-braces: PropertyValueEntryOutputTypeDef](./type_defs.md#propertyvalueentryoutputtypedef) 
## CreateEntityRequestRequestTypeDef

```python
# CreateEntityRequestRequestTypeDef definition

class CreateEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityName: str,
    entityId: NotRequired[str],
    description: NotRequired[str],
    components: NotRequired[Mapping[str, ComponentRequestTypeDef]],  # (1)
    compositeComponents: NotRequired[Mapping[str, CompositeComponentRequestTypeDef]],  # (2)
    parentEntityId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef) 
2. See [:material-code-braces: CompositeComponentRequestTypeDef](./type_defs.md#compositecomponentrequesttypedef) 
## UpdateEntityRequestRequestTypeDef

```python
# UpdateEntityRequestRequestTypeDef definition

class UpdateEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
    entityName: NotRequired[str],
    description: NotRequired[str],
    componentUpdates: NotRequired[Mapping[str, ComponentUpdateRequestTypeDef]],  # (1)
    compositeComponentUpdates: NotRequired[Mapping[str, CompositeComponentUpdateRequestTypeDef]],  # (2)
    parentEntityUpdate: NotRequired[ParentEntityUpdateRequestTypeDef],  # (3)
```

1. See [:material-code-braces: ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef) 
2. See [:material-code-braces: CompositeComponentUpdateRequestTypeDef](./type_defs.md#compositecomponentupdaterequesttypedef) 
3. See [:material-code-braces: ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef) 
