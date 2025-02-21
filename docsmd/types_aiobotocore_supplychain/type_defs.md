# Type definitions

> [Index](../README.md) > [SupplyChain](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_supplychain.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## DataLakeDatasetSchemaUnionTypeDef

```python
# DataLakeDatasetSchemaUnionTypeDef Union usage example

from types_aiobotocore_supplychain.type_defs import DataLakeDatasetSchemaUnionTypeDef


def get_value() -> DataLakeDatasetSchemaUnionTypeDef:
    return ...


# DataLakeDatasetSchemaUnionTypeDef definition

DataLakeDatasetSchemaUnionTypeDef = Union[
    DataLakeDatasetSchemaTypeDef,  # (1)
    DataLakeDatasetSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef) 
2. See [:material-code-braces: DataLakeDatasetSchemaOutputTypeDef](./type_defs.md#datalakedatasetschemaoutputtypedef) 



## BillOfMaterialsImportJobTypeDef

```python
# BillOfMaterialsImportJobTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import BillOfMaterialsImportJobTypeDef


def get_value() -> BillOfMaterialsImportJobTypeDef:
    return {
        "instanceId": ...,
    }


# BillOfMaterialsImportJobTypeDef definition

class BillOfMaterialsImportJobTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
    status: ConfigurationJobStatusType,  # (1)
    s3uri: str,
    message: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationJobStatusType](./literals.md#configurationjobstatustype) 
## CreateBillOfMaterialsImportJobRequestTypeDef

```python
# CreateBillOfMaterialsImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobRequestTypeDef


def get_value() -> CreateBillOfMaterialsImportJobRequestTypeDef:
    return {
        "instanceId": ...,
    }


# CreateBillOfMaterialsImportJobRequestTypeDef definition

class CreateBillOfMaterialsImportJobRequestTypeDef(TypedDict):
    instanceId: str,
    s3uri: str,
    clientToken: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateInstanceRequestTypeDef

```python
# CreateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateInstanceRequestTypeDef


def get_value() -> CreateInstanceRequestTypeDef:
    return {
        "instanceName": ...,
    }


# CreateInstanceRequestTypeDef definition

class CreateInstanceRequestTypeDef(TypedDict):
    instanceName: NotRequired[str],
    instanceDescription: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    webAppDnsDomain: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## InstanceTypeDef

```python
# InstanceTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import InstanceTypeDef


def get_value() -> InstanceTypeDef:
    return {
        "instanceId": ...,
    }


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
# DataIntegrationFlowDatasetOptionsTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowDatasetOptionsTypeDef


def get_value() -> DataIntegrationFlowDatasetOptionsTypeDef:
    return {
        "loadType": ...,
    }


# DataIntegrationFlowDatasetOptionsTypeDef definition

class DataIntegrationFlowDatasetOptionsTypeDef(TypedDict):
    loadType: NotRequired[DataIntegrationFlowLoadTypeType],  # (1)
    dedupeRecords: NotRequired[bool],
```

1. See [:material-code-brackets: DataIntegrationFlowLoadTypeType](./literals.md#dataintegrationflowloadtypetype) 
## DataIntegrationFlowS3OptionsTypeDef

```python
# DataIntegrationFlowS3OptionsTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowS3OptionsTypeDef


def get_value() -> DataIntegrationFlowS3OptionsTypeDef:
    return {
        "fileType": ...,
    }


# DataIntegrationFlowS3OptionsTypeDef definition

class DataIntegrationFlowS3OptionsTypeDef(TypedDict):
    fileType: NotRequired[DataIntegrationFlowFileTypeType],  # (1)
```

1. See [:material-code-brackets: DataIntegrationFlowFileTypeType](./literals.md#dataintegrationflowfiletypetype) 
## DataIntegrationFlowSQLTransformationConfigurationTypeDef

```python
# DataIntegrationFlowSQLTransformationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowSQLTransformationConfigurationTypeDef


def get_value() -> DataIntegrationFlowSQLTransformationConfigurationTypeDef:
    return {
        "query": ...,
    }


# DataIntegrationFlowSQLTransformationConfigurationTypeDef definition

class DataIntegrationFlowSQLTransformationConfigurationTypeDef(TypedDict):
    query: str,
```

## DataLakeDatasetSchemaFieldTypeDef

```python
# DataLakeDatasetSchemaFieldTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataLakeDatasetSchemaFieldTypeDef


def get_value() -> DataLakeDatasetSchemaFieldTypeDef:
    return {
        "name": ...,
    }


# DataLakeDatasetSchemaFieldTypeDef definition

class DataLakeDatasetSchemaFieldTypeDef(TypedDict):
    name: str,
    type: DataLakeDatasetSchemaFieldTypeType,  # (1)
    isRequired: bool,
```

1. See [:material-code-brackets: DataLakeDatasetSchemaFieldTypeType](./literals.md#datalakedatasetschemafieldtypetype) 
## DeleteDataIntegrationFlowRequestTypeDef

```python
# DeleteDataIntegrationFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteDataIntegrationFlowRequestTypeDef


def get_value() -> DeleteDataIntegrationFlowRequestTypeDef:
    return {
        "instanceId": ...,
    }


# DeleteDataIntegrationFlowRequestTypeDef definition

class DeleteDataIntegrationFlowRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
```

## DeleteDataLakeDatasetRequestTypeDef

```python
# DeleteDataLakeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteDataLakeDatasetRequestTypeDef


def get_value() -> DeleteDataLakeDatasetRequestTypeDef:
    return {
        "instanceId": ...,
    }


# DeleteDataLakeDatasetRequestTypeDef definition

class DeleteDataLakeDatasetRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
```

## DeleteInstanceRequestTypeDef

```python
# DeleteInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteInstanceRequestTypeDef


def get_value() -> DeleteInstanceRequestTypeDef:
    return {
        "instanceId": ...,
    }


# DeleteInstanceRequestTypeDef definition

class DeleteInstanceRequestTypeDef(TypedDict):
    instanceId: str,
```

## GetBillOfMaterialsImportJobRequestTypeDef

```python
# GetBillOfMaterialsImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetBillOfMaterialsImportJobRequestTypeDef


def get_value() -> GetBillOfMaterialsImportJobRequestTypeDef:
    return {
        "instanceId": ...,
    }


# GetBillOfMaterialsImportJobRequestTypeDef definition

class GetBillOfMaterialsImportJobRequestTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
```

## GetDataIntegrationFlowRequestTypeDef

```python
# GetDataIntegrationFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetDataIntegrationFlowRequestTypeDef


def get_value() -> GetDataIntegrationFlowRequestTypeDef:
    return {
        "instanceId": ...,
    }


# GetDataIntegrationFlowRequestTypeDef definition

class GetDataIntegrationFlowRequestTypeDef(TypedDict):
    instanceId: str,
    name: str,
```

## GetDataLakeDatasetRequestTypeDef

```python
# GetDataLakeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetDataLakeDatasetRequestTypeDef


def get_value() -> GetDataLakeDatasetRequestTypeDef:
    return {
        "instanceId": ...,
    }


# GetDataLakeDatasetRequestTypeDef definition

class GetDataLakeDatasetRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
```

## GetInstanceRequestTypeDef

```python
# GetInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetInstanceRequestTypeDef


def get_value() -> GetInstanceRequestTypeDef:
    return {
        "instanceId": ...,
    }


# GetInstanceRequestTypeDef definition

class GetInstanceRequestTypeDef(TypedDict):
    instanceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDataIntegrationFlowsRequestTypeDef

```python
# ListDataIntegrationFlowsRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataIntegrationFlowsRequestTypeDef


def get_value() -> ListDataIntegrationFlowsRequestTypeDef:
    return {
        "instanceId": ...,
    }


# ListDataIntegrationFlowsRequestTypeDef definition

class ListDataIntegrationFlowsRequestTypeDef(TypedDict):
    instanceId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDataLakeDatasetsRequestTypeDef

```python
# ListDataLakeDatasetsRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataLakeDatasetsRequestTypeDef


def get_value() -> ListDataLakeDatasetsRequestTypeDef:
    return {
        "instanceId": ...,
    }


# ListDataLakeDatasetsRequestTypeDef definition

class ListDataLakeDatasetsRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListInstancesRequestTypeDef

```python
# ListInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListInstancesRequestTypeDef


def get_value() -> ListInstancesRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListInstancesRequestTypeDef definition

class ListInstancesRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    instanceNameFilter: NotRequired[Sequence[str]],
    instanceStateFilter: NotRequired[Sequence[InstanceStateType]],  # (1)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDataLakeDatasetRequestTypeDef

```python
# UpdateDataLakeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateDataLakeDatasetRequestTypeDef


def get_value() -> UpdateDataLakeDatasetRequestTypeDef:
    return {
        "instanceId": ...,
    }


# UpdateDataLakeDatasetRequestTypeDef definition

class UpdateDataLakeDatasetRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    description: NotRequired[str],
```

## UpdateInstanceRequestTypeDef

```python
# UpdateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateInstanceRequestTypeDef


def get_value() -> UpdateInstanceRequestTypeDef:
    return {
        "instanceId": ...,
    }


# UpdateInstanceRequestTypeDef definition

class UpdateInstanceRequestTypeDef(TypedDict):
    instanceId: str,
    instanceName: NotRequired[str],
    instanceDescription: NotRequired[str],
```

## CreateBillOfMaterialsImportJobResponseTypeDef

```python
# CreateBillOfMaterialsImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobResponseTypeDef


def get_value() -> CreateBillOfMaterialsImportJobResponseTypeDef:
    return {
        "jobId": ...,
    }


# CreateBillOfMaterialsImportJobResponseTypeDef definition

class CreateBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataIntegrationFlowResponseTypeDef

```python
# CreateDataIntegrationFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateDataIntegrationFlowResponseTypeDef


def get_value() -> CreateDataIntegrationFlowResponseTypeDef:
    return {
        "instanceId": ...,
    }


# CreateDataIntegrationFlowResponseTypeDef definition

class CreateDataIntegrationFlowResponseTypeDef(TypedDict):
    instanceId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataIntegrationFlowResponseTypeDef

```python
# DeleteDataIntegrationFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteDataIntegrationFlowResponseTypeDef


def get_value() -> DeleteDataIntegrationFlowResponseTypeDef:
    return {
        "instanceId": ...,
    }


# DeleteDataIntegrationFlowResponseTypeDef definition

class DeleteDataIntegrationFlowResponseTypeDef(TypedDict):
    instanceId: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataLakeDatasetResponseTypeDef

```python
# DeleteDataLakeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteDataLakeDatasetResponseTypeDef


def get_value() -> DeleteDataLakeDatasetResponseTypeDef:
    return {
        "instanceId": ...,
    }


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
# GetBillOfMaterialsImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetBillOfMaterialsImportJobResponseTypeDef


def get_value() -> GetBillOfMaterialsImportJobResponseTypeDef:
    return {
        "job": ...,
    }


# GetBillOfMaterialsImportJobResponseTypeDef definition

class GetBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    job: BillOfMaterialsImportJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillOfMaterialsImportJobTypeDef](./type_defs.md#billofmaterialsimportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDataIntegrationEventResponseTypeDef

```python
# SendDataIntegrationEventResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import SendDataIntegrationEventResponseTypeDef


def get_value() -> SendDataIntegrationEventResponseTypeDef:
    return {
        "eventId": ...,
    }


# SendDataIntegrationEventResponseTypeDef definition

class SendDataIntegrationEventResponseTypeDef(TypedDict):
    eventId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResponseTypeDef

```python
# CreateInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateInstanceResponseTypeDef


def get_value() -> CreateInstanceResponseTypeDef:
    return {
        "instance": ...,
    }


# CreateInstanceResponseTypeDef definition

class CreateInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInstanceResponseTypeDef

```python
# DeleteInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DeleteInstanceResponseTypeDef


def get_value() -> DeleteInstanceResponseTypeDef:
    return {
        "instance": ...,
    }


# DeleteInstanceResponseTypeDef definition

class DeleteInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceResponseTypeDef

```python
# GetInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetInstanceResponseTypeDef


def get_value() -> GetInstanceResponseTypeDef:
    return {
        "instance": ...,
    }


# GetInstanceResponseTypeDef definition

class GetInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListInstancesResponseTypeDef


def get_value() -> ListInstancesResponseTypeDef:
    return {
        "instances": ...,
    }


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
# UpdateInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateInstanceResponseTypeDef


def get_value() -> UpdateInstanceResponseTypeDef:
    return {
        "instance": ...,
    }


# UpdateInstanceResponseTypeDef definition

class UpdateInstanceResponseTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataIntegrationFlowDatasetSourceConfigurationTypeDef

```python
# DataIntegrationFlowDatasetSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowDatasetSourceConfigurationTypeDef


def get_value() -> DataIntegrationFlowDatasetSourceConfigurationTypeDef:
    return {
        "datasetIdentifier": ...,
    }


# DataIntegrationFlowDatasetSourceConfigurationTypeDef definition

class DataIntegrationFlowDatasetSourceConfigurationTypeDef(TypedDict):
    datasetIdentifier: str,
    options: NotRequired[DataIntegrationFlowDatasetOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowDatasetOptionsTypeDef](./type_defs.md#dataintegrationflowdatasetoptionstypedef) 
## DataIntegrationFlowDatasetTargetConfigurationTypeDef

```python
# DataIntegrationFlowDatasetTargetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowDatasetTargetConfigurationTypeDef


def get_value() -> DataIntegrationFlowDatasetTargetConfigurationTypeDef:
    return {
        "datasetIdentifier": ...,
    }


# DataIntegrationFlowDatasetTargetConfigurationTypeDef definition

class DataIntegrationFlowDatasetTargetConfigurationTypeDef(TypedDict):
    datasetIdentifier: str,
    options: NotRequired[DataIntegrationFlowDatasetOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowDatasetOptionsTypeDef](./type_defs.md#dataintegrationflowdatasetoptionstypedef) 
## DataIntegrationFlowS3SourceConfigurationTypeDef

```python
# DataIntegrationFlowS3SourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowS3SourceConfigurationTypeDef


def get_value() -> DataIntegrationFlowS3SourceConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# DataIntegrationFlowS3SourceConfigurationTypeDef definition

class DataIntegrationFlowS3SourceConfigurationTypeDef(TypedDict):
    bucketName: str,
    prefix: str,
    options: NotRequired[DataIntegrationFlowS3OptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowS3OptionsTypeDef](./type_defs.md#dataintegrationflows3optionstypedef) 
## DataIntegrationFlowS3TargetConfigurationTypeDef

```python
# DataIntegrationFlowS3TargetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowS3TargetConfigurationTypeDef


def get_value() -> DataIntegrationFlowS3TargetConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# DataIntegrationFlowS3TargetConfigurationTypeDef definition

class DataIntegrationFlowS3TargetConfigurationTypeDef(TypedDict):
    bucketName: str,
    prefix: str,
    options: NotRequired[DataIntegrationFlowS3OptionsTypeDef],  # (1)
```

1. See [:material-code-braces: DataIntegrationFlowS3OptionsTypeDef](./type_defs.md#dataintegrationflows3optionstypedef) 
## DataIntegrationFlowTransformationTypeDef

```python
# DataIntegrationFlowTransformationTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowTransformationTypeDef


def get_value() -> DataIntegrationFlowTransformationTypeDef:
    return {
        "transformationType": ...,
    }


# DataIntegrationFlowTransformationTypeDef definition

class DataIntegrationFlowTransformationTypeDef(TypedDict):
    transformationType: DataIntegrationFlowTransformationTypeType,  # (1)
    sqlTransformation: NotRequired[DataIntegrationFlowSQLTransformationConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: DataIntegrationFlowTransformationTypeType](./literals.md#dataintegrationflowtransformationtypetype) 
2. See [:material-code-braces: DataIntegrationFlowSQLTransformationConfigurationTypeDef](./type_defs.md#dataintegrationflowsqltransformationconfigurationtypedef) 
## DataLakeDatasetSchemaOutputTypeDef

```python
# DataLakeDatasetSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataLakeDatasetSchemaOutputTypeDef


def get_value() -> DataLakeDatasetSchemaOutputTypeDef:
    return {
        "name": ...,
    }


# DataLakeDatasetSchemaOutputTypeDef definition

class DataLakeDatasetSchemaOutputTypeDef(TypedDict):
    name: str,
    fields: List[DataLakeDatasetSchemaFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeDatasetSchemaFieldTypeDef](./type_defs.md#datalakedatasetschemafieldtypedef) 
## DataLakeDatasetSchemaTypeDef

```python
# DataLakeDatasetSchemaTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataLakeDatasetSchemaTypeDef


def get_value() -> DataLakeDatasetSchemaTypeDef:
    return {
        "name": ...,
    }


# DataLakeDatasetSchemaTypeDef definition

class DataLakeDatasetSchemaTypeDef(TypedDict):
    name: str,
    fields: Sequence[DataLakeDatasetSchemaFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeDatasetSchemaFieldTypeDef](./type_defs.md#datalakedatasetschemafieldtypedef) 
## ListDataIntegrationFlowsRequestPaginateTypeDef

```python
# ListDataIntegrationFlowsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataIntegrationFlowsRequestPaginateTypeDef


def get_value() -> ListDataIntegrationFlowsRequestPaginateTypeDef:
    return {
        "instanceId": ...,
    }


# ListDataIntegrationFlowsRequestPaginateTypeDef definition

class ListDataIntegrationFlowsRequestPaginateTypeDef(TypedDict):
    instanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataLakeDatasetsRequestPaginateTypeDef

```python
# ListDataLakeDatasetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataLakeDatasetsRequestPaginateTypeDef


def get_value() -> ListDataLakeDatasetsRequestPaginateTypeDef:
    return {
        "instanceId": ...,
    }


# ListDataLakeDatasetsRequestPaginateTypeDef definition

class ListDataLakeDatasetsRequestPaginateTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListInstancesRequestPaginateTypeDef


def get_value() -> ListInstancesRequestPaginateTypeDef:
    return {
        "instanceNameFilter": ...,
    }


# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    instanceNameFilter: NotRequired[Sequence[str]],
    instanceStateFilter: NotRequired[Sequence[InstanceStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SendDataIntegrationEventRequestTypeDef

```python
# SendDataIntegrationEventRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import SendDataIntegrationEventRequestTypeDef


def get_value() -> SendDataIntegrationEventRequestTypeDef:
    return {
        "instanceId": ...,
    }


# SendDataIntegrationEventRequestTypeDef definition

class SendDataIntegrationEventRequestTypeDef(TypedDict):
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
# DataIntegrationFlowSourceTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowSourceTypeDef


def get_value() -> DataIntegrationFlowSourceTypeDef:
    return {
        "sourceType": ...,
    }


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
# DataIntegrationFlowTargetTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowTargetTypeDef


def get_value() -> DataIntegrationFlowTargetTypeDef:
    return {
        "targetType": ...,
    }


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
# DataLakeDatasetTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataLakeDatasetTypeDef


def get_value() -> DataLakeDatasetTypeDef:
    return {
        "instanceId": ...,
    }


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
## CreateDataIntegrationFlowRequestTypeDef

```python
# CreateDataIntegrationFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateDataIntegrationFlowRequestTypeDef


def get_value() -> CreateDataIntegrationFlowRequestTypeDef:
    return {
        "instanceId": ...,
    }


# CreateDataIntegrationFlowRequestTypeDef definition

class CreateDataIntegrationFlowRequestTypeDef(TypedDict):
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
# DataIntegrationFlowTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import DataIntegrationFlowTypeDef


def get_value() -> DataIntegrationFlowTypeDef:
    return {
        "instanceId": ...,
    }


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
## UpdateDataIntegrationFlowRequestTypeDef

```python
# UpdateDataIntegrationFlowRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateDataIntegrationFlowRequestTypeDef


def get_value() -> UpdateDataIntegrationFlowRequestTypeDef:
    return {
        "instanceId": ...,
    }


# UpdateDataIntegrationFlowRequestTypeDef definition

class UpdateDataIntegrationFlowRequestTypeDef(TypedDict):
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
# CreateDataLakeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateDataLakeDatasetResponseTypeDef


def get_value() -> CreateDataLakeDatasetResponseTypeDef:
    return {
        "dataset": ...,
    }


# CreateDataLakeDatasetResponseTypeDef definition

class CreateDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataLakeDatasetResponseTypeDef

```python
# GetDataLakeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetDataLakeDatasetResponseTypeDef


def get_value() -> GetDataLakeDatasetResponseTypeDef:
    return {
        "dataset": ...,
    }


# GetDataLakeDatasetResponseTypeDef definition

class GetDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataLakeDatasetsResponseTypeDef

```python
# ListDataLakeDatasetsResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataLakeDatasetsResponseTypeDef


def get_value() -> ListDataLakeDatasetsResponseTypeDef:
    return {
        "datasets": ...,
    }


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
# UpdateDataLakeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateDataLakeDatasetResponseTypeDef


def get_value() -> UpdateDataLakeDatasetResponseTypeDef:
    return {
        "dataset": ...,
    }


# UpdateDataLakeDatasetResponseTypeDef definition

class UpdateDataLakeDatasetResponseTypeDef(TypedDict):
    dataset: DataLakeDatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataLakeDatasetRequestTypeDef

```python
# CreateDataLakeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import CreateDataLakeDatasetRequestTypeDef


def get_value() -> CreateDataLakeDatasetRequestTypeDef:
    return {
        "instanceId": ...,
    }


# CreateDataLakeDatasetRequestTypeDef definition

class CreateDataLakeDatasetRequestTypeDef(TypedDict):
    instanceId: str,
    namespace: str,
    name: str,
    schema: NotRequired[DataLakeDatasetSchemaUnionTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef) [:material-code-braces: DataLakeDatasetSchemaOutputTypeDef](./type_defs.md#datalakedatasetschemaoutputtypedef) 
## GetDataIntegrationFlowResponseTypeDef

```python
# GetDataIntegrationFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import GetDataIntegrationFlowResponseTypeDef


def get_value() -> GetDataIntegrationFlowResponseTypeDef:
    return {
        "flow": ...,
    }


# GetDataIntegrationFlowResponseTypeDef definition

class GetDataIntegrationFlowResponseTypeDef(TypedDict):
    flow: DataIntegrationFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataIntegrationFlowsResponseTypeDef

```python
# ListDataIntegrationFlowsResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import ListDataIntegrationFlowsResponseTypeDef


def get_value() -> ListDataIntegrationFlowsResponseTypeDef:
    return {
        "flows": ...,
    }


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
# UpdateDataIntegrationFlowResponseTypeDef TypedDict usage example

from types_aiobotocore_supplychain.type_defs import UpdateDataIntegrationFlowResponseTypeDef


def get_value() -> UpdateDataIntegrationFlowResponseTypeDef:
    return {
        "flow": ...,
    }


# UpdateDataIntegrationFlowResponseTypeDef definition

class UpdateDataIntegrationFlowResponseTypeDef(TypedDict):
    flow: DataIntegrationFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
