<a id="typed-dictionaries-for-aiobotocore-cognitosync-module"></a>

# Typed dictionaries for aiobotocore CognitoSync module

> [Index](../README.md) > [CognitoSync](./README.md) > Typed dictionaries

Auto-generated documentation for
[CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
type annotations stubs module
[types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

- [Typed dictionaries for aiobotocore CognitoSync module](#typed-dictionaries-for-aiobotocore-cognitosync-module)
  - [BulkPublishRequestRequestTypeDef](#bulkpublishrequestrequesttypedef)
  - [BulkPublishResponseTypeDef](#bulkpublishresponsetypedef)
  - [CognitoStreamsTypeDef](#cognitostreamstypedef)
  - [DatasetTypeDef](#datasettypedef)
  - [DeleteDatasetRequestRequestTypeDef](#deletedatasetrequestrequesttypedef)
  - [DeleteDatasetResponseTypeDef](#deletedatasetresponsetypedef)
  - [DescribeDatasetRequestRequestTypeDef](#describedatasetrequestrequesttypedef)
  - [DescribeDatasetResponseTypeDef](#describedatasetresponsetypedef)
  - [DescribeIdentityPoolUsageRequestRequestTypeDef](#describeidentitypoolusagerequestrequesttypedef)
  - [DescribeIdentityPoolUsageResponseTypeDef](#describeidentitypoolusageresponsetypedef)
  - [DescribeIdentityUsageRequestRequestTypeDef](#describeidentityusagerequestrequesttypedef)
  - [DescribeIdentityUsageResponseTypeDef](#describeidentityusageresponsetypedef)
  - [GetBulkPublishDetailsRequestRequestTypeDef](#getbulkpublishdetailsrequestrequesttypedef)
  - [GetBulkPublishDetailsResponseTypeDef](#getbulkpublishdetailsresponsetypedef)
  - [GetCognitoEventsRequestRequestTypeDef](#getcognitoeventsrequestrequesttypedef)
  - [GetCognitoEventsResponseTypeDef](#getcognitoeventsresponsetypedef)
  - [GetIdentityPoolConfigurationRequestRequestTypeDef](#getidentitypoolconfigurationrequestrequesttypedef)
  - [GetIdentityPoolConfigurationResponseTypeDef](#getidentitypoolconfigurationresponsetypedef)
  - [IdentityPoolUsageTypeDef](#identitypoolusagetypedef)
  - [IdentityUsageTypeDef](#identityusagetypedef)
  - [ListDatasetsRequestRequestTypeDef](#listdatasetsrequestrequesttypedef)
  - [ListDatasetsResponseTypeDef](#listdatasetsresponsetypedef)
  - [ListIdentityPoolUsageRequestRequestTypeDef](#listidentitypoolusagerequestrequesttypedef)
  - [ListIdentityPoolUsageResponseTypeDef](#listidentitypoolusageresponsetypedef)
  - [ListRecordsRequestRequestTypeDef](#listrecordsrequestrequesttypedef)
  - [ListRecordsResponseTypeDef](#listrecordsresponsetypedef)
  - [PushSyncTypeDef](#pushsynctypedef)
  - [RecordPatchTypeDef](#recordpatchtypedef)
  - [RecordTypeDef](#recordtypedef)
  - [RegisterDeviceRequestRequestTypeDef](#registerdevicerequestrequesttypedef)
  - [RegisterDeviceResponseTypeDef](#registerdeviceresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [SetCognitoEventsRequestRequestTypeDef](#setcognitoeventsrequestrequesttypedef)
  - [SetIdentityPoolConfigurationRequestRequestTypeDef](#setidentitypoolconfigurationrequestrequesttypedef)
  - [SetIdentityPoolConfigurationResponseTypeDef](#setidentitypoolconfigurationresponsetypedef)
  - [SubscribeToDatasetRequestRequestTypeDef](#subscribetodatasetrequestrequesttypedef)
  - [UnsubscribeFromDatasetRequestRequestTypeDef](#unsubscribefromdatasetrequestrequesttypedef)
  - [UpdateRecordsRequestRequestTypeDef](#updaterecordsrequestrequesttypedef)
  - [UpdateRecordsResponseTypeDef](#updaterecordsresponsetypedef)

<a id="bulkpublishrequestrequesttypedef"></a>

## BulkPublishRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

<a id="bulkpublishresponsetypedef"></a>

## BulkPublishResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import BulkPublishResponseTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="cognitostreamstypedef"></a>

## CognitoStreamsTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import CognitoStreamsTypeDef
```

Optional fields:

- `StreamName`: `str`
- `RoleArn`: `str`
- `StreamingStatus`: [StreamingStatusType](./literals.md#streamingstatustype)

<a id="datasettypedef"></a>

## DatasetTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DatasetTypeDef
```

Optional fields:

- `IdentityId`: `str`
- `DatasetName`: `str`
- `CreationDate`: `datetime`
- `LastModifiedDate`: `datetime`
- `LastModifiedBy`: `str`
- `DataStorage`: `int`
- `NumRecords`: `int`

<a id="deletedatasetrequestrequesttypedef"></a>

## DeleteDatasetRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DeleteDatasetRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`

<a id="deletedatasetresponsetypedef"></a>

## DeleteDatasetResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DeleteDatasetResponseTypeDef
```

Required fields:

- `Dataset`: [DatasetTypeDef](./type_defs.md#datasettypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describedatasetrequestrequesttypedef"></a>

## DescribeDatasetRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeDatasetRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`

<a id="describedatasetresponsetypedef"></a>

## DescribeDatasetResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeDatasetResponseTypeDef
```

Required fields:

- `Dataset`: [DatasetTypeDef](./type_defs.md#datasettypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeidentitypoolusagerequestrequesttypedef"></a>

## DescribeIdentityPoolUsageRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeIdentityPoolUsageRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

<a id="describeidentitypoolusageresponsetypedef"></a>

## DescribeIdentityPoolUsageResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeIdentityPoolUsageResponseTypeDef
```

Required fields:

- `IdentityPoolUsage`:
  [IdentityPoolUsageTypeDef](./type_defs.md#identitypoolusagetypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeidentityusagerequestrequesttypedef"></a>

## DescribeIdentityUsageRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeIdentityUsageRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`

<a id="describeidentityusageresponsetypedef"></a>

## DescribeIdentityUsageResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import DescribeIdentityUsageResponseTypeDef
```

Required fields:

- `IdentityUsage`: [IdentityUsageTypeDef](./type_defs.md#identityusagetypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getbulkpublishdetailsrequestrequesttypedef"></a>

## GetBulkPublishDetailsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetBulkPublishDetailsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

<a id="getbulkpublishdetailsresponsetypedef"></a>

## GetBulkPublishDetailsResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetBulkPublishDetailsResponseTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `BulkPublishStartTime`: `datetime`
- `BulkPublishCompleteTime`: `datetime`
- `BulkPublishStatus`:
  [BulkPublishStatusType](./literals.md#bulkpublishstatustype)
- `FailureMessage`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getcognitoeventsrequestrequesttypedef"></a>

## GetCognitoEventsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetCognitoEventsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

<a id="getcognitoeventsresponsetypedef"></a>

## GetCognitoEventsResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetCognitoEventsResponseTypeDef
```

Required fields:

- `Events`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getidentitypoolconfigurationrequestrequesttypedef"></a>

## GetIdentityPoolConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetIdentityPoolConfigurationRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

<a id="getidentitypoolconfigurationresponsetypedef"></a>

## GetIdentityPoolConfigurationResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import GetIdentityPoolConfigurationResponseTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `PushSync`: [PushSyncTypeDef](./type_defs.md#pushsynctypedef)
- `CognitoStreams`:
  [CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="identitypoolusagetypedef"></a>

## IdentityPoolUsageTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import IdentityPoolUsageTypeDef
```

Optional fields:

- `IdentityPoolId`: `str`
- `SyncSessionsCount`: `int`
- `DataStorage`: `int`
- `LastModifiedDate`: `datetime`

<a id="identityusagetypedef"></a>

## IdentityUsageTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import IdentityUsageTypeDef
```

Optional fields:

- `IdentityId`: `str`
- `IdentityPoolId`: `str`
- `LastModifiedDate`: `datetime`
- `DatasetCount`: `int`
- `DataStorage`: `int`

<a id="listdatasetsrequestrequesttypedef"></a>

## ListDatasetsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListDatasetsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listdatasetsresponsetypedef"></a>

## ListDatasetsResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListDatasetsResponseTypeDef
```

Required fields:

- `Datasets`: `List`\[[DatasetTypeDef](./type_defs.md#datasettypedef)\]
- `Count`: `int`
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listidentitypoolusagerequestrequesttypedef"></a>

## ListIdentityPoolUsageRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListIdentityPoolUsageRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listidentitypoolusageresponsetypedef"></a>

## ListIdentityPoolUsageResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListIdentityPoolUsageResponseTypeDef
```

Required fields:

- `IdentityPoolUsages`:
  `List`\[[IdentityPoolUsageTypeDef](./type_defs.md#identitypoolusagetypedef)\]
- `MaxResults`: `int`
- `Count`: `int`
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listrecordsrequestrequesttypedef"></a>

## ListRecordsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListRecordsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`

Optional fields:

- `LastSyncCount`: `int`
- `NextToken`: `str`
- `MaxResults`: `int`
- `SyncSessionToken`: `str`

<a id="listrecordsresponsetypedef"></a>

## ListRecordsResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ListRecordsResponseTypeDef
```

Required fields:

- `Records`: `List`\[[RecordTypeDef](./type_defs.md#recordtypedef)\]
- `NextToken`: `str`
- `Count`: `int`
- `DatasetSyncCount`: `int`
- `LastModifiedBy`: `str`
- `MergedDatasetNames`: `List`\[`str`\]
- `DatasetExists`: `bool`
- `DatasetDeletedAfterRequestedSyncCount`: `bool`
- `SyncSessionToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="pushsynctypedef"></a>

## PushSyncTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import PushSyncTypeDef
```

Optional fields:

- `ApplicationArns`: `List`\[`str`\]
- `RoleArn`: `str`

<a id="recordpatchtypedef"></a>

## RecordPatchTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import RecordPatchTypeDef
```

Required fields:

- `Op`: [OperationType](./literals.md#operationtype)
- `Key`: `str`
- `SyncCount`: `int`

Optional fields:

- `Value`: `str`
- `DeviceLastModifiedDate`: `Union`\[`datetime`, `str`\]

<a id="recordtypedef"></a>

## RecordTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import RecordTypeDef
```

Optional fields:

- `Key`: `str`
- `Value`: `str`
- `SyncCount`: `int`
- `LastModifiedDate`: `datetime`
- `LastModifiedBy`: `str`
- `DeviceLastModifiedDate`: `datetime`

<a id="registerdevicerequestrequesttypedef"></a>

## RegisterDeviceRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import RegisterDeviceRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `Platform`: [PlatformType](./literals.md#platformtype)
- `Token`: `str`

<a id="registerdeviceresponsetypedef"></a>

## RegisterDeviceResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import RegisterDeviceResponseTypeDef
```

Required fields:

- `DeviceId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="setcognitoeventsrequestrequesttypedef"></a>

## SetCognitoEventsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import SetCognitoEventsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `Events`: `Mapping`\[`str`, `str`\]

<a id="setidentitypoolconfigurationrequestrequesttypedef"></a>

## SetIdentityPoolConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import SetIdentityPoolConfigurationRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`

Optional fields:

- `PushSync`: [PushSyncTypeDef](./type_defs.md#pushsynctypedef)
- `CognitoStreams`:
  [CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef)

<a id="setidentitypoolconfigurationresponsetypedef"></a>

## SetIdentityPoolConfigurationResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import SetIdentityPoolConfigurationResponseTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `PushSync`: [PushSyncTypeDef](./type_defs.md#pushsynctypedef)
- `CognitoStreams`:
  [CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="subscribetodatasetrequestrequesttypedef"></a>

## SubscribeToDatasetRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import SubscribeToDatasetRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`
- `DeviceId`: `str`

<a id="unsubscribefromdatasetrequestrequesttypedef"></a>

## UnsubscribeFromDatasetRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import UnsubscribeFromDatasetRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`
- `DeviceId`: `str`

<a id="updaterecordsrequestrequesttypedef"></a>

## UpdateRecordsRequestRequestTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import UpdateRecordsRequestRequestTypeDef
```

Required fields:

- `IdentityPoolId`: `str`
- `IdentityId`: `str`
- `DatasetName`: `str`
- `SyncSessionToken`: `str`

Optional fields:

- `DeviceId`: `str`
- `RecordPatches`:
  `Sequence`\[[RecordPatchTypeDef](./type_defs.md#recordpatchtypedef)\]
- `ClientContext`: `str`

<a id="updaterecordsresponsetypedef"></a>

## UpdateRecordsResponseTypeDef

```python
from types_aiobotocore_cognito_sync.type_defs import UpdateRecordsResponseTypeDef
```

Required fields:

- `Records`: `List`\[[RecordTypeDef](./type_defs.md#recordtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
