# Type definitions

> [Index](../README.md) > [DynamoDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## TableAttributeValueTypeDef

```python
# TableAttributeValueTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import TableAttributeValueTypeDef


def get_value() -> TableAttributeValueTypeDef:
    return ...


# TableAttributeValueTypeDef definition

TableAttributeValueTypeDef = Union[
    bytes,
    bytearray,
    str,
    int,
    Decimal,
    bool,
    Set[int],
    Set[Decimal],
    Set[str],
    Set[bytes],
    Set[bytearray],
    Sequence[Any],
    Mapping[str, Any],
    None,
]
```


## ConditionBaseImportTypeDef

```python
# ConditionBaseImportTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import ConditionBaseImportTypeDef


def get_value() -> ConditionBaseImportTypeDef:
    return ...


# ConditionBaseImportTypeDef definition

ConditionBaseImportTypeDef = Union[
    str,
    ConditionBase,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## UniversalAttributeValueTypeDef

```python
# UniversalAttributeValueTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import UniversalAttributeValueTypeDef


def get_value() -> UniversalAttributeValueTypeDef:
    return ...


# UniversalAttributeValueTypeDef definition

UniversalAttributeValueTypeDef = Union[
    AttributeValueTypeDef,  # (1)
    bytes,
    bytearray,
    str,
    int,
    Decimal,
    bool,
    Set[int],
    Set[Decimal],
    Set[str],
    Set[bytes],
    Set[bytearray],
    Sequence[Any],
    Mapping[str, Any],
    None,
]
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 

## ProjectionUnionTypeDef

```python
# ProjectionUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import ProjectionUnionTypeDef


def get_value() -> ProjectionUnionTypeDef:
    return ...


# ProjectionUnionTypeDef definition

ProjectionUnionTypeDef = Union[
    ProjectionTypeDef,  # (1)
    ProjectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 

## DeleteRequestServiceResourceUnionTypeDef

```python
# DeleteRequestServiceResourceUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestServiceResourceUnionTypeDef


def get_value() -> DeleteRequestServiceResourceUnionTypeDef:
    return ...


# DeleteRequestServiceResourceUnionTypeDef definition

DeleteRequestServiceResourceUnionTypeDef = Union[
    DeleteRequestServiceResourceTypeDef,  # (1)
    DeleteRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeleteRequestServiceResourceTypeDef](./type_defs.md#deleterequestserviceresourcetypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 

## KeysAndAttributesServiceResourceUnionTypeDef

```python
# KeysAndAttributesServiceResourceUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesServiceResourceUnionTypeDef


def get_value() -> KeysAndAttributesServiceResourceUnionTypeDef:
    return ...


# KeysAndAttributesServiceResourceUnionTypeDef definition

KeysAndAttributesServiceResourceUnionTypeDef = Union[
    KeysAndAttributesServiceResourceTypeDef,  # (1)
    KeysAndAttributesServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) 
2. See [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 

## PutRequestServiceResourceUnionTypeDef

```python
# PutRequestServiceResourceUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestServiceResourceUnionTypeDef


def get_value() -> PutRequestServiceResourceUnionTypeDef:
    return ...


# PutRequestServiceResourceUnionTypeDef definition

PutRequestServiceResourceUnionTypeDef = Union[
    PutRequestServiceResourceTypeDef,  # (1)
    PutRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PutRequestServiceResourceTypeDef](./type_defs.md#putrequestserviceresourcetypedef) 
2. See [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 

## InputFormatOptionsUnionTypeDef

```python
# InputFormatOptionsUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import InputFormatOptionsUnionTypeDef


def get_value() -> InputFormatOptionsUnionTypeDef:
    return ...


# InputFormatOptionsUnionTypeDef definition

InputFormatOptionsUnionTypeDef = Union[
    InputFormatOptionsTypeDef,  # (1)
    InputFormatOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputFormatOptionsTypeDef](./type_defs.md#inputformatoptionstypedef) 
2. See [:material-code-braces: InputFormatOptionsOutputTypeDef](./type_defs.md#inputformatoptionsoutputtypedef) 

## IncrementalExportSpecificationUnionTypeDef

```python
# IncrementalExportSpecificationUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import IncrementalExportSpecificationUnionTypeDef


def get_value() -> IncrementalExportSpecificationUnionTypeDef:
    return ...


# IncrementalExportSpecificationUnionTypeDef definition

IncrementalExportSpecificationUnionTypeDef = Union[
    IncrementalExportSpecificationTypeDef,  # (1)
    IncrementalExportSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IncrementalExportSpecificationTypeDef](./type_defs.md#incrementalexportspecificationtypedef) 
2. See [:material-code-braces: IncrementalExportSpecificationOutputTypeDef](./type_defs.md#incrementalexportspecificationoutputtypedef) 

## DeleteRequestUnionTypeDef

```python
# DeleteRequestUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestUnionTypeDef


def get_value() -> DeleteRequestUnionTypeDef:
    return ...


# DeleteRequestUnionTypeDef definition

DeleteRequestUnionTypeDef = Union[
    DeleteRequestTypeDef,  # (1)
    DeleteRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef) 
2. See [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 

## KeysAndAttributesUnionTypeDef

```python
# KeysAndAttributesUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesUnionTypeDef


def get_value() -> KeysAndAttributesUnionTypeDef:
    return ...


# KeysAndAttributesUnionTypeDef definition

KeysAndAttributesUnionTypeDef = Union[
    KeysAndAttributesTypeDef,  # (1)
    KeysAndAttributesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) 
2. See [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 

## PutRequestUnionTypeDef

```python
# PutRequestUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestUnionTypeDef


def get_value() -> PutRequestUnionTypeDef:
    return ...


# PutRequestUnionTypeDef definition

PutRequestUnionTypeDef = Union[
    PutRequestTypeDef,  # (1)
    PutRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PutRequestTypeDef](./type_defs.md#putrequesttypedef) 
2. See [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 

## GlobalSecondaryIndexUnionTypeDef

```python
# GlobalSecondaryIndexUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexUnionTypeDef


def get_value() -> GlobalSecondaryIndexUnionTypeDef:
    return ...


# GlobalSecondaryIndexUnionTypeDef definition

GlobalSecondaryIndexUnionTypeDef = Union[
    GlobalSecondaryIndexTypeDef,  # (1)
    GlobalSecondaryIndexOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
2. See [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 

## WriteRequestServiceResourceUnionTypeDef

```python
# WriteRequestServiceResourceUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestServiceResourceUnionTypeDef


def get_value() -> WriteRequestServiceResourceUnionTypeDef:
    return ...


# WriteRequestServiceResourceUnionTypeDef definition

WriteRequestServiceResourceUnionTypeDef = Union[
    WriteRequestServiceResourceTypeDef,  # (1)
    WriteRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) 
2. See [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 

## TableCreationParametersUnionTypeDef

```python
# TableCreationParametersUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import TableCreationParametersUnionTypeDef


def get_value() -> TableCreationParametersUnionTypeDef:
    return ...


# TableCreationParametersUnionTypeDef definition

TableCreationParametersUnionTypeDef = Union[
    TableCreationParametersTypeDef,  # (1)
    TableCreationParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TableCreationParametersTypeDef](./type_defs.md#tablecreationparameterstypedef) 
2. See [:material-code-braces: TableCreationParametersOutputTypeDef](./type_defs.md#tablecreationparametersoutputtypedef) 

## WriteRequestUnionTypeDef

```python
# WriteRequestUnionTypeDef Union usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestUnionTypeDef


def get_value() -> WriteRequestUnionTypeDef:
    return ...


# WriteRequestUnionTypeDef definition

WriteRequestUnionTypeDef = Union[
    WriteRequestTypeDef,  # (1)
    WriteRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) 
2. See [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 



## ArchivalSummaryTypeDef

```python
# ArchivalSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ArchivalSummaryTypeDef


def get_value() -> ArchivalSummaryTypeDef:
    return {
        "ArchivalDateTime": ...,
    }


# ArchivalSummaryTypeDef definition

class ArchivalSummaryTypeDef(TypedDict):
    ArchivalDateTime: NotRequired[datetime],
    ArchivalReason: NotRequired[str],
    ArchivalBackupArn: NotRequired[str],
```

## AttributeDefinitionTypeDef

```python
# AttributeDefinitionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AttributeDefinitionTypeDef


def get_value() -> AttributeDefinitionTypeDef:
    return {
        "AttributeName": ...,
    }


# AttributeDefinitionTypeDef definition

class AttributeDefinitionTypeDef(TypedDict):
    AttributeName: str,
    AttributeType: ScalarAttributeTypeType,  # (1)
```

1. See [:material-code-brackets: ScalarAttributeTypeType](./literals.md#scalarattributetypetype) 
## AttributeValueTypeDef

```python
# AttributeValueTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AttributeValueTypeDef


def get_value() -> AttributeValueTypeDef:
    return {
        "S": ...,
    }


# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[str],
    B: NotRequired[bytes],
    SS: NotRequired[Sequence[str]],
    NS: NotRequired[Sequence[str]],
    BS: NotRequired[Sequence[bytes]],
    M: NotRequired[Mapping[str, Any]],
    L: NotRequired[Sequence[Any]],
    NULL: NotRequired[bool],
    BOOL: NotRequired[bool],
```

## AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef

```python
# AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef


def get_value() -> AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef:
    return {
        "DisableScaleIn": ...,
    }


# AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef definition

class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef

```python
# AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef


def get_value() -> AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef:
    return {
        "DisableScaleIn": ...,
    }


# AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef definition

class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## BackupDetailsTypeDef

```python
# BackupDetailsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BackupDetailsTypeDef


def get_value() -> BackupDetailsTypeDef:
    return {
        "BackupArn": ...,
    }


# BackupDetailsTypeDef definition

class BackupDetailsTypeDef(TypedDict):
    BackupArn: str,
    BackupName: str,
    BackupStatus: BackupStatusType,  # (1)
    BackupType: BackupTypeType,  # (2)
    BackupCreationDateTime: datetime,
    BackupSizeBytes: NotRequired[int],
    BackupExpiryDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
## BackupSummaryTypeDef

```python
# BackupSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BackupSummaryTypeDef


def get_value() -> BackupSummaryTypeDef:
    return {
        "TableName": ...,
    }


# BackupSummaryTypeDef definition

class BackupSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableId: NotRequired[str],
    TableArn: NotRequired[str],
    BackupArn: NotRequired[str],
    BackupName: NotRequired[str],
    BackupCreationDateTime: NotRequired[datetime],
    BackupExpiryDateTime: NotRequired[datetime],
    BackupStatus: NotRequired[BackupStatusType],  # (1)
    BackupType: NotRequired[BackupTypeType],  # (2)
    BackupSizeBytes: NotRequired[int],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ResponseMetadataTypeDef


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

## BillingModeSummaryTypeDef

```python
# BillingModeSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BillingModeSummaryTypeDef


def get_value() -> BillingModeSummaryTypeDef:
    return {
        "BillingMode": ...,
    }


# BillingModeSummaryTypeDef definition

class BillingModeSummaryTypeDef(TypedDict):
    BillingMode: NotRequired[BillingModeType],  # (1)
    LastUpdateToPayPerRequestDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## CapacityTypeDef

```python
# CapacityTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CapacityTypeDef


def get_value() -> CapacityTypeDef:
    return {
        "ReadCapacityUnits": ...,
    }


# CapacityTypeDef definition

class CapacityTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    CapacityUnits: NotRequired[float],
```

## PointInTimeRecoveryDescriptionTypeDef

```python
# PointInTimeRecoveryDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PointInTimeRecoveryDescriptionTypeDef


def get_value() -> PointInTimeRecoveryDescriptionTypeDef:
    return {
        "PointInTimeRecoveryStatus": ...,
    }


# PointInTimeRecoveryDescriptionTypeDef definition

class PointInTimeRecoveryDescriptionTypeDef(TypedDict):
    PointInTimeRecoveryStatus: NotRequired[PointInTimeRecoveryStatusType],  # (1)
    RecoveryPeriodInDays: NotRequired[int],
    EarliestRestorableDateTime: NotRequired[datetime],
    LatestRestorableDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## ContributorInsightsSummaryTypeDef

```python
# ContributorInsightsSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ContributorInsightsSummaryTypeDef


def get_value() -> ContributorInsightsSummaryTypeDef:
    return {
        "TableName": ...,
    }


# ContributorInsightsSummaryTypeDef definition

class ContributorInsightsSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    IndexName: NotRequired[str],
    ContributorInsightsStatus: NotRequired[ContributorInsightsStatusType],  # (1)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
## CreateBackupInputTypeDef

```python
# CreateBackupInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateBackupInputTypeDef


def get_value() -> CreateBackupInputTypeDef:
    return {
        "TableName": ...,
    }


# CreateBackupInputTypeDef definition

class CreateBackupInputTypeDef(TypedDict):
    TableName: str,
    BackupName: str,
```

## KeySchemaElementTypeDef

```python
# KeySchemaElementTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KeySchemaElementTypeDef


def get_value() -> KeySchemaElementTypeDef:
    return {
        "AttributeName": ...,
    }


# KeySchemaElementTypeDef definition

class KeySchemaElementTypeDef(TypedDict):
    AttributeName: str,
    KeyType: KeyTypeType,  # (1)
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## OnDemandThroughputTypeDef

```python
# OnDemandThroughputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import OnDemandThroughputTypeDef


def get_value() -> OnDemandThroughputTypeDef:
    return {
        "MaxReadRequestUnits": ...,
    }


# OnDemandThroughputTypeDef definition

class OnDemandThroughputTypeDef(TypedDict):
    MaxReadRequestUnits: NotRequired[int],
    MaxWriteRequestUnits: NotRequired[int],
```

## ProvisionedThroughputTypeDef

```python
# ProvisionedThroughputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ProvisionedThroughputTypeDef


def get_value() -> ProvisionedThroughputTypeDef:
    return {
        "ReadCapacityUnits": ...,
    }


# ProvisionedThroughputTypeDef definition

class ProvisionedThroughputTypeDef(TypedDict):
    ReadCapacityUnits: int,
    WriteCapacityUnits: int,
```

## WarmThroughputTypeDef

```python
# WarmThroughputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WarmThroughputTypeDef


def get_value() -> WarmThroughputTypeDef:
    return {
        "ReadUnitsPerSecond": ...,
    }


# WarmThroughputTypeDef definition

class WarmThroughputTypeDef(TypedDict):
    ReadUnitsPerSecond: NotRequired[int],
    WriteUnitsPerSecond: NotRequired[int],
```

## ReplicaTypeDef

```python
# ReplicaTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaTypeDef


def get_value() -> ReplicaTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaTypeDef definition

class ReplicaTypeDef(TypedDict):
    RegionName: NotRequired[str],
```

## CreateReplicaActionTypeDef

```python
# CreateReplicaActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateReplicaActionTypeDef


def get_value() -> CreateReplicaActionTypeDef:
    return {
        "RegionName": ...,
    }


# CreateReplicaActionTypeDef definition

class CreateReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## OnDemandThroughputOverrideTypeDef

```python
# OnDemandThroughputOverrideTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import OnDemandThroughputOverrideTypeDef


def get_value() -> OnDemandThroughputOverrideTypeDef:
    return {
        "MaxReadRequestUnits": ...,
    }


# OnDemandThroughputOverrideTypeDef definition

class OnDemandThroughputOverrideTypeDef(TypedDict):
    MaxReadRequestUnits: NotRequired[int],
```

## ProvisionedThroughputOverrideTypeDef

```python
# ProvisionedThroughputOverrideTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ProvisionedThroughputOverrideTypeDef


def get_value() -> ProvisionedThroughputOverrideTypeDef:
    return {
        "ReadCapacityUnits": ...,
    }


# ProvisionedThroughputOverrideTypeDef definition

class ProvisionedThroughputOverrideTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[int],
```

## SSESpecificationTypeDef

```python
# SSESpecificationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import SSESpecificationTypeDef


def get_value() -> SSESpecificationTypeDef:
    return {
        "Enabled": ...,
    }


# SSESpecificationTypeDef definition

class SSESpecificationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SSEType: NotRequired[SSETypeType],  # (1)
    KMSMasterKeyId: NotRequired[str],
```

1. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## StreamSpecificationTypeDef

```python
# StreamSpecificationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import StreamSpecificationTypeDef


def get_value() -> StreamSpecificationTypeDef:
    return {
        "StreamEnabled": ...,
    }


# StreamSpecificationTypeDef definition

class StreamSpecificationTypeDef(TypedDict):
    StreamEnabled: bool,
    StreamViewType: NotRequired[StreamViewTypeType],  # (1)
```

1. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CsvOptionsOutputTypeDef

```python
# CsvOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CsvOptionsOutputTypeDef


def get_value() -> CsvOptionsOutputTypeDef:
    return {
        "Delimiter": ...,
    }


# CsvOptionsOutputTypeDef definition

class CsvOptionsOutputTypeDef(TypedDict):
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[List[str]],
```

## CsvOptionsTypeDef

```python
# CsvOptionsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CsvOptionsTypeDef


def get_value() -> CsvOptionsTypeDef:
    return {
        "Delimiter": ...,
    }


# CsvOptionsTypeDef definition

class CsvOptionsTypeDef(TypedDict):
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[Sequence[str]],
```

## DeleteBackupInputTypeDef

```python
# DeleteBackupInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteBackupInputTypeDef


def get_value() -> DeleteBackupInputTypeDef:
    return {
        "BackupArn": ...,
    }


# DeleteBackupInputTypeDef definition

class DeleteBackupInputTypeDef(TypedDict):
    BackupArn: str,
```

## DeleteGlobalSecondaryIndexActionTypeDef

```python
# DeleteGlobalSecondaryIndexActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteGlobalSecondaryIndexActionTypeDef


def get_value() -> DeleteGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
    }


# DeleteGlobalSecondaryIndexActionTypeDef definition

class DeleteGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
```

## DeleteReplicaActionTypeDef

```python
# DeleteReplicaActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteReplicaActionTypeDef


def get_value() -> DeleteReplicaActionTypeDef:
    return {
        "RegionName": ...,
    }


# DeleteReplicaActionTypeDef definition

class DeleteReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteReplicationGroupMemberActionTypeDef

```python
# DeleteReplicationGroupMemberActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteReplicationGroupMemberActionTypeDef


def get_value() -> DeleteReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }


# DeleteReplicationGroupMemberActionTypeDef definition

class DeleteReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteResourcePolicyInputTypeDef

```python
# DeleteResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteResourcePolicyInputTypeDef


def get_value() -> DeleteResourcePolicyInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# DeleteResourcePolicyInputTypeDef definition

class DeleteResourcePolicyInputTypeDef(TypedDict):
    ResourceArn: str,
    ExpectedRevisionId: NotRequired[str],
```

## DeleteTableInputTypeDef

```python
# DeleteTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteTableInputTypeDef


def get_value() -> DeleteTableInputTypeDef:
    return {
        "TableName": ...,
    }


# DeleteTableInputTypeDef definition

class DeleteTableInputTypeDef(TypedDict):
    TableName: str,
```

## DescribeBackupInputTypeDef

```python
# DescribeBackupInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeBackupInputTypeDef


def get_value() -> DescribeBackupInputTypeDef:
    return {
        "BackupArn": ...,
    }


# DescribeBackupInputTypeDef definition

class DescribeBackupInputTypeDef(TypedDict):
    BackupArn: str,
```

## DescribeContinuousBackupsInputTypeDef

```python
# DescribeContinuousBackupsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeContinuousBackupsInputTypeDef


def get_value() -> DescribeContinuousBackupsInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeContinuousBackupsInputTypeDef definition

class DescribeContinuousBackupsInputTypeDef(TypedDict):
    TableName: str,
```

## DescribeContributorInsightsInputTypeDef

```python
# DescribeContributorInsightsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeContributorInsightsInputTypeDef


def get_value() -> DescribeContributorInsightsInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeContributorInsightsInputTypeDef definition

class DescribeContributorInsightsInputTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
```

## FailureExceptionTypeDef

```python
# FailureExceptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import FailureExceptionTypeDef


def get_value() -> FailureExceptionTypeDef:
    return {
        "ExceptionName": ...,
    }


# FailureExceptionTypeDef definition

class FailureExceptionTypeDef(TypedDict):
    ExceptionName: NotRequired[str],
    ExceptionDescription: NotRequired[str],
```

## EndpointTypeDef

```python
# EndpointTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import EndpointTypeDef


def get_value() -> EndpointTypeDef:
    return {
        "Address": ...,
    }


# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: str,
    CachePeriodInMinutes: int,
```

## DescribeExportInputTypeDef

```python
# DescribeExportInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeExportInputTypeDef


def get_value() -> DescribeExportInputTypeDef:
    return {
        "ExportArn": ...,
    }


# DescribeExportInputTypeDef definition

class DescribeExportInputTypeDef(TypedDict):
    ExportArn: str,
```

## DescribeGlobalTableInputTypeDef

```python
# DescribeGlobalTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeGlobalTableInputTypeDef


def get_value() -> DescribeGlobalTableInputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# DescribeGlobalTableInputTypeDef definition

class DescribeGlobalTableInputTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeGlobalTableSettingsInputTypeDef

```python
# DescribeGlobalTableSettingsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeGlobalTableSettingsInputTypeDef


def get_value() -> DescribeGlobalTableSettingsInputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# DescribeGlobalTableSettingsInputTypeDef definition

class DescribeGlobalTableSettingsInputTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeImportInputTypeDef

```python
# DescribeImportInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeImportInputTypeDef


def get_value() -> DescribeImportInputTypeDef:
    return {
        "ImportArn": ...,
    }


# DescribeImportInputTypeDef definition

class DescribeImportInputTypeDef(TypedDict):
    ImportArn: str,
```

## DescribeKinesisStreamingDestinationInputTypeDef

```python
# DescribeKinesisStreamingDestinationInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeKinesisStreamingDestinationInputTypeDef


def get_value() -> DescribeKinesisStreamingDestinationInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeKinesisStreamingDestinationInputTypeDef definition

class DescribeKinesisStreamingDestinationInputTypeDef(TypedDict):
    TableName: str,
```

## KinesisDataStreamDestinationTypeDef

```python
# KinesisDataStreamDestinationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KinesisDataStreamDestinationTypeDef


def get_value() -> KinesisDataStreamDestinationTypeDef:
    return {
        "StreamArn": ...,
    }


# KinesisDataStreamDestinationTypeDef definition

class KinesisDataStreamDestinationTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    DestinationStatus: NotRequired[DestinationStatusType],  # (1)
    DestinationStatusDescription: NotRequired[str],
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (2)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## DescribeTableInputTypeDef

```python
# DescribeTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableInputTypeDef


def get_value() -> DescribeTableInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeTableInputTypeDef definition

class DescribeTableInputTypeDef(TypedDict):
    TableName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeTableReplicaAutoScalingInputTypeDef

```python
# DescribeTableReplicaAutoScalingInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableReplicaAutoScalingInputTypeDef


def get_value() -> DescribeTableReplicaAutoScalingInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeTableReplicaAutoScalingInputTypeDef definition

class DescribeTableReplicaAutoScalingInputTypeDef(TypedDict):
    TableName: str,
```

## DescribeTimeToLiveInputTypeDef

```python
# DescribeTimeToLiveInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTimeToLiveInputTypeDef


def get_value() -> DescribeTimeToLiveInputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeTimeToLiveInputTypeDef definition

class DescribeTimeToLiveInputTypeDef(TypedDict):
    TableName: str,
```

## TimeToLiveDescriptionTypeDef

```python
# TimeToLiveDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TimeToLiveDescriptionTypeDef


def get_value() -> TimeToLiveDescriptionTypeDef:
    return {
        "TimeToLiveStatus": ...,
    }


# TimeToLiveDescriptionTypeDef definition

class TimeToLiveDescriptionTypeDef(TypedDict):
    TimeToLiveStatus: NotRequired[TimeToLiveStatusType],  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-brackets: TimeToLiveStatusType](./literals.md#timetolivestatustype) 
## EnableKinesisStreamingConfigurationTypeDef

```python
# EnableKinesisStreamingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import EnableKinesisStreamingConfigurationTypeDef


def get_value() -> EnableKinesisStreamingConfigurationTypeDef:
    return {
        "ApproximateCreationDateTimePrecision": ...,
    }


# EnableKinesisStreamingConfigurationTypeDef definition

class EnableKinesisStreamingConfigurationTypeDef(TypedDict):
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (1)
```

1. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## IncrementalExportSpecificationOutputTypeDef

```python
# IncrementalExportSpecificationOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import IncrementalExportSpecificationOutputTypeDef


def get_value() -> IncrementalExportSpecificationOutputTypeDef:
    return {
        "ExportFromTime": ...,
    }


# IncrementalExportSpecificationOutputTypeDef definition

class IncrementalExportSpecificationOutputTypeDef(TypedDict):
    ExportFromTime: NotRequired[datetime],
    ExportToTime: NotRequired[datetime],
    ExportViewType: NotRequired[ExportViewTypeType],  # (1)
```

1. See [:material-code-brackets: ExportViewTypeType](./literals.md#exportviewtypetype) 
## ExportSummaryTypeDef

```python
# ExportSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExportSummaryTypeDef


def get_value() -> ExportSummaryTypeDef:
    return {
        "ExportArn": ...,
    }


# ExportSummaryTypeDef definition

class ExportSummaryTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
    ExportType: NotRequired[ExportTypeType],  # (2)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
## GetResourcePolicyInputTypeDef

```python
# GetResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetResourcePolicyInputTypeDef


def get_value() -> GetResourcePolicyInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# GetResourcePolicyInputTypeDef definition

class GetResourcePolicyInputTypeDef(TypedDict):
    ResourceArn: str,
```

## GlobalSecondaryIndexWarmThroughputDescriptionTypeDef

```python
# GlobalSecondaryIndexWarmThroughputDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexWarmThroughputDescriptionTypeDef


def get_value() -> GlobalSecondaryIndexWarmThroughputDescriptionTypeDef:
    return {
        "ReadUnitsPerSecond": ...,
    }


# GlobalSecondaryIndexWarmThroughputDescriptionTypeDef definition

class GlobalSecondaryIndexWarmThroughputDescriptionTypeDef(TypedDict):
    ReadUnitsPerSecond: NotRequired[int],
    WriteUnitsPerSecond: NotRequired[int],
    Status: NotRequired[IndexStatusType],  # (1)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## ProjectionOutputTypeDef

```python
# ProjectionOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ProjectionOutputTypeDef


def get_value() -> ProjectionOutputTypeDef:
    return {
        "ProjectionType": ...,
    }


# ProjectionOutputTypeDef definition

class ProjectionOutputTypeDef(TypedDict):
    ProjectionType: NotRequired[ProjectionTypeType],  # (1)
    NonKeyAttributes: NotRequired[List[str]],
```

1. See [:material-code-brackets: ProjectionTypeType](./literals.md#projectiontypetype) 
## ProvisionedThroughputDescriptionTypeDef

```python
# ProvisionedThroughputDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ProvisionedThroughputDescriptionTypeDef


def get_value() -> ProvisionedThroughputDescriptionTypeDef:
    return {
        "LastIncreaseDateTime": ...,
    }


# ProvisionedThroughputDescriptionTypeDef definition

class ProvisionedThroughputDescriptionTypeDef(TypedDict):
    LastIncreaseDateTime: NotRequired[datetime],
    LastDecreaseDateTime: NotRequired[datetime],
    NumberOfDecreasesToday: NotRequired[int],
    ReadCapacityUnits: NotRequired[int],
    WriteCapacityUnits: NotRequired[int],
```

## S3BucketSourceTypeDef

```python
# S3BucketSourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import S3BucketSourceTypeDef


def get_value() -> S3BucketSourceTypeDef:
    return {
        "S3BucketOwner": ...,
    }


# S3BucketSourceTypeDef definition

class S3BucketSourceTypeDef(TypedDict):
    S3Bucket: str,
    S3BucketOwner: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PaginatorConfigTypeDef


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

## ListContributorInsightsInputTypeDef

```python
# ListContributorInsightsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListContributorInsightsInputTypeDef


def get_value() -> ListContributorInsightsInputTypeDef:
    return {
        "TableName": ...,
    }


# ListContributorInsightsInputTypeDef definition

class ListContributorInsightsInputTypeDef(TypedDict):
    TableName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListExportsInputTypeDef

```python
# ListExportsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListExportsInputTypeDef


def get_value() -> ListExportsInputTypeDef:
    return {
        "TableArn": ...,
    }


# ListExportsInputTypeDef definition

class ListExportsInputTypeDef(TypedDict):
    TableArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGlobalTablesInputTypeDef

```python
# ListGlobalTablesInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListGlobalTablesInputTypeDef


def get_value() -> ListGlobalTablesInputTypeDef:
    return {
        "ExclusiveStartGlobalTableName": ...,
    }


# ListGlobalTablesInputTypeDef definition

class ListGlobalTablesInputTypeDef(TypedDict):
    ExclusiveStartGlobalTableName: NotRequired[str],
    Limit: NotRequired[int],
    RegionName: NotRequired[str],
```

## ListImportsInputTypeDef

```python
# ListImportsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListImportsInputTypeDef


def get_value() -> ListImportsInputTypeDef:
    return {
        "TableArn": ...,
    }


# ListImportsInputTypeDef definition

class ListImportsInputTypeDef(TypedDict):
    TableArn: NotRequired[str],
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTablesInputTypeDef

```python
# ListTablesInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTablesInputTypeDef


def get_value() -> ListTablesInputTypeDef:
    return {
        "ExclusiveStartTableName": ...,
    }


# ListTablesInputTypeDef definition

class ListTablesInputTypeDef(TypedDict):
    ExclusiveStartTableName: NotRequired[str],
    Limit: NotRequired[int],
```

## ListTagsOfResourceInputTypeDef

```python
# ListTagsOfResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTagsOfResourceInputTypeDef


def get_value() -> ListTagsOfResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsOfResourceInputTypeDef definition

class ListTagsOfResourceInputTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
```

## PointInTimeRecoverySpecificationTypeDef

```python
# PointInTimeRecoverySpecificationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PointInTimeRecoverySpecificationTypeDef


def get_value() -> PointInTimeRecoverySpecificationTypeDef:
    return {
        "PointInTimeRecoveryEnabled": ...,
    }


# PointInTimeRecoverySpecificationTypeDef definition

class PointInTimeRecoverySpecificationTypeDef(TypedDict):
    PointInTimeRecoveryEnabled: bool,
    RecoveryPeriodInDays: NotRequired[int],
```

## ProjectionTypeDef

```python
# ProjectionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ProjectionTypeDef


def get_value() -> ProjectionTypeDef:
    return {
        "ProjectionType": ...,
    }


# ProjectionTypeDef definition

class ProjectionTypeDef(TypedDict):
    ProjectionType: NotRequired[ProjectionTypeType],  # (1)
    NonKeyAttributes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ProjectionTypeType](./literals.md#projectiontypetype) 
## PutResourcePolicyInputTypeDef

```python
# PutResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutResourcePolicyInputTypeDef


def get_value() -> PutResourcePolicyInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# PutResourcePolicyInputTypeDef definition

class PutResourcePolicyInputTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    ExpectedRevisionId: NotRequired[str],
    ConfirmRemoveSelfResourceAccess: NotRequired[bool],
```

## TableClassSummaryTypeDef

```python
# TableClassSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableClassSummaryTypeDef


def get_value() -> TableClassSummaryTypeDef:
    return {
        "TableClass": ...,
    }


# TableClassSummaryTypeDef definition

class TableClassSummaryTypeDef(TypedDict):
    TableClass: NotRequired[TableClassType],  # (1)
    LastUpdateDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## TableWarmThroughputDescriptionTypeDef

```python
# TableWarmThroughputDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableWarmThroughputDescriptionTypeDef


def get_value() -> TableWarmThroughputDescriptionTypeDef:
    return {
        "ReadUnitsPerSecond": ...,
    }


# TableWarmThroughputDescriptionTypeDef definition

class TableWarmThroughputDescriptionTypeDef(TypedDict):
    ReadUnitsPerSecond: NotRequired[int],
    WriteUnitsPerSecond: NotRequired[int],
    Status: NotRequired[TableStatusType],  # (1)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
## RestoreSummaryTypeDef

```python
# RestoreSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import RestoreSummaryTypeDef


def get_value() -> RestoreSummaryTypeDef:
    return {
        "SourceBackupArn": ...,
    }


# RestoreSummaryTypeDef definition

class RestoreSummaryTypeDef(TypedDict):
    RestoreDateTime: datetime,
    RestoreInProgress: bool,
    SourceBackupArn: NotRequired[str],
    SourceTableArn: NotRequired[str],
```

## SSEDescriptionTypeDef

```python
# SSEDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import SSEDescriptionTypeDef


def get_value() -> SSEDescriptionTypeDef:
    return {
        "Status": ...,
    }


# SSEDescriptionTypeDef definition

class SSEDescriptionTypeDef(TypedDict):
    Status: NotRequired[SSEStatusType],  # (1)
    SSEType: NotRequired[SSETypeType],  # (2)
    KMSMasterKeyArn: NotRequired[str],
    InaccessibleEncryptionDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SSEStatusType](./literals.md#ssestatustype) 
2. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## TableBatchWriterRequestTypeDef

```python
# TableBatchWriterRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableBatchWriterRequestTypeDef


def get_value() -> TableBatchWriterRequestTypeDef:
    return {
        "overwrite_by_pkeys": ...,
    }


# TableBatchWriterRequestTypeDef definition

class TableBatchWriterRequestTypeDef(TypedDict):
    overwrite_by_pkeys: NotRequired[List[str]],
```

## TimeToLiveSpecificationTypeDef

```python
# TimeToLiveSpecificationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TimeToLiveSpecificationTypeDef


def get_value() -> TimeToLiveSpecificationTypeDef:
    return {
        "Enabled": ...,
    }


# TimeToLiveSpecificationTypeDef definition

class TimeToLiveSpecificationTypeDef(TypedDict):
    Enabled: bool,
    AttributeName: str,
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateContributorInsightsInputTypeDef

```python
# UpdateContributorInsightsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateContributorInsightsInputTypeDef


def get_value() -> UpdateContributorInsightsInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateContributorInsightsInputTypeDef definition

class UpdateContributorInsightsInputTypeDef(TypedDict):
    TableName: str,
    ContributorInsightsAction: ContributorInsightsActionType,  # (1)
    IndexName: NotRequired[str],
```

1. See [:material-code-brackets: ContributorInsightsActionType](./literals.md#contributorinsightsactiontype) 
## UpdateKinesisStreamingConfigurationTypeDef

```python
# UpdateKinesisStreamingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateKinesisStreamingConfigurationTypeDef


def get_value() -> UpdateKinesisStreamingConfigurationTypeDef:
    return {
        "ApproximateCreationDateTimePrecision": ...,
    }


# UpdateKinesisStreamingConfigurationTypeDef definition

class UpdateKinesisStreamingConfigurationTypeDef(TypedDict):
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (1)
```

1. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## BatchStatementErrorTypeDef

```python
# BatchStatementErrorTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchStatementErrorTypeDef


def get_value() -> BatchStatementErrorTypeDef:
    return {
        "Code": ...,
    }


# BatchStatementErrorTypeDef definition

class BatchStatementErrorTypeDef(TypedDict):
    Code: NotRequired[BatchStatementErrorCodeEnumType],  # (1)
    Message: NotRequired[str],
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-brackets: BatchStatementErrorCodeEnumType](./literals.md#batchstatementerrorcodeenumtype) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## DeleteRequestOutputTypeDef

```python
# DeleteRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestOutputTypeDef


def get_value() -> DeleteRequestOutputTypeDef:
    return {
        "Key": ...,
    }


# DeleteRequestOutputTypeDef definition

class DeleteRequestOutputTypeDef(TypedDict):
    Key: Dict[str, AttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ItemCollectionMetricsTypeDef

```python
# ItemCollectionMetricsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ItemCollectionMetricsTypeDef


def get_value() -> ItemCollectionMetricsTypeDef:
    return {
        "ItemCollectionKey": ...,
    }


# ItemCollectionMetricsTypeDef definition

class ItemCollectionMetricsTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
    SizeEstimateRangeGB: NotRequired[List[float]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ItemResponseTypeDef

```python
# ItemResponseTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ItemResponseTypeDef


def get_value() -> ItemResponseTypeDef:
    return {
        "Item": ...,
    }


# ItemResponseTypeDef definition

class ItemResponseTypeDef(TypedDict):
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## KeysAndAttributesOutputTypeDef

```python
# KeysAndAttributesOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesOutputTypeDef


def get_value() -> KeysAndAttributesOutputTypeDef:
    return {
        "Keys": ...,
    }


# KeysAndAttributesOutputTypeDef definition

class KeysAndAttributesOutputTypeDef(TypedDict):
    Keys: List[Dict[str, AttributeValueTypeDef]],  # (1)
    AttributesToGet: NotRequired[List[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## PutRequestOutputTypeDef

```python
# PutRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestOutputTypeDef


def get_value() -> PutRequestOutputTypeDef:
    return {
        "Item": ...,
    }


# PutRequestOutputTypeDef definition

class PutRequestOutputTypeDef(TypedDict):
    Item: Dict[str, AttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## AttributeValueUpdateTableTypeDef

```python
# AttributeValueUpdateTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AttributeValueUpdateTableTypeDef


def get_value() -> AttributeValueUpdateTableTypeDef:
    return {
        "Value": ...,
    }


# AttributeValueUpdateTableTypeDef definition

class AttributeValueUpdateTableTypeDef(TypedDict):
    Value: NotRequired[TableAttributeValueTypeDef],
    Action: NotRequired[AttributeActionType],  # (1)
```

1. See [:material-code-brackets: AttributeActionType](./literals.md#attributeactiontype) 
## ConditionTableTypeDef

```python
# ConditionTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ConditionTableTypeDef


def get_value() -> ConditionTableTypeDef:
    return {
        "AttributeValueList": ...,
    }


# ConditionTableTypeDef definition

class ConditionTableTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AttributeValueList: NotRequired[Sequence[TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## DeleteRequestServiceResourceOutputTypeDef

```python
# DeleteRequestServiceResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestServiceResourceOutputTypeDef


def get_value() -> DeleteRequestServiceResourceOutputTypeDef:
    return {
        "Key": ...,
    }


# DeleteRequestServiceResourceOutputTypeDef definition

class DeleteRequestServiceResourceOutputTypeDef(TypedDict):
    Key: Dict[str, TableAttributeValueTypeDef],
```

## DeleteRequestServiceResourceTypeDef

```python
# DeleteRequestServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestServiceResourceTypeDef


def get_value() -> DeleteRequestServiceResourceTypeDef:
    return {
        "Key": ...,
    }


# DeleteRequestServiceResourceTypeDef definition

class DeleteRequestServiceResourceTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
```

## ExpectedAttributeValueTableTypeDef

```python
# ExpectedAttributeValueTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExpectedAttributeValueTableTypeDef


def get_value() -> ExpectedAttributeValueTableTypeDef:
    return {
        "Value": ...,
    }


# ExpectedAttributeValueTableTypeDef definition

class ExpectedAttributeValueTableTypeDef(TypedDict):
    Value: NotRequired[TableAttributeValueTypeDef],
    Exists: NotRequired[bool],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
    AttributeValueList: NotRequired[Sequence[TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## GetItemInputTableGetItemTypeDef

```python
# GetItemInputTableGetItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetItemInputTableGetItemTypeDef


def get_value() -> GetItemInputTableGetItemTypeDef:
    return {
        "Key": ...,
    }


# GetItemInputTableGetItemTypeDef definition

class GetItemInputTableGetItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (1)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ItemCollectionMetricsServiceResourceTypeDef

```python
# ItemCollectionMetricsServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ItemCollectionMetricsServiceResourceTypeDef


def get_value() -> ItemCollectionMetricsServiceResourceTypeDef:
    return {
        "ItemCollectionKey": ...,
    }


# ItemCollectionMetricsServiceResourceTypeDef definition

class ItemCollectionMetricsServiceResourceTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
    SizeEstimateRangeGB: NotRequired[List[float]],
```

## ItemCollectionMetricsTableTypeDef

```python
# ItemCollectionMetricsTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ItemCollectionMetricsTableTypeDef


def get_value() -> ItemCollectionMetricsTableTypeDef:
    return {
        "ItemCollectionKey": ...,
    }


# ItemCollectionMetricsTableTypeDef definition

class ItemCollectionMetricsTableTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
    SizeEstimateRangeGB: NotRequired[List[float]],
```

## KeysAndAttributesServiceResourceOutputTypeDef

```python
# KeysAndAttributesServiceResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesServiceResourceOutputTypeDef


def get_value() -> KeysAndAttributesServiceResourceOutputTypeDef:
    return {
        "Keys": ...,
    }


# KeysAndAttributesServiceResourceOutputTypeDef definition

class KeysAndAttributesServiceResourceOutputTypeDef(TypedDict):
    Keys: List[Dict[str, TableAttributeValueTypeDef]],
    AttributesToGet: NotRequired[List[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Dict[str, str]],
```

## KeysAndAttributesServiceResourceTypeDef

```python
# KeysAndAttributesServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesServiceResourceTypeDef


def get_value() -> KeysAndAttributesServiceResourceTypeDef:
    return {
        "Keys": ...,
    }


# KeysAndAttributesServiceResourceTypeDef definition

class KeysAndAttributesServiceResourceTypeDef(TypedDict):
    Keys: Sequence[Mapping[str, TableAttributeValueTypeDef]],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

## PutRequestServiceResourceOutputTypeDef

```python
# PutRequestServiceResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestServiceResourceOutputTypeDef


def get_value() -> PutRequestServiceResourceOutputTypeDef:
    return {
        "Item": ...,
    }


# PutRequestServiceResourceOutputTypeDef definition

class PutRequestServiceResourceOutputTypeDef(TypedDict):
    Item: Dict[str, TableAttributeValueTypeDef],
```

## PutRequestServiceResourceTypeDef

```python
# PutRequestServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestServiceResourceTypeDef


def get_value() -> PutRequestServiceResourceTypeDef:
    return {
        "Item": ...,
    }


# PutRequestServiceResourceTypeDef definition

class PutRequestServiceResourceTypeDef(TypedDict):
    Item: Mapping[str, TableAttributeValueTypeDef],
```

## AutoScalingPolicyDescriptionTypeDef

```python
# AutoScalingPolicyDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingPolicyDescriptionTypeDef


def get_value() -> AutoScalingPolicyDescriptionTypeDef:
    return {
        "PolicyName": ...,
    }


# AutoScalingPolicyDescriptionTypeDef definition

class AutoScalingPolicyDescriptionTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    TargetTrackingScalingPolicyConfiguration: NotRequired[AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationdescriptiontypedef) 
## AutoScalingPolicyUpdateTypeDef

```python
# AutoScalingPolicyUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingPolicyUpdateTypeDef


def get_value() -> AutoScalingPolicyUpdateTypeDef:
    return {
        "PolicyName": ...,
    }


# AutoScalingPolicyUpdateTypeDef definition

class AutoScalingPolicyUpdateTypeDef(TypedDict):
    TargetTrackingScalingPolicyConfiguration: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,  # (1)
    PolicyName: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationupdatetypedef) 
## CreateBackupOutputTypeDef

```python
# CreateBackupOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateBackupOutputTypeDef


def get_value() -> CreateBackupOutputTypeDef:
    return {
        "BackupDetails": ...,
    }


# CreateBackupOutputTypeDef definition

class CreateBackupOutputTypeDef(TypedDict):
    BackupDetails: BackupDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyOutputTypeDef

```python
# DeleteResourcePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteResourcePolicyOutputTypeDef


def get_value() -> DeleteResourcePolicyOutputTypeDef:
    return {
        "RevisionId": ...,
    }


# DeleteResourcePolicyOutputTypeDef definition

class DeleteResourcePolicyOutputTypeDef(TypedDict):
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLimitsOutputTypeDef

```python
# DescribeLimitsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeLimitsOutputTypeDef


def get_value() -> DescribeLimitsOutputTypeDef:
    return {
        "AccountMaxReadCapacityUnits": ...,
    }


# DescribeLimitsOutputTypeDef definition

class DescribeLimitsOutputTypeDef(TypedDict):
    AccountMaxReadCapacityUnits: int,
    AccountMaxWriteCapacityUnits: int,
    TableMaxReadCapacityUnits: int,
    TableMaxWriteCapacityUnits: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyOutputTypeDef

```python
# GetResourcePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetResourcePolicyOutputTypeDef


def get_value() -> GetResourcePolicyOutputTypeDef:
    return {
        "Policy": ...,
    }


# GetResourcePolicyOutputTypeDef definition

class GetResourcePolicyOutputTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupsOutputTypeDef

```python
# ListBackupsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListBackupsOutputTypeDef


def get_value() -> ListBackupsOutputTypeDef:
    return {
        "BackupSummaries": ...,
    }


# ListBackupsOutputTypeDef definition

class ListBackupsOutputTypeDef(TypedDict):
    BackupSummaries: List[BackupSummaryTypeDef],  # (1)
    LastEvaluatedBackupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSummaryTypeDef](./type_defs.md#backupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesOutputTypeDef

```python
# ListTablesOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTablesOutputTypeDef


def get_value() -> ListTablesOutputTypeDef:
    return {
        "TableNames": ...,
    }


# ListTablesOutputTypeDef definition

class ListTablesOutputTypeDef(TypedDict):
    TableNames: List[str],
    LastEvaluatedTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyOutputTypeDef

```python
# PutResourcePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutResourcePolicyOutputTypeDef


def get_value() -> PutResourcePolicyOutputTypeDef:
    return {
        "RevisionId": ...,
    }


# PutResourcePolicyOutputTypeDef definition

class PutResourcePolicyOutputTypeDef(TypedDict):
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContributorInsightsOutputTypeDef

```python
# UpdateContributorInsightsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateContributorInsightsOutputTypeDef


def get_value() -> UpdateContributorInsightsOutputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateContributorInsightsOutputTypeDef definition

class UpdateContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConsumedCapacityTypeDef

```python
# ConsumedCapacityTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ConsumedCapacityTypeDef


def get_value() -> ConsumedCapacityTypeDef:
    return {
        "TableName": ...,
    }


# ConsumedCapacityTypeDef definition

class ConsumedCapacityTypeDef(TypedDict):
    TableName: NotRequired[str],
    CapacityUnits: NotRequired[float],
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    Table: NotRequired[CapacityTypeDef],  # (1)
    LocalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
    GlobalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
3. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
## ContinuousBackupsDescriptionTypeDef

```python
# ContinuousBackupsDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ContinuousBackupsDescriptionTypeDef


def get_value() -> ContinuousBackupsDescriptionTypeDef:
    return {
        "ContinuousBackupsStatus": ...,
    }


# ContinuousBackupsDescriptionTypeDef definition

class ContinuousBackupsDescriptionTypeDef(TypedDict):
    ContinuousBackupsStatus: ContinuousBackupsStatusType,  # (1)
    PointInTimeRecoveryDescription: NotRequired[PointInTimeRecoveryDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: ContinuousBackupsStatusType](./literals.md#continuousbackupsstatustype) 
2. See [:material-code-braces: PointInTimeRecoveryDescriptionTypeDef](./type_defs.md#pointintimerecoverydescriptiontypedef) 
## ListContributorInsightsOutputTypeDef

```python
# ListContributorInsightsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListContributorInsightsOutputTypeDef


def get_value() -> ListContributorInsightsOutputTypeDef:
    return {
        "ContributorInsightsSummaries": ...,
    }


# ListContributorInsightsOutputTypeDef definition

class ListContributorInsightsOutputTypeDef(TypedDict):
    ContributorInsightsSummaries: List[ContributorInsightsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContributorInsightsSummaryTypeDef](./type_defs.md#contributorinsightssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceTableDetailsTypeDef

```python
# SourceTableDetailsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import SourceTableDetailsTypeDef


def get_value() -> SourceTableDetailsTypeDef:
    return {
        "TableName": ...,
    }


# SourceTableDetailsTypeDef definition

class SourceTableDetailsTypeDef(TypedDict):
    TableName: str,
    TableId: str,
    KeySchema: List[KeySchemaElementTypeDef],  # (1)
    TableCreationDateTime: datetime,
    ProvisionedThroughput: ProvisionedThroughputTypeDef,  # (2)
    TableArn: NotRequired[str],
    TableSizeBytes: NotRequired[int],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (3)
    ItemCount: NotRequired[int],
    BillingMode: NotRequired[BillingModeType],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
3. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
4. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## UpdateGlobalSecondaryIndexActionTypeDef

```python
# UpdateGlobalSecondaryIndexActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateGlobalSecondaryIndexActionTypeDef


def get_value() -> UpdateGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
    }


# UpdateGlobalSecondaryIndexActionTypeDef definition

class UpdateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (2)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (3)
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
2. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
3. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## CreateGlobalTableInputTypeDef

```python
# CreateGlobalTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateGlobalTableInputTypeDef


def get_value() -> CreateGlobalTableInputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# CreateGlobalTableInputTypeDef definition

class CreateGlobalTableInputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicationGroup: Sequence[ReplicaTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## GlobalTableTypeDef

```python
# GlobalTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalTableTypeDef


def get_value() -> GlobalTableTypeDef:
    return {
        "GlobalTableName": ...,
    }


# GlobalTableTypeDef definition

class GlobalTableTypeDef(TypedDict):
    GlobalTableName: NotRequired[str],
    ReplicationGroup: NotRequired[List[ReplicaTypeDef]],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## ReplicaGlobalSecondaryIndexTypeDef

```python
# ReplicaGlobalSecondaryIndexTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexTypeDef definition

class ReplicaGlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
## ListTagsOfResourceOutputTypeDef

```python
# ListTagsOfResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTagsOfResourceOutputTypeDef


def get_value() -> ListTagsOfResourceOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsOfResourceOutputTypeDef definition

class ListTagsOfResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InputFormatOptionsOutputTypeDef

```python
# InputFormatOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import InputFormatOptionsOutputTypeDef


def get_value() -> InputFormatOptionsOutputTypeDef:
    return {
        "Csv": ...,
    }


# InputFormatOptionsOutputTypeDef definition

class InputFormatOptionsOutputTypeDef(TypedDict):
    Csv: NotRequired[CsvOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CsvOptionsOutputTypeDef](./type_defs.md#csvoptionsoutputtypedef) 
## InputFormatOptionsTypeDef

```python
# InputFormatOptionsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import InputFormatOptionsTypeDef


def get_value() -> InputFormatOptionsTypeDef:
    return {
        "Csv": ...,
    }


# InputFormatOptionsTypeDef definition

class InputFormatOptionsTypeDef(TypedDict):
    Csv: NotRequired[CsvOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef) 
## ReplicaUpdateTypeDef

```python
# ReplicaUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaUpdateTypeDef


def get_value() -> ReplicaUpdateTypeDef:
    return {
        "Create": ...,
    }


# ReplicaUpdateTypeDef definition

class ReplicaUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicaActionTypeDef],  # (1)
    Delete: NotRequired[DeleteReplicaActionTypeDef],  # (2)
```

1. See [:material-code-braces: CreateReplicaActionTypeDef](./type_defs.md#createreplicaactiontypedef) 
2. See [:material-code-braces: DeleteReplicaActionTypeDef](./type_defs.md#deletereplicaactiontypedef) 
## DescribeContributorInsightsOutputTypeDef

```python
# DescribeContributorInsightsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeContributorInsightsOutputTypeDef


def get_value() -> DescribeContributorInsightsOutputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeContributorInsightsOutputTypeDef definition

class DescribeContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsRuleList: List[str],
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    LastUpdateDateTime: datetime,
    FailureException: FailureExceptionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: FailureExceptionTypeDef](./type_defs.md#failureexceptiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeEndpointsResponseTypeDef


def get_value() -> DescribeEndpointsResponseTypeDef:
    return {
        "Endpoints": ...,
    }


# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKinesisStreamingDestinationOutputTypeDef

```python
# DescribeKinesisStreamingDestinationOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeKinesisStreamingDestinationOutputTypeDef


def get_value() -> DescribeKinesisStreamingDestinationOutputTypeDef:
    return {
        "TableName": ...,
    }


# DescribeKinesisStreamingDestinationOutputTypeDef definition

class DescribeKinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    KinesisDataStreamDestinations: List[KinesisDataStreamDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KinesisDataStreamDestinationTypeDef](./type_defs.md#kinesisdatastreamdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableInputWaitExtraTypeDef

```python
# DescribeTableInputWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableInputWaitExtraTypeDef


def get_value() -> DescribeTableInputWaitExtraTypeDef:
    return {
        "TableName": ...,
    }


# DescribeTableInputWaitExtraTypeDef definition

class DescribeTableInputWaitExtraTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTableInputWaitTypeDef

```python
# DescribeTableInputWaitTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableInputWaitTypeDef


def get_value() -> DescribeTableInputWaitTypeDef:
    return {
        "TableName": ...,
    }


# DescribeTableInputWaitTypeDef definition

class DescribeTableInputWaitTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTimeToLiveOutputTypeDef

```python
# DescribeTimeToLiveOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTimeToLiveOutputTypeDef


def get_value() -> DescribeTimeToLiveOutputTypeDef:
    return {
        "TimeToLiveDescription": ...,
    }


# DescribeTimeToLiveOutputTypeDef definition

class DescribeTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveDescription: TimeToLiveDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KinesisStreamingDestinationInputRequestTypeDef

```python
# KinesisStreamingDestinationInputRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KinesisStreamingDestinationInputRequestTypeDef


def get_value() -> KinesisStreamingDestinationInputRequestTypeDef:
    return {
        "TableName": ...,
    }


# KinesisStreamingDestinationInputRequestTypeDef definition

class KinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    EnableKinesisStreamingConfiguration: NotRequired[EnableKinesisStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef) 
## KinesisStreamingDestinationInputTypeDef

```python
# KinesisStreamingDestinationInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KinesisStreamingDestinationInputTypeDef


def get_value() -> KinesisStreamingDestinationInputTypeDef:
    return {
        "TableName": ...,
    }


# KinesisStreamingDestinationInputTypeDef definition

class KinesisStreamingDestinationInputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    EnableKinesisStreamingConfiguration: NotRequired[EnableKinesisStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef) 
## KinesisStreamingDestinationOutputTypeDef

```python
# KinesisStreamingDestinationOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KinesisStreamingDestinationOutputTypeDef


def get_value() -> KinesisStreamingDestinationOutputTypeDef:
    return {
        "TableName": ...,
    }


# KinesisStreamingDestinationOutputTypeDef definition

class KinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    DestinationStatus: DestinationStatusType,  # (1)
    EnableKinesisStreamingConfiguration: EnableKinesisStreamingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-braces: EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportDescriptionTypeDef

```python
# ExportDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExportDescriptionTypeDef


def get_value() -> ExportDescriptionTypeDef:
    return {
        "ExportArn": ...,
    }


# ExportDescriptionTypeDef definition

class ExportDescriptionTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ExportManifest: NotRequired[str],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    ExportTime: NotRequired[datetime],
    ClientToken: NotRequired[str],
    S3Bucket: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (2)
    S3SseKmsKeyId: NotRequired[str],
    FailureCode: NotRequired[str],
    FailureMessage: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (3)
    BilledSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    ExportType: NotRequired[ExportTypeType],  # (4)
    IncrementalExportSpecification: NotRequired[IncrementalExportSpecificationOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
3. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
4. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
5. See [:material-code-braces: IncrementalExportSpecificationOutputTypeDef](./type_defs.md#incrementalexportspecificationoutputtypedef) 
## ListExportsOutputTypeDef

```python
# ListExportsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListExportsOutputTypeDef


def get_value() -> ListExportsOutputTypeDef:
    return {
        "ExportSummaries": ...,
    }


# ListExportsOutputTypeDef definition

class ListExportsOutputTypeDef(TypedDict):
    ExportSummaries: List[ExportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncrementalExportSpecificationTypeDef

```python
# IncrementalExportSpecificationTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import IncrementalExportSpecificationTypeDef


def get_value() -> IncrementalExportSpecificationTypeDef:
    return {
        "ExportFromTime": ...,
    }


# IncrementalExportSpecificationTypeDef definition

class IncrementalExportSpecificationTypeDef(TypedDict):
    ExportFromTime: NotRequired[TimestampTypeDef],
    ExportToTime: NotRequired[TimestampTypeDef],
    ExportViewType: NotRequired[ExportViewTypeType],  # (1)
```

1. See [:material-code-brackets: ExportViewTypeType](./literals.md#exportviewtypetype) 
## ListBackupsInputTypeDef

```python
# ListBackupsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListBackupsInputTypeDef


def get_value() -> ListBackupsInputTypeDef:
    return {
        "TableName": ...,
    }


# ListBackupsInputTypeDef definition

class ListBackupsInputTypeDef(TypedDict):
    TableName: NotRequired[str],
    Limit: NotRequired[int],
    TimeRangeLowerBound: NotRequired[TimestampTypeDef],
    TimeRangeUpperBound: NotRequired[TimestampTypeDef],
    ExclusiveStartBackupArn: NotRequired[str],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
## ReplicaGlobalSecondaryIndexDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexDescriptionTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
    WarmThroughput: NotRequired[GlobalSecondaryIndexWarmThroughputDescriptionTypeDef],  # (3)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
3. See [:material-code-braces: GlobalSecondaryIndexWarmThroughputDescriptionTypeDef](./type_defs.md#globalsecondaryindexwarmthroughputdescriptiontypedef) 
## GlobalSecondaryIndexInfoTypeDef

```python
# GlobalSecondaryIndexInfoTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexInfoTypeDef


def get_value() -> GlobalSecondaryIndexInfoTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalSecondaryIndexInfoTypeDef definition

class GlobalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## GlobalSecondaryIndexOutputTypeDef

```python
# GlobalSecondaryIndexOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexOutputTypeDef


def get_value() -> GlobalSecondaryIndexOutputTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalSecondaryIndexOutputTypeDef definition

class GlobalSecondaryIndexOutputTypeDef(TypedDict):
    IndexName: str,
    KeySchema: List[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionOutputTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (5)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
5. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## LocalSecondaryIndexDescriptionTypeDef

```python
# LocalSecondaryIndexDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import LocalSecondaryIndexDescriptionTypeDef


def get_value() -> LocalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }


# LocalSecondaryIndexDescriptionTypeDef definition

class LocalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## LocalSecondaryIndexInfoTypeDef

```python
# LocalSecondaryIndexInfoTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import LocalSecondaryIndexInfoTypeDef


def get_value() -> LocalSecondaryIndexInfoTypeDef:
    return {
        "IndexName": ...,
    }


# LocalSecondaryIndexInfoTypeDef definition

class LocalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## GlobalSecondaryIndexDescriptionTypeDef

```python
# GlobalSecondaryIndexDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexDescriptionTypeDef


def get_value() -> GlobalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalSecondaryIndexDescriptionTypeDef definition

class GlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    IndexStatus: NotRequired[IndexStatusType],  # (3)
    Backfilling: NotRequired[bool],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
    WarmThroughput: NotRequired[GlobalSecondaryIndexWarmThroughputDescriptionTypeDef],  # (6)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: GlobalSecondaryIndexWarmThroughputDescriptionTypeDef](./type_defs.md#globalsecondaryindexwarmthroughputdescriptiontypedef) 
## ImportSummaryTypeDef

```python
# ImportSummaryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ImportSummaryTypeDef


def get_value() -> ImportSummaryTypeDef:
    return {
        "ImportArn": ...,
    }


# ImportSummaryTypeDef definition

class ImportSummaryTypeDef(TypedDict):
    ImportArn: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    TableArn: NotRequired[str],
    S3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (2)
    CloudWatchLogGroupArn: NotRequired[str],
    InputFormat: NotRequired[InputFormatType],  # (3)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
3. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
## ListBackupsInputPaginateTypeDef

```python
# ListBackupsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListBackupsInputPaginateTypeDef


def get_value() -> ListBackupsInputPaginateTypeDef:
    return {
        "TableName": ...,
    }


# ListBackupsInputPaginateTypeDef definition

class ListBackupsInputPaginateTypeDef(TypedDict):
    TableName: NotRequired[str],
    TimeRangeLowerBound: NotRequired[TimestampTypeDef],
    TimeRangeUpperBound: NotRequired[TimestampTypeDef],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesInputPaginateTypeDef

```python
# ListTablesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTablesInputPaginateTypeDef


def get_value() -> ListTablesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListTablesInputPaginateTypeDef definition

class ListTablesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsOfResourceInputPaginateTypeDef

```python
# ListTagsOfResourceInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListTagsOfResourceInputPaginateTypeDef


def get_value() -> ListTagsOfResourceInputPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsOfResourceInputPaginateTypeDef definition

class ListTagsOfResourceInputPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## UpdateContinuousBackupsInputTypeDef

```python
# UpdateContinuousBackupsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateContinuousBackupsInputTypeDef


def get_value() -> UpdateContinuousBackupsInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateContinuousBackupsInputTypeDef definition

class UpdateContinuousBackupsInputTypeDef(TypedDict):
    TableName: str,
    PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: PointInTimeRecoverySpecificationTypeDef](./type_defs.md#pointintimerecoveryspecificationtypedef) 
## UpdateTimeToLiveInputTypeDef

```python
# UpdateTimeToLiveInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTimeToLiveInputTypeDef


def get_value() -> UpdateTimeToLiveInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateTimeToLiveInputTypeDef definition

class UpdateTimeToLiveInputTypeDef(TypedDict):
    TableName: str,
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
## UpdateTimeToLiveOutputTypeDef

```python
# UpdateTimeToLiveOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTimeToLiveOutputTypeDef


def get_value() -> UpdateTimeToLiveOutputTypeDef:
    return {
        "TimeToLiveSpecification": ...,
    }


# UpdateTimeToLiveOutputTypeDef definition

class UpdateTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKinesisStreamingDestinationInputTypeDef

```python
# UpdateKinesisStreamingDestinationInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateKinesisStreamingDestinationInputTypeDef


def get_value() -> UpdateKinesisStreamingDestinationInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateKinesisStreamingDestinationInputTypeDef definition

class UpdateKinesisStreamingDestinationInputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    UpdateKinesisStreamingConfiguration: NotRequired[UpdateKinesisStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateKinesisStreamingConfigurationTypeDef](./type_defs.md#updatekinesisstreamingconfigurationtypedef) 
## UpdateKinesisStreamingDestinationOutputTypeDef

```python
# UpdateKinesisStreamingDestinationOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateKinesisStreamingDestinationOutputTypeDef


def get_value() -> UpdateKinesisStreamingDestinationOutputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateKinesisStreamingDestinationOutputTypeDef definition

class UpdateKinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    DestinationStatus: DestinationStatusType,  # (1)
    UpdateKinesisStreamingConfiguration: UpdateKinesisStreamingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-braces: UpdateKinesisStreamingConfigurationTypeDef](./type_defs.md#updatekinesisstreamingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStatementResponseTypeDef

```python
# BatchStatementResponseTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchStatementResponseTypeDef


def get_value() -> BatchStatementResponseTypeDef:
    return {
        "Error": ...,
    }


# BatchStatementResponseTypeDef definition

class BatchStatementResponseTypeDef(TypedDict):
    Error: NotRequired[BatchStatementErrorTypeDef],  # (1)
    TableName: NotRequired[str],
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-braces: BatchStatementErrorTypeDef](./type_defs.md#batchstatementerrortypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## WriteRequestOutputTypeDef

```python
# WriteRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestOutputTypeDef


def get_value() -> WriteRequestOutputTypeDef:
    return {
        "PutRequest": ...,
    }


# WriteRequestOutputTypeDef definition

class WriteRequestOutputTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestOutputTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 
2. See [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 
## AttributeValueUpdateTypeDef

```python
# AttributeValueUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AttributeValueUpdateTypeDef


def get_value() -> AttributeValueUpdateTypeDef:
    return {
        "Value": ...,
    }


# AttributeValueUpdateTypeDef definition

class AttributeValueUpdateTypeDef(TypedDict):
    Value: NotRequired[UniversalAttributeValueTypeDef],  # (1)
    Action: NotRequired[AttributeActionType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: AttributeActionType](./literals.md#attributeactiontype) 
## BatchStatementRequestTypeDef

```python
# BatchStatementRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchStatementRequestTypeDef


def get_value() -> BatchStatementRequestTypeDef:
    return {
        "Statement": ...,
    }


# BatchStatementRequestTypeDef definition

class BatchStatementRequestTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ConsistentRead: NotRequired[bool],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ConditionCheckTypeDef

```python
# ConditionCheckTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ConditionCheckTypeDef


def get_value() -> ConditionCheckTypeDef:
    return {
        "Key": ...,
    }


# ConditionCheckTypeDef definition

class ConditionCheckTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: str,
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ConditionTypeDef

```python
# ConditionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ConditionTypeDef


def get_value() -> ConditionTypeDef:
    return {
        "AttributeValueList": ...,
    }


# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (2)
    AttributeValueList: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## DeleteRequestTypeDef

```python
# DeleteRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteRequestTypeDef


def get_value() -> DeleteRequestTypeDef:
    return {
        "Key": ...,
    }


# DeleteRequestTypeDef definition

class DeleteRequestTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## DeleteTypeDef

```python
# DeleteTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteTypeDef


def get_value() -> DeleteTypeDef:
    return {
        "Key": ...,
    }


# DeleteTypeDef definition

class DeleteTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ExecuteStatementInputTypeDef

```python
# ExecuteStatementInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExecuteStatementInputTypeDef


def get_value() -> ExecuteStatementInputTypeDef:
    return {
        "Statement": ...,
    }


# ExecuteStatementInputTypeDef definition

class ExecuteStatementInputTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ConsistentRead: NotRequired[bool],
    NextToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    Limit: NotRequired[int],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ExpectedAttributeValueTypeDef

```python
# ExpectedAttributeValueTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExpectedAttributeValueTypeDef


def get_value() -> ExpectedAttributeValueTypeDef:
    return {
        "Value": ...,
    }


# ExpectedAttributeValueTypeDef definition

class ExpectedAttributeValueTypeDef(TypedDict):
    Value: NotRequired[UniversalAttributeValueTypeDef],  # (1)
    Exists: NotRequired[bool],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (2)
    AttributeValueList: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## GetItemInputTypeDef

```python
# GetItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetItemInputTypeDef


def get_value() -> GetItemInputTypeDef:
    return {
        "TableName": ...,
    }


# GetItemInputTypeDef definition

class GetItemInputTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## GetTypeDef

```python
# GetTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetTypeDef


def get_value() -> GetTypeDef:
    return {
        "Key": ...,
    }


# GetTypeDef definition

class GetTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## KeysAndAttributesTypeDef

```python
# KeysAndAttributesTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import KeysAndAttributesTypeDef


def get_value() -> KeysAndAttributesTypeDef:
    return {
        "Keys": ...,
    }


# KeysAndAttributesTypeDef definition

class KeysAndAttributesTypeDef(TypedDict):
    Keys: Sequence[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ParameterizedStatementTypeDef

```python
# ParameterizedStatementTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ParameterizedStatementTypeDef


def get_value() -> ParameterizedStatementTypeDef:
    return {
        "Statement": ...,
    }


# ParameterizedStatementTypeDef definition

class ParameterizedStatementTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutRequestTypeDef

```python
# PutRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutRequestTypeDef


def get_value() -> PutRequestTypeDef:
    return {
        "Item": ...,
    }


# PutRequestTypeDef definition

class PutRequestTypeDef(TypedDict):
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## PutTypeDef

```python
# PutTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutTypeDef


def get_value() -> PutTypeDef:
    return {
        "Item": ...,
    }


# PutTypeDef definition

class PutTypeDef(TypedDict):
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateTypeDef

```python
# UpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTypeDef


def get_value() -> UpdateTypeDef:
    return {
        "Key": ...,
    }


# UpdateTypeDef definition

class UpdateTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    UpdateExpression: str,
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## QueryInputTableQueryTypeDef

```python
# QueryInputTableQueryTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import QueryInputTableQueryTypeDef


def get_value() -> QueryInputTableQueryTypeDef:
    return {
        "IndexName": ...,
    }


# QueryInputTableQueryTypeDef definition

class QueryInputTableQueryTypeDef(TypedDict):
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[ConditionBaseImportTypeDef],
    KeyConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ScanInputTableScanTypeDef

```python
# ScanInputTableScanTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ScanInputTableScanTypeDef


def get_value() -> ScanInputTableScanTypeDef:
    return {
        "IndexName": ...,
    }


# ScanInputTableScanTypeDef definition

class ScanInputTableScanTypeDef(TypedDict):
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## DeleteItemInputTableDeleteItemTypeDef

```python
# DeleteItemInputTableDeleteItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteItemInputTableDeleteItemTypeDef


def get_value() -> DeleteItemInputTableDeleteItemTypeDef:
    return {
        "Key": ...,
    }


# DeleteItemInputTableDeleteItemTypeDef definition

class DeleteItemInputTableDeleteItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (1)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (6)
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutItemInputTablePutItemTypeDef

```python
# PutItemInputTablePutItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutItemInputTablePutItemTypeDef


def get_value() -> PutItemInputTablePutItemTypeDef:
    return {
        "Item": ...,
    }


# PutItemInputTablePutItemTypeDef definition

class PutItemInputTablePutItemTypeDef(TypedDict):
    Item: Mapping[str, TableAttributeValueTypeDef],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (1)
    ReturnValues: NotRequired[ReturnValueType],  # (2)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (3)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (4)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (5)
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (6)
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateItemInputTableUpdateItemTypeDef

```python
# UpdateItemInputTableUpdateItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateItemInputTableUpdateItemTypeDef


def get_value() -> UpdateItemInputTableUpdateItemTypeDef:
    return {
        "Key": ...,
    }


# UpdateItemInputTableUpdateItemTypeDef definition

class UpdateItemInputTableUpdateItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTableTypeDef]],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (7)
```

1. See [:material-code-braces: AttributeValueUpdateTableTypeDef](./type_defs.md#attributevalueupdatetabletypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## WriteRequestServiceResourceOutputTypeDef

```python
# WriteRequestServiceResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestServiceResourceOutputTypeDef


def get_value() -> WriteRequestServiceResourceOutputTypeDef:
    return {
        "PutRequest": ...,
    }


# WriteRequestServiceResourceOutputTypeDef definition

class WriteRequestServiceResourceOutputTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestServiceResourceOutputTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestServiceResourceOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 
## AutoScalingSettingsDescriptionTypeDef

```python
# AutoScalingSettingsDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingSettingsDescriptionTypeDef


def get_value() -> AutoScalingSettingsDescriptionTypeDef:
    return {
        "MinimumUnits": ...,
    }


# AutoScalingSettingsDescriptionTypeDef definition

class AutoScalingSettingsDescriptionTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicies: NotRequired[List[AutoScalingPolicyDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## AutoScalingSettingsUpdateTypeDef

```python
# AutoScalingSettingsUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import AutoScalingSettingsUpdateTypeDef


def get_value() -> AutoScalingSettingsUpdateTypeDef:
    return {
        "MinimumUnits": ...,
    }


# AutoScalingSettingsUpdateTypeDef definition

class AutoScalingSettingsUpdateTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicyUpdate: NotRequired[AutoScalingPolicyUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyUpdateTypeDef](./type_defs.md#autoscalingpolicyupdatetypedef) 
## BatchGetItemOutputServiceResourceTypeDef

```python
# BatchGetItemOutputServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchGetItemOutputServiceResourceTypeDef


def get_value() -> BatchGetItemOutputServiceResourceTypeDef:
    return {
        "Responses": ...,
    }


# BatchGetItemOutputServiceResourceTypeDef definition

class BatchGetItemOutputServiceResourceTypeDef(TypedDict):
    Responses: Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
    UnprocessedKeys: Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetItemOutputTypeDef

```python
# BatchGetItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchGetItemOutputTypeDef


def get_value() -> BatchGetItemOutputTypeDef:
    return {
        "Responses": ...,
    }


# BatchGetItemOutputTypeDef definition

class BatchGetItemOutputTypeDef(TypedDict):
    Responses: Dict[str, List[Dict[str, AttributeValueTypeDef]]],  # (1)
    UnprocessedKeys: Dict[str, KeysAndAttributesOutputTypeDef],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteItemOutputTableTypeDef

```python
# DeleteItemOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteItemOutputTableTypeDef


def get_value() -> DeleteItemOutputTableTypeDef:
    return {
        "Attributes": ...,
    }


# DeleteItemOutputTableTypeDef definition

class DeleteItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteItemOutputTypeDef

```python
# DeleteItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteItemOutputTypeDef


def get_value() -> DeleteItemOutputTypeDef:
    return {
        "Attributes": ...,
    }


# DeleteItemOutputTypeDef definition

class DeleteItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementOutputTypeDef

```python
# ExecuteStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExecuteStatementOutputTypeDef


def get_value() -> ExecuteStatementOutputTypeDef:
    return {
        "Items": ...,
    }


# ExecuteStatementOutputTypeDef definition

class ExecuteStatementOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
    LastEvaluatedKey: NotRequired[Dict[str, AttributeValueTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteTransactionOutputTypeDef

```python
# ExecuteTransactionOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExecuteTransactionOutputTypeDef


def get_value() -> ExecuteTransactionOutputTypeDef:
    return {
        "Responses": ...,
    }


# ExecuteTransactionOutputTypeDef definition

class ExecuteTransactionOutputTypeDef(TypedDict):
    Responses: List[ItemResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetItemOutputTableTypeDef

```python
# GetItemOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetItemOutputTableTypeDef


def get_value() -> GetItemOutputTableTypeDef:
    return {
        "Item": ...,
    }


# GetItemOutputTableTypeDef definition

class GetItemOutputTableTypeDef(TypedDict):
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    Item: NotRequired[Dict[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetItemOutputTypeDef

```python
# GetItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GetItemOutputTypeDef


def get_value() -> GetItemOutputTypeDef:
    return {
        "Item": ...,
    }


# GetItemOutputTypeDef definition

class GetItemOutputTypeDef(TypedDict):
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutItemOutputTableTypeDef

```python
# PutItemOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutItemOutputTableTypeDef


def get_value() -> PutItemOutputTableTypeDef:
    return {
        "Attributes": ...,
    }


# PutItemOutputTableTypeDef definition

class PutItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutItemOutputTypeDef

```python
# PutItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutItemOutputTypeDef


def get_value() -> PutItemOutputTypeDef:
    return {
        "Attributes": ...,
    }


# PutItemOutputTypeDef definition

class PutItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryOutputTableTypeDef

```python
# QueryOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import QueryOutputTableTypeDef


def get_value() -> QueryOutputTableTypeDef:
    return {
        "Items": ...,
    }


# QueryOutputTableTypeDef definition

class QueryOutputTableTypeDef(TypedDict):
    Items: List[Dict[str, TableAttributeValueTypeDef]],
    Count: int,
    ScannedCount: int,
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    LastEvaluatedKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryOutputTypeDef

```python
# QueryOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import QueryOutputTypeDef


def get_value() -> QueryOutputTypeDef:
    return {
        "Items": ...,
    }


# QueryOutputTypeDef definition

class QueryOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    Count: int,
    ScannedCount: int,
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    LastEvaluatedKey: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanOutputTableTypeDef

```python
# ScanOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ScanOutputTableTypeDef


def get_value() -> ScanOutputTableTypeDef:
    return {
        "Items": ...,
    }


# ScanOutputTableTypeDef definition

class ScanOutputTableTypeDef(TypedDict):
    Items: List[Dict[str, TableAttributeValueTypeDef]],
    Count: int,
    ScannedCount: int,
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    LastEvaluatedKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanOutputTypeDef

```python
# ScanOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ScanOutputTypeDef


def get_value() -> ScanOutputTypeDef:
    return {
        "Items": ...,
    }


# ScanOutputTypeDef definition

class ScanOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    Count: int,
    ScannedCount: int,
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    LastEvaluatedKey: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransactGetItemsOutputTypeDef

```python
# TransactGetItemsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactGetItemsOutputTypeDef


def get_value() -> TransactGetItemsOutputTypeDef:
    return {
        "ConsumedCapacity": ...,
    }


# TransactGetItemsOutputTypeDef definition

class TransactGetItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    Responses: List[ItemResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransactWriteItemsOutputTypeDef

```python
# TransactWriteItemsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactWriteItemsOutputTypeDef


def get_value() -> TransactWriteItemsOutputTypeDef:
    return {
        "ConsumedCapacity": ...,
    }


# TransactWriteItemsOutputTypeDef definition

class TransactWriteItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateItemOutputTableTypeDef

```python
# UpdateItemOutputTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateItemOutputTableTypeDef


def get_value() -> UpdateItemOutputTableTypeDef:
    return {
        "Attributes": ...,
    }


# UpdateItemOutputTableTypeDef definition

class UpdateItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateItemOutputTypeDef

```python
# UpdateItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateItemOutputTypeDef


def get_value() -> UpdateItemOutputTypeDef:
    return {
        "Attributes": ...,
    }


# UpdateItemOutputTypeDef definition

class UpdateItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContinuousBackupsOutputTypeDef

```python
# DescribeContinuousBackupsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeContinuousBackupsOutputTypeDef


def get_value() -> DescribeContinuousBackupsOutputTypeDef:
    return {
        "ContinuousBackupsDescription": ...,
    }


# DescribeContinuousBackupsOutputTypeDef definition

class DescribeContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContinuousBackupsOutputTypeDef

```python
# UpdateContinuousBackupsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateContinuousBackupsOutputTypeDef


def get_value() -> UpdateContinuousBackupsOutputTypeDef:
    return {
        "ContinuousBackupsDescription": ...,
    }


# UpdateContinuousBackupsOutputTypeDef definition

class UpdateContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGlobalTablesOutputTypeDef

```python
# ListGlobalTablesOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListGlobalTablesOutputTypeDef


def get_value() -> ListGlobalTablesOutputTypeDef:
    return {
        "GlobalTables": ...,
    }


# ListGlobalTablesOutputTypeDef definition

class ListGlobalTablesOutputTypeDef(TypedDict):
    GlobalTables: List[GlobalTableTypeDef],  # (1)
    LastEvaluatedGlobalTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableTypeDef](./type_defs.md#globaltabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationGroupMemberActionTypeDef

```python
# CreateReplicationGroupMemberActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateReplicationGroupMemberActionTypeDef


def get_value() -> CreateReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }


# CreateReplicationGroupMemberActionTypeDef definition

class CreateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (3)
    TableClassOverride: NotRequired[TableClassType],  # (4)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
3. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
4. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateReplicationGroupMemberActionTypeDef

```python
# UpdateReplicationGroupMemberActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateReplicationGroupMemberActionTypeDef


def get_value() -> UpdateReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }


# UpdateReplicationGroupMemberActionTypeDef definition

class UpdateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (3)
    TableClassOverride: NotRequired[TableClassType],  # (4)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
3. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
4. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateGlobalTableInputTypeDef

```python
# UpdateGlobalTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateGlobalTableInputTypeDef


def get_value() -> UpdateGlobalTableInputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# UpdateGlobalTableInputTypeDef definition

class UpdateGlobalTableInputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaUpdates: Sequence[ReplicaUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaUpdateTypeDef](./type_defs.md#replicaupdatetypedef) 
## DescribeExportOutputTypeDef

```python
# DescribeExportOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeExportOutputTypeDef


def get_value() -> DescribeExportOutputTypeDef:
    return {
        "ExportDescription": ...,
    }


# DescribeExportOutputTypeDef definition

class DescribeExportOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTableToPointInTimeOutputTypeDef

```python
# ExportTableToPointInTimeOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExportTableToPointInTimeOutputTypeDef


def get_value() -> ExportTableToPointInTimeOutputTypeDef:
    return {
        "ExportDescription": ...,
    }


# ExportTableToPointInTimeOutputTypeDef definition

class ExportTableToPointInTimeOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicaDescriptionTypeDef

```python
# ReplicaDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaDescriptionTypeDef


def get_value() -> ReplicaDescriptionTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaDescriptionTypeDef definition

class ReplicaDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaStatusDescription: NotRequired[str],
    ReplicaStatusPercentProgress: NotRequired[str],
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (2)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (3)
    WarmThroughput: NotRequired[TableWarmThroughputDescriptionTypeDef],  # (4)
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexDescriptionTypeDef]],  # (5)
    ReplicaInaccessibleDateTime: NotRequired[datetime],
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (6)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
3. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
4. See [:material-code-braces: TableWarmThroughputDescriptionTypeDef](./type_defs.md#tablewarmthroughputdescriptiontypedef) 
5. See [:material-code-braces: ReplicaGlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexdescriptiontypedef) 
6. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## TableCreationParametersOutputTypeDef

```python
# TableCreationParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableCreationParametersOutputTypeDef


def get_value() -> TableCreationParametersOutputTypeDef:
    return {
        "TableName": ...,
    }


# TableCreationParametersOutputTypeDef definition

class TableCreationParametersOutputTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: List[AttributeDefinitionTypeDef],  # (1)
    KeySchema: List[KeySchemaElementTypeDef],  # (2)
    BillingMode: NotRequired[BillingModeType],  # (3)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexOutputTypeDef]],  # (7)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
## SourceTableFeatureDetailsTypeDef

```python
# SourceTableFeatureDetailsTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import SourceTableFeatureDetailsTypeDef


def get_value() -> SourceTableFeatureDetailsTypeDef:
    return {
        "LocalSecondaryIndexes": ...,
    }


# SourceTableFeatureDetailsTypeDef definition

class SourceTableFeatureDetailsTypeDef(TypedDict):
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexInfoTypeDef]],  # (1)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexInfoTypeDef]],  # (2)
    StreamDescription: NotRequired[StreamSpecificationTypeDef],  # (3)
    TimeToLiveDescription: NotRequired[TimeToLiveDescriptionTypeDef],  # (4)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (5)
```

1. See [:material-code-braces: LocalSecondaryIndexInfoTypeDef](./type_defs.md#localsecondaryindexinfotypedef) 
2. See [:material-code-braces: GlobalSecondaryIndexInfoTypeDef](./type_defs.md#globalsecondaryindexinfotypedef) 
3. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
4. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
5. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
## ListImportsOutputTypeDef

```python
# ListImportsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ListImportsOutputTypeDef


def get_value() -> ListImportsOutputTypeDef:
    return {
        "ImportSummaryList": ...,
    }


# ListImportsOutputTypeDef definition

class ListImportsOutputTypeDef(TypedDict):
    ImportSummaryList: List[ImportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportSummaryTypeDef](./type_defs.md#importsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGlobalSecondaryIndexActionTypeDef

```python
# CreateGlobalSecondaryIndexActionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateGlobalSecondaryIndexActionTypeDef


def get_value() -> CreateGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
    }


# CreateGlobalSecondaryIndexActionTypeDef definition

class CreateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionUnionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (5)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
5. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## GlobalSecondaryIndexTypeDef

```python
# GlobalSecondaryIndexTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexTypeDef


def get_value() -> GlobalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalSecondaryIndexTypeDef definition

class GlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionUnionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (5)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
5. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## LocalSecondaryIndexTypeDef

```python
# LocalSecondaryIndexTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import LocalSecondaryIndexTypeDef


def get_value() -> LocalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
    }


# LocalSecondaryIndexTypeDef definition

class LocalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionUnionTypeDef,  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## BatchExecuteStatementOutputTypeDef

```python
# BatchExecuteStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementOutputTypeDef


def get_value() -> BatchExecuteStatementOutputTypeDef:
    return {
        "Responses": ...,
    }


# BatchExecuteStatementOutputTypeDef definition

class BatchExecuteStatementOutputTypeDef(TypedDict):
    Responses: List[BatchStatementResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchStatementResponseTypeDef](./type_defs.md#batchstatementresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchWriteItemOutputTypeDef

```python
# BatchWriteItemOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchWriteItemOutputTypeDef


def get_value() -> BatchWriteItemOutputTypeDef:
    return {
        "UnprocessedItems": ...,
    }


# BatchWriteItemOutputTypeDef definition

class BatchWriteItemOutputTypeDef(TypedDict):
    UnprocessedItems: Dict[str, List[WriteRequestOutputTypeDef]],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchExecuteStatementInputTypeDef

```python
# BatchExecuteStatementInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementInputTypeDef


def get_value() -> BatchExecuteStatementInputTypeDef:
    return {
        "Statements": ...,
    }


# BatchExecuteStatementInputTypeDef definition

class BatchExecuteStatementInputTypeDef(TypedDict):
    Statements: Sequence[BatchStatementRequestTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: BatchStatementRequestTypeDef](./type_defs.md#batchstatementrequesttypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## QueryInputPaginateTypeDef

```python
# QueryInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import QueryInputPaginateTypeDef


def get_value() -> QueryInputPaginateTypeDef:
    return {
        "TableName": ...,
    }


# QueryInputPaginateTypeDef definition

class QueryInputPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (6)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (7)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryInputTypeDef

```python
# QueryInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import QueryInputTypeDef


def get_value() -> QueryInputTypeDef:
    return {
        "TableName": ...,
    }


# QueryInputTypeDef definition

class QueryInputTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (6)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
6. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ScanInputPaginateTypeDef

```python
# ScanInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ScanInputPaginateTypeDef


def get_value() -> ScanInputPaginateTypeDef:
    return {
        "TableName": ...,
    }


# ScanInputPaginateTypeDef definition

class ScanInputPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
    ConsistentRead: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ScanInputTypeDef

```python
# ScanInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ScanInputTypeDef


def get_value() -> ScanInputTypeDef:
    return {
        "TableName": ...,
    }


# ScanInputTypeDef definition

class ScanInputTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (4)
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## DeleteItemInputTypeDef

```python
# DeleteItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteItemInputTypeDef


def get_value() -> DeleteItemInputTypeDef:
    return {
        "TableName": ...,
    }


# DeleteItemInputTypeDef definition

class DeleteItemInputTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (8)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
8. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutItemInputTypeDef

```python
# PutItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import PutItemInputTypeDef


def get_value() -> PutItemInputTypeDef:
    return {
        "TableName": ...,
    }


# PutItemInputTypeDef definition

class PutItemInputTypeDef(TypedDict):
    TableName: str,
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (6)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (8)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
8. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateItemInputTypeDef

```python
# UpdateItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateItemInputTypeDef


def get_value() -> UpdateItemInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateItemInputTypeDef definition

class UpdateItemInputTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTypeDef]],  # (2)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (3)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ReturnValues: NotRequired[ReturnValueType],  # (5)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (6)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (7)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (9)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueUpdateTypeDef](./type_defs.md#attributevalueupdatetypedef) 
3. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
6. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
7. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
8. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
9. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## TransactGetItemTypeDef

```python
# TransactGetItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactGetItemTypeDef


def get_value() -> TransactGetItemTypeDef:
    return {
        "Get": ...,
    }


# TransactGetItemTypeDef definition

class TransactGetItemTypeDef(TypedDict):
    Get: GetTypeDef,  # (1)
```

1. See [:material-code-braces: GetTypeDef](./type_defs.md#gettypedef) 
## ExecuteTransactionInputTypeDef

```python
# ExecuteTransactionInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExecuteTransactionInputTypeDef


def get_value() -> ExecuteTransactionInputTypeDef:
    return {
        "TransactStatements": ...,
    }


# ExecuteTransactionInputTypeDef definition

class ExecuteTransactionInputTypeDef(TypedDict):
    TransactStatements: Sequence[ParameterizedStatementTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: ParameterizedStatementTypeDef](./type_defs.md#parameterizedstatementtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## TransactWriteItemTypeDef

```python
# TransactWriteItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactWriteItemTypeDef


def get_value() -> TransactWriteItemTypeDef:
    return {
        "ConditionCheck": ...,
    }


# TransactWriteItemTypeDef definition

class TransactWriteItemTypeDef(TypedDict):
    ConditionCheck: NotRequired[ConditionCheckTypeDef],  # (1)
    Put: NotRequired[PutTypeDef],  # (2)
    Delete: NotRequired[DeleteTypeDef],  # (3)
    Update: NotRequired[UpdateTypeDef],  # (4)
```

1. See [:material-code-braces: ConditionCheckTypeDef](./type_defs.md#conditionchecktypedef) 
2. See [:material-code-braces: PutTypeDef](./type_defs.md#puttypedef) 
3. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
4. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
## BatchGetItemInputServiceResourceBatchGetItemTypeDef

```python
# BatchGetItemInputServiceResourceBatchGetItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchGetItemInputServiceResourceBatchGetItemTypeDef


def get_value() -> BatchGetItemInputServiceResourceBatchGetItemTypeDef:
    return {
        "RequestItems": ...,
    }


# BatchGetItemInputServiceResourceBatchGetItemTypeDef definition

class BatchGetItemInputServiceResourceBatchGetItemTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesServiceResourceUnionTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchWriteItemOutputServiceResourceTypeDef

```python
# BatchWriteItemOutputServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchWriteItemOutputServiceResourceTypeDef


def get_value() -> BatchWriteItemOutputServiceResourceTypeDef:
    return {
        "UnprocessedItems": ...,
    }


# BatchWriteItemOutputServiceResourceTypeDef definition

class BatchWriteItemOutputServiceResourceTypeDef(TypedDict):
    UnprocessedItems: Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: ItemCollectionMetricsServiceResourceTypeDef](./type_defs.md#itemcollectionmetricsserviceresourcetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WriteRequestServiceResourceTypeDef

```python
# WriteRequestServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestServiceResourceTypeDef


def get_value() -> WriteRequestServiceResourceTypeDef:
    return {
        "PutRequest": ...,
    }


# WriteRequestServiceResourceTypeDef definition

class WriteRequestServiceResourceTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestServiceResourceUnionTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestServiceResourceUnionTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestServiceResourceTypeDef](./type_defs.md#putrequestserviceresourcetypedef) [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceTypeDef](./type_defs.md#deleterequestserviceresourcetypedef) [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(TypedDict):
    IndexName: str,
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## GlobalSecondaryIndexAutoScalingUpdateTypeDef

```python
# GlobalSecondaryIndexAutoScalingUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexAutoScalingUpdateTypeDef


def get_value() -> GlobalSecondaryIndexAutoScalingUpdateTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalSecondaryIndexAutoScalingUpdateTypeDef definition

class GlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef

```python
# GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef


def get_value() -> GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef:
    return {
        "IndexName": ...,
    }


# GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef definition

class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef

```python
# ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef definition

class ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef

```python
# ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef


def get_value() -> ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef:
    return {
        "IndexName": ...,
    }


# ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef definition

class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicationGroupUpdateTypeDef

```python
# ReplicationGroupUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicationGroupUpdateTypeDef


def get_value() -> ReplicationGroupUpdateTypeDef:
    return {
        "Create": ...,
    }


# ReplicationGroupUpdateTypeDef definition

class ReplicationGroupUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicationGroupMemberActionTypeDef],  # (1)
    Update: NotRequired[UpdateReplicationGroupMemberActionTypeDef],  # (2)
    Delete: NotRequired[DeleteReplicationGroupMemberActionTypeDef],  # (3)
```

1. See [:material-code-braces: CreateReplicationGroupMemberActionTypeDef](./type_defs.md#createreplicationgroupmemberactiontypedef) 
2. See [:material-code-braces: UpdateReplicationGroupMemberActionTypeDef](./type_defs.md#updatereplicationgroupmemberactiontypedef) 
3. See [:material-code-braces: DeleteReplicationGroupMemberActionTypeDef](./type_defs.md#deletereplicationgroupmemberactiontypedef) 
## ExportTableToPointInTimeInputTypeDef

```python
# ExportTableToPointInTimeInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ExportTableToPointInTimeInputTypeDef


def get_value() -> ExportTableToPointInTimeInputTypeDef:
    return {
        "TableArn": ...,
    }


# ExportTableToPointInTimeInputTypeDef definition

class ExportTableToPointInTimeInputTypeDef(TypedDict):
    TableArn: str,
    S3Bucket: str,
    ExportTime: NotRequired[TimestampTypeDef],
    ClientToken: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (1)
    S3SseKmsKeyId: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (2)
    ExportType: NotRequired[ExportTypeType],  # (3)
    IncrementalExportSpecification: NotRequired[IncrementalExportSpecificationUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
2. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
3. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
4. See [:material-code-braces: IncrementalExportSpecificationTypeDef](./type_defs.md#incrementalexportspecificationtypedef) [:material-code-braces: IncrementalExportSpecificationOutputTypeDef](./type_defs.md#incrementalexportspecificationoutputtypedef) 
## GlobalTableDescriptionTypeDef

```python
# GlobalTableDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalTableDescriptionTypeDef


def get_value() -> GlobalTableDescriptionTypeDef:
    return {
        "ReplicationGroup": ...,
    }


# GlobalTableDescriptionTypeDef definition

class GlobalTableDescriptionTypeDef(TypedDict):
    ReplicationGroup: NotRequired[List[ReplicaDescriptionTypeDef]],  # (1)
    GlobalTableArn: NotRequired[str],
    CreationDateTime: NotRequired[datetime],
    GlobalTableStatus: NotRequired[GlobalTableStatusType],  # (2)
    GlobalTableName: NotRequired[str],
```

1. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
2. See [:material-code-brackets: GlobalTableStatusType](./literals.md#globaltablestatustype) 
## TableDescriptionTypeDef

```python
# TableDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableDescriptionTypeDef


def get_value() -> TableDescriptionTypeDef:
    return {
        "AttributeDefinitions": ...,
    }


# TableDescriptionTypeDef definition

class TableDescriptionTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[List[AttributeDefinitionTypeDef]],  # (1)
    TableName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (2)
    TableStatus: NotRequired[TableStatusType],  # (3)
    CreationDateTime: NotRequired[datetime],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    TableSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    BillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (5)
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexDescriptionTypeDef]],  # (6)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexDescriptionTypeDef]],  # (7)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (8)
    LatestStreamLabel: NotRequired[str],
    LatestStreamArn: NotRequired[str],
    GlobalTableVersion: NotRequired[str],
    Replicas: NotRequired[List[ReplicaDescriptionTypeDef]],  # (9)
    RestoreSummary: NotRequired[RestoreSummaryTypeDef],  # (10)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (11)
    ArchivalSummary: NotRequired[ArchivalSummaryTypeDef],  # (12)
    TableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (13)
    DeletionProtectionEnabled: NotRequired[bool],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (14)
    WarmThroughput: NotRequired[TableWarmThroughputDescriptionTypeDef],  # (15)
    MultiRegionConsistency: NotRequired[MultiRegionConsistencyType],  # (16)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
5. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
6. See [:material-code-braces: LocalSecondaryIndexDescriptionTypeDef](./type_defs.md#localsecondaryindexdescriptiontypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#globalsecondaryindexdescriptiontypedef) 
8. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
9. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
10. See [:material-code-braces: RestoreSummaryTypeDef](./type_defs.md#restoresummarytypedef) 
11. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
12. See [:material-code-braces: ArchivalSummaryTypeDef](./type_defs.md#archivalsummarytypedef) 
13. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
14. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
15. See [:material-code-braces: TableWarmThroughputDescriptionTypeDef](./type_defs.md#tablewarmthroughputdescriptiontypedef) 
16. See [:material-code-brackets: MultiRegionConsistencyType](./literals.md#multiregionconsistencytype) 
## ImportTableDescriptionTypeDef

```python
# ImportTableDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ImportTableDescriptionTypeDef


def get_value() -> ImportTableDescriptionTypeDef:
    return {
        "ImportArn": ...,
    }


# ImportTableDescriptionTypeDef definition

class ImportTableDescriptionTypeDef(TypedDict):
    ImportArn: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    ClientToken: NotRequired[str],
    S3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (2)
    ErrorCount: NotRequired[int],
    CloudWatchLogGroupArn: NotRequired[str],
    InputFormat: NotRequired[InputFormatType],  # (3)
    InputFormatOptions: NotRequired[InputFormatOptionsOutputTypeDef],  # (4)
    InputCompressionType: NotRequired[InputCompressionTypeType],  # (5)
    TableCreationParameters: NotRequired[TableCreationParametersOutputTypeDef],  # (6)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ProcessedSizeBytes: NotRequired[int],
    ProcessedItemCount: NotRequired[int],
    ImportedItemCount: NotRequired[int],
    FailureCode: NotRequired[str],
    FailureMessage: NotRequired[str],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
3. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
4. See [:material-code-braces: InputFormatOptionsOutputTypeDef](./type_defs.md#inputformatoptionsoutputtypedef) 
5. See [:material-code-brackets: InputCompressionTypeType](./literals.md#inputcompressiontypetype) 
6. See [:material-code-braces: TableCreationParametersOutputTypeDef](./type_defs.md#tablecreationparametersoutputtypedef) 
## BackupDescriptionTypeDef

```python
# BackupDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BackupDescriptionTypeDef


def get_value() -> BackupDescriptionTypeDef:
    return {
        "BackupDetails": ...,
    }


# BackupDescriptionTypeDef definition

class BackupDescriptionTypeDef(TypedDict):
    BackupDetails: NotRequired[BackupDetailsTypeDef],  # (1)
    SourceTableDetails: NotRequired[SourceTableDetailsTypeDef],  # (2)
    SourceTableFeatureDetails: NotRequired[SourceTableFeatureDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: SourceTableDetailsTypeDef](./type_defs.md#sourcetabledetailstypedef) 
3. See [:material-code-braces: SourceTableFeatureDetailsTypeDef](./type_defs.md#sourcetablefeaturedetailstypedef) 
## GlobalSecondaryIndexUpdateTypeDef

```python
# GlobalSecondaryIndexUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import GlobalSecondaryIndexUpdateTypeDef


def get_value() -> GlobalSecondaryIndexUpdateTypeDef:
    return {
        "Update": ...,
    }


# GlobalSecondaryIndexUpdateTypeDef definition

class GlobalSecondaryIndexUpdateTypeDef(TypedDict):
    Update: NotRequired[UpdateGlobalSecondaryIndexActionTypeDef],  # (1)
    Create: NotRequired[CreateGlobalSecondaryIndexActionTypeDef],  # (2)
    Delete: NotRequired[DeleteGlobalSecondaryIndexActionTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateGlobalSecondaryIndexActionTypeDef](./type_defs.md#updateglobalsecondaryindexactiontypedef) 
2. See [:material-code-braces: CreateGlobalSecondaryIndexActionTypeDef](./type_defs.md#createglobalsecondaryindexactiontypedef) 
3. See [:material-code-braces: DeleteGlobalSecondaryIndexActionTypeDef](./type_defs.md#deleteglobalsecondaryindexactiontypedef) 
## TableCreationParametersTypeDef

```python
# TableCreationParametersTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableCreationParametersTypeDef


def get_value() -> TableCreationParametersTypeDef:
    return {
        "TableName": ...,
    }


# TableCreationParametersTypeDef definition

class TableCreationParametersTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    BillingMode: NotRequired[BillingModeType],  # (3)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (7)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
## TransactGetItemsInputTypeDef

```python
# TransactGetItemsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactGetItemsInputTypeDef


def get_value() -> TransactGetItemsInputTypeDef:
    return {
        "TransactItems": ...,
    }


# TransactGetItemsInputTypeDef definition

class TransactGetItemsInputTypeDef(TypedDict):
    TransactItems: Sequence[TransactGetItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: TransactGetItemTypeDef](./type_defs.md#transactgetitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchGetItemInputTypeDef

```python
# BatchGetItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchGetItemInputTypeDef


def get_value() -> BatchGetItemInputTypeDef:
    return {
        "RequestItems": ...,
    }


# BatchGetItemInputTypeDef definition

class BatchGetItemInputTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## WriteRequestTypeDef

```python
# WriteRequestTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import WriteRequestTypeDef


def get_value() -> WriteRequestTypeDef:
    return {
        "PutRequest": ...,
    }


# WriteRequestTypeDef definition

class WriteRequestTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestUnionTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestUnionTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestTypeDef](./type_defs.md#putrequesttypedef) [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 
2. See [:material-code-braces: DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef) [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 
## TransactWriteItemsInputTypeDef

```python
# TransactWriteItemsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TransactWriteItemsInputTypeDef


def get_value() -> TransactWriteItemsInputTypeDef:
    return {
        "TransactItems": ...,
    }


# TransactWriteItemsInputTypeDef definition

class TransactWriteItemsInputTypeDef(TypedDict):
    TransactItems: Sequence[TransactWriteItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TransactWriteItemTypeDef](./type_defs.md#transactwriteitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## ReplicaAutoScalingDescriptionTypeDef

```python
# ReplicaAutoScalingDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaAutoScalingDescriptionTypeDef


def get_value() -> ReplicaAutoScalingDescriptionTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaAutoScalingDescriptionTypeDef definition

class ReplicaAutoScalingDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (4)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingdescriptiontypedef) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
## ReplicaSettingsDescriptionTypeDef

```python
# ReplicaSettingsDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaSettingsDescriptionTypeDef


def get_value() -> ReplicaSettingsDescriptionTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaSettingsDescriptionTypeDef definition

class ReplicaSettingsDescriptionTypeDef(TypedDict):
    RegionName: str,
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaBillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (2)
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaProvisionedWriteCapacityUnits: NotRequired[int],
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaGlobalSecondaryIndexSettings: NotRequired[List[ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef]],  # (5)
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (6)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
5. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsdescriptiontypedef) 
6. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## ReplicaAutoScalingUpdateTypeDef

```python
# ReplicaAutoScalingUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaAutoScalingUpdateTypeDef


def get_value() -> ReplicaAutoScalingUpdateTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaAutoScalingUpdateTypeDef definition

class ReplicaAutoScalingUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaGlobalSecondaryIndexUpdates: NotRequired[Sequence[ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaSettingsUpdateTypeDef

```python
# ReplicaSettingsUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ReplicaSettingsUpdateTypeDef


def get_value() -> ReplicaSettingsUpdateTypeDef:
    return {
        "RegionName": ...,
    }


# ReplicaSettingsUpdateTypeDef definition

class ReplicaSettingsUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
    ReplicaGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (2)
    ReplicaTableClass: NotRequired[TableClassType],  # (3)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
2. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsupdatetypedef) 
3. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## CreateGlobalTableOutputTypeDef

```python
# CreateGlobalTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateGlobalTableOutputTypeDef


def get_value() -> CreateGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
    }


# CreateGlobalTableOutputTypeDef definition

class CreateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalTableOutputTypeDef

```python
# DescribeGlobalTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeGlobalTableOutputTypeDef


def get_value() -> DescribeGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
    }


# DescribeGlobalTableOutputTypeDef definition

class DescribeGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalTableOutputTypeDef

```python
# UpdateGlobalTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateGlobalTableOutputTypeDef


def get_value() -> UpdateGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
    }


# UpdateGlobalTableOutputTypeDef definition

class UpdateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableOutputTypeDef

```python
# CreateTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateTableOutputTypeDef


def get_value() -> CreateTableOutputTypeDef:
    return {
        "TableDescription": ...,
    }


# CreateTableOutputTypeDef definition

class CreateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTableOutputTypeDef

```python
# DeleteTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteTableOutputTypeDef


def get_value() -> DeleteTableOutputTypeDef:
    return {
        "TableDescription": ...,
    }


# DeleteTableOutputTypeDef definition

class DeleteTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableOutputTypeDef

```python
# DescribeTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableOutputTypeDef


def get_value() -> DescribeTableOutputTypeDef:
    return {
        "Table": ...,
    }


# DescribeTableOutputTypeDef definition

class DescribeTableOutputTypeDef(TypedDict):
    Table: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableFromBackupOutputTypeDef

```python
# RestoreTableFromBackupOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import RestoreTableFromBackupOutputTypeDef


def get_value() -> RestoreTableFromBackupOutputTypeDef:
    return {
        "TableDescription": ...,
    }


# RestoreTableFromBackupOutputTypeDef definition

class RestoreTableFromBackupOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableToPointInTimeOutputTypeDef

```python
# RestoreTableToPointInTimeOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import RestoreTableToPointInTimeOutputTypeDef


def get_value() -> RestoreTableToPointInTimeOutputTypeDef:
    return {
        "TableDescription": ...,
    }


# RestoreTableToPointInTimeOutputTypeDef definition

class RestoreTableToPointInTimeOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableOutputTypeDef

```python
# UpdateTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTableOutputTypeDef


def get_value() -> UpdateTableOutputTypeDef:
    return {
        "TableDescription": ...,
    }


# UpdateTableOutputTypeDef definition

class UpdateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImportOutputTypeDef

```python
# DescribeImportOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeImportOutputTypeDef


def get_value() -> DescribeImportOutputTypeDef:
    return {
        "ImportTableDescription": ...,
    }


# DescribeImportOutputTypeDef definition

class DescribeImportOutputTypeDef(TypedDict):
    ImportTableDescription: ImportTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTableDescriptionTypeDef](./type_defs.md#importtabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportTableOutputTypeDef

```python
# ImportTableOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ImportTableOutputTypeDef


def get_value() -> ImportTableOutputTypeDef:
    return {
        "ImportTableDescription": ...,
    }


# ImportTableOutputTypeDef definition

class ImportTableOutputTypeDef(TypedDict):
    ImportTableDescription: ImportTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTableDescriptionTypeDef](./type_defs.md#importtabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackupOutputTypeDef

```python
# DeleteBackupOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DeleteBackupOutputTypeDef


def get_value() -> DeleteBackupOutputTypeDef:
    return {
        "BackupDescription": ...,
    }


# DeleteBackupOutputTypeDef definition

class DeleteBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupOutputTypeDef

```python
# DescribeBackupOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeBackupOutputTypeDef


def get_value() -> DescribeBackupOutputTypeDef:
    return {
        "BackupDescription": ...,
    }


# DescribeBackupOutputTypeDef definition

class DescribeBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableInputTableUpdateTypeDef

```python
# UpdateTableInputTableUpdateTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTableInputTableUpdateTypeDef


def get_value() -> UpdateTableInputTableUpdateTypeDef:
    return {
        "AttributeDefinitions": ...,
    }


# UpdateTableInputTableUpdateTypeDef definition

class UpdateTableInputTableUpdateTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
    DeletionProtectionEnabled: NotRequired[bool],
    MultiRegionConsistency: NotRequired[MultiRegionConsistencyType],  # (9)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (10)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (11)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
9. See [:material-code-brackets: MultiRegionConsistencyType](./literals.md#multiregionconsistencytype) 
10. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## UpdateTableInputTypeDef

```python
# UpdateTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTableInputTypeDef


def get_value() -> UpdateTableInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateTableInputTypeDef definition

class UpdateTableInputTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
    DeletionProtectionEnabled: NotRequired[bool],
    MultiRegionConsistency: NotRequired[MultiRegionConsistencyType],  # (9)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (10)
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (11)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
9. See [:material-code-brackets: MultiRegionConsistencyType](./literals.md#multiregionconsistencytype) 
10. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
## CreateTableInputServiceResourceCreateTableTypeDef

```python
# CreateTableInputServiceResourceCreateTableTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateTableInputServiceResourceCreateTableTypeDef


def get_value() -> CreateTableInputServiceResourceCreateTableTypeDef:
    return {
        "AttributeDefinitions": ...,
    }


# CreateTableInputServiceResourceCreateTableTypeDef definition

class CreateTableInputServiceResourceCreateTableTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
    DeletionProtectionEnabled: NotRequired[bool],
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (11)
    ResourcePolicy: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (12)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
12. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## CreateTableInputTypeDef

```python
# CreateTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import CreateTableInputTypeDef


def get_value() -> CreateTableInputTypeDef:
    return {
        "AttributeDefinitions": ...,
    }


# CreateTableInputTypeDef definition

class CreateTableInputTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
    DeletionProtectionEnabled: NotRequired[bool],
    WarmThroughput: NotRequired[WarmThroughputTypeDef],  # (11)
    ResourcePolicy: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (12)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
12. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## RestoreTableFromBackupInputTypeDef

```python
# RestoreTableFromBackupInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import RestoreTableFromBackupInputTypeDef


def get_value() -> RestoreTableFromBackupInputTypeDef:
    return {
        "TargetTableName": ...,
    }


# RestoreTableFromBackupInputTypeDef definition

class RestoreTableFromBackupInputTypeDef(TypedDict):
    TargetTableName: str,
    BackupArn: str,
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (6)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## RestoreTableToPointInTimeInputTypeDef

```python
# RestoreTableToPointInTimeInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import RestoreTableToPointInTimeInputTypeDef


def get_value() -> RestoreTableToPointInTimeInputTypeDef:
    return {
        "TargetTableName": ...,
    }


# RestoreTableToPointInTimeInputTypeDef definition

class RestoreTableToPointInTimeInputTypeDef(TypedDict):
    TargetTableName: str,
    SourceTableArn: NotRequired[str],
    SourceTableName: NotRequired[str],
    UseLatestRestorableTime: NotRequired[bool],
    RestoreDateTime: NotRequired[TimestampTypeDef],
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (6)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## BatchWriteItemInputServiceResourceBatchWriteItemTypeDef

```python
# BatchWriteItemInputServiceResourceBatchWriteItemTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchWriteItemInputServiceResourceBatchWriteItemTypeDef


def get_value() -> BatchWriteItemInputServiceResourceBatchWriteItemTypeDef:
    return {
        "RequestItems": ...,
    }


# BatchWriteItemInputServiceResourceBatchWriteItemTypeDef definition

class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceUnionTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## TableAutoScalingDescriptionTypeDef

```python
# TableAutoScalingDescriptionTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import TableAutoScalingDescriptionTypeDef


def get_value() -> TableAutoScalingDescriptionTypeDef:
    return {
        "TableName": ...,
    }


# TableAutoScalingDescriptionTypeDef definition

class TableAutoScalingDescriptionTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableStatus: NotRequired[TableStatusType],  # (1)
    Replicas: NotRequired[List[ReplicaAutoScalingDescriptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: ReplicaAutoScalingDescriptionTypeDef](./type_defs.md#replicaautoscalingdescriptiontypedef) 
## DescribeGlobalTableSettingsOutputTypeDef

```python
# DescribeGlobalTableSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeGlobalTableSettingsOutputTypeDef


def get_value() -> DescribeGlobalTableSettingsOutputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# DescribeGlobalTableSettingsOutputTypeDef definition

class DescribeGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalTableSettingsOutputTypeDef

```python
# UpdateGlobalTableSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateGlobalTableSettingsOutputTypeDef


def get_value() -> UpdateGlobalTableSettingsOutputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# UpdateGlobalTableSettingsOutputTypeDef definition

class UpdateGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableReplicaAutoScalingInputTypeDef

```python
# UpdateTableReplicaAutoScalingInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTableReplicaAutoScalingInputTypeDef


def get_value() -> UpdateTableReplicaAutoScalingInputTypeDef:
    return {
        "TableName": ...,
    }


# UpdateTableReplicaAutoScalingInputTypeDef definition

class UpdateTableReplicaAutoScalingInputTypeDef(TypedDict):
    TableName: str,
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    ReplicaUpdates: NotRequired[Sequence[ReplicaAutoScalingUpdateTypeDef]],  # (3)
```

1. See [:material-code-braces: GlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#globalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: ReplicaAutoScalingUpdateTypeDef](./type_defs.md#replicaautoscalingupdatetypedef) 
## UpdateGlobalTableSettingsInputTypeDef

```python
# UpdateGlobalTableSettingsInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateGlobalTableSettingsInputTypeDef


def get_value() -> UpdateGlobalTableSettingsInputTypeDef:
    return {
        "GlobalTableName": ...,
    }


# UpdateGlobalTableSettingsInputTypeDef definition

class UpdateGlobalTableSettingsInputTypeDef(TypedDict):
    GlobalTableName: str,
    GlobalTableBillingMode: NotRequired[BillingModeType],  # (1)
    GlobalTableProvisionedWriteCapacityUnits: NotRequired[int],
    GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    GlobalTableGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (3)
    ReplicaSettingsUpdate: NotRequired[Sequence[ReplicaSettingsUpdateTypeDef]],  # (4)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#globaltableglobalsecondaryindexsettingsupdatetypedef) 
4. See [:material-code-braces: ReplicaSettingsUpdateTypeDef](./type_defs.md#replicasettingsupdatetypedef) 
## ImportTableInputTypeDef

```python
# ImportTableInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import ImportTableInputTypeDef


def get_value() -> ImportTableInputTypeDef:
    return {
        "S3BucketSource": ...,
    }


# ImportTableInputTypeDef definition

class ImportTableInputTypeDef(TypedDict):
    S3BucketSource: S3BucketSourceTypeDef,  # (1)
    InputFormat: InputFormatType,  # (2)
    TableCreationParameters: TableCreationParametersUnionTypeDef,  # (3)
    ClientToken: NotRequired[str],
    InputFormatOptions: NotRequired[InputFormatOptionsUnionTypeDef],  # (4)
    InputCompressionType: NotRequired[InputCompressionTypeType],  # (5)
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
2. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
3. See [:material-code-braces: TableCreationParametersTypeDef](./type_defs.md#tablecreationparameterstypedef) [:material-code-braces: TableCreationParametersOutputTypeDef](./type_defs.md#tablecreationparametersoutputtypedef) 
4. See [:material-code-braces: InputFormatOptionsTypeDef](./type_defs.md#inputformatoptionstypedef) [:material-code-braces: InputFormatOptionsOutputTypeDef](./type_defs.md#inputformatoptionsoutputtypedef) 
5. See [:material-code-brackets: InputCompressionTypeType](./literals.md#inputcompressiontypetype) 
## BatchWriteItemInputTypeDef

```python
# BatchWriteItemInputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import BatchWriteItemInputTypeDef


def get_value() -> BatchWriteItemInputTypeDef:
    return {
        "RequestItems": ...,
    }


# BatchWriteItemInputTypeDef definition

class BatchWriteItemInputTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## DescribeTableReplicaAutoScalingOutputTypeDef

```python
# DescribeTableReplicaAutoScalingOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import DescribeTableReplicaAutoScalingOutputTypeDef


def get_value() -> DescribeTableReplicaAutoScalingOutputTypeDef:
    return {
        "TableAutoScalingDescription": ...,
    }


# DescribeTableReplicaAutoScalingOutputTypeDef definition

class DescribeTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableReplicaAutoScalingOutputTypeDef

```python
# UpdateTableReplicaAutoScalingOutputTypeDef TypedDict usage example

from types_aiobotocore_dynamodb.type_defs import UpdateTableReplicaAutoScalingOutputTypeDef


def get_value() -> UpdateTableReplicaAutoScalingOutputTypeDef:
    return {
        "TableAutoScalingDescription": ...,
    }


# UpdateTableReplicaAutoScalingOutputTypeDef definition

class UpdateTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
