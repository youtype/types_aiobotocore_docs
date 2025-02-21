# Type definitions

> [Index](../README.md) > [QLDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#qldb)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_qldb.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CancelJournalKinesisStreamRequestTypeDef

```python
# CancelJournalKinesisStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestTypeDef


def get_value() -> CancelJournalKinesisStreamRequestTypeDef:
    return {
        "LedgerName": ...,
    }


# CancelJournalKinesisStreamRequestTypeDef definition

class CancelJournalKinesisStreamRequestTypeDef(TypedDict):
    LedgerName: str,
    StreamId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ResponseMetadataTypeDef


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

## CreateLedgerRequestTypeDef

```python
# CreateLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import CreateLedgerRequestTypeDef


def get_value() -> CreateLedgerRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateLedgerRequestTypeDef definition

class CreateLedgerRequestTypeDef(TypedDict):
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
    Tags: NotRequired[Mapping[str, str]],
    DeletionProtection: NotRequired[bool],
    KmsKey: NotRequired[str],
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
## DeleteLedgerRequestTypeDef

```python
# DeleteLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DeleteLedgerRequestTypeDef


def get_value() -> DeleteLedgerRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteLedgerRequestTypeDef definition

class DeleteLedgerRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeJournalKinesisStreamRequestTypeDef

```python
# DescribeJournalKinesisStreamRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeJournalKinesisStreamRequestTypeDef


def get_value() -> DescribeJournalKinesisStreamRequestTypeDef:
    return {
        "LedgerName": ...,
    }


# DescribeJournalKinesisStreamRequestTypeDef definition

class DescribeJournalKinesisStreamRequestTypeDef(TypedDict):
    LedgerName: str,
    StreamId: str,
```

## DescribeJournalS3ExportRequestTypeDef

```python
# DescribeJournalS3ExportRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeJournalS3ExportRequestTypeDef


def get_value() -> DescribeJournalS3ExportRequestTypeDef:
    return {
        "Name": ...,
    }


# DescribeJournalS3ExportRequestTypeDef definition

class DescribeJournalS3ExportRequestTypeDef(TypedDict):
    Name: str,
    ExportId: str,
```

## DescribeLedgerRequestTypeDef

```python
# DescribeLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeLedgerRequestTypeDef


def get_value() -> DescribeLedgerRequestTypeDef:
    return {
        "Name": ...,
    }


# DescribeLedgerRequestTypeDef definition

class DescribeLedgerRequestTypeDef(TypedDict):
    Name: str,
```

## LedgerEncryptionDescriptionTypeDef

```python
# LedgerEncryptionDescriptionTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import LedgerEncryptionDescriptionTypeDef


def get_value() -> LedgerEncryptionDescriptionTypeDef:
    return {
        "KmsKeyArn": ...,
    }


# LedgerEncryptionDescriptionTypeDef definition

class LedgerEncryptionDescriptionTypeDef(TypedDict):
    KmsKeyArn: str,
    EncryptionStatus: EncryptionStatusType,  # (1)
    InaccessibleKmsKeyDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype) 
## ValueHolderTypeDef

```python
# ValueHolderTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ValueHolderTypeDef


def get_value() -> ValueHolderTypeDef:
    return {
        "IonText": ...,
    }


# ValueHolderTypeDef definition

class ValueHolderTypeDef(TypedDict):
    IonText: NotRequired[str],
```

## GetDigestRequestTypeDef

```python
# GetDigestRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetDigestRequestTypeDef


def get_value() -> GetDigestRequestTypeDef:
    return {
        "Name": ...,
    }


# GetDigestRequestTypeDef definition

class GetDigestRequestTypeDef(TypedDict):
    Name: str,
```

## KinesisConfigurationTypeDef

```python
# KinesisConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import KinesisConfigurationTypeDef


def get_value() -> KinesisConfigurationTypeDef:
    return {
        "StreamArn": ...,
    }


# KinesisConfigurationTypeDef definition

class KinesisConfigurationTypeDef(TypedDict):
    StreamArn: str,
    AggregationEnabled: NotRequired[bool],
```

