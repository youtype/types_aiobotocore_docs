# Type definitions

> [Index](../README.md) > [CognitoSync](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
    type annotations stubs module [types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BulkPublishRequestRequestTypeDef

```python
# BulkPublishRequestRequestTypeDef definition

class BulkPublishRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
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

## CognitoStreamsTypeDef

```python
# CognitoStreamsTypeDef definition

class CognitoStreamsTypeDef(TypedDict):
    StreamName: NotRequired[str],
    RoleArn: NotRequired[str],
    StreamingStatus: NotRequired[StreamingStatusType],  # (1)
```

1. See [:material-code-brackets: StreamingStatusType](./literals.md#streamingstatustype) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    IdentityId: NotRequired[str],
    DatasetName: NotRequired[str],
    CreationDate: NotRequired[datetime],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    DataStorage: NotRequired[int],
    NumRecords: NotRequired[int],
```

## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
```

## DescribeIdentityPoolUsageRequestRequestTypeDef

```python
# DescribeIdentityPoolUsageRequestRequestTypeDef definition

class DescribeIdentityPoolUsageRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## IdentityPoolUsageTypeDef

```python
# IdentityPoolUsageTypeDef definition

class IdentityPoolUsageTypeDef(TypedDict):
    IdentityPoolId: NotRequired[str],
    SyncSessionsCount: NotRequired[int],
    DataStorage: NotRequired[int],
    LastModifiedDate: NotRequired[datetime],
```

## DescribeIdentityUsageRequestRequestTypeDef

```python
# DescribeIdentityUsageRequestRequestTypeDef definition

class DescribeIdentityUsageRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
```

## IdentityUsageTypeDef

```python
# IdentityUsageTypeDef definition

class IdentityUsageTypeDef(TypedDict):
    IdentityId: NotRequired[str],
    IdentityPoolId: NotRequired[str],
    LastModifiedDate: NotRequired[datetime],
    DatasetCount: NotRequired[int],
    DataStorage: NotRequired[int],
```

## GetBulkPublishDetailsRequestRequestTypeDef

```python
# GetBulkPublishDetailsRequestRequestTypeDef definition

class GetBulkPublishDetailsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## GetCognitoEventsRequestRequestTypeDef

```python
# GetCognitoEventsRequestRequestTypeDef definition

class GetCognitoEventsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## GetIdentityPoolConfigurationRequestRequestTypeDef

```python
# GetIdentityPoolConfigurationRequestRequestTypeDef definition

class GetIdentityPoolConfigurationRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
```

## PushSyncTypeDef

```python
# PushSyncTypeDef definition

class PushSyncTypeDef(TypedDict):
    ApplicationArns: NotRequired[List[str]],
    RoleArn: NotRequired[str],
```

## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIdentityPoolUsageRequestRequestTypeDef

```python
# ListIdentityPoolUsageRequestRequestTypeDef definition

class ListIdentityPoolUsageRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRecordsRequestRequestTypeDef

```python
# ListRecordsRequestRequestTypeDef definition

class ListRecordsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    LastSyncCount: NotRequired[int],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SyncSessionToken: NotRequired[str],
```

## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    SyncCount: NotRequired[int],
    LastModifiedDate: NotRequired[datetime],
    LastModifiedBy: NotRequired[str],
    DeviceLastModifiedDate: NotRequired[datetime],
```

## RegisterDeviceRequestRequestTypeDef

```python
# RegisterDeviceRequestRequestTypeDef definition

class RegisterDeviceRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    Platform: PlatformType,  # (1)
    Token: str,
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## SetCognitoEventsRequestRequestTypeDef

```python
# SetCognitoEventsRequestRequestTypeDef definition

class SetCognitoEventsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    Events: Mapping[str, str],
```

## SubscribeToDatasetRequestRequestTypeDef

```python
# SubscribeToDatasetRequestRequestTypeDef definition

class SubscribeToDatasetRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    DeviceId: str,
```

## UnsubscribeFromDatasetRequestRequestTypeDef

```python
# UnsubscribeFromDatasetRequestRequestTypeDef definition

class UnsubscribeFromDatasetRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    DeviceId: str,
```

## BulkPublishResponseTypeDef

```python
# BulkPublishResponseTypeDef definition

class BulkPublishResponseTypeDef(TypedDict):
    IdentityPoolId: str,
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
## GetBulkPublishDetailsResponseTypeDef

```python
# GetBulkPublishDetailsResponseTypeDef definition

class GetBulkPublishDetailsResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    BulkPublishStartTime: datetime,
    BulkPublishCompleteTime: datetime,
    BulkPublishStatus: BulkPublishStatusType,  # (1)
    FailureMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BulkPublishStatusType](./literals.md#bulkpublishstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCognitoEventsResponseTypeDef

```python
# GetCognitoEventsResponseTypeDef definition

class GetCognitoEventsResponseTypeDef(TypedDict):
    Events: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDeviceResponseTypeDef

```python
# RegisterDeviceResponseTypeDef definition

class RegisterDeviceResponseTypeDef(TypedDict):
    DeviceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDatasetResponseTypeDef

```python
# DeleteDatasetResponseTypeDef definition

class DeleteDatasetResponseTypeDef(TypedDict):
    Dataset: DatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    Dataset: DatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    Datasets: List[DatasetTypeDef],  # (1)
    Count: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIdentityPoolUsageResponseTypeDef

```python
# DescribeIdentityPoolUsageResponseTypeDef definition

class DescribeIdentityPoolUsageResponseTypeDef(TypedDict):
    IdentityPoolUsage: IdentityPoolUsageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityPoolUsageTypeDef](./type_defs.md#identitypoolusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityPoolUsageResponseTypeDef

```python
# ListIdentityPoolUsageResponseTypeDef definition

class ListIdentityPoolUsageResponseTypeDef(TypedDict):
    IdentityPoolUsages: List[IdentityPoolUsageTypeDef],  # (1)
    MaxResults: int,
    Count: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityPoolUsageTypeDef](./type_defs.md#identitypoolusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIdentityUsageResponseTypeDef

```python
# DescribeIdentityUsageResponseTypeDef definition

class DescribeIdentityUsageResponseTypeDef(TypedDict):
    IdentityUsage: IdentityUsageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityUsageTypeDef](./type_defs.md#identityusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityPoolConfigurationResponseTypeDef

```python
# GetIdentityPoolConfigurationResponseTypeDef definition

class GetIdentityPoolConfigurationResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    PushSync: PushSyncTypeDef,  # (1)
    CognitoStreams: CognitoStreamsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PushSyncTypeDef](./type_defs.md#pushsynctypedef) 
2. See [:material-code-braces: CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetIdentityPoolConfigurationRequestRequestTypeDef

```python
# SetIdentityPoolConfigurationRequestRequestTypeDef definition

class SetIdentityPoolConfigurationRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    PushSync: NotRequired[PushSyncTypeDef],  # (1)
    CognitoStreams: NotRequired[CognitoStreamsTypeDef],  # (2)
```

1. See [:material-code-braces: PushSyncTypeDef](./type_defs.md#pushsynctypedef) 
2. See [:material-code-braces: CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef) 
## SetIdentityPoolConfigurationResponseTypeDef

```python
# SetIdentityPoolConfigurationResponseTypeDef definition

class SetIdentityPoolConfigurationResponseTypeDef(TypedDict):
    IdentityPoolId: str,
    PushSync: PushSyncTypeDef,  # (1)
    CognitoStreams: CognitoStreamsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PushSyncTypeDef](./type_defs.md#pushsynctypedef) 
2. See [:material-code-braces: CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecordsResponseTypeDef

```python
# ListRecordsResponseTypeDef definition

class ListRecordsResponseTypeDef(TypedDict):
    Records: List[RecordTypeDef],  # (1)
    NextToken: str,
    Count: int,
    DatasetSyncCount: int,
    LastModifiedBy: str,
    MergedDatasetNames: List[str],
    DatasetExists: bool,
    DatasetDeletedAfterRequestedSyncCount: bool,
    SyncSessionToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecordsResponseTypeDef

```python
# UpdateRecordsResponseTypeDef definition

class UpdateRecordsResponseTypeDef(TypedDict):
    Records: List[RecordTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecordPatchTypeDef

```python
# RecordPatchTypeDef definition

class RecordPatchTypeDef(TypedDict):
    Op: OperationType,  # (1)
    Key: str,
    SyncCount: int,
    Value: NotRequired[str],
    DeviceLastModifiedDate: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
## UpdateRecordsRequestRequestTypeDef

```python
# UpdateRecordsRequestRequestTypeDef definition

class UpdateRecordsRequestRequestTypeDef(TypedDict):
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    SyncSessionToken: str,
    DeviceId: NotRequired[str],
    RecordPatches: NotRequired[Sequence[RecordPatchTypeDef]],  # (1)
    ClientContext: NotRequired[str],
```

1. See [:material-code-braces: RecordPatchTypeDef](./type_defs.md#recordpatchtypedef) 
