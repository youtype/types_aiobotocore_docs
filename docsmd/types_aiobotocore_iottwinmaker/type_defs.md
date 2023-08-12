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

## BundleInformationTypeDef

```python
# BundleInformationTypeDef definition

class BundleInformationTypeDef(TypedDict):
    bundleNames: List[str],
    pricingTier: NotRequired[PricingTierType],  # (1)
```

1. See [:material-code-brackets: PricingTierType](./literals.md#pricingtiertype) 
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
## PropertyDefinitionRequestTypeDef

```python
# PropertyDefinitionRequestTypeDef definition

class PropertyDefinitionRequestTypeDef(TypedDict):
    dataType: NotRequired[DataTypeTypeDef],  # (1)
    isRequiredInEntity: NotRequired[bool],
    isExternalId: NotRequired[bool],
    isStoredExternally: NotRequired[bool],
    isTimeSeries: NotRequired[bool],
    defaultValue: NotRequired[DataValueTypeDef],  # (2)
    configuration: NotRequired[Mapping[str, str]],
    displayName: NotRequired[str],
```

1. See [:material-code-braces: DataTypeTypeDef](./type_defs.md#datatypetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
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
    s3Location: str,
    role: str,
    description: NotRequired[str],
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

## EntityPropertyReferenceTypeDef

```python
# EntityPropertyReferenceTypeDef definition

class EntityPropertyReferenceTypeDef(TypedDict):
    propertyName: str,
    componentName: NotRequired[str],
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

## GetComponentTypeRequestRequestTypeDef

```python
# GetComponentTypeRequestRequestTypeDef definition

class GetComponentTypeRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    componentTypeId: str,
```

## PropertyDefinitionResponseTypeDef

```python
# PropertyDefinitionResponseTypeDef definition

class PropertyDefinitionResponseTypeDef(TypedDict):
    dataType: DataTypeTypeDef,  # (1)
    isTimeSeries: bool,
    isRequiredInEntity: bool,
    isExternalId: bool,
    isStoredExternally: bool,
    isImported: bool,
    isFinal: bool,
    isInherited: bool,
    defaultValue: NotRequired[DataValueTypeDef],  # (2)
    configuration: NotRequired[Dict[str, str]],
    displayName: NotRequired[str],
```

1. See [:material-code-braces: DataTypeTypeDef](./type_defs.md#datatypetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
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

## InterpolationParametersTypeDef

```python
# InterpolationParametersTypeDef definition

class InterpolationParametersTypeDef(TypedDict):
    interpolationType: NotRequired[InterpolationTypeType],  # (1)
    intervalInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: InterpolationTypeType](./literals.md#interpolationtypetype) 
## PropertyFilterTypeDef

```python
# PropertyFilterTypeDef definition

class PropertyFilterTypeDef(TypedDict):
    propertyName: NotRequired[str],
    operator: NotRequired[str],
    value: NotRequired[DataValueTypeDef],  # (1)
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
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

## ListEntitiesFilterTypeDef

```python
# ListEntitiesFilterTypeDef definition

class ListEntitiesFilterTypeDef(TypedDict):
    parentEntityId: NotRequired[str],
    componentTypeId: NotRequired[str],
    externalId: NotRequired[str],
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
## GetWorkspaceResponseTypeDef

```python
# GetWorkspaceResponseTypeDef definition

class GetWorkspaceResponseTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    description: str,
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
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
## PropertyRequestTypeDef

```python
# PropertyRequestTypeDef definition

class PropertyRequestTypeDef(TypedDict):
    definition: NotRequired[PropertyDefinitionRequestTypeDef],  # (1)
    value: NotRequired[DataValueTypeDef],  # (2)
    updateType: NotRequired[PropertyUpdateTypeType],  # (3)
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
3. See [:material-code-brackets: PropertyUpdateTypeType](./literals.md#propertyupdatetypetype) 
## DataConnectorTypeDef

```python
# DataConnectorTypeDef definition

class DataConnectorTypeDef(TypedDict):
    lambda: NotRequired[LambdaFunctionTypeDef],  # (1)
    isNative: NotRequired[bool],
```

1. See [:material-code-braces: LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef) 
## DataTypeTypeDef

```python
# DataTypeTypeDef definition

class DataTypeTypeDef(TypedDict):
    type: TypeType,  # (1)
    nestedType: NotRequired[DataTypeTypeDef],  # (2)
    allowedValues: NotRequired[Sequence[DataValueTypeDef]],  # (3)
    unitOfMeasure: NotRequired[str],
    relationship: NotRequired[RelationshipTypeDef],  # (4)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: DataTypeTypeDef](./type_defs.md#datatypetypedef) 
3. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
4. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
## DataValueTypeDef

```python
# DataValueTypeDef definition

class DataValueTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    integerValue: NotRequired[int],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
    listValue: NotRequired[Sequence[DataValueTypeDef]],  # (1)
    mapValue: NotRequired[Mapping[str, DataValueTypeDef]],  # (2)
    relationshipValue: NotRequired[RelationshipValueTypeDef],  # (3)
    expression: NotRequired[str],
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
3. See [:material-code-braces: RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef) 
## PropertyLatestValueTypeDef

```python
# PropertyLatestValueTypeDef definition

class PropertyLatestValueTypeDef(TypedDict):
    propertyReference: EntityPropertyReferenceTypeDef,  # (1)
    propertyValue: NotRequired[DataValueTypeDef],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ColumnDescriptionTypeDef](./type_defs.md#columndescriptiontypedef) 
2. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyResponseTypeDef

```python
# PropertyResponseTypeDef definition

class PropertyResponseTypeDef(TypedDict):
    definition: NotRequired[PropertyDefinitionResponseTypeDef],  # (1)
    value: NotRequired[DataValueTypeDef],  # (2)
```

1. See [:material-code-braces: PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
## GetPropertyValueHistoryRequestRequestTypeDef

```python
# GetPropertyValueHistoryRequestRequestTypeDef definition

class GetPropertyValueHistoryRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    selectedProperties: Sequence[str],
    entityId: NotRequired[str],
    componentName: NotRequired[str],
    componentTypeId: NotRequired[str],
    propertyFilters: NotRequired[Sequence[PropertyFilterTypeDef]],  # (1)
    startDateTime: NotRequired[Union[datetime, str]],
    endDateTime: NotRequired[Union[datetime, str]],
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
## PropertyValueTypeDef

```python
# PropertyValueTypeDef definition

class PropertyValueTypeDef(TypedDict):
    value: DataValueTypeDef,  # (1)
    timestamp: NotRequired[Union[datetime, str]],
    time: NotRequired[str],
```

1. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
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
## ListScenesResponseTypeDef

```python
# ListScenesResponseTypeDef definition

class ListScenesResponseTypeDef(TypedDict):
    sceneSummaries: List[SceneSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TabularConditionsTypeDef

```python
# TabularConditionsTypeDef definition

class TabularConditionsTypeDef(TypedDict):
    orderBy: NotRequired[Sequence[OrderByTypeDef]],  # (1)
    propertyFilters: NotRequired[Sequence[PropertyFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
2. See [:material-code-braces: PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef) 
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
## GetPropertyValueResponseTypeDef

```python
# GetPropertyValueResponseTypeDef definition

class GetPropertyValueResponseTypeDef(TypedDict):
    propertyValues: Dict[str, PropertyLatestValueTypeDef],  # (1)
    nextToken: str,
    tabularPropertyValues: List[List[Dict[str, DataValueTypeDef]]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PropertyLatestValueTypeDef](./type_defs.md#propertylatestvaluetypedef) 
2. See [:material-code-braces: DataValueTypeDef](./type_defs.md#datavaluetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
2. See [:material-code-braces: PropertyResponseTypeDef](./type_defs.md#propertyresponsetypedef) 
3. See [:material-code-braces: ComponentPropertyGroupResponseTypeDef](./type_defs.md#componentpropertygroupresponsetypedef) 
## PropertyValueEntryTypeDef

```python
# PropertyValueEntryTypeDef definition

class PropertyValueEntryTypeDef(TypedDict):
    entityPropertyReference: EntityPropertyReferenceTypeDef,  # (1)
    propertyValues: NotRequired[Sequence[PropertyValueTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef) 
2. See [:material-code-braces: PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef) 
## PropertyValueHistoryTypeDef

```python
# PropertyValueHistoryTypeDef definition

class PropertyValueHistoryTypeDef(TypedDict):
    entityPropertyReference: EntityPropertyReferenceTypeDef,  # (1)
    values: NotRequired[List[PropertyValueTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef) 
2. See [:material-code-braces: PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef) 
## GetPropertyValueRequestRequestTypeDef

```python
# GetPropertyValueRequestRequestTypeDef definition

class GetPropertyValueRequestRequestTypeDef(TypedDict):
    selectedProperties: Sequence[str],
    workspaceId: str,
    componentName: NotRequired[str],
    componentTypeId: NotRequired[str],
    entityId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    propertyGroupName: NotRequired[str],
    tabularConditions: NotRequired[TabularConditionsTypeDef],  # (1)
```

1. See [:material-code-braces: TabularConditionsTypeDef](./type_defs.md#tabularconditionstypedef) 
## CreateEntityRequestRequestTypeDef

```python
# CreateEntityRequestRequestTypeDef definition

class CreateEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityName: str,
    entityId: NotRequired[str],
    description: NotRequired[str],
    components: NotRequired[Mapping[str, ComponentRequestTypeDef]],  # (1)
    parentEntityId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef) 
## UpdateEntityRequestRequestTypeDef

```python
# UpdateEntityRequestRequestTypeDef definition

class UpdateEntityRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entityId: str,
    entityName: NotRequired[str],
    description: NotRequired[str],
    componentUpdates: NotRequired[Mapping[str, ComponentUpdateRequestTypeDef]],  # (1)
    parentEntityUpdate: NotRequired[ParentEntityUpdateRequestTypeDef],  # (2)
```

1. See [:material-code-braces: ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef) 
2. See [:material-code-braces: ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef) 
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
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
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
```

1. See [:material-code-braces: PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef) 
2. See [:material-code-braces: FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef) 
3. See [:material-code-braces: PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef) 
2. See [:material-code-braces: FunctionResponseTypeDef](./type_defs.md#functionresponsetypedef) 
3. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
4. See [:material-code-braces: PropertyGroupResponseTypeDef](./type_defs.md#propertygroupresponsetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentTypesResponseTypeDef

```python
# ListComponentTypesResponseTypeDef definition

class ListComponentTypesResponseTypeDef(TypedDict):
    workspaceId: str,
    componentTypeSummaries: List[ComponentTypeSummaryTypeDef],  # (1)
    nextToken: str,
    maxResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeSummaryTypeDef](./type_defs.md#componenttypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitiesResponseTypeDef

```python
# ListEntitiesResponseTypeDef definition

class ListEntitiesResponseTypeDef(TypedDict):
    entitySummaries: List[EntitySummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSyncJobsResponseTypeDef

```python
# ListSyncJobsResponseTypeDef definition

class ListSyncJobsResponseTypeDef(TypedDict):
    syncJobSummaries: List[SyncJobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SyncJobSummaryTypeDef](./type_defs.md#syncjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSyncResourcesResponseTypeDef

```python
# ListSyncResourcesResponseTypeDef definition

class ListSyncResourcesResponseTypeDef(TypedDict):
    syncResources: List[SyncResourceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SyncResourceSummaryTypeDef](./type_defs.md#syncresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
2. See [:material-code-braces: ComponentResponseTypeDef](./type_defs.md#componentresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutPropertyErrorTypeDef

```python
# BatchPutPropertyErrorTypeDef definition

class BatchPutPropertyErrorTypeDef(TypedDict):
    errorCode: str,
    errorMessage: str,
    entry: PropertyValueEntryTypeDef,  # (1)
```

1. See [:material-code-braces: PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef) 
## BatchPutPropertyValuesRequestRequestTypeDef

```python
# BatchPutPropertyValuesRequestRequestTypeDef definition

class BatchPutPropertyValuesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    entries: Sequence[PropertyValueEntryTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef) 
## GetPropertyValueHistoryResponseTypeDef

```python
# GetPropertyValueHistoryResponseTypeDef definition

class GetPropertyValueHistoryResponseTypeDef(TypedDict):
    propertyValues: List[PropertyValueHistoryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PropertyValueHistoryTypeDef](./type_defs.md#propertyvaluehistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutPropertyErrorEntryTypeDef

```python
# BatchPutPropertyErrorEntryTypeDef definition

class BatchPutPropertyErrorEntryTypeDef(TypedDict):
    errors: List[BatchPutPropertyErrorTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutPropertyErrorTypeDef](./type_defs.md#batchputpropertyerrortypedef) 
## BatchPutPropertyValuesResponseTypeDef

```python
# BatchPutPropertyValuesResponseTypeDef definition

class BatchPutPropertyValuesResponseTypeDef(TypedDict):
    errorEntries: List[BatchPutPropertyErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutPropertyErrorEntryTypeDef](./type_defs.md#batchputpropertyerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
