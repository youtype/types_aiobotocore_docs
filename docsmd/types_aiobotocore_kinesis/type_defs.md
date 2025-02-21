# Type definitions

> [Index](../README.md) > [Kinesis](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_kinesis.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_kinesis.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AddTagsToStreamInputTypeDef

```python
# AddTagsToStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import AddTagsToStreamInputTypeDef


def get_value() -> AddTagsToStreamInputTypeDef:
    return {
        "Tags": ...,
    }


# AddTagsToStreamInputTypeDef definition

class AddTagsToStreamInputTypeDef(TypedDict):
    Tags: Mapping[str, str],
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## HashKeyRangeTypeDef

```python
# HashKeyRangeTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import HashKeyRangeTypeDef


def get_value() -> HashKeyRangeTypeDef:
    return {
        "StartingHashKey": ...,
    }


# HashKeyRangeTypeDef definition

class HashKeyRangeTypeDef(TypedDict):
    StartingHashKey: str,
    EndingHashKey: str,
```

## ConsumerDescriptionTypeDef

```python
# ConsumerDescriptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ConsumerDescriptionTypeDef


def get_value() -> ConsumerDescriptionTypeDef:
    return {
        "ConsumerName": ...,
    }


# ConsumerDescriptionTypeDef definition

class ConsumerDescriptionTypeDef(TypedDict):
    ConsumerName: str,
    ConsumerARN: str,
    ConsumerStatus: ConsumerStatusType,  # (1)
    ConsumerCreationTimestamp: datetime,
    StreamARN: str,
```

1. See [:material-code-brackets: ConsumerStatusType](./literals.md#consumerstatustype) 
## ConsumerTypeDef

```python
# ConsumerTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ConsumerTypeDef


def get_value() -> ConsumerTypeDef:
    return {
        "ConsumerName": ...,
    }


# ConsumerTypeDef definition

class ConsumerTypeDef(TypedDict):
    ConsumerName: str,
    ConsumerARN: str,
    ConsumerStatus: ConsumerStatusType,  # (1)
    ConsumerCreationTimestamp: datetime,
```

1. See [:material-code-brackets: ConsumerStatusType](./literals.md#consumerstatustype) 
## StreamModeDetailsTypeDef

```python
# StreamModeDetailsTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StreamModeDetailsTypeDef


def get_value() -> StreamModeDetailsTypeDef:
    return {
        "StreamMode": ...,
    }


# StreamModeDetailsTypeDef definition

class StreamModeDetailsTypeDef(TypedDict):
    StreamMode: StreamModeType,  # (1)
```

1. See [:material-code-brackets: StreamModeType](./literals.md#streammodetype) 
## DecreaseStreamRetentionPeriodInputTypeDef

```python
# DecreaseStreamRetentionPeriodInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DecreaseStreamRetentionPeriodInputTypeDef


def get_value() -> DecreaseStreamRetentionPeriodInputTypeDef:
    return {
        "RetentionPeriodHours": ...,
    }


# DecreaseStreamRetentionPeriodInputTypeDef definition

class DecreaseStreamRetentionPeriodInputTypeDef(TypedDict):
    RetentionPeriodHours: int,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## DeleteResourcePolicyInputTypeDef

```python
# DeleteResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DeleteResourcePolicyInputTypeDef


def get_value() -> DeleteResourcePolicyInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# DeleteResourcePolicyInputTypeDef definition

class DeleteResourcePolicyInputTypeDef(TypedDict):
    ResourceARN: str,
```

## DeleteStreamInputTypeDef

```python
# DeleteStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DeleteStreamInputTypeDef


def get_value() -> DeleteStreamInputTypeDef:
    return {
        "StreamName": ...,
    }


# DeleteStreamInputTypeDef definition

class DeleteStreamInputTypeDef(TypedDict):
    StreamName: NotRequired[str],
    EnforceConsumerDeletion: NotRequired[bool],
    StreamARN: NotRequired[str],
```

## DeregisterStreamConsumerInputTypeDef

```python
# DeregisterStreamConsumerInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DeregisterStreamConsumerInputTypeDef


def get_value() -> DeregisterStreamConsumerInputTypeDef:
    return {
        "StreamARN": ...,
    }


# DeregisterStreamConsumerInputTypeDef definition

class DeregisterStreamConsumerInputTypeDef(TypedDict):
    StreamARN: NotRequired[str],
    ConsumerName: NotRequired[str],
    ConsumerARN: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ResponseMetadataTypeDef


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

## DescribeStreamConsumerInputTypeDef

```python
# DescribeStreamConsumerInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamConsumerInputTypeDef


def get_value() -> DescribeStreamConsumerInputTypeDef:
    return {
        "StreamARN": ...,
    }


# DescribeStreamConsumerInputTypeDef definition

class DescribeStreamConsumerInputTypeDef(TypedDict):
    StreamARN: NotRequired[str],
    ConsumerName: NotRequired[str],
    ConsumerARN: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PaginatorConfigTypeDef


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

## DescribeStreamInputTypeDef

```python
# DescribeStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamInputTypeDef


def get_value() -> DescribeStreamInputTypeDef:
    return {
        "StreamName": ...,
    }


# DescribeStreamInputTypeDef definition

class DescribeStreamInputTypeDef(TypedDict):
    StreamName: NotRequired[str],
    Limit: NotRequired[int],
    ExclusiveStartShardId: NotRequired[str],
    StreamARN: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeStreamSummaryInputTypeDef

```python
# DescribeStreamSummaryInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamSummaryInputTypeDef


def get_value() -> DescribeStreamSummaryInputTypeDef:
    return {
        "StreamName": ...,
    }


# DescribeStreamSummaryInputTypeDef definition

class DescribeStreamSummaryInputTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## DisableEnhancedMonitoringInputTypeDef

```python
# DisableEnhancedMonitoringInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DisableEnhancedMonitoringInputTypeDef


def get_value() -> DisableEnhancedMonitoringInputTypeDef:
    return {
        "ShardLevelMetrics": ...,
    }


# DisableEnhancedMonitoringInputTypeDef definition

class DisableEnhancedMonitoringInputTypeDef(TypedDict):
    ShardLevelMetrics: Sequence[MetricsNameType],  # (1)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
## EnableEnhancedMonitoringInputTypeDef

```python
# EnableEnhancedMonitoringInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import EnableEnhancedMonitoringInputTypeDef


def get_value() -> EnableEnhancedMonitoringInputTypeDef:
    return {
        "ShardLevelMetrics": ...,
    }


# EnableEnhancedMonitoringInputTypeDef definition

class EnableEnhancedMonitoringInputTypeDef(TypedDict):
    ShardLevelMetrics: Sequence[MetricsNameType],  # (1)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
## EnhancedMetricsTypeDef

```python
# EnhancedMetricsTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import EnhancedMetricsTypeDef


def get_value() -> EnhancedMetricsTypeDef:
    return {
        "ShardLevelMetrics": ...,
    }


# EnhancedMetricsTypeDef definition

class EnhancedMetricsTypeDef(TypedDict):
    ShardLevelMetrics: NotRequired[List[MetricsNameType]],  # (1)
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
## GetRecordsInputTypeDef

```python
# GetRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetRecordsInputTypeDef


def get_value() -> GetRecordsInputTypeDef:
    return {
        "ShardIterator": ...,
    }


# GetRecordsInputTypeDef definition

class GetRecordsInputTypeDef(TypedDict):
    ShardIterator: str,
    Limit: NotRequired[int],
    StreamARN: NotRequired[str],
```

## RecordTypeDef

```python
# RecordTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import RecordTypeDef


def get_value() -> RecordTypeDef:
    return {
        "SequenceNumber": ...,
    }


# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    SequenceNumber: str,
    Data: bytes,
    PartitionKey: str,
    ApproximateArrivalTimestamp: NotRequired[datetime],
    EncryptionType: NotRequired[EncryptionTypeType],  # (1)
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## GetResourcePolicyInputTypeDef

```python
# GetResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetResourcePolicyInputTypeDef


def get_value() -> GetResourcePolicyInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# GetResourcePolicyInputTypeDef definition

class GetResourcePolicyInputTypeDef(TypedDict):
    ResourceARN: str,
```

## IncreaseStreamRetentionPeriodInputTypeDef

```python
# IncreaseStreamRetentionPeriodInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import IncreaseStreamRetentionPeriodInputTypeDef


def get_value() -> IncreaseStreamRetentionPeriodInputTypeDef:
    return {
        "RetentionPeriodHours": ...,
    }


# IncreaseStreamRetentionPeriodInputTypeDef definition

class IncreaseStreamRetentionPeriodInputTypeDef(TypedDict):
    RetentionPeriodHours: int,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## InternalFailureExceptionTypeDef

```python
# InternalFailureExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import InternalFailureExceptionTypeDef


def get_value() -> InternalFailureExceptionTypeDef:
    return {
        "message": ...,
    }


# InternalFailureExceptionTypeDef definition

class InternalFailureExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSAccessDeniedExceptionTypeDef

```python
# KMSAccessDeniedExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSAccessDeniedExceptionTypeDef


def get_value() -> KMSAccessDeniedExceptionTypeDef:
    return {
        "message": ...,
    }


# KMSAccessDeniedExceptionTypeDef definition

class KMSAccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSDisabledExceptionTypeDef

```python
# KMSDisabledExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSDisabledExceptionTypeDef


def get_value() -> KMSDisabledExceptionTypeDef:
    return {
        "message": ...,
    }


# KMSDisabledExceptionTypeDef definition

class KMSDisabledExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSInvalidStateExceptionTypeDef

```python
# KMSInvalidStateExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSInvalidStateExceptionTypeDef


def get_value() -> KMSInvalidStateExceptionTypeDef:
    return {
        "message": ...,
    }


# KMSInvalidStateExceptionTypeDef definition

class KMSInvalidStateExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSNotFoundExceptionTypeDef

```python
# KMSNotFoundExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSNotFoundExceptionTypeDef


def get_value() -> KMSNotFoundExceptionTypeDef:
    return {
        "message": ...,
    }


# KMSNotFoundExceptionTypeDef definition

class KMSNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSOptInRequiredTypeDef

```python
# KMSOptInRequiredTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSOptInRequiredTypeDef


def get_value() -> KMSOptInRequiredTypeDef:
    return {
        "message": ...,
    }


# KMSOptInRequiredTypeDef definition

class KMSOptInRequiredTypeDef(TypedDict):
    message: NotRequired[str],
```

## KMSThrottlingExceptionTypeDef

```python
# KMSThrottlingExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import KMSThrottlingExceptionTypeDef


def get_value() -> KMSThrottlingExceptionTypeDef:
    return {
        "message": ...,
    }


# KMSThrottlingExceptionTypeDef definition

class KMSThrottlingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ListStreamsInputTypeDef

```python
# ListStreamsInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamsInputTypeDef


def get_value() -> ListStreamsInputTypeDef:
    return {
        "Limit": ...,
    }


# ListStreamsInputTypeDef definition

class ListStreamsInputTypeDef(TypedDict):
    Limit: NotRequired[int],
    ExclusiveStartStreamName: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListTagsForStreamInputTypeDef

```python
# ListTagsForStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListTagsForStreamInputTypeDef


def get_value() -> ListTagsForStreamInputTypeDef:
    return {
        "StreamName": ...,
    }


# ListTagsForStreamInputTypeDef definition

class ListTagsForStreamInputTypeDef(TypedDict):
    StreamName: NotRequired[str],
    ExclusiveStartTagKey: NotRequired[str],
    Limit: NotRequired[int],
    StreamARN: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## MergeShardsInputTypeDef

```python
# MergeShardsInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import MergeShardsInputTypeDef


def get_value() -> MergeShardsInputTypeDef:
    return {
        "ShardToMerge": ...,
    }


# MergeShardsInputTypeDef definition

class MergeShardsInputTypeDef(TypedDict):
    ShardToMerge: str,
    AdjacentShardToMerge: str,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## PutRecordsResultEntryTypeDef

```python
# PutRecordsResultEntryTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordsResultEntryTypeDef


def get_value() -> PutRecordsResultEntryTypeDef:
    return {
        "SequenceNumber": ...,
    }


# PutRecordsResultEntryTypeDef definition

class PutRecordsResultEntryTypeDef(TypedDict):
    SequenceNumber: NotRequired[str],
    ShardId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## PutResourcePolicyInputTypeDef

```python
# PutResourcePolicyInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutResourcePolicyInputTypeDef


def get_value() -> PutResourcePolicyInputTypeDef:
    return {
        "ResourceARN": ...,
    }


# PutResourcePolicyInputTypeDef definition

class PutResourcePolicyInputTypeDef(TypedDict):
    ResourceARN: str,
    Policy: str,
```

## RegisterStreamConsumerInputTypeDef

```python
# RegisterStreamConsumerInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import RegisterStreamConsumerInputTypeDef


def get_value() -> RegisterStreamConsumerInputTypeDef:
    return {
        "StreamARN": ...,
    }


# RegisterStreamConsumerInputTypeDef definition

class RegisterStreamConsumerInputTypeDef(TypedDict):
    StreamARN: str,
    ConsumerName: str,
```

## RemoveTagsFromStreamInputTypeDef

```python
# RemoveTagsFromStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import RemoveTagsFromStreamInputTypeDef


def get_value() -> RemoveTagsFromStreamInputTypeDef:
    return {
        "TagKeys": ...,
    }


# RemoveTagsFromStreamInputTypeDef definition

class RemoveTagsFromStreamInputTypeDef(TypedDict):
    TagKeys: Sequence[str],
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## ResourceInUseExceptionTypeDef

```python
# ResourceInUseExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ResourceInUseExceptionTypeDef


def get_value() -> ResourceInUseExceptionTypeDef:
    return {
        "message": ...,
    }


# ResourceInUseExceptionTypeDef definition

class ResourceInUseExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ResourceNotFoundExceptionTypeDef


def get_value() -> ResourceNotFoundExceptionTypeDef:
    return {
        "message": ...,
    }


# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## SequenceNumberRangeTypeDef

```python
# SequenceNumberRangeTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SequenceNumberRangeTypeDef


def get_value() -> SequenceNumberRangeTypeDef:
    return {
        "StartingSequenceNumber": ...,
    }


# SequenceNumberRangeTypeDef definition

class SequenceNumberRangeTypeDef(TypedDict):
    StartingSequenceNumber: str,
    EndingSequenceNumber: NotRequired[str],
```

## SplitShardInputTypeDef

```python
# SplitShardInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SplitShardInputTypeDef


def get_value() -> SplitShardInputTypeDef:
    return {
        "ShardToSplit": ...,
    }


# SplitShardInputTypeDef definition

class SplitShardInputTypeDef(TypedDict):
    ShardToSplit: str,
    NewStartingHashKey: str,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## StartStreamEncryptionInputTypeDef

```python
# StartStreamEncryptionInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StartStreamEncryptionInputTypeDef


def get_value() -> StartStreamEncryptionInputTypeDef:
    return {
        "EncryptionType": ...,
    }


# StartStreamEncryptionInputTypeDef definition

class StartStreamEncryptionInputTypeDef(TypedDict):
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## StopStreamEncryptionInputTypeDef

```python
# StopStreamEncryptionInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StopStreamEncryptionInputTypeDef


def get_value() -> StopStreamEncryptionInputTypeDef:
    return {
        "EncryptionType": ...,
    }


# StopStreamEncryptionInputTypeDef definition

class StopStreamEncryptionInputTypeDef(TypedDict):
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## UpdateShardCountInputTypeDef

```python
# UpdateShardCountInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import UpdateShardCountInputTypeDef


def get_value() -> UpdateShardCountInputTypeDef:
    return {
        "TargetShardCount": ...,
    }


# UpdateShardCountInputTypeDef definition

class UpdateShardCountInputTypeDef(TypedDict):
    TargetShardCount: int,
    ScalingType: ScalingTypeType,  # (1)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: ScalingTypeType](./literals.md#scalingtypetype) 
## PutRecordInputTypeDef

```python
# PutRecordInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordInputTypeDef


def get_value() -> PutRecordInputTypeDef:
    return {
        "Data": ...,
    }


# PutRecordInputTypeDef definition

class PutRecordInputTypeDef(TypedDict):
    Data: BlobTypeDef,
    PartitionKey: str,
    StreamName: NotRequired[str],
    ExplicitHashKey: NotRequired[str],
    SequenceNumberForOrdering: NotRequired[str],
    StreamARN: NotRequired[str],
```

## PutRecordsRequestEntryTypeDef

```python
# PutRecordsRequestEntryTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordsRequestEntryTypeDef


def get_value() -> PutRecordsRequestEntryTypeDef:
    return {
        "Data": ...,
    }


# PutRecordsRequestEntryTypeDef definition

class PutRecordsRequestEntryTypeDef(TypedDict):
    Data: BlobTypeDef,
    PartitionKey: str,
    ExplicitHashKey: NotRequired[str],
```

## ChildShardTypeDef

```python
# ChildShardTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ChildShardTypeDef


def get_value() -> ChildShardTypeDef:
    return {
        "ShardId": ...,
    }


# ChildShardTypeDef definition

class ChildShardTypeDef(TypedDict):
    ShardId: str,
    ParentShards: List[str],
    HashKeyRange: HashKeyRangeTypeDef,  # (1)
```

1. See [:material-code-braces: HashKeyRangeTypeDef](./type_defs.md#hashkeyrangetypedef) 
## CreateStreamInputTypeDef

```python
# CreateStreamInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import CreateStreamInputTypeDef


def get_value() -> CreateStreamInputTypeDef:
    return {
        "StreamName": ...,
    }


# CreateStreamInputTypeDef definition

class CreateStreamInputTypeDef(TypedDict):
    StreamName: str,
    ShardCount: NotRequired[int],
    StreamModeDetails: NotRequired[StreamModeDetailsTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
## StreamSummaryTypeDef

```python
# StreamSummaryTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StreamSummaryTypeDef


def get_value() -> StreamSummaryTypeDef:
    return {
        "StreamName": ...,
    }


# StreamSummaryTypeDef definition

class StreamSummaryTypeDef(TypedDict):
    StreamName: str,
    StreamARN: str,
    StreamStatus: StreamStatusType,  # (1)
    StreamModeDetails: NotRequired[StreamModeDetailsTypeDef],  # (2)
    StreamCreationTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StreamStatusType](./literals.md#streamstatustype) 
2. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
## UpdateStreamModeInputTypeDef

```python
# UpdateStreamModeInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import UpdateStreamModeInputTypeDef


def get_value() -> UpdateStreamModeInputTypeDef:
    return {
        "StreamARN": ...,
    }


# UpdateStreamModeInputTypeDef definition

class UpdateStreamModeInputTypeDef(TypedDict):
    StreamARN: str,
    StreamModeDetails: StreamModeDetailsTypeDef,  # (1)
```

1. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
## DescribeLimitsOutputTypeDef

```python
# DescribeLimitsOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeLimitsOutputTypeDef


def get_value() -> DescribeLimitsOutputTypeDef:
    return {
        "ShardLimit": ...,
    }


# DescribeLimitsOutputTypeDef definition

class DescribeLimitsOutputTypeDef(TypedDict):
    ShardLimit: int,
    OpenShardCount: int,
    OnDemandStreamCount: int,
    OnDemandStreamCountLimit: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStreamConsumerOutputTypeDef

```python
# DescribeStreamConsumerOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamConsumerOutputTypeDef


def get_value() -> DescribeStreamConsumerOutputTypeDef:
    return {
        "ConsumerDescription": ...,
    }


# DescribeStreamConsumerOutputTypeDef definition

class DescribeStreamConsumerOutputTypeDef(TypedDict):
    ConsumerDescription: ConsumerDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumerDescriptionTypeDef](./type_defs.md#consumerdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnhancedMonitoringOutputTypeDef

```python
# EnhancedMonitoringOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import EnhancedMonitoringOutputTypeDef


def get_value() -> EnhancedMonitoringOutputTypeDef:
    return {
        "StreamName": ...,
    }


# EnhancedMonitoringOutputTypeDef definition

class EnhancedMonitoringOutputTypeDef(TypedDict):
    StreamName: str,
    CurrentShardLevelMetrics: List[MetricsNameType],  # (1)
    DesiredShardLevelMetrics: List[MetricsNameType],  # (1)
    StreamARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
2. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyOutputTypeDef

```python
# GetResourcePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetResourcePolicyOutputTypeDef


def get_value() -> GetResourcePolicyOutputTypeDef:
    return {
        "Policy": ...,
    }


# GetResourcePolicyOutputTypeDef definition

class GetResourcePolicyOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetShardIteratorOutputTypeDef

```python
# GetShardIteratorOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetShardIteratorOutputTypeDef


def get_value() -> GetShardIteratorOutputTypeDef:
    return {
        "ShardIterator": ...,
    }


# GetShardIteratorOutputTypeDef definition

class GetShardIteratorOutputTypeDef(TypedDict):
    ShardIterator: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamConsumersOutputTypeDef

```python
# ListStreamConsumersOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamConsumersOutputTypeDef


def get_value() -> ListStreamConsumersOutputTypeDef:
    return {
        "Consumers": ...,
    }


# ListStreamConsumersOutputTypeDef definition

class ListStreamConsumersOutputTypeDef(TypedDict):
    Consumers: List[ConsumerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConsumerTypeDef](./type_defs.md#consumertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRecordOutputTypeDef

```python
# PutRecordOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordOutputTypeDef


def get_value() -> PutRecordOutputTypeDef:
    return {
        "ShardId": ...,
    }


# PutRecordOutputTypeDef definition

class PutRecordOutputTypeDef(TypedDict):
    ShardId: str,
    SequenceNumber: str,
    EncryptionType: EncryptionTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterStreamConsumerOutputTypeDef

```python
# RegisterStreamConsumerOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import RegisterStreamConsumerOutputTypeDef


def get_value() -> RegisterStreamConsumerOutputTypeDef:
    return {
        "Consumer": ...,
    }


# RegisterStreamConsumerOutputTypeDef definition

class RegisterStreamConsumerOutputTypeDef(TypedDict):
    Consumer: ConsumerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumerTypeDef](./type_defs.md#consumertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateShardCountOutputTypeDef

```python
# UpdateShardCountOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import UpdateShardCountOutputTypeDef


def get_value() -> UpdateShardCountOutputTypeDef:
    return {
        "StreamName": ...,
    }


# UpdateShardCountOutputTypeDef definition

class UpdateShardCountOutputTypeDef(TypedDict):
    StreamName: str,
    CurrentShardCount: int,
    TargetShardCount: int,
    StreamARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStreamInputPaginateTypeDef

```python
# DescribeStreamInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamInputPaginateTypeDef


def get_value() -> DescribeStreamInputPaginateTypeDef:
    return {
        "StreamName": ...,
    }


# DescribeStreamInputPaginateTypeDef definition

class DescribeStreamInputPaginateTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamsInputPaginateTypeDef

```python
# ListStreamsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamsInputPaginateTypeDef


def get_value() -> ListStreamsInputPaginateTypeDef:
    return {
        "ExclusiveStartStreamName": ...,
    }


# ListStreamsInputPaginateTypeDef definition

class ListStreamsInputPaginateTypeDef(TypedDict):
    ExclusiveStartStreamName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStreamInputWaitExtraTypeDef

```python
# DescribeStreamInputWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamInputWaitExtraTypeDef


def get_value() -> DescribeStreamInputWaitExtraTypeDef:
    return {
        "StreamName": ...,
    }


# DescribeStreamInputWaitExtraTypeDef definition

class DescribeStreamInputWaitExtraTypeDef(TypedDict):
    StreamName: NotRequired[str],
    Limit: NotRequired[int],
    ExclusiveStartShardId: NotRequired[str],
    StreamARN: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeStreamInputWaitTypeDef

```python
# DescribeStreamInputWaitTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamInputWaitTypeDef


def get_value() -> DescribeStreamInputWaitTypeDef:
    return {
        "StreamName": ...,
    }


# DescribeStreamInputWaitTypeDef definition

class DescribeStreamInputWaitTypeDef(TypedDict):
    StreamName: NotRequired[str],
    Limit: NotRequired[int],
    ExclusiveStartShardId: NotRequired[str],
    StreamARN: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## StreamDescriptionSummaryTypeDef

```python
# StreamDescriptionSummaryTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StreamDescriptionSummaryTypeDef


def get_value() -> StreamDescriptionSummaryTypeDef:
    return {
        "StreamName": ...,
    }


# StreamDescriptionSummaryTypeDef definition

class StreamDescriptionSummaryTypeDef(TypedDict):
    StreamName: str,
    StreamARN: str,
    StreamStatus: StreamStatusType,  # (1)
    RetentionPeriodHours: int,
    StreamCreationTimestamp: datetime,
    EnhancedMonitoring: List[EnhancedMetricsTypeDef],  # (3)
    OpenShardCount: int,
    StreamModeDetails: NotRequired[StreamModeDetailsTypeDef],  # (2)
    EncryptionType: NotRequired[EncryptionTypeType],  # (4)
    KeyId: NotRequired[str],
    ConsumerCount: NotRequired[int],
```

1. See [:material-code-brackets: StreamStatusType](./literals.md#streamstatustype) 
2. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
3. See [:material-code-braces: EnhancedMetricsTypeDef](./type_defs.md#enhancedmetricstypedef) 
4. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## GetShardIteratorInputTypeDef

```python
# GetShardIteratorInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetShardIteratorInputTypeDef


def get_value() -> GetShardIteratorInputTypeDef:
    return {
        "ShardId": ...,
    }


# GetShardIteratorInputTypeDef definition

class GetShardIteratorInputTypeDef(TypedDict):
    ShardId: str,
    ShardIteratorType: ShardIteratorTypeType,  # (1)
    StreamName: NotRequired[str],
    StartingSequenceNumber: NotRequired[str],
    Timestamp: NotRequired[TimestampTypeDef],
    StreamARN: NotRequired[str],
```

1. See [:material-code-brackets: ShardIteratorTypeType](./literals.md#sharditeratortypetype) 
## ListStreamConsumersInputPaginateTypeDef

```python
# ListStreamConsumersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamConsumersInputPaginateTypeDef


def get_value() -> ListStreamConsumersInputPaginateTypeDef:
    return {
        "StreamARN": ...,
    }


# ListStreamConsumersInputPaginateTypeDef definition

class ListStreamConsumersInputPaginateTypeDef(TypedDict):
    StreamARN: str,
    StreamCreationTimestamp: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamConsumersInputTypeDef

```python
# ListStreamConsumersInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamConsumersInputTypeDef


def get_value() -> ListStreamConsumersInputTypeDef:
    return {
        "StreamARN": ...,
    }


# ListStreamConsumersInputTypeDef definition

class ListStreamConsumersInputTypeDef(TypedDict):
    StreamARN: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StreamCreationTimestamp: NotRequired[TimestampTypeDef],
```

## ShardFilterTypeDef

```python
# ShardFilterTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ShardFilterTypeDef


def get_value() -> ShardFilterTypeDef:
    return {
        "Type": ...,
    }


# ShardFilterTypeDef definition

class ShardFilterTypeDef(TypedDict):
    Type: ShardFilterTypeType,  # (1)
    ShardId: NotRequired[str],
    Timestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ShardFilterTypeType](./literals.md#shardfiltertypetype) 
## StartingPositionTypeDef

```python
# StartingPositionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StartingPositionTypeDef


def get_value() -> StartingPositionTypeDef:
    return {
        "Type": ...,
    }


# StartingPositionTypeDef definition

class StartingPositionTypeDef(TypedDict):
    Type: ShardIteratorTypeType,  # (1)
    SequenceNumber: NotRequired[str],
    Timestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ShardIteratorTypeType](./literals.md#sharditeratortypetype) 
## ListTagsForStreamOutputTypeDef

```python
# ListTagsForStreamOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListTagsForStreamOutputTypeDef


def get_value() -> ListTagsForStreamOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForStreamOutputTypeDef definition

class ListTagsForStreamOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    HasMoreTags: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRecordsOutputTypeDef

```python
# PutRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordsOutputTypeDef


def get_value() -> PutRecordsOutputTypeDef:
    return {
        "FailedRecordCount": ...,
    }


# PutRecordsOutputTypeDef definition

class PutRecordsOutputTypeDef(TypedDict):
    FailedRecordCount: int,
    Records: List[PutRecordsResultEntryTypeDef],  # (1)
    EncryptionType: EncryptionTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PutRecordsResultEntryTypeDef](./type_defs.md#putrecordsresultentrytypedef) 
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ShardTypeDef

```python
# ShardTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ShardTypeDef


def get_value() -> ShardTypeDef:
    return {
        "ShardId": ...,
    }


# ShardTypeDef definition

class ShardTypeDef(TypedDict):
    ShardId: str,
    HashKeyRange: HashKeyRangeTypeDef,  # (1)
    SequenceNumberRange: SequenceNumberRangeTypeDef,  # (2)
    ParentShardId: NotRequired[str],
    AdjacentParentShardId: NotRequired[str],
```

1. See [:material-code-braces: HashKeyRangeTypeDef](./type_defs.md#hashkeyrangetypedef) 
2. See [:material-code-braces: SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef) 
## PutRecordsInputTypeDef

```python
# PutRecordsInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import PutRecordsInputTypeDef


def get_value() -> PutRecordsInputTypeDef:
    return {
        "Records": ...,
    }


# PutRecordsInputTypeDef definition

class PutRecordsInputTypeDef(TypedDict):
    Records: Sequence[PutRecordsRequestEntryTypeDef],  # (1)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-braces: PutRecordsRequestEntryTypeDef](./type_defs.md#putrecordsrequestentrytypedef) 
## GetRecordsOutputTypeDef

```python
# GetRecordsOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import GetRecordsOutputTypeDef


def get_value() -> GetRecordsOutputTypeDef:
    return {
        "Records": ...,
    }


# GetRecordsOutputTypeDef definition

class GetRecordsOutputTypeDef(TypedDict):
    Records: List[RecordTypeDef],  # (1)
    NextShardIterator: str,
    MillisBehindLatest: int,
    ChildShards: List[ChildShardTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: ChildShardTypeDef](./type_defs.md#childshardtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribeToShardEventTypeDef

```python
# SubscribeToShardEventTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SubscribeToShardEventTypeDef


def get_value() -> SubscribeToShardEventTypeDef:
    return {
        "Records": ...,
    }


# SubscribeToShardEventTypeDef definition

class SubscribeToShardEventTypeDef(TypedDict):
    Records: List[RecordTypeDef],  # (1)
    ContinuationSequenceNumber: str,
    MillisBehindLatest: int,
    ChildShards: NotRequired[List[ChildShardTypeDef]],  # (2)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: ChildShardTypeDef](./type_defs.md#childshardtypedef) 
## ListStreamsOutputTypeDef

```python
# ListStreamsOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListStreamsOutputTypeDef


def get_value() -> ListStreamsOutputTypeDef:
    return {
        "StreamNames": ...,
    }


# ListStreamsOutputTypeDef definition

class ListStreamsOutputTypeDef(TypedDict):
    StreamNames: List[str],
    HasMoreStreams: bool,
    StreamSummaries: List[StreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSummaryTypeDef](./type_defs.md#streamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStreamSummaryOutputTypeDef

```python
# DescribeStreamSummaryOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamSummaryOutputTypeDef


def get_value() -> DescribeStreamSummaryOutputTypeDef:
    return {
        "StreamDescriptionSummary": ...,
    }


# DescribeStreamSummaryOutputTypeDef definition

class DescribeStreamSummaryOutputTypeDef(TypedDict):
    StreamDescriptionSummary: StreamDescriptionSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamDescriptionSummaryTypeDef](./type_defs.md#streamdescriptionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListShardsInputPaginateTypeDef

```python
# ListShardsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListShardsInputPaginateTypeDef


def get_value() -> ListShardsInputPaginateTypeDef:
    return {
        "StreamName": ...,
    }


# ListShardsInputPaginateTypeDef definition

class ListShardsInputPaginateTypeDef(TypedDict):
    StreamName: NotRequired[str],
    ExclusiveStartShardId: NotRequired[str],
    StreamCreationTimestamp: NotRequired[TimestampTypeDef],
    ShardFilter: NotRequired[ShardFilterTypeDef],  # (1)
    StreamARN: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ShardFilterTypeDef](./type_defs.md#shardfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListShardsInputTypeDef

```python
# ListShardsInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListShardsInputTypeDef


def get_value() -> ListShardsInputTypeDef:
    return {
        "StreamName": ...,
    }


# ListShardsInputTypeDef definition

class ListShardsInputTypeDef(TypedDict):
    StreamName: NotRequired[str],
    NextToken: NotRequired[str],
    ExclusiveStartShardId: NotRequired[str],
    MaxResults: NotRequired[int],
    StreamCreationTimestamp: NotRequired[TimestampTypeDef],
    ShardFilter: NotRequired[ShardFilterTypeDef],  # (1)
    StreamARN: NotRequired[str],
```

1. See [:material-code-braces: ShardFilterTypeDef](./type_defs.md#shardfiltertypedef) 
## SubscribeToShardInputTypeDef

```python
# SubscribeToShardInputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SubscribeToShardInputTypeDef


def get_value() -> SubscribeToShardInputTypeDef:
    return {
        "ConsumerARN": ...,
    }


# SubscribeToShardInputTypeDef definition

class SubscribeToShardInputTypeDef(TypedDict):
    ConsumerARN: str,
    ShardId: str,
    StartingPosition: StartingPositionTypeDef,  # (1)
```

1. See [:material-code-braces: StartingPositionTypeDef](./type_defs.md#startingpositiontypedef) 
## ListShardsOutputTypeDef

```python
# ListShardsOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import ListShardsOutputTypeDef


def get_value() -> ListShardsOutputTypeDef:
    return {
        "Shards": ...,
    }


# ListShardsOutputTypeDef definition

class ListShardsOutputTypeDef(TypedDict):
    Shards: List[ShardTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ShardTypeDef](./type_defs.md#shardtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamDescriptionTypeDef

```python
# StreamDescriptionTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import StreamDescriptionTypeDef


def get_value() -> StreamDescriptionTypeDef:
    return {
        "StreamName": ...,
    }


# StreamDescriptionTypeDef definition

class StreamDescriptionTypeDef(TypedDict):
    StreamName: str,
    StreamARN: str,
    StreamStatus: StreamStatusType,  # (1)
    Shards: List[ShardTypeDef],  # (3)
    HasMoreShards: bool,
    RetentionPeriodHours: int,
    StreamCreationTimestamp: datetime,
    EnhancedMonitoring: List[EnhancedMetricsTypeDef],  # (4)
    StreamModeDetails: NotRequired[StreamModeDetailsTypeDef],  # (2)
    EncryptionType: NotRequired[EncryptionTypeType],  # (5)
    KeyId: NotRequired[str],
```

1. See [:material-code-brackets: StreamStatusType](./literals.md#streamstatustype) 
2. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
3. See [:material-code-braces: ShardTypeDef](./type_defs.md#shardtypedef) 
4. See [:material-code-braces: EnhancedMetricsTypeDef](./type_defs.md#enhancedmetricstypedef) 
5. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## SubscribeToShardEventStreamTypeDef

```python
# SubscribeToShardEventStreamTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SubscribeToShardEventStreamTypeDef


def get_value() -> SubscribeToShardEventStreamTypeDef:
    return {
        "SubscribeToShardEvent": ...,
    }


# SubscribeToShardEventStreamTypeDef definition

class SubscribeToShardEventStreamTypeDef(TypedDict):
    SubscribeToShardEvent: SubscribeToShardEventTypeDef,  # (1)
    ResourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (2)
    ResourceInUseException: NotRequired[ResourceInUseExceptionTypeDef],  # (3)
    KMSDisabledException: NotRequired[KMSDisabledExceptionTypeDef],  # (4)
    KMSInvalidStateException: NotRequired[KMSInvalidStateExceptionTypeDef],  # (5)
    KMSAccessDeniedException: NotRequired[KMSAccessDeniedExceptionTypeDef],  # (6)
    KMSNotFoundException: NotRequired[KMSNotFoundExceptionTypeDef],  # (7)
    KMSOptInRequired: NotRequired[KMSOptInRequiredTypeDef],  # (8)
    KMSThrottlingException: NotRequired[KMSThrottlingExceptionTypeDef],  # (9)
    InternalFailureException: NotRequired[InternalFailureExceptionTypeDef],  # (10)
```

1. See [:material-code-braces: SubscribeToShardEventTypeDef](./type_defs.md#subscribetoshardeventtypedef) 
2. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
3. See [:material-code-braces: ResourceInUseExceptionTypeDef](./type_defs.md#resourceinuseexceptiontypedef) 
4. See [:material-code-braces: KMSDisabledExceptionTypeDef](./type_defs.md#kmsdisabledexceptiontypedef) 
5. See [:material-code-braces: KMSInvalidStateExceptionTypeDef](./type_defs.md#kmsinvalidstateexceptiontypedef) 
6. See [:material-code-braces: KMSAccessDeniedExceptionTypeDef](./type_defs.md#kmsaccessdeniedexceptiontypedef) 
7. See [:material-code-braces: KMSNotFoundExceptionTypeDef](./type_defs.md#kmsnotfoundexceptiontypedef) 
8. See [:material-code-braces: KMSOptInRequiredTypeDef](./type_defs.md#kmsoptinrequiredtypedef) 
9. See [:material-code-braces: KMSThrottlingExceptionTypeDef](./type_defs.md#kmsthrottlingexceptiontypedef) 
10. See [:material-code-braces: InternalFailureExceptionTypeDef](./type_defs.md#internalfailureexceptiontypedef) 
## DescribeStreamOutputTypeDef

```python
# DescribeStreamOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import DescribeStreamOutputTypeDef


def get_value() -> DescribeStreamOutputTypeDef:
    return {
        "StreamDescription": ...,
    }


# DescribeStreamOutputTypeDef definition

class DescribeStreamOutputTypeDef(TypedDict):
    StreamDescription: StreamDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamDescriptionTypeDef](./type_defs.md#streamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribeToShardOutputTypeDef

```python
# SubscribeToShardOutputTypeDef TypedDict usage example

from types_aiobotocore_kinesis.type_defs import SubscribeToShardOutputTypeDef


def get_value() -> SubscribeToShardOutputTypeDef:
    return {
        "EventStream": ...,
    }


# SubscribeToShardOutputTypeDef definition

class SubscribeToShardOutputTypeDef(TypedDict):
    EventStream: AioEventStream[SubscribeToShardEventStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscribeToShardEventStreamTypeDef](./type_defs.md#subscribetoshardeventstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