## LedgerSummaryTypeDef

```python
# LedgerSummaryTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import LedgerSummaryTypeDef


def get_value() -> LedgerSummaryTypeDef:
    return {
        "Name": ...,
    }


# LedgerSummaryTypeDef definition

class LedgerSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[LedgerStateType],  # (1)
    CreationDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: LedgerStateType](./literals.md#ledgerstatetype) 
## ListJournalKinesisStreamsForLedgerRequestTypeDef

```python
# ListJournalKinesisStreamsForLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalKinesisStreamsForLedgerRequestTypeDef


def get_value() -> ListJournalKinesisStreamsForLedgerRequestTypeDef:
    return {
        "LedgerName": ...,
    }


# ListJournalKinesisStreamsForLedgerRequestTypeDef definition

class ListJournalKinesisStreamsForLedgerRequestTypeDef(TypedDict):
    LedgerName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJournalS3ExportsForLedgerRequestTypeDef

```python
# ListJournalS3ExportsForLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalS3ExportsForLedgerRequestTypeDef


def get_value() -> ListJournalS3ExportsForLedgerRequestTypeDef:
    return {
        "Name": ...,
    }


# ListJournalS3ExportsForLedgerRequestTypeDef definition

class ListJournalS3ExportsForLedgerRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJournalS3ExportsRequestTypeDef

```python
# ListJournalS3ExportsRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalS3ExportsRequestTypeDef


def get_value() -> ListJournalS3ExportsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListJournalS3ExportsRequestTypeDef definition

class ListJournalS3ExportsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLedgersRequestTypeDef

```python
# ListLedgersRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListLedgersRequestTypeDef


def get_value() -> ListLedgersRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListLedgersRequestTypeDef definition

class ListLedgersRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## S3EncryptionConfigurationTypeDef

```python
# S3EncryptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import S3EncryptionConfigurationTypeDef


def get_value() -> S3EncryptionConfigurationTypeDef:
    return {
        "ObjectEncryptionType": ...,
    }


# S3EncryptionConfigurationTypeDef definition

