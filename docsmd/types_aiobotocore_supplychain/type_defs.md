# Type definitions

> [Index](../README.md) > [SupplyChain](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BillOfMaterialsImportJobTypeDef

```python
# BillOfMaterialsImportJobTypeDef definition

class BillOfMaterialsImportJobTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
    status: ConfigurationJobStatusType,  # (1)
    s3uri: str,
    message: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationJobStatusType](./literals.md#configurationjobstatustype) 
## CreateBillOfMaterialsImportJobRequestRequestTypeDef

```python
# CreateBillOfMaterialsImportJobRequestRequestTypeDef definition

class CreateBillOfMaterialsImportJobRequestRequestTypeDef(TypedDict):
    instanceId: str,
    s3uri: str,
    clientToken: NotRequired[str],
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

## CreateInstanceRequestRequestTypeDef

```python
# CreateInstanceRequestRequestTypeDef definition

class CreateInstanceRequestRequestTypeDef(TypedDict):
    instanceName: NotRequired[str],
    instanceDescription: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    webAppDnsDomain: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    instanceId: str,
    awsAccountId: str,
    state: InstanceStateType,  # (1)
    errorMessage: NotRequired[str],
    webAppDnsDomain: NotRequired[str],
    createdTime: NotRequired[datetime],
    lastModifiedTime: NotRequired[datetime],
    instanceName: NotRequired[str],
    instanceDescription: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    versionNumber: NotRequired[float],
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## DataIntegrationFlowDatasetOptionsTypeDef

```python
# DataIntegrationFlowDatasetOptionsTypeDef definition

class DataIntegrationFlowDatasetOptionsTypeDef(TypedDict):
    loadType: NotRequired[DataIntegrationFlowLoadTypeType],  # (1)
    dedupeRecords: NotRequired[bool],
```

1. See [:material-code-brackets: DataIntegrationFlowLoadTypeType](./literals.md#dataintegrationflowloadtypetype) 
## DataIntegrationFlowS3OptionsTypeDef

```python
# DataIntegrationFlowS3OptionsTypeDef definition

class DataIntegrationFlowS3OptionsTypeDef(TypedDict):
    fileType: NotRequired[DataIntegrationFlowFileTypeType],  # (1)
```

1. See [:material-code-brackets: DataIntegrationFlowFileTypeType](./literals.md#dataintegrationflowfiletypetype) 
## DataIntegrationFlowSQLTransformationConfigurationTypeDef

```python
# DataIntegrationFlowSQLTransformationConfigurationTypeDef definition

class DataIntegrationFlowSQLTransformationConfigurationTypeDef(TypedDict):
    query: str,
```

## DataLakeDatasetSchemaFieldTypeDef

```python
# DataLakeDatasetSchemaFieldTypeDef definition

class DataLakeDatasetSchemaFieldTypeDef(TypedDict):
    name: str,
    type: DataLakeDatasetSchemaFieldTypeType,  # (1)
    isRequired: bool,
```

1. See [:material-code-brackets: DataLakeDatasetSchemaFieldTypeType](./literals.md#datalakedatasetschemafieldtypetype) 
## DeleteDataIntegrationFlowRequestRequestTypeDef

```python
# DeleteDataIntegrationFlowRequestRequestTypeDef definition

class DeleteDataIntegrationFlowRequestRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
```

## DeleteDataLakeDatasetRequestRequestTypeDef

```python
# DeleteDataLakeDatasetRequestRequestTypeDef definition

class DeleteDataLakeDatasetRequestRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
```

## DeleteInstanceRequestRequestTypeDef

```python
# DeleteInstanceRequestRequestTypeDef definition

class DeleteInstanceRequestRequestTypeDef(TypedDict):
    instanceId: str,
```

## GetBillOfMaterialsImportJobRequestRequestTypeDef

```python
# GetBillOfMaterialsImportJobRequestRequestTypeDef definition

class GetBillOfMaterialsImportJobRequestRequestTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
```

## GetDataIntegrationFlowRequestRequestTypeDef

```python
# GetDataIntegrationFlowRequestRequestTypeDef definition

class GetDataIntegrationFlowRequestRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
```

## GetDataLakeDatasetRequestRequestTypeDef

```python
# GetDataLakeDatasetRequestRequestTypeDef definition

class GetDataLakeDatasetRequestRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
```

## GetInstanceRequestRequestTypeDef

```python
# GetInstanceRequestRequestTypeDef definition

class GetInstanceRequestRequestTypeDef(TypedDict):
    instanceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDataIntegrationFlowsRequestRequestTypeDef

```python
# ListDataIntegrationFlowsRequestRequestTypeDef definition

class ListDataIntegrationFlowsRequestRequestTypeDef(TypedDict):
    instanceId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDataLakeDatasetsRequestRequestTypeDef

```python
# ListDataLakeDatasetsRequestRequestTypeDef definition

class ListDataLakeDatasetsRequestRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    instanceNameFilter: NotRequired[Sequence[str]],
    instanceStateFilter: NotRequired[Sequence[InstanceStateType]],  # (1)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## UpdateDataLakeDatasetRequestRequestTypeDef

```python
# UpdateDataLakeDatasetRequestRequestTypeDef definition

class UpdateDataLakeDatasetRequestRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    description: NotRequired[str],
```

## UpdateInstanceRequestRequestTypeDef

```python
# UpdateInstanceRequestRequestTypeDef definition

class UpdateInstanceRequestRequestTypeDef(TypedDict):
    instanceId: str,
    instanceName: NotRequired[str],
    instanceDescription: NotRequired[str],
```

## CreateBillOfMaterialsImportJobResponseTypeDef

```python
# CreateBillOfMaterialsImportJobResponseTypeDef definition

class CreateBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataIntegrationFlowResponseTypeDef

```python
# CreateDataIntegrationFlowResponseTypeDef definition

class CreateDataIntegrationFlowResponseTypeDef(TypedDict):
    instanceId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataIntegrationFlowResponseTypeDef

```python
# DeleteDataIntegrationFlowResponseTypeDef definition

class DeleteDataIntegrationFlowResponseTypeDef(TypedDict):
    instanceId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataLakeDatasetResponseTypeDef

```python
# DeleteDataLakeDatasetResponseTypeDef definition

class DeleteDataLakeDatasetResponseTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBillOfMaterialsImportJobResponseTypeDef

```python
# GetBillOfMaterialsImportJobResponseTypeDef definition

class GetBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    job: BillOfMaterialsImportJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillOfMaterialsImportJobTypeDef](./type_defs.md#billofmaterialsimportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDataIntegrationEventResponseTypeDef

```python
# SendDataIntegrationEventResponseTypeDef definition

class SendDataIntegrationEventResponseTypeDef(TypedDict):
    eventId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResponseTypeDef

```python
# CreateInstanceResponseTypeDef definition

class CreateInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInstanceResponseTypeDef

```python
# DeleteInstanceResponseTypeDef definition

class DeleteInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceResponseTypeDef

```python
# GetInstanceResponseTypeDef definition

class GetInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceResponseTypeDef

```python
# UpdateInstanceResponseTypeDef definition

class UpdateInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataIntegrationFlowDatasetSourceConfigurationTypeDef

```python
# DataIntegrationFlowDatasetSourceConfigurationTypeDef definition

class DataIntegrationFlowDatasetSourceConfigurationTypeDef(TypedDict):
    datasetIdentifier: str,
    options: NotRequired[DataIntegrationFlowDatasetOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowDatasetOptionsTypeDef](./type_defs.md#dataintegrationflowdatasetoptionstypedef) 
## DataIntegrationFlowDatasetTargetConfigurationTypeDef

```python
# DataIntegrationFlowDatasetTargetConfigurationTypeDef definition

class DataIntegrationFlowDatasetTargetConfigurationTypeDef(TypedDict):
    datasetIdentifier: str,
    options: NotRequired[DataIntegrationFlowDatasetOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowDatasetOptionsTypeDef](./type_defs.md#dataintegrationflowdatasetoptionstypedef) 
## DataIntegrationFlowS3SourceConfigurationTypeDef

```python
# DataIntegrationFlowS3SourceConfigurationTypeDef definition

class DataIntegrationFlowS3SourceConfigurationTypeDef(TypedDict):
    bucketName: str,
    prefix: str,
    options: NotRequired[DataIntegrationFlowS3OptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowS3OptionsTypeDef](./type_defs.md#dataintegrationflows3optionstypedef) 
## DataIntegrationFlowS3TargetConfigurationTypeDef

```python
# DataIntegrationFlowS3TargetConfigurationTypeDef definition

class DataIntegrationFlowS3TargetConfigurationTypeDef(TypedDict):
    bucketName: str,
    prefix: str,
    options: NotRequired[DataIntegrationFlowS3OptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowS3OptionsTypeDef](./type_defs.md#dataintegrationflows3optionstypedef) 
## DataIntegrationFlowTransformationTypeDef

```python
# DataIntegrationFlowTransformationTypeDef definition

class DataIntegrationFlowTransformationTypeDef(TypedDict):
    transformationType: DataIntegrationFlowTransformationTypeType,  # (1)
    sqlTransformation: NotRequired[DataIntegrationFlowSQLTransformationConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: DataIntegrationFlowTransformationTypeType](./literals.md#dataintegrationflowtransformationtypetype) 
2. See [:material-code-braces: DataIntegrationFlowSQLTransformationConfigurationTypeDef](./type_defs.md#dataintegrationflowsqltransformationconfigurationtypedef) 
## DataLakeDatasetSchemaOutputTypeDef

```python
# DataLakeDatasetSchemaOutputTypeDef definition

class DataLakeDatasetSchemaOutputTypeDef(TypedDict):
    name: str,
    fields: List[DataLakeDatasetSchemaFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeDatasetSchemaFieldTypeDef](./type_defs.md#datalakedatasetschemafieldtypedef) 
## DataLakeDatasetSchemaTypeDef

```python
# DataLakeDatasetSchemaTypeDef definition

class DataLakeDatasetSchemaTypeDef(TypedDict):
    name: str,
    fields: Sequence[DataLakeDatasetSchemaFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeDatasetSchemaFieldTypeDef](./type_defs.md#datalakedatasetschemafieldtypedef) 
## ListDataIntegrationFlowsRequestPaginateTypeDef

```python
# ListDataIntegrationFlowsRequestPaginateTypeDef definition

class ListDataIntegrationFlowsRequestPaginateTypeDef(TypedDict):
    instanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataLakeDatasetsRequestPaginateTypeDef

```python
# ListDataLakeDatasetsRequestPaginateTypeDef definition

class ListDataLakeDatasetsRequestPaginateTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    instanceNameFilter: NotRequired[Sequence[str]],
    instanceStateFilter: NotRequired[Sequence[InstanceStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SendDataIntegrationEventRequestRequestTypeDef

```python
# SendDataIntegrationEventRequestRequestTypeDef definition

class SendDataIntegrationEventRequestRequestTypeDef(TypedDict):
    instanceId: str,
    eventType: DataIntegrationEventTypeType,  # (1)
    data: str,
    eventGroupId: str,
    eventTimestamp: NotRequired[TimestampTypeDef],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: DataIntegrationEventTypeType](./literals.md#dataintegrationeventtypetype) 
## DataIntegrationFlowSourceTypeDef

```python
# DataIntegrationFlowSourceTypeDef definition

class DataIntegrationFlowSourceTypeDef(TypedDict):
    sourceType: DataIntegrationFlowSourceTypeType,  # (1)
    sourceName: str,
    s3Source: NotRequired[DataIntegrationFlowS3SourceConfigurationTypeDef],  # (2)
    datasetSource: NotRequired[DataIntegrationFlowDatasetSourceConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: DataIntegrationFlowSourceTypeType](./literals.md#dataintegrationflowsourcetypetype) 
2. See [:material-code-braces: DataIntegrationFlowS3SourceConfigurationTypeDef](./type_defs.md#dataintegrationflows3sourceconfigurationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowDatasetSourceConfigurationTypeDef](./type_defs.md#dataintegrationflowdatasetsourceconfigurationtypedef) 
## DataIntegrationFlowTargetTypeDef

```python
# DataIntegrationFlowTargetTypeDef definition

class DataIntegrationFlowTargetTypeDef(TypedDict):
    targetType: DataIntegrationFlowTargetTypeType,  # (1)
    s3Target: NotRequired[DataIntegrationFlowS3TargetConfigurationTypeDef],  # (2)
    datasetTarget: NotRequired[DataIntegrationFlowDatasetTargetConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: DataIntegrationFlowTargetTypeType](./literals.md#dataintegrationflowtargettypetype) 
2. See [:material-code-braces: DataIntegrationFlowS3TargetConfigurationTypeDef](./type_defs.md#dataintegrationflows3targetconfigurationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowDatasetTargetConfigurationTypeDef](./type_defs.md#dataintegrationflowdatasettargetconfigurationtypedef) 
## DataLakeDatasetTypeDef

```python
# DataLakeDatasetTypeDef definition

class DataLakeDatasetTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    arn: str,
    schema: DataLakeDatasetSchemaOutputTypeDef,  # (1)
    createdTime: datetime,
    lastModifiedTime: datetime,
    description: NotRequired[str],
```

1. See [:material-code-braces: DataLakeDatasetSchemaOutputTypeDef](./type_defs.md#datalakedatasetschemaoutputtypedef) 
## CreateDataLakeDatasetRequestRequestTypeDef

```python
# CreateDataLakeDatasetRequestRequestTypeDef definition

class CreateDataLakeDatasetRequestRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    schema: NotRequired[DataLakeDatasetSchemaTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef) 
## CreateDataIntegrationFlowRequestRequestTypeDef

```python
# CreateDataIntegrationFlowRequestRequestTypeDef definition

class CreateDataIntegrationFlowRequestRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
    sources: Sequence[DataIntegrationFlowSourceTypeDef],  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef,  # (2)
    target: DataIntegrationFlowTargetTypeDef,  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
## DataIntegrationFlowTypeDef

```python
# DataIntegrationFlowTypeDef definition

class DataIntegrationFlowTypeDef(TypedDict):
    instanceId: str,
    name: str,
    sources: List[DataIntegrationFlowSourceTypeDef],  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef,  # (2)
    target: DataIntegrationFlowTargetTypeDef,  # (3)
    createdTime: datetime,
    lastModifiedTime: datetime,
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
## UpdateDataIntegrationFlowRequestRequestTypeDef

```python
# UpdateDataIntegrationFlowRequestRequestTypeDef definition

class UpdateDataIntegrationFlowRequestRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
    sources: NotRequired[Sequence[DataIntegrationFlowSourceTypeDef]],  # (1)
    transformation: NotRequired[DataIntegrationFlowTransformationTypeDef],  # (2)
    target: NotRequired[DataIntegrationFlowTargetTypeDef],  # (3)
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
## CreateDataLakeDatasetResponseTypeDef

```python
# CreateDataLakeDatasetResponseTypeDef definition

class CreateDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataLakeDatasetResponseTypeDef

```python
# GetDataLakeDatasetResponseTypeDef definition

class GetDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataLakeDatasetsResponseTypeDef

```python
# ListDataLakeDatasetsResponseTypeDef definition

class ListDataLakeDatasetsResponseTypeDef(TypedDict):
    datasets: List[DataLakeDatasetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataLakeDatasetResponseTypeDef

```python
# UpdateDataLakeDatasetResponseTypeDef definition

class UpdateDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataIntegrationFlowResponseTypeDef

```python
# GetDataIntegrationFlowResponseTypeDef definition

class GetDataIntegrationFlowResponseTypeDef(TypedDict):
    flow: DataIntegrationFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataIntegrationFlowsResponseTypeDef

```python
# ListDataIntegrationFlowsResponseTypeDef definition

class ListDataIntegrationFlowsResponseTypeDef(TypedDict):
    flows: List[DataIntegrationFlowTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataIntegrationFlowResponseTypeDef

```python
# UpdateDataIntegrationFlowResponseTypeDef definition

class UpdateDataIntegrationFlowResponseTypeDef(TypedDict):
    flow: DataIntegrationFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
