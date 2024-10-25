# Type definitions

> [Index](../README.md) > [Firehose](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Firehose](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
    type annotations stubs module [types-aiobotocore-firehose](https://pypi.org/project/types-aiobotocore-firehose/).

## BlobTypeDef

```python
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
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## DestinationTableConfigurationUnionTypeDef

```python
# DestinationTableConfigurationUnionTypeDef definition

DestinationTableConfigurationUnionTypeDef = Union[
    DestinationTableConfigurationTypeDef,  # (1)
    DestinationTableConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DestinationTableConfigurationTypeDef](./type_defs.md#destinationtableconfigurationtypedef) 
2. See [:material-code-braces: DestinationTableConfigurationOutputTypeDef](./type_defs.md#destinationtableconfigurationoutputtypedef) 

## HiveJsonSerDeUnionTypeDef

```python
# HiveJsonSerDeUnionTypeDef definition

HiveJsonSerDeUnionTypeDef = Union[
    HiveJsonSerDeTypeDef,  # (1)
    HiveJsonSerDeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HiveJsonSerDeTypeDef](./type_defs.md#hivejsonserdetypedef) 
2. See [:material-code-braces: HiveJsonSerDeOutputTypeDef](./type_defs.md#hivejsonserdeoutputtypedef) 

## OpenXJsonSerDeUnionTypeDef

```python
# OpenXJsonSerDeUnionTypeDef definition

OpenXJsonSerDeUnionTypeDef = Union[
    OpenXJsonSerDeTypeDef,  # (1)
    OpenXJsonSerDeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpenXJsonSerDeTypeDef](./type_defs.md#openxjsonserdetypedef) 
2. See [:material-code-braces: OpenXJsonSerDeOutputTypeDef](./type_defs.md#openxjsonserdeoutputtypedef) 

## OrcSerDeUnionTypeDef

```python
# OrcSerDeUnionTypeDef definition

OrcSerDeUnionTypeDef = Union[
    OrcSerDeTypeDef,  # (1)
    OrcSerDeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OrcSerDeTypeDef](./type_defs.md#orcserdetypedef) 
2. See [:material-code-braces: OrcSerDeOutputTypeDef](./type_defs.md#orcserdeoutputtypedef) 

## HttpEndpointRequestConfigurationUnionTypeDef

```python
# HttpEndpointRequestConfigurationUnionTypeDef definition

HttpEndpointRequestConfigurationUnionTypeDef = Union[
    HttpEndpointRequestConfigurationTypeDef,  # (1)
    HttpEndpointRequestConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HttpEndpointRequestConfigurationTypeDef](./type_defs.md#httpendpointrequestconfigurationtypedef) 
2. See [:material-code-braces: HttpEndpointRequestConfigurationOutputTypeDef](./type_defs.md#httpendpointrequestconfigurationoutputtypedef) 

## ProcessorUnionTypeDef

```python
# ProcessorUnionTypeDef definition

ProcessorUnionTypeDef = Union[
    ProcessorTypeDef,  # (1)
    ProcessorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) 
2. See [:material-code-braces: ProcessorOutputTypeDef](./type_defs.md#processoroutputtypedef) 

## DeserializerUnionTypeDef

```python
# DeserializerUnionTypeDef definition

DeserializerUnionTypeDef = Union[
    DeserializerTypeDef,  # (1)
    DeserializerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeserializerTypeDef](./type_defs.md#deserializertypedef) 
2. See [:material-code-braces: DeserializerOutputTypeDef](./type_defs.md#deserializeroutputtypedef) 

## SerializerUnionTypeDef

```python
# SerializerUnionTypeDef definition

SerializerUnionTypeDef = Union[
    SerializerTypeDef,  # (1)
    SerializerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SerializerTypeDef](./type_defs.md#serializertypedef) 
2. See [:material-code-braces: SerializerOutputTypeDef](./type_defs.md#serializeroutputtypedef) 

## ProcessingConfigurationUnionTypeDef

```python
# ProcessingConfigurationUnionTypeDef definition

ProcessingConfigurationUnionTypeDef = Union[
    ProcessingConfigurationTypeDef,  # (1)
    ProcessingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) 
2. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 

## InputFormatConfigurationUnionTypeDef

```python
# InputFormatConfigurationUnionTypeDef definition

InputFormatConfigurationUnionTypeDef = Union[
    InputFormatConfigurationTypeDef,  # (1)
    InputFormatConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputFormatConfigurationTypeDef](./type_defs.md#inputformatconfigurationtypedef) 
2. See [:material-code-braces: InputFormatConfigurationOutputTypeDef](./type_defs.md#inputformatconfigurationoutputtypedef) 

## OutputFormatConfigurationUnionTypeDef

```python
# OutputFormatConfigurationUnionTypeDef definition

OutputFormatConfigurationUnionTypeDef = Union[
    OutputFormatConfigurationTypeDef,  # (1)
    OutputFormatConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputFormatConfigurationTypeDef](./type_defs.md#outputformatconfigurationtypedef) 
2. See [:material-code-braces: OutputFormatConfigurationOutputTypeDef](./type_defs.md#outputformatconfigurationoutputtypedef) 

## DataFormatConversionConfigurationUnionTypeDef

```python
# DataFormatConversionConfigurationUnionTypeDef definition

DataFormatConversionConfigurationUnionTypeDef = Union[
    DataFormatConversionConfigurationTypeDef,  # (1)
    DataFormatConversionConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataFormatConversionConfigurationTypeDef](./type_defs.md#dataformatconversionconfigurationtypedef) 
2. See [:material-code-braces: DataFormatConversionConfigurationOutputTypeDef](./type_defs.md#dataformatconversionconfigurationoutputtypedef) 



## AmazonOpenSearchServerlessBufferingHintsTypeDef

```python
# AmazonOpenSearchServerlessBufferingHintsTypeDef definition

class AmazonOpenSearchServerlessBufferingHintsTypeDef(TypedDict):
    IntervalInSeconds: NotRequired[int],
    SizeInMBs: NotRequired[int],
```

## AmazonOpenSearchServerlessRetryOptionsTypeDef

```python
# AmazonOpenSearchServerlessRetryOptionsTypeDef definition

class AmazonOpenSearchServerlessRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## CloudWatchLoggingOptionsTypeDef

```python
# CloudWatchLoggingOptionsTypeDef definition

class CloudWatchLoggingOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    LogGroupName: NotRequired[str],
    LogStreamName: NotRequired[str],
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    RoleARN: str,
    SecurityGroupIds: Sequence[str],
```

## VpcConfigurationDescriptionTypeDef

```python
# VpcConfigurationDescriptionTypeDef definition

class VpcConfigurationDescriptionTypeDef(TypedDict):
    SubnetIds: List[str],
    RoleARN: str,
    SecurityGroupIds: List[str],
    VpcId: str,
```

## AmazonopensearchserviceBufferingHintsTypeDef

```python
# AmazonopensearchserviceBufferingHintsTypeDef definition

class AmazonopensearchserviceBufferingHintsTypeDef(TypedDict):
    IntervalInSeconds: NotRequired[int],
    SizeInMBs: NotRequired[int],
```

## AmazonopensearchserviceRetryOptionsTypeDef

```python
# AmazonopensearchserviceRetryOptionsTypeDef definition

class AmazonopensearchserviceRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## DocumentIdOptionsTypeDef

```python
# DocumentIdOptionsTypeDef definition

class DocumentIdOptionsTypeDef(TypedDict):
    DefaultDocumentIdFormat: DefaultDocumentIdFormatType,  # (1)
```

1. See [:material-code-brackets: DefaultDocumentIdFormatType](./literals.md#defaultdocumentidformattype) 
## AuthenticationConfigurationTypeDef

```python
# AuthenticationConfigurationTypeDef definition

class AuthenticationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    Connectivity: ConnectivityType,  # (1)
```

1. See [:material-code-brackets: ConnectivityType](./literals.md#connectivitytype) 
## BufferingHintsTypeDef

```python
# BufferingHintsTypeDef definition

class BufferingHintsTypeDef(TypedDict):
    SizeInMBs: NotRequired[int],
    IntervalInSeconds: NotRequired[int],
```

## CatalogConfigurationTypeDef

```python
# CatalogConfigurationTypeDef definition

class CatalogConfigurationTypeDef(TypedDict):
    CatalogARN: NotRequired[str],
```

## CopyCommandTypeDef

```python
# CopyCommandTypeDef definition

class CopyCommandTypeDef(TypedDict):
    DataTableName: str,
    DataTableColumns: NotRequired[str],
    CopyOptions: NotRequired[str],
```

## DeliveryStreamEncryptionConfigurationInputTypeDef

```python
# DeliveryStreamEncryptionConfigurationInputTypeDef definition

class DeliveryStreamEncryptionConfigurationInputTypeDef(TypedDict):
    KeyType: KeyTypeType,  # (1)
    KeyARN: NotRequired[str],
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## KinesisStreamSourceConfigurationTypeDef

```python
# KinesisStreamSourceConfigurationTypeDef definition

class KinesisStreamSourceConfigurationTypeDef(TypedDict):
    KinesisStreamARN: str,
    RoleARN: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
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

## SchemaConfigurationTypeDef

```python
# SchemaConfigurationTypeDef definition

class SchemaConfigurationTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    Region: NotRequired[str],
    VersionId: NotRequired[str],
```

## DeleteDeliveryStreamInputRequestTypeDef

```python
# DeleteDeliveryStreamInputRequestTypeDef definition

class DeleteDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    AllowForceDelete: NotRequired[bool],
```

## FailureDescriptionTypeDef

```python
# FailureDescriptionTypeDef definition

class FailureDescriptionTypeDef(TypedDict):
    Type: DeliveryStreamFailureTypeType,  # (1)
    Details: str,
```

1. See [:material-code-brackets: DeliveryStreamFailureTypeType](./literals.md#deliverystreamfailuretypetype) 
## DescribeDeliveryStreamInputRequestTypeDef

```python
# DescribeDeliveryStreamInputRequestTypeDef definition

class DescribeDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    Limit: NotRequired[int],
    ExclusiveStartDestinationId: NotRequired[str],
```

## HiveJsonSerDeOutputTypeDef

```python
# HiveJsonSerDeOutputTypeDef definition

class HiveJsonSerDeOutputTypeDef(TypedDict):
    TimestampFormats: NotRequired[List[str]],
```

## OpenXJsonSerDeOutputTypeDef

```python
# OpenXJsonSerDeOutputTypeDef definition

class OpenXJsonSerDeOutputTypeDef(TypedDict):
    ConvertDotsInJsonKeysToUnderscores: NotRequired[bool],
    CaseInsensitive: NotRequired[bool],
    ColumnToJsonKeyMappings: NotRequired[Dict[str, str]],
```

## DestinationTableConfigurationOutputTypeDef

```python
# DestinationTableConfigurationOutputTypeDef definition

class DestinationTableConfigurationOutputTypeDef(TypedDict):
    DestinationTableName: str,
    DestinationDatabaseName: str,
    UniqueKeys: NotRequired[List[str]],
    S3ErrorOutputPrefix: NotRequired[str],
```

## DestinationTableConfigurationTypeDef

```python
# DestinationTableConfigurationTypeDef definition

class DestinationTableConfigurationTypeDef(TypedDict):
    DestinationTableName: str,
    DestinationDatabaseName: str,
    UniqueKeys: NotRequired[Sequence[str]],
    S3ErrorOutputPrefix: NotRequired[str],
```

## RetryOptionsTypeDef

```python
# RetryOptionsTypeDef definition

class RetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## ElasticsearchBufferingHintsTypeDef

```python
# ElasticsearchBufferingHintsTypeDef definition

class ElasticsearchBufferingHintsTypeDef(TypedDict):
    IntervalInSeconds: NotRequired[int],
    SizeInMBs: NotRequired[int],
```

## ElasticsearchRetryOptionsTypeDef

```python
# ElasticsearchRetryOptionsTypeDef definition

class ElasticsearchRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## KMSEncryptionConfigTypeDef

```python
# KMSEncryptionConfigTypeDef definition

class KMSEncryptionConfigTypeDef(TypedDict):
    AWSKMSKeyARN: str,
```

## HiveJsonSerDeTypeDef

```python
# HiveJsonSerDeTypeDef definition

class HiveJsonSerDeTypeDef(TypedDict):
    TimestampFormats: NotRequired[Sequence[str]],
```

## HttpEndpointBufferingHintsTypeDef

```python
# HttpEndpointBufferingHintsTypeDef definition

class HttpEndpointBufferingHintsTypeDef(TypedDict):
    SizeInMBs: NotRequired[int],
    IntervalInSeconds: NotRequired[int],
```

## HttpEndpointCommonAttributeTypeDef

```python
# HttpEndpointCommonAttributeTypeDef definition

class HttpEndpointCommonAttributeTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: str,
```

## HttpEndpointConfigurationTypeDef

```python
# HttpEndpointConfigurationTypeDef definition

class HttpEndpointConfigurationTypeDef(TypedDict):
    Url: str,
    Name: NotRequired[str],
    AccessKey: NotRequired[str],
```

## HttpEndpointDescriptionTypeDef

```python
# HttpEndpointDescriptionTypeDef definition

class HttpEndpointDescriptionTypeDef(TypedDict):
    Url: NotRequired[str],
    Name: NotRequired[str],
```

## HttpEndpointRetryOptionsTypeDef

```python
# HttpEndpointRetryOptionsTypeDef definition

class HttpEndpointRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## SecretsManagerConfigurationTypeDef

```python
# SecretsManagerConfigurationTypeDef definition

class SecretsManagerConfigurationTypeDef(TypedDict):
    Enabled: bool,
    SecretARN: NotRequired[str],
    RoleARN: NotRequired[str],
```

## KinesisStreamSourceDescriptionTypeDef

```python
# KinesisStreamSourceDescriptionTypeDef definition

class KinesisStreamSourceDescriptionTypeDef(TypedDict):
    KinesisStreamARN: NotRequired[str],
    RoleARN: NotRequired[str],
    DeliveryStartTimestamp: NotRequired[datetime],
```

## ListDeliveryStreamsInputRequestTypeDef

```python
# ListDeliveryStreamsInputRequestTypeDef definition

class ListDeliveryStreamsInputRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    DeliveryStreamType: NotRequired[DeliveryStreamTypeType],  # (1)
    ExclusiveStartDeliveryStreamName: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryStreamTypeType](./literals.md#deliverystreamtypetype) 
## ListTagsForDeliveryStreamInputRequestTypeDef

```python
# ListTagsForDeliveryStreamInputRequestTypeDef definition

class ListTagsForDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    ExclusiveStartTagKey: NotRequired[str],
    Limit: NotRequired[int],
```

## OpenXJsonSerDeTypeDef

```python
# OpenXJsonSerDeTypeDef definition

class OpenXJsonSerDeTypeDef(TypedDict):
    ConvertDotsInJsonKeysToUnderscores: NotRequired[bool],
    CaseInsensitive: NotRequired[bool],
    ColumnToJsonKeyMappings: NotRequired[Mapping[str, str]],
```

## OrcSerDeOutputTypeDef

```python
# OrcSerDeOutputTypeDef definition

class OrcSerDeOutputTypeDef(TypedDict):
    StripeSizeBytes: NotRequired[int],
    BlockSizeBytes: NotRequired[int],
    RowIndexStride: NotRequired[int],
    EnablePadding: NotRequired[bool],
    PaddingTolerance: NotRequired[float],
    Compression: NotRequired[OrcCompressionType],  # (1)
    BloomFilterColumns: NotRequired[List[str]],
    BloomFilterFalsePositiveProbability: NotRequired[float],
    DictionaryKeyThreshold: NotRequired[float],
    FormatVersion: NotRequired[OrcFormatVersionType],  # (2)
```

1. See [:material-code-brackets: OrcCompressionType](./literals.md#orccompressiontype) 
2. See [:material-code-brackets: OrcFormatVersionType](./literals.md#orcformatversiontype) 
## OrcSerDeTypeDef

```python
# OrcSerDeTypeDef definition

class OrcSerDeTypeDef(TypedDict):
    StripeSizeBytes: NotRequired[int],
    BlockSizeBytes: NotRequired[int],
    RowIndexStride: NotRequired[int],
    EnablePadding: NotRequired[bool],
    PaddingTolerance: NotRequired[float],
    Compression: NotRequired[OrcCompressionType],  # (1)
    BloomFilterColumns: NotRequired[Sequence[str]],
    BloomFilterFalsePositiveProbability: NotRequired[float],
    DictionaryKeyThreshold: NotRequired[float],
    FormatVersion: NotRequired[OrcFormatVersionType],  # (2)
```

1. See [:material-code-brackets: OrcCompressionType](./literals.md#orccompressiontype) 
2. See [:material-code-brackets: OrcFormatVersionType](./literals.md#orcformatversiontype) 
## ParquetSerDeTypeDef

```python
# ParquetSerDeTypeDef definition

class ParquetSerDeTypeDef(TypedDict):
    BlockSizeBytes: NotRequired[int],
    PageSizeBytes: NotRequired[int],
    Compression: NotRequired[ParquetCompressionType],  # (1)
    EnableDictionaryCompression: NotRequired[bool],
    MaxPaddingBytes: NotRequired[int],
    WriterVersion: NotRequired[ParquetWriterVersionType],  # (2)
```

1. See [:material-code-brackets: ParquetCompressionType](./literals.md#parquetcompressiontype) 
2. See [:material-code-brackets: ParquetWriterVersionType](./literals.md#parquetwriterversiontype) 
## ProcessorParameterTypeDef

```python
# ProcessorParameterTypeDef definition

class ProcessorParameterTypeDef(TypedDict):
    ParameterName: ProcessorParameterNameType,  # (1)
    ParameterValue: str,
```

1. See [:material-code-brackets: ProcessorParameterNameType](./literals.md#processorparameternametype) 
## PutRecordBatchResponseEntryTypeDef

```python
# PutRecordBatchResponseEntryTypeDef definition

class PutRecordBatchResponseEntryTypeDef(TypedDict):
    RecordId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## RedshiftRetryOptionsTypeDef

```python
# RedshiftRetryOptionsTypeDef definition

class RedshiftRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## SnowflakeBufferingHintsTypeDef

```python
# SnowflakeBufferingHintsTypeDef definition

class SnowflakeBufferingHintsTypeDef(TypedDict):
    SizeInMBs: NotRequired[int],
    IntervalInSeconds: NotRequired[int],
```

## SnowflakeRetryOptionsTypeDef

```python
# SnowflakeRetryOptionsTypeDef definition

class SnowflakeRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## SnowflakeRoleConfigurationTypeDef

```python
# SnowflakeRoleConfigurationTypeDef definition

class SnowflakeRoleConfigurationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SnowflakeRole: NotRequired[str],
```

## SnowflakeVpcConfigurationTypeDef

```python
# SnowflakeVpcConfigurationTypeDef definition

class SnowflakeVpcConfigurationTypeDef(TypedDict):
    PrivateLinkVpceId: str,
```

## SplunkBufferingHintsTypeDef

```python
# SplunkBufferingHintsTypeDef definition

class SplunkBufferingHintsTypeDef(TypedDict):
    IntervalInSeconds: NotRequired[int],
    SizeInMBs: NotRequired[int],
```

## SplunkRetryOptionsTypeDef

```python
# SplunkRetryOptionsTypeDef definition

class SplunkRetryOptionsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
```

## StopDeliveryStreamEncryptionInputRequestTypeDef

```python
# StopDeliveryStreamEncryptionInputRequestTypeDef definition

class StopDeliveryStreamEncryptionInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
```

## UntagDeliveryStreamInputRequestTypeDef

```python
# UntagDeliveryStreamInputRequestTypeDef definition

class UntagDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    TagKeys: Sequence[str],
```

## MSKSourceDescriptionTypeDef

```python
# MSKSourceDescriptionTypeDef definition

class MSKSourceDescriptionTypeDef(TypedDict):
    MSKClusterARN: NotRequired[str],
    TopicName: NotRequired[str],
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationTypeDef],  # (1)
    DeliveryStartTimestamp: NotRequired[datetime],
    ReadFromTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    Data: BlobTypeDef,
```

## StartDeliveryStreamEncryptionInputRequestTypeDef

```python
# StartDeliveryStreamEncryptionInputRequestTypeDef definition

class StartDeliveryStreamEncryptionInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    DeliveryStreamEncryptionConfigurationInput: NotRequired[DeliveryStreamEncryptionConfigurationInputTypeDef],  # (1)
```

1. See [:material-code-braces: DeliveryStreamEncryptionConfigurationInputTypeDef](./type_defs.md#deliverystreamencryptionconfigurationinputtypedef) 
## TagDeliveryStreamInputRequestTypeDef

```python
# TagDeliveryStreamInputRequestTypeDef definition

class TagDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDeliveryStreamOutputTypeDef

```python
# CreateDeliveryStreamOutputTypeDef definition

class CreateDeliveryStreamOutputTypeDef(TypedDict):
    DeliveryStreamARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeliveryStreamsOutputTypeDef

```python
# ListDeliveryStreamsOutputTypeDef definition

class ListDeliveryStreamsOutputTypeDef(TypedDict):
    DeliveryStreamNames: List[str],
    HasMoreDeliveryStreams: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForDeliveryStreamOutputTypeDef

```python
# ListTagsForDeliveryStreamOutputTypeDef definition

class ListTagsForDeliveryStreamOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    HasMoreTags: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRecordOutputTypeDef

```python
# PutRecordOutputTypeDef definition

class PutRecordOutputTypeDef(TypedDict):
    RecordId: str,
    Encrypted: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeliveryStreamEncryptionConfigurationTypeDef

```python
# DeliveryStreamEncryptionConfigurationTypeDef definition

class DeliveryStreamEncryptionConfigurationTypeDef(TypedDict):
    KeyARN: NotRequired[str],
    KeyType: NotRequired[KeyTypeType],  # (1)
    Status: NotRequired[DeliveryStreamEncryptionStatusType],  # (2)
    FailureDescription: NotRequired[FailureDescriptionTypeDef],  # (3)
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
2. See [:material-code-brackets: DeliveryStreamEncryptionStatusType](./literals.md#deliverystreamencryptionstatustype) 
3. See [:material-code-braces: FailureDescriptionTypeDef](./type_defs.md#failuredescriptiontypedef) 
## DeserializerOutputTypeDef

```python
# DeserializerOutputTypeDef definition

class DeserializerOutputTypeDef(TypedDict):
    OpenXJsonSerDe: NotRequired[OpenXJsonSerDeOutputTypeDef],  # (1)
    HiveJsonSerDe: NotRequired[HiveJsonSerDeOutputTypeDef],  # (2)
```

1. See [:material-code-braces: OpenXJsonSerDeOutputTypeDef](./type_defs.md#openxjsonserdeoutputtypedef) 
2. See [:material-code-braces: HiveJsonSerDeOutputTypeDef](./type_defs.md#hivejsonserdeoutputtypedef) 
## DynamicPartitioningConfigurationTypeDef

```python
# DynamicPartitioningConfigurationTypeDef definition

class DynamicPartitioningConfigurationTypeDef(TypedDict):
    RetryOptions: NotRequired[RetryOptionsTypeDef],  # (1)
    Enabled: NotRequired[bool],
```

1. See [:material-code-braces: RetryOptionsTypeDef](./type_defs.md#retryoptionstypedef) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    NoEncryptionConfig: NotRequired[NoEncryptionConfigType],  # (1)
    KMSEncryptionConfig: NotRequired[KMSEncryptionConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NoEncryptionConfigType](./literals.md#noencryptionconfigtype) 
2. See [:material-code-braces: KMSEncryptionConfigTypeDef](./type_defs.md#kmsencryptionconfigtypedef) 
## HttpEndpointRequestConfigurationOutputTypeDef

```python
# HttpEndpointRequestConfigurationOutputTypeDef definition

class HttpEndpointRequestConfigurationOutputTypeDef(TypedDict):
    ContentEncoding: NotRequired[ContentEncodingType],  # (1)
    CommonAttributes: NotRequired[List[HttpEndpointCommonAttributeTypeDef]],  # (2)
```

1. See [:material-code-brackets: ContentEncodingType](./literals.md#contentencodingtype) 
2. See [:material-code-braces: HttpEndpointCommonAttributeTypeDef](./type_defs.md#httpendpointcommonattributetypedef) 
## HttpEndpointRequestConfigurationTypeDef

```python
# HttpEndpointRequestConfigurationTypeDef definition

class HttpEndpointRequestConfigurationTypeDef(TypedDict):
    ContentEncoding: NotRequired[ContentEncodingType],  # (1)
    CommonAttributes: NotRequired[Sequence[HttpEndpointCommonAttributeTypeDef]],  # (2)
```

1. See [:material-code-brackets: ContentEncodingType](./literals.md#contentencodingtype) 
2. See [:material-code-braces: HttpEndpointCommonAttributeTypeDef](./type_defs.md#httpendpointcommonattributetypedef) 
## MSKSourceConfigurationTypeDef

```python
# MSKSourceConfigurationTypeDef definition

class MSKSourceConfigurationTypeDef(TypedDict):
    MSKClusterARN: str,
    TopicName: str,
    AuthenticationConfiguration: AuthenticationConfigurationTypeDef,  # (1)
    ReadFromTimestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
## SerializerOutputTypeDef

```python
# SerializerOutputTypeDef definition

class SerializerOutputTypeDef(TypedDict):
    ParquetSerDe: NotRequired[ParquetSerDeTypeDef],  # (1)
    OrcSerDe: NotRequired[OrcSerDeOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ParquetSerDeTypeDef](./type_defs.md#parquetserdetypedef) 
2. See [:material-code-braces: OrcSerDeOutputTypeDef](./type_defs.md#orcserdeoutputtypedef) 
## ProcessorOutputTypeDef

```python
# ProcessorOutputTypeDef definition

class ProcessorOutputTypeDef(TypedDict):
    Type: ProcessorTypeType,  # (1)
    Parameters: NotRequired[List[ProcessorParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProcessorTypeType](./literals.md#processortypetype) 
2. See [:material-code-braces: ProcessorParameterTypeDef](./type_defs.md#processorparametertypedef) 
## ProcessorTypeDef

```python
# ProcessorTypeDef definition

class ProcessorTypeDef(TypedDict):
    Type: ProcessorTypeType,  # (1)
    Parameters: NotRequired[Sequence[ProcessorParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProcessorTypeType](./literals.md#processortypetype) 
2. See [:material-code-braces: ProcessorParameterTypeDef](./type_defs.md#processorparametertypedef) 
## PutRecordBatchOutputTypeDef

```python
# PutRecordBatchOutputTypeDef definition

class PutRecordBatchOutputTypeDef(TypedDict):
    FailedPutCount: int,
    Encrypted: bool,
    RequestResponses: List[PutRecordBatchResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PutRecordBatchResponseEntryTypeDef](./type_defs.md#putrecordbatchresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceDescriptionTypeDef

```python
# SourceDescriptionTypeDef definition

class SourceDescriptionTypeDef(TypedDict):
    KinesisStreamSourceDescription: NotRequired[KinesisStreamSourceDescriptionTypeDef],  # (1)
    MSKSourceDescription: NotRequired[MSKSourceDescriptionTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamSourceDescriptionTypeDef](./type_defs.md#kinesisstreamsourcedescriptiontypedef) 
2. See [:material-code-braces: MSKSourceDescriptionTypeDef](./type_defs.md#msksourcedescriptiontypedef) 
## PutRecordBatchInputRequestTypeDef

```python
# PutRecordBatchInputRequestTypeDef definition

class PutRecordBatchInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    Records: Sequence[RecordTypeDef],  # (1)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
## PutRecordInputRequestTypeDef

```python
# PutRecordInputRequestTypeDef definition

class PutRecordInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    Record: RecordTypeDef,  # (1)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
## InputFormatConfigurationOutputTypeDef

```python
# InputFormatConfigurationOutputTypeDef definition

class InputFormatConfigurationOutputTypeDef(TypedDict):
    Deserializer: NotRequired[DeserializerOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DeserializerOutputTypeDef](./type_defs.md#deserializeroutputtypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    BucketARN: str,
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (1)
    CompressionFormat: NotRequired[CompressionFormatType],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
## S3DestinationDescriptionTypeDef

```python
# S3DestinationDescriptionTypeDef definition

class S3DestinationDescriptionTypeDef(TypedDict):
    RoleARN: str,
    BucketARN: str,
    BufferingHints: BufferingHintsTypeDef,  # (1)
    CompressionFormat: CompressionFormatType,  # (2)
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (3)
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
## S3DestinationUpdateTypeDef

```python
# S3DestinationUpdateTypeDef definition

class S3DestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    BucketARN: NotRequired[str],
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (1)
    CompressionFormat: NotRequired[CompressionFormatType],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
## DeserializerTypeDef

```python
# DeserializerTypeDef definition

class DeserializerTypeDef(TypedDict):
    OpenXJsonSerDe: NotRequired[OpenXJsonSerDeUnionTypeDef],  # (1)
    HiveJsonSerDe: NotRequired[HiveJsonSerDeUnionTypeDef],  # (2)
```

1. See [:material-code-braces: OpenXJsonSerDeTypeDef](./type_defs.md#openxjsonserdetypedef) [:material-code-braces: OpenXJsonSerDeOutputTypeDef](./type_defs.md#openxjsonserdeoutputtypedef) 
2. See [:material-code-braces: HiveJsonSerDeTypeDef](./type_defs.md#hivejsonserdetypedef) [:material-code-braces: HiveJsonSerDeOutputTypeDef](./type_defs.md#hivejsonserdeoutputtypedef) 
## SerializerTypeDef

```python
# SerializerTypeDef definition

class SerializerTypeDef(TypedDict):
    ParquetSerDe: NotRequired[ParquetSerDeTypeDef],  # (1)
    OrcSerDe: NotRequired[OrcSerDeUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ParquetSerDeTypeDef](./type_defs.md#parquetserdetypedef) 
2. See [:material-code-braces: OrcSerDeTypeDef](./type_defs.md#orcserdetypedef) [:material-code-braces: OrcSerDeOutputTypeDef](./type_defs.md#orcserdeoutputtypedef) 
## OutputFormatConfigurationOutputTypeDef

```python
# OutputFormatConfigurationOutputTypeDef definition

class OutputFormatConfigurationOutputTypeDef(TypedDict):
    Serializer: NotRequired[SerializerOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SerializerOutputTypeDef](./type_defs.md#serializeroutputtypedef) 
## ProcessingConfigurationOutputTypeDef

```python
# ProcessingConfigurationOutputTypeDef definition

class ProcessingConfigurationOutputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Processors: NotRequired[List[ProcessorOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ProcessorOutputTypeDef](./type_defs.md#processoroutputtypedef) 
## DataFormatConversionConfigurationOutputTypeDef

```python
# DataFormatConversionConfigurationOutputTypeDef definition

class DataFormatConversionConfigurationOutputTypeDef(TypedDict):
    SchemaConfiguration: NotRequired[SchemaConfigurationTypeDef],  # (1)
    InputFormatConfiguration: NotRequired[InputFormatConfigurationOutputTypeDef],  # (2)
    OutputFormatConfiguration: NotRequired[OutputFormatConfigurationOutputTypeDef],  # (3)
    Enabled: NotRequired[bool],
```

1. See [:material-code-braces: SchemaConfigurationTypeDef](./type_defs.md#schemaconfigurationtypedef) 
2. See [:material-code-braces: InputFormatConfigurationOutputTypeDef](./type_defs.md#inputformatconfigurationoutputtypedef) 
3. See [:material-code-braces: OutputFormatConfigurationOutputTypeDef](./type_defs.md#outputformatconfigurationoutputtypedef) 
## AmazonOpenSearchServerlessDestinationDescriptionTypeDef

```python
# AmazonOpenSearchServerlessDestinationDescriptionTypeDef definition

class AmazonOpenSearchServerlessDestinationDescriptionTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    CollectionEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    BufferingHints: NotRequired[AmazonOpenSearchServerlessBufferingHintsTypeDef],  # (1)
    RetryOptions: NotRequired[AmazonOpenSearchServerlessRetryOptionsTypeDef],  # (2)
    S3BackupMode: NotRequired[AmazonOpenSearchServerlessS3BackupModeType],  # (3)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    VpcConfigurationDescription: NotRequired[VpcConfigurationDescriptionTypeDef],  # (7)
```

1. See [:material-code-braces: AmazonOpenSearchServerlessBufferingHintsTypeDef](./type_defs.md#amazonopensearchserverlessbufferinghintstypedef) 
2. See [:material-code-braces: AmazonOpenSearchServerlessRetryOptionsTypeDef](./type_defs.md#amazonopensearchserverlessretryoptionstypedef) 
3. See [:material-code-brackets: AmazonOpenSearchServerlessS3BackupModeType](./literals.md#amazonopensearchserverlesss3backupmodetype) 
4. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
5. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: VpcConfigurationDescriptionTypeDef](./type_defs.md#vpcconfigurationdescriptiontypedef) 
## AmazonopensearchserviceDestinationDescriptionTypeDef

```python
# AmazonopensearchserviceDestinationDescriptionTypeDef definition

class AmazonopensearchserviceDestinationDescriptionTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[AmazonopensearchserviceIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[AmazonopensearchserviceBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[AmazonopensearchserviceRetryOptionsTypeDef],  # (3)
    S3BackupMode: NotRequired[AmazonopensearchserviceS3BackupModeType],  # (4)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (5)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (6)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    VpcConfigurationDescription: NotRequired[VpcConfigurationDescriptionTypeDef],  # (8)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (9)
```

1. See [:material-code-brackets: AmazonopensearchserviceIndexRotationPeriodType](./literals.md#amazonopensearchserviceindexrotationperiodtype) 
2. See [:material-code-braces: AmazonopensearchserviceBufferingHintsTypeDef](./type_defs.md#amazonopensearchservicebufferinghintstypedef) 
3. See [:material-code-braces: AmazonopensearchserviceRetryOptionsTypeDef](./type_defs.md#amazonopensearchserviceretryoptionstypedef) 
4. See [:material-code-brackets: AmazonopensearchserviceS3BackupModeType](./literals.md#amazonopensearchservices3backupmodetype) 
5. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
6. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: VpcConfigurationDescriptionTypeDef](./type_defs.md#vpcconfigurationdescriptiontypedef) 
9. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## ElasticsearchDestinationDescriptionTypeDef

```python
# ElasticsearchDestinationDescriptionTypeDef definition

class ElasticsearchDestinationDescriptionTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[ElasticsearchIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[ElasticsearchBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[ElasticsearchRetryOptionsTypeDef],  # (3)
    S3BackupMode: NotRequired[ElasticsearchS3BackupModeType],  # (4)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (5)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (6)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    VpcConfigurationDescription: NotRequired[VpcConfigurationDescriptionTypeDef],  # (8)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (9)
```

1. See [:material-code-brackets: ElasticsearchIndexRotationPeriodType](./literals.md#elasticsearchindexrotationperiodtype) 
2. See [:material-code-braces: ElasticsearchBufferingHintsTypeDef](./type_defs.md#elasticsearchbufferinghintstypedef) 
3. See [:material-code-braces: ElasticsearchRetryOptionsTypeDef](./type_defs.md#elasticsearchretryoptionstypedef) 
4. See [:material-code-brackets: ElasticsearchS3BackupModeType](./literals.md#elasticsearchs3backupmodetype) 
5. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
6. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: VpcConfigurationDescriptionTypeDef](./type_defs.md#vpcconfigurationdescriptiontypedef) 
9. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## HttpEndpointDestinationDescriptionTypeDef

```python
# HttpEndpointDestinationDescriptionTypeDef definition

class HttpEndpointDestinationDescriptionTypeDef(TypedDict):
    EndpointConfiguration: NotRequired[HttpEndpointDescriptionTypeDef],  # (1)
    BufferingHints: NotRequired[HttpEndpointBufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    RequestConfiguration: NotRequired[HttpEndpointRequestConfigurationOutputTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (5)
    RoleARN: NotRequired[str],
    RetryOptions: NotRequired[HttpEndpointRetryOptionsTypeDef],  # (6)
    S3BackupMode: NotRequired[HttpEndpointS3BackupModeType],  # (7)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (8)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (9)
```

1. See [:material-code-braces: HttpEndpointDescriptionTypeDef](./type_defs.md#httpendpointdescriptiontypedef) 
2. See [:material-code-braces: HttpEndpointBufferingHintsTypeDef](./type_defs.md#httpendpointbufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: HttpEndpointRequestConfigurationOutputTypeDef](./type_defs.md#httpendpointrequestconfigurationoutputtypedef) 
5. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: HttpEndpointRetryOptionsTypeDef](./type_defs.md#httpendpointretryoptionstypedef) 
7. See [:material-code-brackets: HttpEndpointS3BackupModeType](./literals.md#httpendpoints3backupmodetype) 
8. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
9. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## IcebergDestinationDescriptionTypeDef

```python
# IcebergDestinationDescriptionTypeDef definition

class IcebergDestinationDescriptionTypeDef(TypedDict):
    DestinationTableConfigurationList: NotRequired[List[DestinationTableConfigurationOutputTypeDef]],  # (1)
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (4)
    S3BackupMode: NotRequired[IcebergS3BackupModeType],  # (5)
    RetryOptions: NotRequired[RetryOptionsTypeDef],  # (6)
    RoleARN: NotRequired[str],
    CatalogConfiguration: NotRequired[CatalogConfigurationTypeDef],  # (7)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (8)
```

1. See [:material-code-braces: DestinationTableConfigurationOutputTypeDef](./type_defs.md#destinationtableconfigurationoutputtypedef) 
2. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: IcebergS3BackupModeType](./literals.md#icebergs3backupmodetype) 
6. See [:material-code-braces: RetryOptionsTypeDef](./type_defs.md#retryoptionstypedef) 
7. See [:material-code-braces: CatalogConfigurationTypeDef](./type_defs.md#catalogconfigurationtypedef) 
8. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
## RedshiftDestinationDescriptionTypeDef

```python
# RedshiftDestinationDescriptionTypeDef definition

class RedshiftDestinationDescriptionTypeDef(TypedDict):
    RoleARN: str,
    ClusterJDBCURL: str,
    CopyCommand: CopyCommandTypeDef,  # (1)
    S3DestinationDescription: S3DestinationDescriptionTypeDef,  # (3)
    Username: NotRequired[str],
    RetryOptions: NotRequired[RedshiftRetryOptionsTypeDef],  # (2)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (4)
    S3BackupMode: NotRequired[RedshiftS3BackupModeType],  # (5)
    S3BackupDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: CopyCommandTypeDef](./type_defs.md#copycommandtypedef) 
2. See [:material-code-braces: RedshiftRetryOptionsTypeDef](./type_defs.md#redshiftretryoptionstypedef) 
3. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
4. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: RedshiftS3BackupModeType](./literals.md#redshifts3backupmodetype) 
6. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## SnowflakeDestinationDescriptionTypeDef

```python
# SnowflakeDestinationDescriptionTypeDef definition

class SnowflakeDestinationDescriptionTypeDef(TypedDict):
    AccountUrl: NotRequired[str],
    User: NotRequired[str],
    Database: NotRequired[str],
    Schema: NotRequired[str],
    Table: NotRequired[str],
    SnowflakeRoleConfiguration: NotRequired[SnowflakeRoleConfigurationTypeDef],  # (1)
    DataLoadingOption: NotRequired[SnowflakeDataLoadingOptionType],  # (2)
    MetaDataColumnName: NotRequired[str],
    ContentColumnName: NotRequired[str],
    SnowflakeVpcConfiguration: NotRequired[SnowflakeVpcConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (5)
    RoleARN: NotRequired[str],
    RetryOptions: NotRequired[SnowflakeRetryOptionsTypeDef],  # (6)
    S3BackupMode: NotRequired[SnowflakeS3BackupModeType],  # (7)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (8)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (9)
    BufferingHints: NotRequired[SnowflakeBufferingHintsTypeDef],  # (10)
```

1. See [:material-code-braces: SnowflakeRoleConfigurationTypeDef](./type_defs.md#snowflakeroleconfigurationtypedef) 
2. See [:material-code-brackets: SnowflakeDataLoadingOptionType](./literals.md#snowflakedataloadingoptiontype) 
3. See [:material-code-braces: SnowflakeVpcConfigurationTypeDef](./type_defs.md#snowflakevpcconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
5. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: SnowflakeRetryOptionsTypeDef](./type_defs.md#snowflakeretryoptionstypedef) 
7. See [:material-code-brackets: SnowflakeS3BackupModeType](./literals.md#snowflakes3backupmodetype) 
8. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
9. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
10. See [:material-code-braces: SnowflakeBufferingHintsTypeDef](./type_defs.md#snowflakebufferinghintstypedef) 
## SplunkDestinationDescriptionTypeDef

```python
# SplunkDestinationDescriptionTypeDef definition

class SplunkDestinationDescriptionTypeDef(TypedDict):
    HECEndpoint: NotRequired[str],
    HECEndpointType: NotRequired[HECEndpointTypeType],  # (1)
    HECToken: NotRequired[str],
    HECAcknowledgmentTimeoutInSeconds: NotRequired[int],
    RetryOptions: NotRequired[SplunkRetryOptionsTypeDef],  # (2)
    S3BackupMode: NotRequired[SplunkS3BackupModeType],  # (3)
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    BufferingHints: NotRequired[SplunkBufferingHintsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-brackets: HECEndpointTypeType](./literals.md#hecendpointtypetype) 
2. See [:material-code-braces: SplunkRetryOptionsTypeDef](./type_defs.md#splunkretryoptionstypedef) 
3. See [:material-code-brackets: SplunkS3BackupModeType](./literals.md#splunks3backupmodetype) 
4. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
5. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: SplunkBufferingHintsTypeDef](./type_defs.md#splunkbufferinghintstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## ProcessingConfigurationTypeDef

```python
# ProcessingConfigurationTypeDef definition

class ProcessingConfigurationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Processors: NotRequired[Sequence[ProcessorUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ProcessorTypeDef](./type_defs.md#processortypedef) [:material-code-braces: ProcessorOutputTypeDef](./type_defs.md#processoroutputtypedef) 
## InputFormatConfigurationTypeDef

```python
# InputFormatConfigurationTypeDef definition

class InputFormatConfigurationTypeDef(TypedDict):
    Deserializer: NotRequired[DeserializerUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DeserializerTypeDef](./type_defs.md#deserializertypedef) [:material-code-braces: DeserializerOutputTypeDef](./type_defs.md#deserializeroutputtypedef) 
## OutputFormatConfigurationTypeDef

```python
# OutputFormatConfigurationTypeDef definition

class OutputFormatConfigurationTypeDef(TypedDict):
    Serializer: NotRequired[SerializerUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SerializerTypeDef](./type_defs.md#serializertypedef) [:material-code-braces: SerializerOutputTypeDef](./type_defs.md#serializeroutputtypedef) 
## ExtendedS3DestinationDescriptionTypeDef

```python
# ExtendedS3DestinationDescriptionTypeDef definition

class ExtendedS3DestinationDescriptionTypeDef(TypedDict):
    RoleARN: str,
    BucketARN: str,
    BufferingHints: BufferingHintsTypeDef,  # (1)
    CompressionFormat: CompressionFormatType,  # (2)
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (3)
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationOutputTypeDef],  # (5)
    S3BackupMode: NotRequired[S3BackupModeType],  # (6)
    S3BackupDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (7)
    DataFormatConversionConfiguration: NotRequired[DataFormatConversionConfigurationOutputTypeDef],  # (8)
    DynamicPartitioningConfiguration: NotRequired[DynamicPartitioningConfigurationTypeDef],  # (9)
    FileExtension: NotRequired[str],
    CustomTimeZone: NotRequired[str],
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
5. See [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-brackets: S3BackupModeType](./literals.md#s3backupmodetype) 
7. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
8. See [:material-code-braces: DataFormatConversionConfigurationOutputTypeDef](./type_defs.md#dataformatconversionconfigurationoutputtypedef) 
9. See [:material-code-braces: DynamicPartitioningConfigurationTypeDef](./type_defs.md#dynamicpartitioningconfigurationtypedef) 
## DestinationDescriptionTypeDef

```python
# DestinationDescriptionTypeDef definition

class DestinationDescriptionTypeDef(TypedDict):
    DestinationId: str,
    S3DestinationDescription: NotRequired[S3DestinationDescriptionTypeDef],  # (1)
    ExtendedS3DestinationDescription: NotRequired[ExtendedS3DestinationDescriptionTypeDef],  # (2)
    RedshiftDestinationDescription: NotRequired[RedshiftDestinationDescriptionTypeDef],  # (3)
    ElasticsearchDestinationDescription: NotRequired[ElasticsearchDestinationDescriptionTypeDef],  # (4)
    AmazonopensearchserviceDestinationDescription: NotRequired[AmazonopensearchserviceDestinationDescriptionTypeDef],  # (5)
    SplunkDestinationDescription: NotRequired[SplunkDestinationDescriptionTypeDef],  # (6)
    HttpEndpointDestinationDescription: NotRequired[HttpEndpointDestinationDescriptionTypeDef],  # (7)
    SnowflakeDestinationDescription: NotRequired[SnowflakeDestinationDescriptionTypeDef],  # (8)
    AmazonOpenSearchServerlessDestinationDescription: NotRequired[AmazonOpenSearchServerlessDestinationDescriptionTypeDef],  # (9)
    IcebergDestinationDescription: NotRequired[IcebergDestinationDescriptionTypeDef],  # (10)
```

1. See [:material-code-braces: S3DestinationDescriptionTypeDef](./type_defs.md#s3destinationdescriptiontypedef) 
2. See [:material-code-braces: ExtendedS3DestinationDescriptionTypeDef](./type_defs.md#extendeds3destinationdescriptiontypedef) 
3. See [:material-code-braces: RedshiftDestinationDescriptionTypeDef](./type_defs.md#redshiftdestinationdescriptiontypedef) 
4. See [:material-code-braces: ElasticsearchDestinationDescriptionTypeDef](./type_defs.md#elasticsearchdestinationdescriptiontypedef) 
5. See [:material-code-braces: AmazonopensearchserviceDestinationDescriptionTypeDef](./type_defs.md#amazonopensearchservicedestinationdescriptiontypedef) 
6. See [:material-code-braces: SplunkDestinationDescriptionTypeDef](./type_defs.md#splunkdestinationdescriptiontypedef) 
7. See [:material-code-braces: HttpEndpointDestinationDescriptionTypeDef](./type_defs.md#httpendpointdestinationdescriptiontypedef) 
8. See [:material-code-braces: SnowflakeDestinationDescriptionTypeDef](./type_defs.md#snowflakedestinationdescriptiontypedef) 
9. See [:material-code-braces: AmazonOpenSearchServerlessDestinationDescriptionTypeDef](./type_defs.md#amazonopensearchserverlessdestinationdescriptiontypedef) 
10. See [:material-code-braces: IcebergDestinationDescriptionTypeDef](./type_defs.md#icebergdestinationdescriptiontypedef) 
## AmazonOpenSearchServerlessDestinationConfigurationTypeDef

```python
# AmazonOpenSearchServerlessDestinationConfigurationTypeDef definition

class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    IndexName: str,
    S3Configuration: S3DestinationConfigurationTypeDef,  # (4)
    CollectionEndpoint: NotRequired[str],
    BufferingHints: NotRequired[AmazonOpenSearchServerlessBufferingHintsTypeDef],  # (1)
    RetryOptions: NotRequired[AmazonOpenSearchServerlessRetryOptionsTypeDef],  # (2)
    S3BackupMode: NotRequired[AmazonOpenSearchServerlessS3BackupModeType],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (7)
```

1. See [:material-code-braces: AmazonOpenSearchServerlessBufferingHintsTypeDef](./type_defs.md#amazonopensearchserverlessbufferinghintstypedef) 
2. See [:material-code-braces: AmazonOpenSearchServerlessRetryOptionsTypeDef](./type_defs.md#amazonopensearchserverlessretryoptionstypedef) 
3. See [:material-code-brackets: AmazonOpenSearchServerlessS3BackupModeType](./literals.md#amazonopensearchserverlesss3backupmodetype) 
4. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## AmazonOpenSearchServerlessDestinationUpdateTypeDef

```python
# AmazonOpenSearchServerlessDestinationUpdateTypeDef definition

class AmazonOpenSearchServerlessDestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    CollectionEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    BufferingHints: NotRequired[AmazonOpenSearchServerlessBufferingHintsTypeDef],  # (1)
    RetryOptions: NotRequired[AmazonOpenSearchServerlessRetryOptionsTypeDef],  # (2)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (5)
```

1. See [:material-code-braces: AmazonOpenSearchServerlessBufferingHintsTypeDef](./type_defs.md#amazonopensearchserverlessbufferinghintstypedef) 
2. See [:material-code-braces: AmazonOpenSearchServerlessRetryOptionsTypeDef](./type_defs.md#amazonopensearchserverlessretryoptionstypedef) 
3. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
## AmazonopensearchserviceDestinationConfigurationTypeDef

```python
# AmazonopensearchserviceDestinationConfigurationTypeDef definition

class AmazonopensearchserviceDestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    IndexName: str,
    S3Configuration: S3DestinationConfigurationTypeDef,  # (5)
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[AmazonopensearchserviceIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[AmazonopensearchserviceBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[AmazonopensearchserviceRetryOptionsTypeDef],  # (3)
    S3BackupMode: NotRequired[AmazonopensearchserviceS3BackupModeType],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (6)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (8)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (9)
```

1. See [:material-code-brackets: AmazonopensearchserviceIndexRotationPeriodType](./literals.md#amazonopensearchserviceindexrotationperiodtype) 
2. See [:material-code-braces: AmazonopensearchserviceBufferingHintsTypeDef](./type_defs.md#amazonopensearchservicebufferinghintstypedef) 
3. See [:material-code-braces: AmazonopensearchserviceRetryOptionsTypeDef](./type_defs.md#amazonopensearchserviceretryoptionstypedef) 
4. See [:material-code-brackets: AmazonopensearchserviceS3BackupModeType](./literals.md#amazonopensearchservices3backupmodetype) 
5. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
6. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
9. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## AmazonopensearchserviceDestinationUpdateTypeDef

```python
# AmazonopensearchserviceDestinationUpdateTypeDef definition

class AmazonopensearchserviceDestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[AmazonopensearchserviceIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[AmazonopensearchserviceBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[AmazonopensearchserviceRetryOptionsTypeDef],  # (3)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (7)
```

1. See [:material-code-brackets: AmazonopensearchserviceIndexRotationPeriodType](./literals.md#amazonopensearchserviceindexrotationperiodtype) 
2. See [:material-code-braces: AmazonopensearchserviceBufferingHintsTypeDef](./type_defs.md#amazonopensearchservicebufferinghintstypedef) 
3. See [:material-code-braces: AmazonopensearchserviceRetryOptionsTypeDef](./type_defs.md#amazonopensearchserviceretryoptionstypedef) 
4. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## ElasticsearchDestinationConfigurationTypeDef

```python
# ElasticsearchDestinationConfigurationTypeDef definition

class ElasticsearchDestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    IndexName: str,
    S3Configuration: S3DestinationConfigurationTypeDef,  # (5)
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[ElasticsearchIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[ElasticsearchBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[ElasticsearchRetryOptionsTypeDef],  # (3)
    S3BackupMode: NotRequired[ElasticsearchS3BackupModeType],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (6)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (8)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (9)
```

1. See [:material-code-brackets: ElasticsearchIndexRotationPeriodType](./literals.md#elasticsearchindexrotationperiodtype) 
2. See [:material-code-braces: ElasticsearchBufferingHintsTypeDef](./type_defs.md#elasticsearchbufferinghintstypedef) 
3. See [:material-code-braces: ElasticsearchRetryOptionsTypeDef](./type_defs.md#elasticsearchretryoptionstypedef) 
4. See [:material-code-brackets: ElasticsearchS3BackupModeType](./literals.md#elasticsearchs3backupmodetype) 
5. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
6. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
9. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## ElasticsearchDestinationUpdateTypeDef

```python
# ElasticsearchDestinationUpdateTypeDef definition

class ElasticsearchDestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    DomainARN: NotRequired[str],
    ClusterEndpoint: NotRequired[str],
    IndexName: NotRequired[str],
    TypeName: NotRequired[str],
    IndexRotationPeriod: NotRequired[ElasticsearchIndexRotationPeriodType],  # (1)
    BufferingHints: NotRequired[ElasticsearchBufferingHintsTypeDef],  # (2)
    RetryOptions: NotRequired[ElasticsearchRetryOptionsTypeDef],  # (3)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    DocumentIdOptions: NotRequired[DocumentIdOptionsTypeDef],  # (7)
```

1. See [:material-code-brackets: ElasticsearchIndexRotationPeriodType](./literals.md#elasticsearchindexrotationperiodtype) 
2. See [:material-code-braces: ElasticsearchBufferingHintsTypeDef](./type_defs.md#elasticsearchbufferinghintstypedef) 
3. See [:material-code-braces: ElasticsearchRetryOptionsTypeDef](./type_defs.md#elasticsearchretryoptionstypedef) 
4. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: DocumentIdOptionsTypeDef](./type_defs.md#documentidoptionstypedef) 
## HttpEndpointDestinationConfigurationTypeDef

```python
# HttpEndpointDestinationConfigurationTypeDef definition

class HttpEndpointDestinationConfigurationTypeDef(TypedDict):
    EndpointConfiguration: HttpEndpointConfigurationTypeDef,  # (1)
    S3Configuration: S3DestinationConfigurationTypeDef,  # (8)
    BufferingHints: NotRequired[HttpEndpointBufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    RequestConfiguration: NotRequired[HttpEndpointRequestConfigurationUnionTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    RoleARN: NotRequired[str],
    RetryOptions: NotRequired[HttpEndpointRetryOptionsTypeDef],  # (6)
    S3BackupMode: NotRequired[HttpEndpointS3BackupModeType],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (9)
```

1. See [:material-code-braces: HttpEndpointConfigurationTypeDef](./type_defs.md#httpendpointconfigurationtypedef) 
2. See [:material-code-braces: HttpEndpointBufferingHintsTypeDef](./type_defs.md#httpendpointbufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: HttpEndpointRequestConfigurationTypeDef](./type_defs.md#httpendpointrequestconfigurationtypedef) [:material-code-braces: HttpEndpointRequestConfigurationOutputTypeDef](./type_defs.md#httpendpointrequestconfigurationoutputtypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: HttpEndpointRetryOptionsTypeDef](./type_defs.md#httpendpointretryoptionstypedef) 
7. See [:material-code-brackets: HttpEndpointS3BackupModeType](./literals.md#httpendpoints3backupmodetype) 
8. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
9. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## HttpEndpointDestinationUpdateTypeDef

```python
# HttpEndpointDestinationUpdateTypeDef definition

class HttpEndpointDestinationUpdateTypeDef(TypedDict):
    EndpointConfiguration: NotRequired[HttpEndpointConfigurationTypeDef],  # (1)
    BufferingHints: NotRequired[HttpEndpointBufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    RequestConfiguration: NotRequired[HttpEndpointRequestConfigurationUnionTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    RoleARN: NotRequired[str],
    RetryOptions: NotRequired[HttpEndpointRetryOptionsTypeDef],  # (6)
    S3BackupMode: NotRequired[HttpEndpointS3BackupModeType],  # (7)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (8)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (9)
```

1. See [:material-code-braces: HttpEndpointConfigurationTypeDef](./type_defs.md#httpendpointconfigurationtypedef) 
2. See [:material-code-braces: HttpEndpointBufferingHintsTypeDef](./type_defs.md#httpendpointbufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: HttpEndpointRequestConfigurationTypeDef](./type_defs.md#httpendpointrequestconfigurationtypedef) [:material-code-braces: HttpEndpointRequestConfigurationOutputTypeDef](./type_defs.md#httpendpointrequestconfigurationoutputtypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: HttpEndpointRetryOptionsTypeDef](./type_defs.md#httpendpointretryoptionstypedef) 
7. See [:material-code-brackets: HttpEndpointS3BackupModeType](./literals.md#httpendpoints3backupmodetype) 
8. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
9. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## IcebergDestinationConfigurationTypeDef

```python
# IcebergDestinationConfigurationTypeDef definition

class IcebergDestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    CatalogConfiguration: CatalogConfigurationTypeDef,  # (7)
    S3Configuration: S3DestinationConfigurationTypeDef,  # (8)
    DestinationTableConfigurationList: NotRequired[Sequence[DestinationTableConfigurationUnionTypeDef]],  # (1)
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    S3BackupMode: NotRequired[IcebergS3BackupModeType],  # (5)
    RetryOptions: NotRequired[RetryOptionsTypeDef],  # (6)
```

1. See [:material-code-braces: DestinationTableConfigurationTypeDef](./type_defs.md#destinationtableconfigurationtypedef) [:material-code-braces: DestinationTableConfigurationOutputTypeDef](./type_defs.md#destinationtableconfigurationoutputtypedef) 
2. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: IcebergS3BackupModeType](./literals.md#icebergs3backupmodetype) 
6. See [:material-code-braces: RetryOptionsTypeDef](./type_defs.md#retryoptionstypedef) 
7. See [:material-code-braces: CatalogConfigurationTypeDef](./type_defs.md#catalogconfigurationtypedef) 
8. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## IcebergDestinationUpdateTypeDef

```python
# IcebergDestinationUpdateTypeDef definition

class IcebergDestinationUpdateTypeDef(TypedDict):
    DestinationTableConfigurationList: NotRequired[Sequence[DestinationTableConfigurationUnionTypeDef]],  # (1)
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    S3BackupMode: NotRequired[IcebergS3BackupModeType],  # (5)
    RetryOptions: NotRequired[RetryOptionsTypeDef],  # (6)
    RoleARN: NotRequired[str],
    CatalogConfiguration: NotRequired[CatalogConfigurationTypeDef],  # (7)
    S3Configuration: NotRequired[S3DestinationConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: DestinationTableConfigurationTypeDef](./type_defs.md#destinationtableconfigurationtypedef) [:material-code-braces: DestinationTableConfigurationOutputTypeDef](./type_defs.md#destinationtableconfigurationoutputtypedef) 
2. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: IcebergS3BackupModeType](./literals.md#icebergs3backupmodetype) 
6. See [:material-code-braces: RetryOptionsTypeDef](./type_defs.md#retryoptionstypedef) 
7. See [:material-code-braces: CatalogConfigurationTypeDef](./type_defs.md#catalogconfigurationtypedef) 
8. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## RedshiftDestinationConfigurationTypeDef

```python
# RedshiftDestinationConfigurationTypeDef definition

class RedshiftDestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    ClusterJDBCURL: str,
    CopyCommand: CopyCommandTypeDef,  # (1)
    S3Configuration: S3DestinationConfigurationTypeDef,  # (3)
    Username: NotRequired[str],
    Password: NotRequired[str],
    RetryOptions: NotRequired[RedshiftRetryOptionsTypeDef],  # (2)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    S3BackupMode: NotRequired[RedshiftS3BackupModeType],  # (5)
    S3BackupConfiguration: NotRequired[S3DestinationConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: CopyCommandTypeDef](./type_defs.md#copycommandtypedef) 
2. See [:material-code-braces: RedshiftRetryOptionsTypeDef](./type_defs.md#redshiftretryoptionstypedef) 
3. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: RedshiftS3BackupModeType](./literals.md#redshifts3backupmodetype) 
6. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## RedshiftDestinationUpdateTypeDef

```python
# RedshiftDestinationUpdateTypeDef definition

class RedshiftDestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    ClusterJDBCURL: NotRequired[str],
    CopyCommand: NotRequired[CopyCommandTypeDef],  # (1)
    Username: NotRequired[str],
    Password: NotRequired[str],
    RetryOptions: NotRequired[RedshiftRetryOptionsTypeDef],  # (2)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    S3BackupMode: NotRequired[RedshiftS3BackupModeType],  # (5)
    S3BackupUpdate: NotRequired[S3DestinationUpdateTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: CopyCommandTypeDef](./type_defs.md#copycommandtypedef) 
2. See [:material-code-braces: RedshiftRetryOptionsTypeDef](./type_defs.md#redshiftretryoptionstypedef) 
3. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-brackets: RedshiftS3BackupModeType](./literals.md#redshifts3backupmodetype) 
6. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
7. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## SnowflakeDestinationConfigurationTypeDef

```python
# SnowflakeDestinationConfigurationTypeDef definition

class SnowflakeDestinationConfigurationTypeDef(TypedDict):
    AccountUrl: str,
    Database: str,
    Schema: str,
    Table: str,
    RoleARN: str,
    S3Configuration: S3DestinationConfigurationTypeDef,  # (8)
    PrivateKey: NotRequired[str],
    KeyPassphrase: NotRequired[str],
    User: NotRequired[str],
    SnowflakeRoleConfiguration: NotRequired[SnowflakeRoleConfigurationTypeDef],  # (1)
    DataLoadingOption: NotRequired[SnowflakeDataLoadingOptionType],  # (2)
    MetaDataColumnName: NotRequired[str],
    ContentColumnName: NotRequired[str],
    SnowflakeVpcConfiguration: NotRequired[SnowflakeVpcConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    RetryOptions: NotRequired[SnowflakeRetryOptionsTypeDef],  # (6)
    S3BackupMode: NotRequired[SnowflakeS3BackupModeType],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (9)
    BufferingHints: NotRequired[SnowflakeBufferingHintsTypeDef],  # (10)
```

1. See [:material-code-braces: SnowflakeRoleConfigurationTypeDef](./type_defs.md#snowflakeroleconfigurationtypedef) 
2. See [:material-code-brackets: SnowflakeDataLoadingOptionType](./literals.md#snowflakedataloadingoptiontype) 
3. See [:material-code-braces: SnowflakeVpcConfigurationTypeDef](./type_defs.md#snowflakevpcconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: SnowflakeRetryOptionsTypeDef](./type_defs.md#snowflakeretryoptionstypedef) 
7. See [:material-code-brackets: SnowflakeS3BackupModeType](./literals.md#snowflakes3backupmodetype) 
8. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
9. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
10. See [:material-code-braces: SnowflakeBufferingHintsTypeDef](./type_defs.md#snowflakebufferinghintstypedef) 
## SnowflakeDestinationUpdateTypeDef

```python
# SnowflakeDestinationUpdateTypeDef definition

class SnowflakeDestinationUpdateTypeDef(TypedDict):
    AccountUrl: NotRequired[str],
    PrivateKey: NotRequired[str],
    KeyPassphrase: NotRequired[str],
    User: NotRequired[str],
    Database: NotRequired[str],
    Schema: NotRequired[str],
    Table: NotRequired[str],
    SnowflakeRoleConfiguration: NotRequired[SnowflakeRoleConfigurationTypeDef],  # (1)
    DataLoadingOption: NotRequired[SnowflakeDataLoadingOptionType],  # (2)
    MetaDataColumnName: NotRequired[str],
    ContentColumnName: NotRequired[str],
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (4)
    RoleARN: NotRequired[str],
    RetryOptions: NotRequired[SnowflakeRetryOptionsTypeDef],  # (5)
    S3BackupMode: NotRequired[SnowflakeS3BackupModeType],  # (6)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
    BufferingHints: NotRequired[SnowflakeBufferingHintsTypeDef],  # (9)
```

1. See [:material-code-braces: SnowflakeRoleConfigurationTypeDef](./type_defs.md#snowflakeroleconfigurationtypedef) 
2. See [:material-code-brackets: SnowflakeDataLoadingOptionType](./literals.md#snowflakedataloadingoptiontype) 
3. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
4. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
5. See [:material-code-braces: SnowflakeRetryOptionsTypeDef](./type_defs.md#snowflakeretryoptionstypedef) 
6. See [:material-code-brackets: SnowflakeS3BackupModeType](./literals.md#snowflakes3backupmodetype) 
7. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
9. See [:material-code-braces: SnowflakeBufferingHintsTypeDef](./type_defs.md#snowflakebufferinghintstypedef) 
## SplunkDestinationConfigurationTypeDef

```python
# SplunkDestinationConfigurationTypeDef definition

class SplunkDestinationConfigurationTypeDef(TypedDict):
    HECEndpoint: str,
    HECEndpointType: HECEndpointTypeType,  # (1)
    S3Configuration: S3DestinationConfigurationTypeDef,  # (4)
    HECToken: NotRequired[str],
    HECAcknowledgmentTimeoutInSeconds: NotRequired[int],
    RetryOptions: NotRequired[SplunkRetryOptionsTypeDef],  # (2)
    S3BackupMode: NotRequired[SplunkS3BackupModeType],  # (3)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    BufferingHints: NotRequired[SplunkBufferingHintsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-brackets: HECEndpointTypeType](./literals.md#hecendpointtypetype) 
2. See [:material-code-braces: SplunkRetryOptionsTypeDef](./type_defs.md#splunkretryoptionstypedef) 
3. See [:material-code-brackets: SplunkS3BackupModeType](./literals.md#splunks3backupmodetype) 
4. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: SplunkBufferingHintsTypeDef](./type_defs.md#splunkbufferinghintstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## SplunkDestinationUpdateTypeDef

```python
# SplunkDestinationUpdateTypeDef definition

class SplunkDestinationUpdateTypeDef(TypedDict):
    HECEndpoint: NotRequired[str],
    HECEndpointType: NotRequired[HECEndpointTypeType],  # (1)
    HECToken: NotRequired[str],
    HECAcknowledgmentTimeoutInSeconds: NotRequired[int],
    RetryOptions: NotRequired[SplunkRetryOptionsTypeDef],  # (2)
    S3BackupMode: NotRequired[SplunkS3BackupModeType],  # (3)
    S3Update: NotRequired[S3DestinationUpdateTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (6)
    BufferingHints: NotRequired[SplunkBufferingHintsTypeDef],  # (7)
    SecretsManagerConfiguration: NotRequired[SecretsManagerConfigurationTypeDef],  # (8)
```

1. See [:material-code-brackets: HECEndpointTypeType](./literals.md#hecendpointtypetype) 
2. See [:material-code-braces: SplunkRetryOptionsTypeDef](./type_defs.md#splunkretryoptionstypedef) 
3. See [:material-code-brackets: SplunkS3BackupModeType](./literals.md#splunks3backupmodetype) 
4. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
7. See [:material-code-braces: SplunkBufferingHintsTypeDef](./type_defs.md#splunkbufferinghintstypedef) 
8. See [:material-code-braces: SecretsManagerConfigurationTypeDef](./type_defs.md#secretsmanagerconfigurationtypedef) 
## DataFormatConversionConfigurationTypeDef

```python
# DataFormatConversionConfigurationTypeDef definition

class DataFormatConversionConfigurationTypeDef(TypedDict):
    SchemaConfiguration: NotRequired[SchemaConfigurationTypeDef],  # (1)
    InputFormatConfiguration: NotRequired[InputFormatConfigurationUnionTypeDef],  # (2)
    OutputFormatConfiguration: NotRequired[OutputFormatConfigurationUnionTypeDef],  # (3)
    Enabled: NotRequired[bool],
```

1. See [:material-code-braces: SchemaConfigurationTypeDef](./type_defs.md#schemaconfigurationtypedef) 
2. See [:material-code-braces: InputFormatConfigurationTypeDef](./type_defs.md#inputformatconfigurationtypedef) [:material-code-braces: InputFormatConfigurationOutputTypeDef](./type_defs.md#inputformatconfigurationoutputtypedef) 
3. See [:material-code-braces: OutputFormatConfigurationTypeDef](./type_defs.md#outputformatconfigurationtypedef) [:material-code-braces: OutputFormatConfigurationOutputTypeDef](./type_defs.md#outputformatconfigurationoutputtypedef) 
## DeliveryStreamDescriptionTypeDef

```python
# DeliveryStreamDescriptionTypeDef definition

class DeliveryStreamDescriptionTypeDef(TypedDict):
    DeliveryStreamName: str,
    DeliveryStreamARN: str,
    DeliveryStreamStatus: DeliveryStreamStatusType,  # (1)
    DeliveryStreamType: DeliveryStreamTypeType,  # (4)
    VersionId: str,
    Destinations: List[DestinationDescriptionTypeDef],  # (6)
    HasMoreDestinations: bool,
    FailureDescription: NotRequired[FailureDescriptionTypeDef],  # (2)
    DeliveryStreamEncryptionConfiguration: NotRequired[DeliveryStreamEncryptionConfigurationTypeDef],  # (3)
    CreateTimestamp: NotRequired[datetime],
    LastUpdateTimestamp: NotRequired[datetime],
    Source: NotRequired[SourceDescriptionTypeDef],  # (5)
```

1. See [:material-code-brackets: DeliveryStreamStatusType](./literals.md#deliverystreamstatustype) 
2. See [:material-code-braces: FailureDescriptionTypeDef](./type_defs.md#failuredescriptiontypedef) 
3. See [:material-code-braces: DeliveryStreamEncryptionConfigurationTypeDef](./type_defs.md#deliverystreamencryptionconfigurationtypedef) 
4. See [:material-code-brackets: DeliveryStreamTypeType](./literals.md#deliverystreamtypetype) 
5. See [:material-code-braces: SourceDescriptionTypeDef](./type_defs.md#sourcedescriptiontypedef) 
6. See [:material-code-braces: DestinationDescriptionTypeDef](./type_defs.md#destinationdescriptiontypedef) 
## DescribeDeliveryStreamOutputTypeDef

```python
# DescribeDeliveryStreamOutputTypeDef definition

class DescribeDeliveryStreamOutputTypeDef(TypedDict):
    DeliveryStreamDescription: DeliveryStreamDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryStreamDescriptionTypeDef](./type_defs.md#deliverystreamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtendedS3DestinationConfigurationTypeDef

```python
# ExtendedS3DestinationConfigurationTypeDef definition

class ExtendedS3DestinationConfigurationTypeDef(TypedDict):
    RoleARN: str,
    BucketARN: str,
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (1)
    CompressionFormat: NotRequired[CompressionFormatType],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    S3BackupMode: NotRequired[S3BackupModeType],  # (6)
    S3BackupConfiguration: NotRequired[S3DestinationConfigurationTypeDef],  # (7)
    DataFormatConversionConfiguration: NotRequired[DataFormatConversionConfigurationUnionTypeDef],  # (8)
    DynamicPartitioningConfiguration: NotRequired[DynamicPartitioningConfigurationTypeDef],  # (9)
    FileExtension: NotRequired[str],
    CustomTimeZone: NotRequired[str],
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-brackets: S3BackupModeType](./literals.md#s3backupmodetype) 
7. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
8. See [:material-code-braces: DataFormatConversionConfigurationTypeDef](./type_defs.md#dataformatconversionconfigurationtypedef) [:material-code-braces: DataFormatConversionConfigurationOutputTypeDef](./type_defs.md#dataformatconversionconfigurationoutputtypedef) 
9. See [:material-code-braces: DynamicPartitioningConfigurationTypeDef](./type_defs.md#dynamicpartitioningconfigurationtypedef) 
## ExtendedS3DestinationUpdateTypeDef

```python
# ExtendedS3DestinationUpdateTypeDef definition

class ExtendedS3DestinationUpdateTypeDef(TypedDict):
    RoleARN: NotRequired[str],
    BucketARN: NotRequired[str],
    Prefix: NotRequired[str],
    ErrorOutputPrefix: NotRequired[str],
    BufferingHints: NotRequired[BufferingHintsTypeDef],  # (1)
    CompressionFormat: NotRequired[CompressionFormatType],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    CloudWatchLoggingOptions: NotRequired[CloudWatchLoggingOptionsTypeDef],  # (4)
    ProcessingConfiguration: NotRequired[ProcessingConfigurationUnionTypeDef],  # (5)
    S3BackupMode: NotRequired[S3BackupModeType],  # (6)
    S3BackupUpdate: NotRequired[S3DestinationUpdateTypeDef],  # (7)
    DataFormatConversionConfiguration: NotRequired[DataFormatConversionConfigurationUnionTypeDef],  # (8)
    DynamicPartitioningConfiguration: NotRequired[DynamicPartitioningConfigurationTypeDef],  # (9)
    FileExtension: NotRequired[str],
    CustomTimeZone: NotRequired[str],
```

1. See [:material-code-braces: BufferingHintsTypeDef](./type_defs.md#bufferinghintstypedef) 
2. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionsTypeDef](./type_defs.md#cloudwatchloggingoptionstypedef) 
5. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) [:material-code-braces: ProcessingConfigurationOutputTypeDef](./type_defs.md#processingconfigurationoutputtypedef) 
6. See [:material-code-brackets: S3BackupModeType](./literals.md#s3backupmodetype) 
7. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
8. See [:material-code-braces: DataFormatConversionConfigurationTypeDef](./type_defs.md#dataformatconversionconfigurationtypedef) [:material-code-braces: DataFormatConversionConfigurationOutputTypeDef](./type_defs.md#dataformatconversionconfigurationoutputtypedef) 
9. See [:material-code-braces: DynamicPartitioningConfigurationTypeDef](./type_defs.md#dynamicpartitioningconfigurationtypedef) 
## CreateDeliveryStreamInputRequestTypeDef

```python
# CreateDeliveryStreamInputRequestTypeDef definition

class CreateDeliveryStreamInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    DeliveryStreamType: NotRequired[DeliveryStreamTypeType],  # (1)
    KinesisStreamSourceConfiguration: NotRequired[KinesisStreamSourceConfigurationTypeDef],  # (2)
    DeliveryStreamEncryptionConfigurationInput: NotRequired[DeliveryStreamEncryptionConfigurationInputTypeDef],  # (3)
    S3DestinationConfiguration: NotRequired[S3DestinationConfigurationTypeDef],  # (4)
    ExtendedS3DestinationConfiguration: NotRequired[ExtendedS3DestinationConfigurationTypeDef],  # (5)
    RedshiftDestinationConfiguration: NotRequired[RedshiftDestinationConfigurationTypeDef],  # (6)
    ElasticsearchDestinationConfiguration: NotRequired[ElasticsearchDestinationConfigurationTypeDef],  # (7)
    AmazonopensearchserviceDestinationConfiguration: NotRequired[AmazonopensearchserviceDestinationConfigurationTypeDef],  # (8)
    SplunkDestinationConfiguration: NotRequired[SplunkDestinationConfigurationTypeDef],  # (9)
    HttpEndpointDestinationConfiguration: NotRequired[HttpEndpointDestinationConfigurationTypeDef],  # (10)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (11)
    AmazonOpenSearchServerlessDestinationConfiguration: NotRequired[AmazonOpenSearchServerlessDestinationConfigurationTypeDef],  # (12)
    MSKSourceConfiguration: NotRequired[MSKSourceConfigurationTypeDef],  # (13)
    SnowflakeDestinationConfiguration: NotRequired[SnowflakeDestinationConfigurationTypeDef],  # (14)
    IcebergDestinationConfiguration: NotRequired[IcebergDestinationConfigurationTypeDef],  # (15)
```

1. See [:material-code-brackets: DeliveryStreamTypeType](./literals.md#deliverystreamtypetype) 
2. See [:material-code-braces: KinesisStreamSourceConfigurationTypeDef](./type_defs.md#kinesisstreamsourceconfigurationtypedef) 
3. See [:material-code-braces: DeliveryStreamEncryptionConfigurationInputTypeDef](./type_defs.md#deliverystreamencryptionconfigurationinputtypedef) 
4. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
5. See [:material-code-braces: ExtendedS3DestinationConfigurationTypeDef](./type_defs.md#extendeds3destinationconfigurationtypedef) 
6. See [:material-code-braces: RedshiftDestinationConfigurationTypeDef](./type_defs.md#redshiftdestinationconfigurationtypedef) 
7. See [:material-code-braces: ElasticsearchDestinationConfigurationTypeDef](./type_defs.md#elasticsearchdestinationconfigurationtypedef) 
8. See [:material-code-braces: AmazonopensearchserviceDestinationConfigurationTypeDef](./type_defs.md#amazonopensearchservicedestinationconfigurationtypedef) 
9. See [:material-code-braces: SplunkDestinationConfigurationTypeDef](./type_defs.md#splunkdestinationconfigurationtypedef) 
10. See [:material-code-braces: HttpEndpointDestinationConfigurationTypeDef](./type_defs.md#httpendpointdestinationconfigurationtypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-braces: AmazonOpenSearchServerlessDestinationConfigurationTypeDef](./type_defs.md#amazonopensearchserverlessdestinationconfigurationtypedef) 
13. See [:material-code-braces: MSKSourceConfigurationTypeDef](./type_defs.md#msksourceconfigurationtypedef) 
14. See [:material-code-braces: SnowflakeDestinationConfigurationTypeDef](./type_defs.md#snowflakedestinationconfigurationtypedef) 
15. See [:material-code-braces: IcebergDestinationConfigurationTypeDef](./type_defs.md#icebergdestinationconfigurationtypedef) 
## UpdateDestinationInputRequestTypeDef

```python
# UpdateDestinationInputRequestTypeDef definition

class UpdateDestinationInputRequestTypeDef(TypedDict):
    DeliveryStreamName: str,
    CurrentDeliveryStreamVersionId: str,
    DestinationId: str,
    S3DestinationUpdate: NotRequired[S3DestinationUpdateTypeDef],  # (1)
    ExtendedS3DestinationUpdate: NotRequired[ExtendedS3DestinationUpdateTypeDef],  # (2)
    RedshiftDestinationUpdate: NotRequired[RedshiftDestinationUpdateTypeDef],  # (3)
    ElasticsearchDestinationUpdate: NotRequired[ElasticsearchDestinationUpdateTypeDef],  # (4)
    AmazonopensearchserviceDestinationUpdate: NotRequired[AmazonopensearchserviceDestinationUpdateTypeDef],  # (5)
    SplunkDestinationUpdate: NotRequired[SplunkDestinationUpdateTypeDef],  # (6)
    HttpEndpointDestinationUpdate: NotRequired[HttpEndpointDestinationUpdateTypeDef],  # (7)
    AmazonOpenSearchServerlessDestinationUpdate: NotRequired[AmazonOpenSearchServerlessDestinationUpdateTypeDef],  # (8)
    SnowflakeDestinationUpdate: NotRequired[SnowflakeDestinationUpdateTypeDef],  # (9)
    IcebergDestinationUpdate: NotRequired[IcebergDestinationUpdateTypeDef],  # (10)
```

1. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
2. See [:material-code-braces: ExtendedS3DestinationUpdateTypeDef](./type_defs.md#extendeds3destinationupdatetypedef) 
3. See [:material-code-braces: RedshiftDestinationUpdateTypeDef](./type_defs.md#redshiftdestinationupdatetypedef) 
4. See [:material-code-braces: ElasticsearchDestinationUpdateTypeDef](./type_defs.md#elasticsearchdestinationupdatetypedef) 
5. See [:material-code-braces: AmazonopensearchserviceDestinationUpdateTypeDef](./type_defs.md#amazonopensearchservicedestinationupdatetypedef) 
6. See [:material-code-braces: SplunkDestinationUpdateTypeDef](./type_defs.md#splunkdestinationupdatetypedef) 
7. See [:material-code-braces: HttpEndpointDestinationUpdateTypeDef](./type_defs.md#httpendpointdestinationupdatetypedef) 
8. See [:material-code-braces: AmazonOpenSearchServerlessDestinationUpdateTypeDef](./type_defs.md#amazonopensearchserverlessdestinationupdatetypedef) 
9. See [:material-code-braces: SnowflakeDestinationUpdateTypeDef](./type_defs.md#snowflakedestinationupdatetypedef) 
10. See [:material-code-braces: IcebergDestinationUpdateTypeDef](./type_defs.md#icebergdestinationupdatetypedef) 
