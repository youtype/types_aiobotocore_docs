# Type definitions

> [Index](../README.md) > [QLDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#qldb)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CancelJournalKinesisStreamRequestRequestTypeDef

```python
# CancelJournalKinesisStreamRequestRequestTypeDef definition

class CancelJournalKinesisStreamRequestRequestTypeDef(TypedDict):
    LedgerName: str,
    StreamId: str,
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

## CreateLedgerRequestRequestTypeDef

```python
# CreateLedgerRequestRequestTypeDef definition

class CreateLedgerRequestRequestTypeDef(TypedDict):
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
    Tags: NotRequired[Mapping[str, str]],
    DeletionProtection: NotRequired[bool],
    KmsKey: NotRequired[str],
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
## DeleteLedgerRequestRequestTypeDef

```python
# DeleteLedgerRequestRequestTypeDef definition

class DeleteLedgerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeJournalKinesisStreamRequestRequestTypeDef

```python
# DescribeJournalKinesisStreamRequestRequestTypeDef definition

class DescribeJournalKinesisStreamRequestRequestTypeDef(TypedDict):
    LedgerName: str,
    StreamId: str,
```

## DescribeJournalS3ExportRequestRequestTypeDef

```python
# DescribeJournalS3ExportRequestRequestTypeDef definition

class DescribeJournalS3ExportRequestRequestTypeDef(TypedDict):
    Name: str,
    ExportId: str,
```

## DescribeLedgerRequestRequestTypeDef

```python
# DescribeLedgerRequestRequestTypeDef definition

class DescribeLedgerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## LedgerEncryptionDescriptionTypeDef

```python
# LedgerEncryptionDescriptionTypeDef definition

class LedgerEncryptionDescriptionTypeDef(TypedDict):
    KmsKeyArn: str,
    EncryptionStatus: EncryptionStatusType,  # (1)
    InaccessibleKmsKeyDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype) 
## ValueHolderTypeDef

```python
# ValueHolderTypeDef definition

class ValueHolderTypeDef(TypedDict):
    IonText: NotRequired[str],
```

## GetDigestRequestRequestTypeDef

```python
# GetDigestRequestRequestTypeDef definition

class GetDigestRequestRequestTypeDef(TypedDict):
    Name: str,
```

## KinesisConfigurationTypeDef

```python
# KinesisConfigurationTypeDef definition

class KinesisConfigurationTypeDef(TypedDict):
    StreamArn: str,
    AggregationEnabled: NotRequired[bool],
```

## LedgerSummaryTypeDef

```python
# LedgerSummaryTypeDef definition

class LedgerSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[LedgerStateType],  # (1)
    CreationDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: LedgerStateType](./literals.md#ledgerstatetype) 
## ListJournalKinesisStreamsForLedgerRequestRequestTypeDef

```python
# ListJournalKinesisStreamsForLedgerRequestRequestTypeDef definition

class ListJournalKinesisStreamsForLedgerRequestRequestTypeDef(TypedDict):
    LedgerName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJournalS3ExportsForLedgerRequestRequestTypeDef

```python
# ListJournalS3ExportsForLedgerRequestRequestTypeDef definition

class ListJournalS3ExportsForLedgerRequestRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJournalS3ExportsRequestRequestTypeDef

```python
# ListJournalS3ExportsRequestRequestTypeDef definition

class ListJournalS3ExportsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLedgersRequestRequestTypeDef

```python
# ListLedgersRequestRequestTypeDef definition

class ListLedgersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## S3EncryptionConfigurationTypeDef

```python
# S3EncryptionConfigurationTypeDef definition

class S3EncryptionConfigurationTypeDef(TypedDict):
    ObjectEncryptionType: S3ObjectEncryptionTypeType,  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3ObjectEncryptionTypeType](./literals.md#s3objectencryptiontypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateLedgerPermissionsModeRequestRequestTypeDef

```python
# UpdateLedgerPermissionsModeRequestRequestTypeDef definition

class UpdateLedgerPermissionsModeRequestRequestTypeDef(TypedDict):
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
## UpdateLedgerRequestRequestTypeDef

```python
# UpdateLedgerRequestRequestTypeDef definition

class UpdateLedgerRequestRequestTypeDef(TypedDict):
    Name: str,
    DeletionProtection: NotRequired[bool],
    KmsKey: NotRequired[str],
```

## CancelJournalKinesisStreamResponseTypeDef

```python
# CancelJournalKinesisStreamResponseTypeDef definition

class CancelJournalKinesisStreamResponseTypeDef(TypedDict):
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLedgerResponseTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportJournalToS3ResponseTypeDef

```python
# ExportJournalToS3ResponseTypeDef definition

class ExportJournalToS3ResponseTypeDef(TypedDict):
    ExportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamJournalToKinesisResponseTypeDef

```python
# StreamJournalToKinesisResponseTypeDef definition

class StreamJournalToKinesisResponseTypeDef(TypedDict):
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLedgerPermissionsModeResponseTypeDef

```python
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
## GetBlockRequestRequestTypeDef

```python
# GetBlockRequestRequestTypeDef definition

class GetBlockRequestRequestTypeDef(TypedDict):
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DigestTipAddress: NotRequired[ValueHolderTypeDef],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
## GetBlockResponseTypeDef

```python
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
# GetDigestResponseTypeDef definition

class GetDigestResponseTypeDef(TypedDict):
    Digest: bytes,
    DigestTipAddress: ValueHolderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRevisionRequestRequestTypeDef

```python
# GetRevisionRequestRequestTypeDef definition

class GetRevisionRequestRequestTypeDef(TypedDict):
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DocumentId: str,
    DigestTipAddress: NotRequired[ValueHolderTypeDef],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
## GetRevisionResponseTypeDef

```python
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
## StreamJournalToKinesisRequestRequestTypeDef

```python
# StreamJournalToKinesisRequestRequestTypeDef definition

class StreamJournalToKinesisRequestRequestTypeDef(TypedDict):
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
# S3ExportConfigurationTypeDef definition

class S3ExportConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: str,
    EncryptionConfiguration: S3EncryptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: S3EncryptionConfigurationTypeDef](./type_defs.md#s3encryptionconfigurationtypedef) 
## DescribeJournalKinesisStreamResponseTypeDef

```python
# DescribeJournalKinesisStreamResponseTypeDef definition

class DescribeJournalKinesisStreamResponseTypeDef(TypedDict):
    Stream: JournalKinesisStreamDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JournalKinesisStreamDescriptionTypeDef](./type_defs.md#journalkinesisstreamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJournalKinesisStreamsForLedgerResponseTypeDef

```python
# ListJournalKinesisStreamsForLedgerResponseTypeDef definition

class ListJournalKinesisStreamsForLedgerResponseTypeDef(TypedDict):
    Streams: List[JournalKinesisStreamDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JournalKinesisStreamDescriptionTypeDef](./type_defs.md#journalkinesisstreamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportJournalToS3RequestRequestTypeDef

```python
# ExportJournalToS3RequestRequestTypeDef definition

class ExportJournalToS3RequestRequestTypeDef(TypedDict):
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
# DescribeJournalS3ExportResponseTypeDef definition

class DescribeJournalS3ExportResponseTypeDef(TypedDict):
    ExportDescription: JournalS3ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJournalS3ExportsForLedgerResponseTypeDef

```python
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
# ListJournalS3ExportsResponseTypeDef definition

class ListJournalS3ExportsResponseTypeDef(TypedDict):
    JournalS3Exports: List[JournalS3ExportDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