class S3EncryptionConfigurationTypeDef(TypedDict):
    ObjectEncryptionType: S3ObjectEncryptionTypeType,  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3ObjectEncryptionTypeType](./literals.md#s3objectencryptiontypetype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateLedgerPermissionsModeRequestTypeDef

```python
# UpdateLedgerPermissionsModeRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import UpdateLedgerPermissionsModeRequestTypeDef


def get_value() -> UpdateLedgerPermissionsModeRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateLedgerPermissionsModeRequestTypeDef definition

class UpdateLedgerPermissionsModeRequestTypeDef(TypedDict):
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
## UpdateLedgerRequestTypeDef

```python
# UpdateLedgerRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import UpdateLedgerRequestTypeDef


def get_value() -> UpdateLedgerRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateLedgerRequestTypeDef definition

class UpdateLedgerRequestTypeDef(TypedDict):
    Name: str,
    DeletionProtection: NotRequired[bool],
    KmsKey: NotRequired[str],
```

## CancelJournalKinesisStreamResponseTypeDef

```python
# CancelJournalKinesisStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamResponseTypeDef


def get_value() -> CancelJournalKinesisStreamResponseTypeDef:
    return {
        "StreamId": ...,
    }


# CancelJournalKinesisStreamResponseTypeDef definition

class CancelJournalKinesisStreamResponseTypeDef(TypedDict):
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLedgerResponseTypeDef

```python
# CreateLedgerResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import CreateLedgerResponseTypeDef


def get_value() -> CreateLedgerResponseTypeDef:
    return {
        "Name": ...,
    }


# CreateLedgerResponseTypeDef definition

class CreateLedgerResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    State: LedgerStateType,  # (1)
    CreationDateTime: datetime,
    PermissionsMode: PermissionsModeType,  # (2)
    DeletionProtection: bool,
    KmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LedgerStateType](./literals.md#ledgerstatetype) 
2. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportJournalToS3ResponseTypeDef

```python
# ExportJournalToS3ResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ExportJournalToS3ResponseTypeDef


def get_value() -> ExportJournalToS3ResponseTypeDef:
    return {
        "ExportId": ...,
    }


# ExportJournalToS3ResponseTypeDef definition

class ExportJournalToS3ResponseTypeDef(TypedDict):
    ExportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamJournalToKinesisResponseTypeDef

```python
# StreamJournalToKinesisResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import StreamJournalToKinesisResponseTypeDef


def get_value() -> StreamJournalToKinesisResponseTypeDef:
    return {
        "StreamId": ...,
    }


# StreamJournalToKinesisResponseTypeDef definition

class StreamJournalToKinesisResponseTypeDef(TypedDict):
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLedgerPermissionsModeResponseTypeDef

```python
# UpdateLedgerPermissionsModeResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import UpdateLedgerPermissionsModeResponseTypeDef


def get_value() -> UpdateLedgerPermissionsModeResponseTypeDef:
    return {
        "Name": ...,
    }


# UpdateLedgerPermissionsModeResponseTypeDef definition

class UpdateLedgerPermissionsModeResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    PermissionsMode: PermissionsModeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLedgerResponseTypeDef

```python
# DescribeLedgerResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeLedgerResponseTypeDef


def get_value() -> DescribeLedgerResponseTypeDef:
    return {
        "Name": ...,
    }


# DescribeLedgerResponseTypeDef definition

class DescribeLedgerResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    State: LedgerStateType,  # (1)
    CreationDateTime: datetime,
    PermissionsMode: PermissionsModeType,  # (2)
    DeletionProtection: bool,
    EncryptionDescription: LedgerEncryptionDescriptionTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LedgerStateType](./literals.md#ledgerstatetype) 
2. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
3. See [:material-code-braces: LedgerEncryptionDescriptionTypeDef](./type_defs.md#ledgerencryptiondescriptiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLedgerResponseTypeDef

```python
# UpdateLedgerResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import UpdateLedgerResponseTypeDef


def get_value() -> UpdateLedgerResponseTypeDef:
    return {
        "Name": ...,
    }


# UpdateLedgerResponseTypeDef definition

class UpdateLedgerResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    State: LedgerStateType,  # (1)
    CreationDateTime: datetime,
    DeletionProtection: bool,
    EncryptionDescription: LedgerEncryptionDescriptionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LedgerStateType](./literals.md#ledgerstatetype) 
2. See [:material-code-braces: LedgerEncryptionDescriptionTypeDef](./type_defs.md#ledgerencryptiondescriptiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlockRequestTypeDef

```python
# GetBlockRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetBlockRequestTypeDef


def get_value() -> GetBlockRequestTypeDef:
    return {
        "Name": ...,
    }


# GetBlockRequestTypeDef definition

class GetBlockRequestTypeDef(TypedDict):
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DigestTipAddress: NotRequired[ValueHolderTypeDef],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
## GetBlockResponseTypeDef

```python
# GetBlockResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetBlockResponseTypeDef


def get_value() -> GetBlockResponseTypeDef:
    return {
        "Block": ...,
    }


# GetBlockResponseTypeDef definition

class GetBlockResponseTypeDef(TypedDict):
    Block: ValueHolderTypeDef,  # (1)
    Proof: ValueHolderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDigestResponseTypeDef

```python
# GetDigestResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetDigestResponseTypeDef


def get_value() -> GetDigestResponseTypeDef:
    return {
        "Digest": ...,
    }


# GetDigestResponseTypeDef definition

class GetDigestResponseTypeDef(TypedDict):
    Digest: bytes,
    DigestTipAddress: ValueHolderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRevisionRequestTypeDef

```python
# GetRevisionRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetRevisionRequestTypeDef


def get_value() -> GetRevisionRequestTypeDef:
    return {
        "Name": ...,
    }


# GetRevisionRequestTypeDef definition

class GetRevisionRequestTypeDef(TypedDict):
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DocumentId: str,
    DigestTipAddress: NotRequired[ValueHolderTypeDef],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
## GetRevisionResponseTypeDef

```python
# GetRevisionResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import GetRevisionResponseTypeDef


def get_value() -> GetRevisionResponseTypeDef:
    return {
        "Proof": ...,
    }


# GetRevisionResponseTypeDef definition

class GetRevisionResponseTypeDef(TypedDict):
    Proof: ValueHolderTypeDef,  # (1)
    Revision: ValueHolderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JournalKinesisStreamDescriptionTypeDef

```python
# JournalKinesisStreamDescriptionTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import JournalKinesisStreamDescriptionTypeDef


def get_value() -> JournalKinesisStreamDescriptionTypeDef:
    return {
        "LedgerName": ...,
    }


# JournalKinesisStreamDescriptionTypeDef definition

class JournalKinesisStreamDescriptionTypeDef(TypedDict):
    LedgerName: str,
    RoleArn: str,
    StreamId: str,
    Status: StreamStatusType,  # (1)
    KinesisConfiguration: KinesisConfigurationTypeDef,  # (2)
    StreamName: str,
    CreationTime: NotRequired[datetime],
    InclusiveStartTime: NotRequired[datetime],
    ExclusiveEndTime: NotRequired[datetime],
    Arn: NotRequired[str],
    ErrorCause: NotRequired[ErrorCauseType],  # (3)
```

1. See [:material-code-brackets: StreamStatusType](./literals.md#streamstatustype) 
2. See [:material-code-braces: KinesisConfigurationTypeDef](./type_defs.md#kinesisconfigurationtypedef) 
3. See [:material-code-brackets: ErrorCauseType](./literals.md#errorcausetype) 
## StreamJournalToKinesisRequestTypeDef

```python
# StreamJournalToKinesisRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import StreamJournalToKinesisRequestTypeDef


def get_value() -> StreamJournalToKinesisRequestTypeDef:
    return {
        "LedgerName": ...,
    }


# StreamJournalToKinesisRequestTypeDef definition

class StreamJournalToKinesisRequestTypeDef(TypedDict):
    LedgerName: str,
    RoleArn: str,
    InclusiveStartTime: TimestampTypeDef,
    KinesisConfiguration: KinesisConfigurationTypeDef,  # (1)
    StreamName: str,
    Tags: NotRequired[Mapping[str, str]],
    ExclusiveEndTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: KinesisConfigurationTypeDef](./type_defs.md#kinesisconfigurationtypedef) 
## ListLedgersResponseTypeDef

```python
# ListLedgersResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListLedgersResponseTypeDef


def get_value() -> ListLedgersResponseTypeDef:
    return {
        "Ledgers": ...,
    }


# ListLedgersResponseTypeDef definition

class ListLedgersResponseTypeDef(TypedDict):
    Ledgers: List[LedgerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LedgerSummaryTypeDef](./type_defs.md#ledgersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3ExportConfigurationTypeDef

```python
# S3ExportConfigurationTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import S3ExportConfigurationTypeDef


def get_value() -> S3ExportConfigurationTypeDef:
    return {
        "Bucket": ...,
    }


# S3ExportConfigurationTypeDef definition

class S3ExportConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: str,
    EncryptionConfiguration: S3EncryptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: S3EncryptionConfigurationTypeDef](./type_defs.md#s3encryptionconfigurationtypedef) 
## DescribeJournalKinesisStreamResponseTypeDef

```python
# DescribeJournalKinesisStreamResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeJournalKinesisStreamResponseTypeDef


def get_value() -> DescribeJournalKinesisStreamResponseTypeDef:
    return {
        "Stream": ...,
    }


# DescribeJournalKinesisStreamResponseTypeDef definition

class DescribeJournalKinesisStreamResponseTypeDef(TypedDict):
    Stream: JournalKinesisStreamDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JournalKinesisStreamDescriptionTypeDef](./type_defs.md#journalkinesisstreamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJournalKinesisStreamsForLedgerResponseTypeDef

```python
# ListJournalKinesisStreamsForLedgerResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalKinesisStreamsForLedgerResponseTypeDef


def get_value() -> ListJournalKinesisStreamsForLedgerResponseTypeDef:
    return {
        "Streams": ...,
    }


# ListJournalKinesisStreamsForLedgerResponseTypeDef definition

class ListJournalKinesisStreamsForLedgerResponseTypeDef(TypedDict):
    Streams: List[JournalKinesisStreamDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JournalKinesisStreamDescriptionTypeDef](./type_defs.md#journalkinesisstreamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportJournalToS3RequestTypeDef

```python
# ExportJournalToS3RequestTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ExportJournalToS3RequestTypeDef


def get_value() -> ExportJournalToS3RequestTypeDef:
    return {
        "Name": ...,
    }


# ExportJournalToS3RequestTypeDef definition

class ExportJournalToS3RequestTypeDef(TypedDict):
    Name: str,
    InclusiveStartTime: TimestampTypeDef,
    ExclusiveEndTime: TimestampTypeDef,
    S3ExportConfiguration: S3ExportConfigurationTypeDef,  # (1)
    RoleArn: str,
    OutputFormat: NotRequired[OutputFormatType],  # (2)
```

1. See [:material-code-braces: S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## JournalS3ExportDescriptionTypeDef

```python
# JournalS3ExportDescriptionTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import JournalS3ExportDescriptionTypeDef


def get_value() -> JournalS3ExportDescriptionTypeDef:
    return {
        "LedgerName": ...,
    }


# JournalS3ExportDescriptionTypeDef definition

class JournalS3ExportDescriptionTypeDef(TypedDict):
    LedgerName: str,
    ExportId: str,
    ExportCreationTime: datetime,
    Status: ExportStatusType,  # (1)
    InclusiveStartTime: datetime,
    ExclusiveEndTime: datetime,
    S3ExportConfiguration: S3ExportConfigurationTypeDef,  # (2)
    RoleArn: str,
    OutputFormat: NotRequired[OutputFormatType],  # (3)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-braces: S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef) 
3. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## DescribeJournalS3ExportResponseTypeDef

```python
# DescribeJournalS3ExportResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import DescribeJournalS3ExportResponseTypeDef


def get_value() -> DescribeJournalS3ExportResponseTypeDef:
    return {
        "ExportDescription": ...,
    }


# DescribeJournalS3ExportResponseTypeDef definition

class DescribeJournalS3ExportResponseTypeDef(TypedDict):
    ExportDescription: JournalS3ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJournalS3ExportsForLedgerResponseTypeDef

```python
# ListJournalS3ExportsForLedgerResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalS3ExportsForLedgerResponseTypeDef


def get_value() -> ListJournalS3ExportsForLedgerResponseTypeDef:
    return {
        "JournalS3Exports": ...,
    }


# ListJournalS3ExportsForLedgerResponseTypeDef definition

class ListJournalS3ExportsForLedgerResponseTypeDef(TypedDict):
    JournalS3Exports: List[JournalS3ExportDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJournalS3ExportsResponseTypeDef

```python
# ListJournalS3ExportsResponseTypeDef TypedDict usage example

from types_aiobotocore_qldb.type_defs import ListJournalS3ExportsResponseTypeDef


def get_value() -> ListJournalS3ExportsResponseTypeDef:
    return {
        "JournalS3Exports": ...,
    }


# ListJournalS3ExportsResponseTypeDef definition

class ListJournalS3ExportsResponseTypeDef(TypedDict):
    JournalS3Exports: List[JournalS3ExportDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
