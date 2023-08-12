# Type definitions

> [Index](../README.md) > [S3](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

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


## FileobjTypeDef

```python
# FileobjTypeDef definition

FileobjTypeDef = Union[
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


## CopySourceOrStrTypeDef

```python
# CopySourceOrStrTypeDef definition

CopySourceOrStrTypeDef = Union[
    str,
    CopySourceTypeDef,  # (1)
]
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 



## AbortIncompleteMultipartUploadTypeDef

```python
# AbortIncompleteMultipartUploadTypeDef definition

class AbortIncompleteMultipartUploadTypeDef(TypedDict):
    DaysAfterInitiation: NotRequired[int],
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

## AbortMultipartUploadRequestMultipartUploadAbortTypeDef

```python
# AbortMultipartUploadRequestMultipartUploadAbortTypeDef definition

class AbortMultipartUploadRequestMultipartUploadAbortTypeDef(TypedDict):
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## AbortMultipartUploadRequestRequestTypeDef

```python
# AbortMultipartUploadRequestRequestTypeDef definition

class AbortMultipartUploadRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    UploadId: str,
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## AccelerateConfigurationTypeDef

```python
# AccelerateConfigurationTypeDef definition

class AccelerateConfigurationTypeDef(TypedDict):
    Status: NotRequired[BucketAccelerateStatusType],  # (1)
```

1. See [:material-code-brackets: BucketAccelerateStatusType](./literals.md#bucketacceleratestatustype) 
## AccessControlTranslationTypeDef

```python
# AccessControlTranslationTypeDef definition

class AccessControlTranslationTypeDef(TypedDict):
    Owner: OwnerOverrideType,  # (1)
```

1. See [:material-code-brackets: OwnerOverrideType](./literals.md#owneroverridetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AnalyticsS3BucketDestinationTypeDef

```python
# AnalyticsS3BucketDestinationTypeDef definition

class AnalyticsS3BucketDestinationTypeDef(TypedDict):
    Format: AnalyticsS3ExportFileFormatType,  # (1)
    Bucket: str,
    BucketAccountId: NotRequired[str],
    Prefix: NotRequired[str],
```

1. See [:material-code-brackets: AnalyticsS3ExportFileFormatType](./literals.md#analyticss3exportfileformattype) 
## CopySourceTypeDef

```python
# CopySourceTypeDef definition

class CopySourceTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
```

## BucketDownloadFileRequestTypeDef

```python
# BucketDownloadFileRequestTypeDef definition

class BucketDownloadFileRequestTypeDef(TypedDict):
    Key: str,
    Filename: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## BucketTypeDef

```python
# BucketTypeDef definition

class BucketTypeDef(TypedDict):
    Name: NotRequired[str],
    CreationDate: NotRequired[datetime],
```

## BucketUploadFileRequestTypeDef

```python
# BucketUploadFileRequestTypeDef definition

class BucketUploadFileRequestTypeDef(TypedDict):
    Filename: str,
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## CORSRuleBucketCorsTypeDef

```python
# CORSRuleBucketCorsTypeDef definition

class CORSRuleBucketCorsTypeDef(TypedDict):
    AllowedMethods: Sequence[str],
    AllowedOrigins: Sequence[str],
    ID: NotRequired[str],
    AllowedHeaders: NotRequired[Sequence[str]],
    ExposeHeaders: NotRequired[Sequence[str]],
    MaxAgeSeconds: NotRequired[int],
```

## CORSRuleTypeDef

```python
# CORSRuleTypeDef definition

class CORSRuleTypeDef(TypedDict):
    AllowedMethods: List[str],
    AllowedOrigins: List[str],
    ID: NotRequired[str],
    AllowedHeaders: NotRequired[List[str]],
    ExposeHeaders: NotRequired[List[str]],
    MaxAgeSeconds: NotRequired[int],
```

## CSVInputTypeDef

```python
# CSVInputTypeDef definition

class CSVInputTypeDef(TypedDict):
    FileHeaderInfo: NotRequired[FileHeaderInfoType],  # (1)
    Comments: NotRequired[str],
    QuoteEscapeCharacter: NotRequired[str],
    RecordDelimiter: NotRequired[str],
    FieldDelimiter: NotRequired[str],
    QuoteCharacter: NotRequired[str],
    AllowQuotedRecordDelimiter: NotRequired[bool],
```

1. See [:material-code-brackets: FileHeaderInfoType](./literals.md#fileheaderinfotype) 
## CSVOutputTypeDef

```python
# CSVOutputTypeDef definition

class CSVOutputTypeDef(TypedDict):
    QuoteFields: NotRequired[QuoteFieldsType],  # (1)
    QuoteEscapeCharacter: NotRequired[str],
    RecordDelimiter: NotRequired[str],
    FieldDelimiter: NotRequired[str],
    QuoteCharacter: NotRequired[str],
```

1. See [:material-code-brackets: QuoteFieldsType](./literals.md#quotefieldstype) 
## ChecksumTypeDef

```python
# ChecksumTypeDef definition

class ChecksumTypeDef(TypedDict):
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
```

## ClientDownloadFileRequestTypeDef

```python
# ClientDownloadFileRequestTypeDef definition

class ClientDownloadFileRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Filename: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ClientGeneratePresignedPostRequestTypeDef

```python
# ClientGeneratePresignedPostRequestTypeDef definition

class ClientGeneratePresignedPostRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Fields: NotRequired[Dict[str, Any]],
    Conditions: NotRequired[Union[List[Any], Dict[str, Any]]],
    ExpiresIn: NotRequired[int],
```

## ClientUploadFileRequestTypeDef

```python
# ClientUploadFileRequestTypeDef definition

class ClientUploadFileRequestTypeDef(TypedDict):
    Filename: str,
    Bucket: str,
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## CloudFunctionConfigurationTypeDef

```python
# CloudFunctionConfigurationTypeDef definition

class CloudFunctionConfigurationTypeDef(TypedDict):
    Id: NotRequired[str],
    Event: NotRequired[EventType],  # (1)
    Events: NotRequired[List[EventType]],  # (2)
    CloudFunction: NotRequired[str],
    InvocationRole: NotRequired[str],
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-brackets: EventType](./literals.md#eventtype) 
## CommonPrefixTypeDef

```python
# CommonPrefixTypeDef definition

class CommonPrefixTypeDef(TypedDict):
    Prefix: NotRequired[str],
```

## CompletedPartTypeDef

```python
# CompletedPartTypeDef definition

class CompletedPartTypeDef(TypedDict):
    ETag: NotRequired[str],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    PartNumber: NotRequired[int],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    HttpErrorCodeReturnedEquals: NotRequired[str],
    KeyPrefixEquals: NotRequired[str],
```

## CopyObjectResultTypeDef

```python
# CopyObjectResultTypeDef definition

class CopyObjectResultTypeDef(TypedDict):
    ETag: NotRequired[str],
    LastModified: NotRequired[datetime],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
```

## CopyPartResultTypeDef

```python
# CopyPartResultTypeDef definition

class CopyPartResultTypeDef(TypedDict):
    ETag: NotRequired[str],
    LastModified: NotRequired[datetime],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
```

## CreateBucketConfigurationTypeDef

```python
# CreateBucketConfigurationTypeDef definition

class CreateBucketConfigurationTypeDef(TypedDict):
    LocationConstraint: NotRequired[BucketLocationConstraintType],  # (1)
```

1. See [:material-code-brackets: BucketLocationConstraintType](./literals.md#bucketlocationconstrainttype) 
## DefaultRetentionTypeDef

```python
# DefaultRetentionTypeDef definition

class DefaultRetentionTypeDef(TypedDict):
    Mode: NotRequired[ObjectLockRetentionModeType],  # (1)
    Days: NotRequired[int],
    Years: NotRequired[int],
```

1. See [:material-code-brackets: ObjectLockRetentionModeType](./literals.md#objectlockretentionmodetype) 
## DeleteBucketAnalyticsConfigurationRequestRequestTypeDef

```python
# DeleteBucketAnalyticsConfigurationRequestRequestTypeDef definition

class DeleteBucketAnalyticsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketCorsRequestBucketCorsDeleteTypeDef

```python
# DeleteBucketCorsRequestBucketCorsDeleteTypeDef definition

class DeleteBucketCorsRequestBucketCorsDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketCorsRequestRequestTypeDef

```python
# DeleteBucketCorsRequestRequestTypeDef definition

class DeleteBucketCorsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketEncryptionRequestRequestTypeDef

```python
# DeleteBucketEncryptionRequestRequestTypeDef definition

class DeleteBucketEncryptionRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef

```python
# DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef definition

class DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
```

## DeleteBucketInventoryConfigurationRequestRequestTypeDef

```python
# DeleteBucketInventoryConfigurationRequestRequestTypeDef definition

class DeleteBucketInventoryConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef

```python
# DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef definition

class DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef

```python
# DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef definition

class DeleteBucketLifecycleRequestBucketLifecycleDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketLifecycleRequestRequestTypeDef

```python
# DeleteBucketLifecycleRequestRequestTypeDef definition

class DeleteBucketLifecycleRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketMetricsConfigurationRequestRequestTypeDef

```python
# DeleteBucketMetricsConfigurationRequestRequestTypeDef definition

class DeleteBucketMetricsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketOwnershipControlsRequestRequestTypeDef

```python
# DeleteBucketOwnershipControlsRequestRequestTypeDef definition

class DeleteBucketOwnershipControlsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef

```python
# DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef definition

class DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketPolicyRequestRequestTypeDef

```python
# DeleteBucketPolicyRequestRequestTypeDef definition

class DeleteBucketPolicyRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketReplicationRequestRequestTypeDef

```python
# DeleteBucketReplicationRequestRequestTypeDef definition

class DeleteBucketReplicationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketRequestBucketDeleteTypeDef

```python
# DeleteBucketRequestBucketDeleteTypeDef definition

class DeleteBucketRequestBucketDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketRequestRequestTypeDef

```python
# DeleteBucketRequestRequestTypeDef definition

class DeleteBucketRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef

```python
# DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef definition

class DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketTaggingRequestRequestTypeDef

```python
# DeleteBucketTaggingRequestRequestTypeDef definition

class DeleteBucketTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef

```python
# DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef definition

class DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef(TypedDict):
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteBucketWebsiteRequestRequestTypeDef

```python
# DeleteBucketWebsiteRequestRequestTypeDef definition

class DeleteBucketWebsiteRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## DeleteMarkerReplicationTypeDef

```python
# DeleteMarkerReplicationTypeDef definition

class DeleteMarkerReplicationTypeDef(TypedDict):
    Status: NotRequired[DeleteMarkerReplicationStatusType],  # (1)
```

1. See [:material-code-brackets: DeleteMarkerReplicationStatusType](./literals.md#deletemarkerreplicationstatustype) 
## DeleteObjectRequestObjectDeleteTypeDef

```python
# DeleteObjectRequestObjectDeleteTypeDef definition

class DeleteObjectRequestObjectDeleteTypeDef(TypedDict):
    MFA: NotRequired[str],
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## DeleteObjectRequestObjectSummaryDeleteTypeDef

```python
# DeleteObjectRequestObjectSummaryDeleteTypeDef definition

class DeleteObjectRequestObjectSummaryDeleteTypeDef(TypedDict):
    MFA: NotRequired[str],
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## DeleteObjectRequestObjectVersionDeleteTypeDef

```python
# DeleteObjectRequestObjectVersionDeleteTypeDef definition

class DeleteObjectRequestObjectVersionDeleteTypeDef(TypedDict):
    MFA: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## DeleteObjectRequestRequestTypeDef

```python
# DeleteObjectRequestRequestTypeDef definition

class DeleteObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    MFA: NotRequired[str],
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## DeleteObjectTaggingRequestRequestTypeDef

```python
# DeleteObjectTaggingRequestRequestTypeDef definition

class DeleteObjectTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

## DeletedObjectTypeDef

```python
# DeletedObjectTypeDef definition

class DeletedObjectTypeDef(TypedDict):
    Key: NotRequired[str],
    VersionId: NotRequired[str],
    DeleteMarker: NotRequired[bool],
    DeleteMarkerVersionId: NotRequired[str],
```

## ErrorTypeDef

```python
# ErrorTypeDef definition

class ErrorTypeDef(TypedDict):
    Key: NotRequired[str],
    VersionId: NotRequired[str],
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## DeletePublicAccessBlockRequestRequestTypeDef

```python
# DeletePublicAccessBlockRequestRequestTypeDef definition

class DeletePublicAccessBlockRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## ObjectIdentifierTypeDef

```python
# ObjectIdentifierTypeDef definition

class ObjectIdentifierTypeDef(TypedDict):
    Key: str,
    VersionId: NotRequired[str],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    ReplicaKmsKeyID: NotRequired[str],
```

## EncryptionTypeDef

```python
# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    EncryptionType: ServerSideEncryptionType,  # (1)
    KMSKeyId: NotRequired[str],
    KMSContext: NotRequired[str],
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
## ErrorDocumentTypeDef

```python
# ErrorDocumentTypeDef definition

class ErrorDocumentTypeDef(TypedDict):
    Key: str,
```

## ExistingObjectReplicationTypeDef

```python
# ExistingObjectReplicationTypeDef definition

class ExistingObjectReplicationTypeDef(TypedDict):
    Status: ExistingObjectReplicationStatusType,  # (1)
```

1. See [:material-code-brackets: ExistingObjectReplicationStatusType](./literals.md#existingobjectreplicationstatustype) 
## FilterRuleTypeDef

```python
# FilterRuleTypeDef definition

class FilterRuleTypeDef(TypedDict):
    Name: NotRequired[FilterRuleNameType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FilterRuleNameType](./literals.md#filterrulenametype) 
## GetBucketAccelerateConfigurationRequestRequestTypeDef

```python
# GetBucketAccelerateConfigurationRequestRequestTypeDef definition

class GetBucketAccelerateConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## GetBucketAclRequestRequestTypeDef

```python
# GetBucketAclRequestRequestTypeDef definition

class GetBucketAclRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketAnalyticsConfigurationRequestRequestTypeDef

```python
# GetBucketAnalyticsConfigurationRequestRequestTypeDef definition

class GetBucketAnalyticsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketCorsRequestRequestTypeDef

```python
# GetBucketCorsRequestRequestTypeDef definition

class GetBucketCorsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketEncryptionRequestRequestTypeDef

```python
# GetBucketEncryptionRequestRequestTypeDef definition

class GetBucketEncryptionRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketIntelligentTieringConfigurationRequestRequestTypeDef

```python
# GetBucketIntelligentTieringConfigurationRequestRequestTypeDef definition

class GetBucketIntelligentTieringConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
```

## GetBucketInventoryConfigurationRequestRequestTypeDef

```python
# GetBucketInventoryConfigurationRequestRequestTypeDef definition

class GetBucketInventoryConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketLifecycleConfigurationRequestRequestTypeDef

```python
# GetBucketLifecycleConfigurationRequestRequestTypeDef definition

class GetBucketLifecycleConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketLifecycleRequestRequestTypeDef

```python
# GetBucketLifecycleRequestRequestTypeDef definition

class GetBucketLifecycleRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketLocationRequestRequestTypeDef

```python
# GetBucketLocationRequestRequestTypeDef definition

class GetBucketLocationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketLoggingRequestRequestTypeDef

```python
# GetBucketLoggingRequestRequestTypeDef definition

class GetBucketLoggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketMetricsConfigurationRequestRequestTypeDef

```python
# GetBucketMetricsConfigurationRequestRequestTypeDef definition

class GetBucketMetricsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketNotificationConfigurationRequestRequestTypeDef

```python
# GetBucketNotificationConfigurationRequestRequestTypeDef definition

class GetBucketNotificationConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketOwnershipControlsRequestRequestTypeDef

```python
# GetBucketOwnershipControlsRequestRequestTypeDef definition

class GetBucketOwnershipControlsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketPolicyRequestRequestTypeDef

```python
# GetBucketPolicyRequestRequestTypeDef definition

class GetBucketPolicyRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## PolicyStatusTypeDef

```python
# PolicyStatusTypeDef definition

class PolicyStatusTypeDef(TypedDict):
    IsPublic: NotRequired[bool],
```

## GetBucketPolicyStatusRequestRequestTypeDef

```python
# GetBucketPolicyStatusRequestRequestTypeDef definition

class GetBucketPolicyStatusRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketReplicationRequestRequestTypeDef

```python
# GetBucketReplicationRequestRequestTypeDef definition

class GetBucketReplicationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketRequestPaymentRequestRequestTypeDef

```python
# GetBucketRequestPaymentRequestRequestTypeDef definition

class GetBucketRequestPaymentRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketTaggingRequestRequestTypeDef

```python
# GetBucketTaggingRequestRequestTypeDef definition

class GetBucketTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetBucketVersioningRequestRequestTypeDef

```python
# GetBucketVersioningRequestRequestTypeDef definition

class GetBucketVersioningRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## IndexDocumentTypeDef

```python
# IndexDocumentTypeDef definition

class IndexDocumentTypeDef(TypedDict):
    Suffix: str,
```

## RedirectAllRequestsToTypeDef

```python
# RedirectAllRequestsToTypeDef definition

class RedirectAllRequestsToTypeDef(TypedDict):
    HostName: str,
    Protocol: NotRequired[ProtocolType],  # (1)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## GetBucketWebsiteRequestRequestTypeDef

```python
# GetBucketWebsiteRequestRequestTypeDef definition

class GetBucketWebsiteRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GetObjectAclRequestRequestTypeDef

```python
# GetObjectAclRequestRequestTypeDef definition

class GetObjectAclRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## ObjectPartTypeDef

```python
# ObjectPartTypeDef definition

class ObjectPartTypeDef(TypedDict):
    PartNumber: NotRequired[int],
    Size: NotRequired[int],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
```

## GetObjectAttributesRequestRequestTypeDef

```python
# GetObjectAttributesRequestRequestTypeDef definition

class GetObjectAttributesRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    ObjectAttributes: Sequence[ObjectAttributesType],  # (1)
    VersionId: NotRequired[str],
    MaxParts: NotRequired[int],
    PartNumberMarker: NotRequired[int],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectAttributesType](./literals.md#objectattributestype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## ObjectLockLegalHoldTypeDef

```python
# ObjectLockLegalHoldTypeDef definition

class ObjectLockLegalHoldTypeDef(TypedDict):
    Status: NotRequired[ObjectLockLegalHoldStatusType],  # (1)
```

1. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## GetObjectLegalHoldRequestRequestTypeDef

```python
# GetObjectLegalHoldRequestRequestTypeDef definition

class GetObjectLegalHoldRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## GetObjectLockConfigurationRequestRequestTypeDef

```python
# GetObjectLockConfigurationRequestRequestTypeDef definition

class GetObjectLockConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## ObjectLockRetentionTypeDef

```python
# ObjectLockRetentionTypeDef definition

class ObjectLockRetentionTypeDef(TypedDict):
    Mode: NotRequired[ObjectLockRetentionModeType],  # (1)
    RetainUntilDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ObjectLockRetentionModeType](./literals.md#objectlockretentionmodetype) 
## GetObjectRetentionRequestRequestTypeDef

```python
# GetObjectRetentionRequestRequestTypeDef definition

class GetObjectRetentionRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## GetObjectTaggingRequestRequestTypeDef

```python
# GetObjectTaggingRequestRequestTypeDef definition

class GetObjectTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## GetObjectTorrentRequestRequestTypeDef

```python
# GetObjectTorrentRequestRequestTypeDef definition

class GetObjectTorrentRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## PublicAccessBlockConfigurationTypeDef

```python
# PublicAccessBlockConfigurationTypeDef definition

class PublicAccessBlockConfigurationTypeDef(TypedDict):
    BlockPublicAcls: NotRequired[bool],
    IgnorePublicAcls: NotRequired[bool],
    BlockPublicPolicy: NotRequired[bool],
    RestrictPublicBuckets: NotRequired[bool],
```

## GetPublicAccessBlockRequestRequestTypeDef

```python
# GetPublicAccessBlockRequestRequestTypeDef definition

class GetPublicAccessBlockRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## GlacierJobParametersTypeDef

```python
# GlacierJobParametersTypeDef definition

class GlacierJobParametersTypeDef(TypedDict):
    Tier: TierType,  # (1)
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## GranteeTypeDef

```python
# GranteeTypeDef definition

class GranteeTypeDef(TypedDict):
    Type: TypeType,  # (1)
    DisplayName: NotRequired[str],
    EmailAddress: NotRequired[str],
    ID: NotRequired[str],
    URI: NotRequired[str],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## HeadBucketRequestRequestTypeDef

```python
# HeadBucketRequestRequestTypeDef definition

class HeadBucketRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
```

## InitiatorTypeDef

```python
# InitiatorTypeDef definition

class InitiatorTypeDef(TypedDict):
    ID: NotRequired[str],
    DisplayName: NotRequired[str],
```

## JSONInputTypeDef

```python
# JSONInputTypeDef definition

class JSONInputTypeDef(TypedDict):
    Type: NotRequired[JSONTypeType],  # (1)
```

1. See [:material-code-brackets: JSONTypeType](./literals.md#jsontypetype) 
## TieringTypeDef

```python
# TieringTypeDef definition

class TieringTypeDef(TypedDict):
    Days: int,
    AccessTier: IntelligentTieringAccessTierType,  # (1)
```

1. See [:material-code-brackets: IntelligentTieringAccessTierType](./literals.md#intelligenttieringaccesstiertype) 
## InventoryFilterTypeDef

```python
# InventoryFilterTypeDef definition

class InventoryFilterTypeDef(TypedDict):
    Prefix: str,
```

## InventoryScheduleTypeDef

```python
# InventoryScheduleTypeDef definition

class InventoryScheduleTypeDef(TypedDict):
    Frequency: InventoryFrequencyType,  # (1)
```

1. See [:material-code-brackets: InventoryFrequencyType](./literals.md#inventoryfrequencytype) 
## SSEKMSTypeDef

```python
# SSEKMSTypeDef definition

class SSEKMSTypeDef(TypedDict):
    KeyId: str,
```

## JSONOutputTypeDef

```python
# JSONOutputTypeDef definition

class JSONOutputTypeDef(TypedDict):
    RecordDelimiter: NotRequired[str],
```

## LifecycleExpirationTypeDef

```python
# LifecycleExpirationTypeDef definition

class LifecycleExpirationTypeDef(TypedDict):
    Date: NotRequired[datetime],
    Days: NotRequired[int],
    ExpiredObjectDeleteMarker: NotRequired[bool],
```

## NoncurrentVersionExpirationTypeDef

```python
# NoncurrentVersionExpirationTypeDef definition

class NoncurrentVersionExpirationTypeDef(TypedDict):
    NoncurrentDays: NotRequired[int],
    NewerNoncurrentVersions: NotRequired[int],
```

## NoncurrentVersionTransitionTypeDef

```python
# NoncurrentVersionTransitionTypeDef definition

class NoncurrentVersionTransitionTypeDef(TypedDict):
    NoncurrentDays: NotRequired[int],
    StorageClass: NotRequired[TransitionStorageClassType],  # (1)
    NewerNoncurrentVersions: NotRequired[int],
```

1. See [:material-code-brackets: TransitionStorageClassType](./literals.md#transitionstorageclasstype) 
## TransitionTypeDef

```python
# TransitionTypeDef definition

class TransitionTypeDef(TypedDict):
    Date: NotRequired[datetime],
    Days: NotRequired[int],
    StorageClass: NotRequired[TransitionStorageClassType],  # (1)
```

1. See [:material-code-brackets: TransitionStorageClassType](./literals.md#transitionstorageclasstype) 
## ListBucketAnalyticsConfigurationsRequestRequestTypeDef

```python
# ListBucketAnalyticsConfigurationsRequestRequestTypeDef definition

class ListBucketAnalyticsConfigurationsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ContinuationToken: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

## ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef

```python
# ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef definition

class ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ContinuationToken: NotRequired[str],
```

## ListBucketInventoryConfigurationsRequestRequestTypeDef

```python
# ListBucketInventoryConfigurationsRequestRequestTypeDef definition

class ListBucketInventoryConfigurationsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ContinuationToken: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

## ListBucketMetricsConfigurationsRequestRequestTypeDef

```python
# ListBucketMetricsConfigurationsRequestRequestTypeDef definition

class ListBucketMetricsConfigurationsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ContinuationToken: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMultipartUploadsRequestRequestTypeDef

```python
# ListMultipartUploadsRequestRequestTypeDef definition

class ListMultipartUploadsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    KeyMarker: NotRequired[str],
    MaxUploads: NotRequired[int],
    Prefix: NotRequired[str],
    UploadIdMarker: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## ListObjectVersionsRequestRequestTypeDef

```python
# ListObjectVersionsRequestRequestTypeDef definition

class ListObjectVersionsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    KeyMarker: NotRequired[str],
    MaxKeys: NotRequired[int],
    Prefix: NotRequired[str],
    VersionIdMarker: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
## ListObjectsRequestRequestTypeDef

```python
# ListObjectsRequestRequestTypeDef definition

class ListObjectsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Marker: NotRequired[str],
    MaxKeys: NotRequired[int],
    Prefix: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
## ListObjectsV2RequestRequestTypeDef

```python
# ListObjectsV2RequestRequestTypeDef definition

class ListObjectsV2RequestRequestTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    MaxKeys: NotRequired[int],
    Prefix: NotRequired[str],
    ContinuationToken: NotRequired[str],
    FetchOwner: NotRequired[bool],
    StartAfter: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
## PartTypeDef

```python
# PartTypeDef definition

class PartTypeDef(TypedDict):
    PartNumber: NotRequired[int],
    LastModified: NotRequired[datetime],
    ETag: NotRequired[str],
    Size: NotRequired[int],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
```

## ListPartsRequestRequestTypeDef

```python
# ListPartsRequestRequestTypeDef definition

class ListPartsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    UploadId: str,
    MaxParts: NotRequired[int],
    PartNumberMarker: NotRequired[int],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## MetadataEntryTypeDef

```python
# MetadataEntryTypeDef definition

class MetadataEntryTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ReplicationTimeValueTypeDef

```python
# ReplicationTimeValueTypeDef definition

class ReplicationTimeValueTypeDef(TypedDict):
    Minutes: NotRequired[int],
```

## QueueConfigurationDeprecatedTypeDef

```python
# QueueConfigurationDeprecatedTypeDef definition

class QueueConfigurationDeprecatedTypeDef(TypedDict):
    Id: NotRequired[str],
    Event: NotRequired[EventType],  # (1)
    Events: NotRequired[List[EventType]],  # (2)
    Queue: NotRequired[str],
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-brackets: EventType](./literals.md#eventtype) 
## TopicConfigurationDeprecatedTypeDef

```python
# TopicConfigurationDeprecatedTypeDef definition

class TopicConfigurationDeprecatedTypeDef(TypedDict):
    Id: NotRequired[str],
    Events: NotRequired[List[EventType]],  # (1)
    Event: NotRequired[EventType],  # (2)
    Topic: NotRequired[str],
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-brackets: EventType](./literals.md#eventtype) 
## ObjectDownloadFileRequestTypeDef

```python
# ObjectDownloadFileRequestTypeDef definition

class ObjectDownloadFileRequestTypeDef(TypedDict):
    Filename: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ObjectUploadFileRequestTypeDef

```python
# ObjectUploadFileRequestTypeDef definition

class ObjectUploadFileRequestTypeDef(TypedDict):
    Filename: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## OwnershipControlsRuleTypeDef

```python
# OwnershipControlsRuleTypeDef definition

class OwnershipControlsRuleTypeDef(TypedDict):
    ObjectOwnership: ObjectOwnershipType,  # (1)
```

1. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 
## ProgressTypeDef

```python
# ProgressTypeDef definition

class ProgressTypeDef(TypedDict):
    BytesScanned: NotRequired[int],
    BytesProcessed: NotRequired[int],
    BytesReturned: NotRequired[int],
```

## PutBucketPolicyRequestBucketPolicyPutTypeDef

```python
# PutBucketPolicyRequestBucketPolicyPutTypeDef definition

class PutBucketPolicyRequestBucketPolicyPutTypeDef(TypedDict):
    Policy: str,
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    ConfirmRemoveSelfBucketAccess: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketPolicyRequestRequestTypeDef

```python
# PutBucketPolicyRequestRequestTypeDef definition

class PutBucketPolicyRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Policy: str,
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    ConfirmRemoveSelfBucketAccess: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## RequestPaymentConfigurationTypeDef

```python
# RequestPaymentConfigurationTypeDef definition

class RequestPaymentConfigurationTypeDef(TypedDict):
    Payer: PayerType,  # (1)
```

1. See [:material-code-brackets: PayerType](./literals.md#payertype) 
## PutBucketVersioningRequestBucketVersioningEnableTypeDef

```python
# PutBucketVersioningRequestBucketVersioningEnableTypeDef definition

class PutBucketVersioningRequestBucketVersioningEnableTypeDef(TypedDict):
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    MFA: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## VersioningConfigurationTypeDef

```python
# VersioningConfigurationTypeDef definition

class VersioningConfigurationTypeDef(TypedDict):
    MFADelete: NotRequired[MFADeleteType],  # (1)
    Status: NotRequired[BucketVersioningStatusType],  # (2)
```

1. See [:material-code-brackets: MFADeleteType](./literals.md#mfadeletetype) 
2. See [:material-code-brackets: BucketVersioningStatusType](./literals.md#bucketversioningstatustype) 
## PutBucketVersioningRequestBucketVersioningSuspendTypeDef

```python
# PutBucketVersioningRequestBucketVersioningSuspendTypeDef definition

class PutBucketVersioningRequestBucketVersioningSuspendTypeDef(TypedDict):
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    MFA: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## RecordsEventTypeDef

```python
# RecordsEventTypeDef definition

class RecordsEventTypeDef(TypedDict):
    Payload: NotRequired[bytes],
```

## RedirectTypeDef

```python
# RedirectTypeDef definition

class RedirectTypeDef(TypedDict):
    HostName: NotRequired[str],
    HttpRedirectCode: NotRequired[str],
    Protocol: NotRequired[ProtocolType],  # (1)
    ReplaceKeyPrefixWith: NotRequired[str],
    ReplaceKeyWith: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## ReplicaModificationsTypeDef

```python
# ReplicaModificationsTypeDef definition

class ReplicaModificationsTypeDef(TypedDict):
    Status: ReplicaModificationsStatusType,  # (1)
```

1. See [:material-code-brackets: ReplicaModificationsStatusType](./literals.md#replicamodificationsstatustype) 
## RequestProgressTypeDef

```python
# RequestProgressTypeDef definition

class RequestProgressTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## ScanRangeTypeDef

```python
# ScanRangeTypeDef definition

class ScanRangeTypeDef(TypedDict):
    Start: NotRequired[int],
    End: NotRequired[int],
```

## ServerSideEncryptionByDefaultTypeDef

```python
# ServerSideEncryptionByDefaultTypeDef definition

class ServerSideEncryptionByDefaultTypeDef(TypedDict):
    SSEAlgorithm: ServerSideEncryptionType,  # (1)
    KMSMasterKeyID: NotRequired[str],
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
## SseKmsEncryptedObjectsTypeDef

```python
# SseKmsEncryptedObjectsTypeDef definition

class SseKmsEncryptedObjectsTypeDef(TypedDict):
    Status: SseKmsEncryptedObjectsStatusType,  # (1)
```

1. See [:material-code-brackets: SseKmsEncryptedObjectsStatusType](./literals.md#ssekmsencryptedobjectsstatustype) 
## StatsTypeDef

```python
# StatsTypeDef definition

class StatsTypeDef(TypedDict):
    BytesScanned: NotRequired[int],
    BytesProcessed: NotRequired[int],
    BytesReturned: NotRequired[int],
```

## AbortMultipartUploadOutputTypeDef

```python
# AbortMultipartUploadOutputTypeDef definition

class AbortMultipartUploadOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompleteMultipartUploadOutputTypeDef

```python
# CompleteMultipartUploadOutputTypeDef definition

class CompleteMultipartUploadOutputTypeDef(TypedDict):
    Location: str,
    Bucket: str,
    Key: str,
    Expiration: str,
    ETag: str,
    ChecksumCRC32: str,
    ChecksumCRC32C: str,
    ChecksumSHA1: str,
    ChecksumSHA256: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (1)
    VersionId: str,
    SSEKMSKeyId: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBucketOutputTypeDef

```python
# CreateBucketOutputTypeDef definition

class CreateBucketOutputTypeDef(TypedDict):
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultipartUploadOutputTypeDef

```python
# CreateMultipartUploadOutputTypeDef definition

class CreateMultipartUploadOutputTypeDef(TypedDict):
    AbortDate: datetime,
    AbortRuleId: str,
    Bucket: str,
    Key: str,
    UploadId: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (1)
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    SSEKMSEncryptionContext: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (2)
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteObjectOutputTypeDef

```python
# DeleteObjectOutputTypeDef definition

class DeleteObjectOutputTypeDef(TypedDict):
    DeleteMarker: bool,
    VersionId: str,
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteObjectTaggingOutputTypeDef

```python
# DeleteObjectTaggingOutputTypeDef definition

class DeleteObjectTaggingOutputTypeDef(TypedDict):
    VersionId: str,
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
## ErrorDocumentResponseTypeDef

```python
# ErrorDocumentResponseTypeDef definition

class ErrorDocumentResponseTypeDef(TypedDict):
    Key: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketAccelerateConfigurationOutputTypeDef

```python
# GetBucketAccelerateConfigurationOutputTypeDef definition

class GetBucketAccelerateConfigurationOutputTypeDef(TypedDict):
    Status: BucketAccelerateStatusType,  # (1)
    RequestCharged: RequestChargedType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: BucketAccelerateStatusType](./literals.md#bucketacceleratestatustype) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketLocationOutputTypeDef

```python
# GetBucketLocationOutputTypeDef definition

class GetBucketLocationOutputTypeDef(TypedDict):
    LocationConstraint: BucketLocationConstraintType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BucketLocationConstraintType](./literals.md#bucketlocationconstrainttype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketPolicyOutputTypeDef

```python
# GetBucketPolicyOutputTypeDef definition

class GetBucketPolicyOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketRequestPaymentOutputTypeDef

```python
# GetBucketRequestPaymentOutputTypeDef definition

class GetBucketRequestPaymentOutputTypeDef(TypedDict):
    Payer: PayerType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PayerType](./literals.md#payertype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketVersioningOutputTypeDef

```python
# GetBucketVersioningOutputTypeDef definition

class GetBucketVersioningOutputTypeDef(TypedDict):
    Status: BucketVersioningStatusType,  # (1)
    MFADelete: MFADeleteStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: BucketVersioningStatusType](./literals.md#bucketversioningstatustype) 
2. See [:material-code-brackets: MFADeleteStatusType](./literals.md#mfadeletestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectOutputTypeDef

```python
# GetObjectOutputTypeDef definition

class GetObjectOutputTypeDef(TypedDict):
    Body: StreamingBody,
    DeleteMarker: bool,
    AcceptRanges: str,
    Expiration: str,
    Restore: str,
    LastModified: datetime,
    ContentLength: int,
    ETag: str,
    ChecksumCRC32: str,
    ChecksumCRC32C: str,
    ChecksumSHA1: str,
    ChecksumSHA256: str,
    MissingMeta: int,
    VersionId: str,
    CacheControl: str,
    ContentDisposition: str,
    ContentEncoding: str,
    ContentLanguage: str,
    ContentRange: str,
    ContentType: str,
    Expires: datetime,
    WebsiteRedirectLocation: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (1)
    Metadata: Dict[str, str],
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    BucketKeyEnabled: bool,
    StorageClass: StorageClassType,  # (2)
    RequestCharged: RequestChargedType,  # (3)
    ReplicationStatus: ReplicationStatusType,  # (4)
    PartsCount: int,
    TagCount: int,
    ObjectLockMode: ObjectLockModeType,  # (5)
    ObjectLockRetainUntilDate: datetime,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
2. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
3. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
4. See [:material-code-brackets: ReplicationStatusType](./literals.md#replicationstatustype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectTorrentOutputTypeDef

```python
# GetObjectTorrentOutputTypeDef definition

class GetObjectTorrentOutputTypeDef(TypedDict):
    Body: StreamingBody,
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HeadObjectOutputTypeDef

```python
# HeadObjectOutputTypeDef definition

class HeadObjectOutputTypeDef(TypedDict):
    DeleteMarker: bool,
    AcceptRanges: str,
    Expiration: str,
    Restore: str,
    ArchiveStatus: ArchiveStatusType,  # (1)
    LastModified: datetime,
    ContentLength: int,
    ChecksumCRC32: str,
    ChecksumCRC32C: str,
    ChecksumSHA1: str,
    ChecksumSHA256: str,
    ETag: str,
    MissingMeta: int,
    VersionId: str,
    CacheControl: str,
    ContentDisposition: str,
    ContentEncoding: str,
    ContentLanguage: str,
    ContentType: str,
    Expires: datetime,
    WebsiteRedirectLocation: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (2)
    Metadata: Dict[str, str],
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    BucketKeyEnabled: bool,
    StorageClass: StorageClassType,  # (3)
    RequestCharged: RequestChargedType,  # (4)
    ReplicationStatus: ReplicationStatusType,  # (5)
    PartsCount: int,
    ObjectLockMode: ObjectLockModeType,  # (6)
    ObjectLockRetainUntilDate: datetime,
    ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: ArchiveStatusType](./literals.md#archivestatustype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
5. See [:material-code-brackets: ReplicationStatusType](./literals.md#replicationstatustype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndexDocumentResponseTypeDef

```python
# IndexDocumentResponseTypeDef definition

class IndexDocumentResponseTypeDef(TypedDict):
    Suffix: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiatorResponseTypeDef

```python
# InitiatorResponseTypeDef definition

class InitiatorResponseTypeDef(TypedDict):
    ID: str,
    DisplayName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OwnerResponseTypeDef

```python
# OwnerResponseTypeDef definition

class OwnerResponseTypeDef(TypedDict):
    DisplayName: str,
    ID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OwnerTypeDef

```python
# OwnerTypeDef definition

class OwnerTypeDef(TypedDict):
    DisplayName: str,
    ID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectAclOutputTypeDef

```python
# PutObjectAclOutputTypeDef definition

class PutObjectAclOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectLegalHoldOutputTypeDef

```python
# PutObjectLegalHoldOutputTypeDef definition

class PutObjectLegalHoldOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectLockConfigurationOutputTypeDef

```python
# PutObjectLockConfigurationOutputTypeDef definition

class PutObjectLockConfigurationOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectOutputTypeDef

```python
# PutObjectOutputTypeDef definition

class PutObjectOutputTypeDef(TypedDict):
    Expiration: str,
    ETag: str,
    ChecksumCRC32: str,
    ChecksumCRC32C: str,
    ChecksumSHA1: str,
    ChecksumSHA256: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (1)
    VersionId: str,
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    SSEKMSEncryptionContext: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectRetentionOutputTypeDef

```python
# PutObjectRetentionOutputTypeDef definition

class PutObjectRetentionOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectTaggingOutputTypeDef

```python
# PutObjectTaggingOutputTypeDef definition

class PutObjectTaggingOutputTypeDef(TypedDict):
    VersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RedirectAllRequestsToResponseTypeDef

```python
# RedirectAllRequestsToResponseTypeDef definition

class RedirectAllRequestsToResponseTypeDef(TypedDict):
    HostName: str,
    Protocol: ProtocolType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreObjectOutputTypeDef

```python
# RestoreObjectOutputTypeDef definition

class RestoreObjectOutputTypeDef(TypedDict):
    RequestCharged: RequestChargedType,  # (1)
    RestoreOutputPath: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreStatusResponseTypeDef

```python
# RestoreStatusResponseTypeDef definition

class RestoreStatusResponseTypeDef(TypedDict):
    IsRestoreInProgress: bool,
    RestoreExpiryDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreStatusTypeDef

```python
# RestoreStatusTypeDef definition

class RestoreStatusTypeDef(TypedDict):
    IsRestoreInProgress: bool,
    RestoreExpiryDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadPartOutputTypeDef

```python
# UploadPartOutputTypeDef definition

class UploadPartOutputTypeDef(TypedDict):
    ServerSideEncryption: ServerSideEncryptionType,  # (1)
    ETag: str,
    ChecksumCRC32: str,
    ChecksumCRC32C: str,
    ChecksumSHA1: str,
    ChecksumSHA256: str,
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketAccelerateConfigurationRequestRequestTypeDef

```python
# PutBucketAccelerateConfigurationRequestRequestTypeDef definition

class PutBucketAccelerateConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    AccelerateConfiguration: AccelerateConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
```

1. See [:material-code-braces: AccelerateConfigurationTypeDef](./type_defs.md#accelerateconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## AnalyticsAndOperatorTypeDef

```python
# AnalyticsAndOperatorTypeDef definition

class AnalyticsAndOperatorTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetBucketTaggingOutputTypeDef

```python
# GetBucketTaggingOutputTypeDef definition

class GetBucketTaggingOutputTypeDef(TypedDict):
    TagSet: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectTaggingOutputTypeDef

```python
# GetObjectTaggingOutputTypeDef definition

class GetObjectTaggingOutputTypeDef(TypedDict):
    VersionId: str,
    TagSet: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntelligentTieringAndOperatorTypeDef

```python
# IntelligentTieringAndOperatorTypeDef definition

class IntelligentTieringAndOperatorTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef

```python
# LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef definition

class LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ObjectSizeGreaterThan: NotRequired[int],
    ObjectSizeLessThan: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LifecycleRuleAndOperatorTypeDef

```python
# LifecycleRuleAndOperatorTypeDef definition

class LifecycleRuleAndOperatorTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    ObjectSizeGreaterThan: NotRequired[int],
    ObjectSizeLessThan: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MetricsAndOperatorTypeDef

```python
# MetricsAndOperatorTypeDef definition

class MetricsAndOperatorTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    AccessPointArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ReplicationRuleAndOperatorTypeDef

```python
# ReplicationRuleAndOperatorTypeDef definition

class ReplicationRuleAndOperatorTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TaggingTypeDef

```python
# TaggingTypeDef definition

class TaggingTypeDef(TypedDict):
    TagSet: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AnalyticsExportDestinationTypeDef

```python
# AnalyticsExportDestinationTypeDef definition

class AnalyticsExportDestinationTypeDef(TypedDict):
    S3BucketDestination: AnalyticsS3BucketDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: AnalyticsS3BucketDestinationTypeDef](./type_defs.md#analyticss3bucketdestinationtypedef) 
## UploadPartRequestMultipartUploadPartUploadTypeDef

```python
# UploadPartRequestMultipartUploadPartUploadTypeDef definition

class UploadPartRequestMultipartUploadPartUploadTypeDef(TypedDict):
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## UploadPartRequestRequestTypeDef

```python
# UploadPartRequestRequestTypeDef definition

class UploadPartRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    PartNumber: int,
    UploadId: str,
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## BucketCopyRequestTypeDef

```python
# BucketCopyRequestTypeDef definition

class BucketCopyRequestTypeDef(TypedDict):
    CopySource: CopySourceTypeDef,  # (1)
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    SourceClient: NotRequired[AioBaseClient],
    Config: NotRequired[TransferConfig],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
## ClientCopyRequestTypeDef

```python
# ClientCopyRequestTypeDef definition

class ClientCopyRequestTypeDef(TypedDict):
    CopySource: CopySourceTypeDef,  # (1)
    Bucket: str,
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    SourceClient: NotRequired[AioBaseClient],
    Config: NotRequired[TransferConfig],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
## ObjectCopyRequestTypeDef

```python
# ObjectCopyRequestTypeDef definition

class ObjectCopyRequestTypeDef(TypedDict):
    CopySource: CopySourceTypeDef,  # (1)
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    SourceClient: NotRequired[AioBaseClient],
    Config: NotRequired[TransferConfig],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
## BucketDownloadFileobjRequestTypeDef

```python
# BucketDownloadFileobjRequestTypeDef definition

class BucketDownloadFileobjRequestTypeDef(TypedDict):
    Key: str,
    Fileobj: Union[IO[Any], StreamingBody],
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## BucketUploadFileobjRequestTypeDef

```python
# BucketUploadFileobjRequestTypeDef definition

class BucketUploadFileobjRequestTypeDef(TypedDict):
    Fileobj: Union[IO[Any], StreamingBody],
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ClientDownloadFileobjRequestTypeDef

```python
# ClientDownloadFileobjRequestTypeDef definition

class ClientDownloadFileobjRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Fileobj: Union[IO[Any], StreamingBody],
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ClientUploadFileobjRequestTypeDef

```python
# ClientUploadFileobjRequestTypeDef definition

class ClientUploadFileobjRequestTypeDef(TypedDict):
    Fileobj: Union[IO[Any], StreamingBody],
    Bucket: str,
    Key: str,
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ObjectDownloadFileobjRequestTypeDef

```python
# ObjectDownloadFileobjRequestTypeDef definition

class ObjectDownloadFileobjRequestTypeDef(TypedDict):
    Fileobj: Union[IO[Any], StreamingBody],
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## ObjectUploadFileobjRequestTypeDef

```python
# ObjectUploadFileobjRequestTypeDef definition

class ObjectUploadFileobjRequestTypeDef(TypedDict):
    Fileobj: Union[IO[Any], StreamingBody],
    ExtraArgs: NotRequired[Dict[str, Any]],
    Callback: NotRequired[Callable[..., Any]],
    Config: NotRequired[TransferConfig],
```

## CORSConfigurationBucketCorsTypeDef

```python
# CORSConfigurationBucketCorsTypeDef definition

class CORSConfigurationBucketCorsTypeDef(TypedDict):
    CORSRules: Sequence[CORSRuleBucketCorsTypeDef],  # (1)
```

1. See [:material-code-braces: CORSRuleBucketCorsTypeDef](./type_defs.md#corsrulebucketcorstypedef) 
## CORSConfigurationTypeDef

```python
# CORSConfigurationTypeDef definition

class CORSConfigurationTypeDef(TypedDict):
    CORSRules: Sequence[CORSRuleTypeDef],  # (1)
```

1. See [:material-code-braces: CORSRuleTypeDef](./type_defs.md#corsruletypedef) 
## GetBucketCorsOutputTypeDef

```python
# GetBucketCorsOutputTypeDef definition

class GetBucketCorsOutputTypeDef(TypedDict):
    CORSRules: List[CORSRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CORSRuleTypeDef](./type_defs.md#corsruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompletedMultipartUploadTypeDef

```python
# CompletedMultipartUploadTypeDef definition

class CompletedMultipartUploadTypeDef(TypedDict):
    Parts: NotRequired[Sequence[CompletedPartTypeDef]],  # (1)
```

1. See [:material-code-braces: CompletedPartTypeDef](./type_defs.md#completedparttypedef) 
## CopyObjectOutputTypeDef

```python
# CopyObjectOutputTypeDef definition

class CopyObjectOutputTypeDef(TypedDict):
    CopyObjectResult: CopyObjectResultTypeDef,  # (1)
    Expiration: str,
    CopySourceVersionId: str,
    VersionId: str,
    ServerSideEncryption: ServerSideEncryptionType,  # (2)
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    SSEKMSEncryptionContext: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: CopyObjectResultTypeDef](./type_defs.md#copyobjectresulttypedef) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyObjectRequestObjectCopyFromTypeDef

```python
# CopyObjectRequestObjectCopyFromTypeDef definition

class CopyObjectRequestObjectCopyFromTypeDef(TypedDict):
    CopySource: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    CacheControl: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    CopySourceIfMatch: NotRequired[str],
    CopySourceIfModifiedSince: NotRequired[Union[datetime, str]],
    CopySourceIfNoneMatch: NotRequired[str],
    CopySourceIfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    MetadataDirective: NotRequired[MetadataDirectiveType],  # (3)
    TaggingDirective: NotRequired[TaggingDirectiveType],  # (4)
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (5)
    StorageClass: NotRequired[StorageClassType],  # (6)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    CopySourceSSECustomerAlgorithm: NotRequired[str],
    CopySourceSSECustomerKey: NotRequired[str],
    CopySourceSSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (7)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (8)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (9)
    ExpectedBucketOwner: NotRequired[str],
    ExpectedSourceBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: MetadataDirectiveType](./literals.md#metadatadirectivetype) 
4. See [:material-code-brackets: TaggingDirectiveType](./literals.md#taggingdirectivetype) 
5. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
6. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
7. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
8. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
9. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## CopyObjectRequestObjectSummaryCopyFromTypeDef

```python
# CopyObjectRequestObjectSummaryCopyFromTypeDef definition

class CopyObjectRequestObjectSummaryCopyFromTypeDef(TypedDict):
    CopySource: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    CacheControl: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    CopySourceIfMatch: NotRequired[str],
    CopySourceIfModifiedSince: NotRequired[Union[datetime, str]],
    CopySourceIfNoneMatch: NotRequired[str],
    CopySourceIfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    MetadataDirective: NotRequired[MetadataDirectiveType],  # (3)
    TaggingDirective: NotRequired[TaggingDirectiveType],  # (4)
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (5)
    StorageClass: NotRequired[StorageClassType],  # (6)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    CopySourceSSECustomerAlgorithm: NotRequired[str],
    CopySourceSSECustomerKey: NotRequired[str],
    CopySourceSSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (7)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (8)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (9)
    ExpectedBucketOwner: NotRequired[str],
    ExpectedSourceBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: MetadataDirectiveType](./literals.md#metadatadirectivetype) 
4. See [:material-code-brackets: TaggingDirectiveType](./literals.md#taggingdirectivetype) 
5. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
6. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
7. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
8. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
9. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef

```python
# CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef definition

class CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef(TypedDict):
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (2)
    StorageClass: NotRequired[StorageClassType],  # (3)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (4)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (5)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (6)
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (7)
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef

```python
# CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef definition

class CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef(TypedDict):
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (2)
    StorageClass: NotRequired[StorageClassType],  # (3)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (4)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (5)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (6)
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (7)
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## CreateMultipartUploadRequestRequestTypeDef

```python
# CreateMultipartUploadRequestRequestTypeDef definition

class CreateMultipartUploadRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (2)
    StorageClass: NotRequired[StorageClassType],  # (3)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (4)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (5)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (6)
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (7)
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
5. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
6. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
7. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetObjectRequestObjectGetTypeDef

```python
# GetObjectRequestObjectGetTypeDef definition

class GetObjectRequestObjectGetTypeDef(TypedDict):
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    ResponseCacheControl: NotRequired[str],
    ResponseContentDisposition: NotRequired[str],
    ResponseContentEncoding: NotRequired[str],
    ResponseContentLanguage: NotRequired[str],
    ResponseContentType: NotRequired[str],
    ResponseExpires: NotRequired[Union[datetime, str]],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## GetObjectRequestObjectSummaryGetTypeDef

```python
# GetObjectRequestObjectSummaryGetTypeDef definition

class GetObjectRequestObjectSummaryGetTypeDef(TypedDict):
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    ResponseCacheControl: NotRequired[str],
    ResponseContentDisposition: NotRequired[str],
    ResponseContentEncoding: NotRequired[str],
    ResponseContentLanguage: NotRequired[str],
    ResponseContentType: NotRequired[str],
    ResponseExpires: NotRequired[Union[datetime, str]],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## GetObjectRequestObjectVersionGetTypeDef

```python
# GetObjectRequestObjectVersionGetTypeDef definition

class GetObjectRequestObjectVersionGetTypeDef(TypedDict):
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    ResponseCacheControl: NotRequired[str],
    ResponseContentDisposition: NotRequired[str],
    ResponseContentEncoding: NotRequired[str],
    ResponseContentLanguage: NotRequired[str],
    ResponseContentType: NotRequired[str],
    ResponseExpires: NotRequired[Union[datetime, str]],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## GetObjectRequestRequestTypeDef

```python
# GetObjectRequestRequestTypeDef definition

class GetObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    ResponseCacheControl: NotRequired[str],
    ResponseContentDisposition: NotRequired[str],
    ResponseContentEncoding: NotRequired[str],
    ResponseContentLanguage: NotRequired[str],
    ResponseContentType: NotRequired[str],
    ResponseExpires: NotRequired[Union[datetime, str]],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## HeadObjectRequestObjectVersionHeadTypeDef

```python
# HeadObjectRequestObjectVersionHeadTypeDef definition

class HeadObjectRequestObjectVersionHeadTypeDef(TypedDict):
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## HeadObjectRequestRequestTypeDef

```python
# HeadObjectRequestRequestTypeDef definition

class HeadObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
## LifecycleExpirationBucketLifecycleConfigurationTypeDef

```python
# LifecycleExpirationBucketLifecycleConfigurationTypeDef definition

class LifecycleExpirationBucketLifecycleConfigurationTypeDef(TypedDict):
    Date: NotRequired[Union[datetime, str]],
    Days: NotRequired[int],
    ExpiredObjectDeleteMarker: NotRequired[bool],
```

## LifecycleExpirationBucketLifecycleTypeDef

```python
# LifecycleExpirationBucketLifecycleTypeDef definition

class LifecycleExpirationBucketLifecycleTypeDef(TypedDict):
    Date: NotRequired[Union[datetime, str]],
    Days: NotRequired[int],
    ExpiredObjectDeleteMarker: NotRequired[bool],
```

## PutObjectRequestBucketPutObjectTypeDef

```python
# PutObjectRequestBucketPutObjectTypeDef definition

class PutObjectRequestBucketPutObjectTypeDef(TypedDict):
    Key: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ContentType: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (3)
    StorageClass: NotRequired[StorageClassType],  # (4)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (5)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (6)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (7)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## PutObjectRequestObjectPutTypeDef

```python
# PutObjectRequestObjectPutTypeDef definition

class PutObjectRequestObjectPutTypeDef(TypedDict):
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ContentType: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (3)
    StorageClass: NotRequired[StorageClassType],  # (4)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (5)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (6)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (7)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## PutObjectRequestObjectSummaryPutTypeDef

```python
# PutObjectRequestObjectSummaryPutTypeDef definition

class PutObjectRequestObjectSummaryPutTypeDef(TypedDict):
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ContentType: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (3)
    StorageClass: NotRequired[StorageClassType],  # (4)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (5)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (6)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (7)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## PutObjectRequestRequestTypeDef

```python
# PutObjectRequestRequestTypeDef definition

class PutObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentLength: NotRequired[int],
    ContentMD5: NotRequired[str],
    ContentType: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (3)
    StorageClass: NotRequired[StorageClassType],  # (4)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    RequestPayer: NotRequired[RequestPayerType],  # (5)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (6)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (7)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
6. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
7. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## TransitionBucketLifecycleConfigurationTypeDef

```python
# TransitionBucketLifecycleConfigurationTypeDef definition

class TransitionBucketLifecycleConfigurationTypeDef(TypedDict):
    Date: NotRequired[Union[datetime, str]],
    Days: NotRequired[int],
    StorageClass: NotRequired[TransitionStorageClassType],  # (1)
```

1. See [:material-code-brackets: TransitionStorageClassType](./literals.md#transitionstorageclasstype) 
## TransitionBucketLifecycleTypeDef

```python
# TransitionBucketLifecycleTypeDef definition

class TransitionBucketLifecycleTypeDef(TypedDict):
    Date: NotRequired[Union[datetime, str]],
    Days: NotRequired[int],
    StorageClass: NotRequired[TransitionStorageClassType],  # (1)
```

1. See [:material-code-brackets: TransitionStorageClassType](./literals.md#transitionstorageclasstype) 
## WriteGetObjectResponseRequestRequestTypeDef

```python
# WriteGetObjectResponseRequestRequestTypeDef definition

class WriteGetObjectResponseRequestRequestTypeDef(TypedDict):
    RequestRoute: str,
    RequestToken: str,
    Body: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    StatusCode: NotRequired[int],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    AcceptRanges: NotRequired[str],
    CacheControl: NotRequired[str],
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentLength: NotRequired[int],
    ContentRange: NotRequired[str],
    ContentType: NotRequired[str],
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    DeleteMarker: NotRequired[bool],
    ETag: NotRequired[str],
    Expires: NotRequired[Union[datetime, str]],
    Expiration: NotRequired[str],
    LastModified: NotRequired[Union[datetime, str]],
    MissingMeta: NotRequired[int],
    Metadata: NotRequired[Mapping[str, str]],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (1)
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (2)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    PartsCount: NotRequired[int],
    ReplicationStatus: NotRequired[ReplicationStatusType],  # (3)
    RequestCharged: NotRequired[RequestChargedType],  # (4)
    Restore: NotRequired[str],
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (5)
    SSECustomerAlgorithm: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    StorageClass: NotRequired[StorageClassType],  # (6)
    TagCount: NotRequired[int],
    VersionId: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
2. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
3. See [:material-code-brackets: ReplicationStatusType](./literals.md#replicationstatustype) 
4. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
5. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
6. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
## UploadPartCopyOutputTypeDef

```python
# UploadPartCopyOutputTypeDef definition

class UploadPartCopyOutputTypeDef(TypedDict):
    CopySourceVersionId: str,
    CopyPartResult: CopyPartResultTypeDef,  # (1)
    ServerSideEncryption: ServerSideEncryptionType,  # (2)
    SSECustomerAlgorithm: str,
    SSECustomerKeyMD5: str,
    SSEKMSKeyId: str,
    BucketKeyEnabled: bool,
    RequestCharged: RequestChargedType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: CopyPartResultTypeDef](./type_defs.md#copypartresulttypedef) 
2. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
3. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBucketRequestBucketCreateTypeDef

```python
# CreateBucketRequestBucketCreateTypeDef definition

class CreateBucketRequestBucketCreateTypeDef(TypedDict):
    ACL: NotRequired[BucketCannedACLType],  # (1)
    CreateBucketConfiguration: NotRequired[CreateBucketConfigurationTypeDef],  # (2)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    ObjectLockEnabledForBucket: NotRequired[bool],
    ObjectOwnership: NotRequired[ObjectOwnershipType],  # (3)
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 
## CreateBucketRequestRequestTypeDef

```python
# CreateBucketRequestRequestTypeDef definition

class CreateBucketRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ACL: NotRequired[BucketCannedACLType],  # (1)
    CreateBucketConfiguration: NotRequired[CreateBucketConfigurationTypeDef],  # (2)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    ObjectLockEnabledForBucket: NotRequired[bool],
    ObjectOwnership: NotRequired[ObjectOwnershipType],  # (3)
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 
## CreateBucketRequestServiceResourceCreateBucketTypeDef

```python
# CreateBucketRequestServiceResourceCreateBucketTypeDef definition

class CreateBucketRequestServiceResourceCreateBucketTypeDef(TypedDict):
    Bucket: str,
    ACL: NotRequired[BucketCannedACLType],  # (1)
    CreateBucketConfiguration: NotRequired[CreateBucketConfigurationTypeDef],  # (2)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    ObjectLockEnabledForBucket: NotRequired[bool],
    ObjectOwnership: NotRequired[ObjectOwnershipType],  # (3)
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: CreateBucketConfigurationTypeDef](./type_defs.md#createbucketconfigurationtypedef) 
3. See [:material-code-brackets: ObjectOwnershipType](./literals.md#objectownershiptype) 
## ObjectLockRuleTypeDef

```python
# ObjectLockRuleTypeDef definition

class ObjectLockRuleTypeDef(TypedDict):
    DefaultRetention: NotRequired[DefaultRetentionTypeDef],  # (1)
```

1. See [:material-code-braces: DefaultRetentionTypeDef](./type_defs.md#defaultretentiontypedef) 
## DeleteObjectsOutputTypeDef

```python
# DeleteObjectsOutputTypeDef definition

class DeleteObjectsOutputTypeDef(TypedDict):
    Deleted: List[DeletedObjectTypeDef],  # (1)
    RequestCharged: RequestChargedType,  # (2)
    Errors: List[ErrorTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DeletedObjectTypeDef](./type_defs.md#deletedobjecttypedef) 
2. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
3. See [:material-code-braces: ErrorTypeDef](./type_defs.md#errortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTypeDef

```python
# DeleteTypeDef definition

class DeleteTypeDef(TypedDict):
    Objects: Sequence[ObjectIdentifierTypeDef],  # (1)
    Quiet: NotRequired[bool],
```

1. See [:material-code-braces: ObjectIdentifierTypeDef](./type_defs.md#objectidentifiertypedef) 
## S3KeyFilterBucketNotificationTypeDef

```python
# S3KeyFilterBucketNotificationTypeDef definition

class S3KeyFilterBucketNotificationTypeDef(TypedDict):
    FilterRules: NotRequired[Sequence[FilterRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
## S3KeyFilterTypeDef

```python
# S3KeyFilterTypeDef definition

class S3KeyFilterTypeDef(TypedDict):
    FilterRules: NotRequired[List[FilterRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
## GetBucketPolicyStatusOutputTypeDef

```python
# GetBucketPolicyStatusOutputTypeDef definition

class GetBucketPolicyStatusOutputTypeDef(TypedDict):
    PolicyStatus: PolicyStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyStatusTypeDef](./type_defs.md#policystatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectAttributesPartsTypeDef

```python
# GetObjectAttributesPartsTypeDef definition

class GetObjectAttributesPartsTypeDef(TypedDict):
    TotalPartsCount: NotRequired[int],
    PartNumberMarker: NotRequired[int],
    NextPartNumberMarker: NotRequired[int],
    MaxParts: NotRequired[int],
    IsTruncated: NotRequired[bool],
    Parts: NotRequired[List[ObjectPartTypeDef]],  # (1)
```

1. See [:material-code-braces: ObjectPartTypeDef](./type_defs.md#objectparttypedef) 
## GetObjectLegalHoldOutputTypeDef

```python
# GetObjectLegalHoldOutputTypeDef definition

class GetObjectLegalHoldOutputTypeDef(TypedDict):
    LegalHold: ObjectLockLegalHoldTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ObjectLockLegalHoldTypeDef](./type_defs.md#objectlocklegalholdtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectLegalHoldRequestRequestTypeDef

```python
# PutObjectLegalHoldRequestRequestTypeDef definition

class PutObjectLegalHoldRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    LegalHold: NotRequired[ObjectLockLegalHoldTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    VersionId: NotRequired[str],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: ObjectLockLegalHoldTypeDef](./type_defs.md#objectlocklegalholdtypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetObjectRetentionOutputTypeDef

```python
# GetObjectRetentionOutputTypeDef definition

class GetObjectRetentionOutputTypeDef(TypedDict):
    Retention: ObjectLockRetentionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ObjectLockRetentionTypeDef](./type_defs.md#objectlockretentiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectRetentionRequestRequestTypeDef

```python
# PutObjectRetentionRequestRequestTypeDef definition

class PutObjectRetentionRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Retention: NotRequired[ObjectLockRetentionTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    VersionId: NotRequired[str],
    BypassGovernanceRetention: NotRequired[bool],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: ObjectLockRetentionTypeDef](./type_defs.md#objectlockretentiontypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetPublicAccessBlockOutputTypeDef

```python
# GetPublicAccessBlockOutputTypeDef definition

class GetPublicAccessBlockOutputTypeDef(TypedDict):
    PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPublicAccessBlockRequestRequestTypeDef

```python
# PutPublicAccessBlockRequestRequestTypeDef definition

class PutPublicAccessBlockRequestRequestTypeDef(TypedDict):
    Bucket: str,
    PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,  # (1)
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: PublicAccessBlockConfigurationTypeDef](./type_defs.md#publicaccessblockconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GrantTypeDef

```python
# GrantTypeDef definition

class GrantTypeDef(TypedDict):
    Grantee: NotRequired[GranteeTypeDef],  # (1)
    Permission: NotRequired[PermissionType],  # (2)
```

1. See [:material-code-braces: GranteeTypeDef](./type_defs.md#granteetypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## TargetGrantTypeDef

```python
# TargetGrantTypeDef definition

class TargetGrantTypeDef(TypedDict):
    Grantee: NotRequired[GranteeTypeDef],  # (1)
    Permission: NotRequired[BucketLogsPermissionType],  # (2)
```

1. See [:material-code-braces: GranteeTypeDef](./type_defs.md#granteetypedef) 
2. See [:material-code-brackets: BucketLogsPermissionType](./literals.md#bucketlogspermissiontype) 
## HeadBucketRequestBucketExistsWaitTypeDef

```python
# HeadBucketRequestBucketExistsWaitTypeDef definition

class HeadBucketRequestBucketExistsWaitTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## HeadBucketRequestBucketNotExistsWaitTypeDef

```python
# HeadBucketRequestBucketNotExistsWaitTypeDef definition

class HeadBucketRequestBucketNotExistsWaitTypeDef(TypedDict):
    Bucket: str,
    ExpectedBucketOwner: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## HeadObjectRequestObjectExistsWaitTypeDef

```python
# HeadObjectRequestObjectExistsWaitTypeDef definition

class HeadObjectRequestObjectExistsWaitTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## HeadObjectRequestObjectNotExistsWaitTypeDef

```python
# HeadObjectRequestObjectNotExistsWaitTypeDef definition

class HeadObjectRequestObjectNotExistsWaitTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    IfMatch: NotRequired[str],
    IfModifiedSince: NotRequired[Union[datetime, str]],
    IfNoneMatch: NotRequired[str],
    IfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Range: NotRequired[str],
    VersionId: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    PartNumber: NotRequired[int],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumMode: NotRequired[ChecksumModeType],  # (2)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-brackets: ChecksumModeType](./literals.md#checksummodetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## InputSerializationTypeDef

```python
# InputSerializationTypeDef definition

class InputSerializationTypeDef(TypedDict):
    CSV: NotRequired[CSVInputTypeDef],  # (1)
    CompressionType: NotRequired[CompressionTypeType],  # (2)
    JSON: NotRequired[JSONInputTypeDef],  # (3)
    Parquet: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: CSVInputTypeDef](./type_defs.md#csvinputtypedef) 
2. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
3. See [:material-code-braces: JSONInputTypeDef](./type_defs.md#jsoninputtypedef) 
## InventoryEncryptionTypeDef

```python
# InventoryEncryptionTypeDef definition

class InventoryEncryptionTypeDef(TypedDict):
    SSES3: NotRequired[Dict[str, Any]],
    SSEKMS: NotRequired[SSEKMSTypeDef],  # (1)
```

1. See [:material-code-braces: SSEKMSTypeDef](./type_defs.md#ssekmstypedef) 
## OutputSerializationTypeDef

```python
# OutputSerializationTypeDef definition

class OutputSerializationTypeDef(TypedDict):
    CSV: NotRequired[CSVOutputTypeDef],  # (1)
    JSON: NotRequired[JSONOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CSVOutputTypeDef](./type_defs.md#csvoutputtypedef) 
2. See [:material-code-braces: JSONOutputTypeDef](./type_defs.md#jsonoutputtypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Prefix: str,
    Status: ExpirationStatusType,  # (2)
    Expiration: NotRequired[LifecycleExpirationTypeDef],  # (1)
    ID: NotRequired[str],
    Transition: NotRequired[TransitionTypeDef],  # (3)
    NoncurrentVersionTransition: NotRequired[NoncurrentVersionTransitionTypeDef],  # (4)
    NoncurrentVersionExpiration: NotRequired[NoncurrentVersionExpirationTypeDef],  # (5)
    AbortIncompleteMultipartUpload: NotRequired[AbortIncompleteMultipartUploadTypeDef],  # (6)
```

1. See [:material-code-braces: LifecycleExpirationTypeDef](./type_defs.md#lifecycleexpirationtypedef) 
2. See [:material-code-brackets: ExpirationStatusType](./literals.md#expirationstatustype) 
3. See [:material-code-braces: TransitionTypeDef](./type_defs.md#transitiontypedef) 
4. See [:material-code-braces: NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef) 
5. See [:material-code-braces: NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef) 
6. See [:material-code-braces: AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef) 
## ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef

```python
# ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef definition

class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Prefix: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectVersionsRequestListObjectVersionsPaginateTypeDef

```python
# ListObjectVersionsRequestListObjectVersionsPaginateTypeDef definition

class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Prefix: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectsRequestListObjectsPaginateTypeDef

```python
# ListObjectsRequestListObjectsPaginateTypeDef definition

class ListObjectsRequestListObjectsPaginateTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Prefix: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectsV2RequestListObjectsV2PaginateTypeDef

```python
# ListObjectsV2RequestListObjectsV2PaginateTypeDef definition

class ListObjectsV2RequestListObjectsV2PaginateTypeDef(TypedDict):
    Bucket: str,
    Delimiter: NotRequired[str],
    EncodingType: NotRequired[EncodingTypeType],  # (1)
    Prefix: NotRequired[str],
    FetchOwner: NotRequired[bool],
    StartAfter: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    OptionalObjectAttributes: NotRequired[Sequence[OptionalObjectAttributesType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPartsRequestListPartsPaginateTypeDef

```python
# ListPartsRequestListPartsPaginateTypeDef definition

class ListPartsRequestListPartsPaginateTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    UploadId: str,
    RequestPayer: NotRequired[RequestPayerType],  # (1)
    ExpectedBucketOwner: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MetricsTypeDef

```python
# MetricsTypeDef definition

class MetricsTypeDef(TypedDict):
    Status: MetricsStatusType,  # (1)
    EventThreshold: NotRequired[ReplicationTimeValueTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
2. See [:material-code-braces: ReplicationTimeValueTypeDef](./type_defs.md#replicationtimevaluetypedef) 
## ReplicationTimeTypeDef

```python
# ReplicationTimeTypeDef definition

class ReplicationTimeTypeDef(TypedDict):
    Status: ReplicationTimeStatusType,  # (1)
    Time: ReplicationTimeValueTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplicationTimeStatusType](./literals.md#replicationtimestatustype) 
2. See [:material-code-braces: ReplicationTimeValueTypeDef](./type_defs.md#replicationtimevaluetypedef) 
## NotificationConfigurationDeprecatedResponseTypeDef

```python
# NotificationConfigurationDeprecatedResponseTypeDef definition

class NotificationConfigurationDeprecatedResponseTypeDef(TypedDict):
    TopicConfiguration: TopicConfigurationDeprecatedTypeDef,  # (1)
    QueueConfiguration: QueueConfigurationDeprecatedTypeDef,  # (2)
    CloudFunctionConfiguration: CloudFunctionConfigurationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TopicConfigurationDeprecatedTypeDef](./type_defs.md#topicconfigurationdeprecatedtypedef) 
2. See [:material-code-braces: QueueConfigurationDeprecatedTypeDef](./type_defs.md#queueconfigurationdeprecatedtypedef) 
3. See [:material-code-braces: CloudFunctionConfigurationTypeDef](./type_defs.md#cloudfunctionconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotificationConfigurationDeprecatedTypeDef

```python
# NotificationConfigurationDeprecatedTypeDef definition

class NotificationConfigurationDeprecatedTypeDef(TypedDict):
    TopicConfiguration: NotRequired[TopicConfigurationDeprecatedTypeDef],  # (1)
    QueueConfiguration: NotRequired[QueueConfigurationDeprecatedTypeDef],  # (2)
    CloudFunctionConfiguration: NotRequired[CloudFunctionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: TopicConfigurationDeprecatedTypeDef](./type_defs.md#topicconfigurationdeprecatedtypedef) 
2. See [:material-code-braces: QueueConfigurationDeprecatedTypeDef](./type_defs.md#queueconfigurationdeprecatedtypedef) 
3. See [:material-code-braces: CloudFunctionConfigurationTypeDef](./type_defs.md#cloudfunctionconfigurationtypedef) 
## OwnershipControlsTypeDef

```python
# OwnershipControlsTypeDef definition

class OwnershipControlsTypeDef(TypedDict):
    Rules: List[OwnershipControlsRuleTypeDef],  # (1)
```

1. See [:material-code-braces: OwnershipControlsRuleTypeDef](./type_defs.md#ownershipcontrolsruletypedef) 
## ProgressEventTypeDef

```python
# ProgressEventTypeDef definition

class ProgressEventTypeDef(TypedDict):
    Details: NotRequired[ProgressTypeDef],  # (1)
```

1. See [:material-code-braces: ProgressTypeDef](./type_defs.md#progresstypedef) 
## PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef

```python
# PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef definition

class PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef(TypedDict):
    RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: RequestPaymentConfigurationTypeDef](./type_defs.md#requestpaymentconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketRequestPaymentRequestRequestTypeDef

```python
# PutBucketRequestPaymentRequestRequestTypeDef definition

class PutBucketRequestPaymentRequestRequestTypeDef(TypedDict):
    Bucket: str,
    RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: RequestPaymentConfigurationTypeDef](./type_defs.md#requestpaymentconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketVersioningRequestBucketVersioningPutTypeDef

```python
# PutBucketVersioningRequestBucketVersioningPutTypeDef definition

class PutBucketVersioningRequestBucketVersioningPutTypeDef(TypedDict):
    VersioningConfiguration: VersioningConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    MFA: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketVersioningRequestRequestTypeDef

```python
# PutBucketVersioningRequestRequestTypeDef definition

class PutBucketVersioningRequestRequestTypeDef(TypedDict):
    Bucket: str,
    VersioningConfiguration: VersioningConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    MFA: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## RoutingRuleTypeDef

```python
# RoutingRuleTypeDef definition

class RoutingRuleTypeDef(TypedDict):
    Redirect: RedirectTypeDef,  # (2)
    Condition: NotRequired[ConditionTypeDef],  # (1)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: RedirectTypeDef](./type_defs.md#redirecttypedef) 
## ServerSideEncryptionRuleTypeDef

```python
# ServerSideEncryptionRuleTypeDef definition

class ServerSideEncryptionRuleTypeDef(TypedDict):
    ApplyServerSideEncryptionByDefault: NotRequired[ServerSideEncryptionByDefaultTypeDef],  # (1)
    BucketKeyEnabled: NotRequired[bool],
```

1. See [:material-code-braces: ServerSideEncryptionByDefaultTypeDef](./type_defs.md#serversideencryptionbydefaulttypedef) 
## SourceSelectionCriteriaTypeDef

```python
# SourceSelectionCriteriaTypeDef definition

class SourceSelectionCriteriaTypeDef(TypedDict):
    SseKmsEncryptedObjects: NotRequired[SseKmsEncryptedObjectsTypeDef],  # (1)
    ReplicaModifications: NotRequired[ReplicaModificationsTypeDef],  # (2)
```

1. See [:material-code-braces: SseKmsEncryptedObjectsTypeDef](./type_defs.md#ssekmsencryptedobjectstypedef) 
2. See [:material-code-braces: ReplicaModificationsTypeDef](./type_defs.md#replicamodificationstypedef) 
## StatsEventTypeDef

```python
# StatsEventTypeDef definition

class StatsEventTypeDef(TypedDict):
    Details: NotRequired[StatsTypeDef],  # (1)
```

1. See [:material-code-braces: StatsTypeDef](./type_defs.md#statstypedef) 
## DeleteMarkerEntryTypeDef

```python
# DeleteMarkerEntryTypeDef definition

class DeleteMarkerEntryTypeDef(TypedDict):
    Owner: NotRequired[OwnerTypeDef],  # (1)
    Key: NotRequired[str],
    VersionId: NotRequired[str],
    IsLatest: NotRequired[bool],
    LastModified: NotRequired[datetime],
```

1. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
## ListBucketsOutputTypeDef

```python
# ListBucketsOutputTypeDef definition

class ListBucketsOutputTypeDef(TypedDict):
    Buckets: List[BucketTypeDef],  # (1)
    Owner: OwnerTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
2. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPartsOutputTypeDef

```python
# ListPartsOutputTypeDef definition

class ListPartsOutputTypeDef(TypedDict):
    AbortDate: datetime,
    AbortRuleId: str,
    Bucket: str,
    Key: str,
    UploadId: str,
    PartNumberMarker: int,
    NextPartNumberMarker: int,
    MaxParts: int,
    IsTruncated: bool,
    Parts: List[PartTypeDef],  # (1)
    Initiator: InitiatorTypeDef,  # (2)
    Owner: OwnerTypeDef,  # (3)
    StorageClass: StorageClassType,  # (4)
    RequestCharged: RequestChargedType,  # (5)
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: PartTypeDef](./type_defs.md#parttypedef) 
2. See [:material-code-braces: InitiatorTypeDef](./type_defs.md#initiatortypedef) 
3. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
6. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MultipartUploadTypeDef

```python
# MultipartUploadTypeDef definition

class MultipartUploadTypeDef(TypedDict):
    UploadId: NotRequired[str],
    Key: NotRequired[str],
    Initiated: NotRequired[datetime],
    StorageClass: NotRequired[StorageClassType],  # (1)
    Owner: NotRequired[OwnerTypeDef],  # (2)
    Initiator: NotRequired[InitiatorTypeDef],  # (3)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (4)
```

1. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
2. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
3. See [:material-code-braces: InitiatorTypeDef](./type_defs.md#initiatortypedef) 
4. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## ObjectTypeDef

```python
# ObjectTypeDef definition

class ObjectTypeDef(TypedDict):
    Key: NotRequired[str],
    LastModified: NotRequired[datetime],
    ETag: NotRequired[str],
    ChecksumAlgorithm: NotRequired[List[ChecksumAlgorithmType]],  # (1)
    Size: NotRequired[int],
    StorageClass: NotRequired[ObjectStorageClassType],  # (2)
    Owner: NotRequired[OwnerTypeDef],  # (3)
    RestoreStatus: NotRequired[RestoreStatusTypeDef],  # (4)
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: ObjectStorageClassType](./literals.md#objectstorageclasstype) 
3. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
4. See [:material-code-braces: RestoreStatusTypeDef](./type_defs.md#restorestatustypedef) 
## ObjectVersionTypeDef

```python
# ObjectVersionTypeDef definition

class ObjectVersionTypeDef(TypedDict):
    ETag: NotRequired[str],
    ChecksumAlgorithm: NotRequired[List[ChecksumAlgorithmType]],  # (1)
    Size: NotRequired[int],
    StorageClass: NotRequired[ObjectVersionStorageClassType],  # (2)
    Key: NotRequired[str],
    VersionId: NotRequired[str],
    IsLatest: NotRequired[bool],
    LastModified: NotRequired[datetime],
    Owner: NotRequired[OwnerTypeDef],  # (3)
    RestoreStatus: NotRequired[RestoreStatusTypeDef],  # (4)
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: ObjectVersionStorageClassType](./literals.md#objectversionstorageclasstype) 
3. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
4. See [:material-code-braces: RestoreStatusTypeDef](./type_defs.md#restorestatustypedef) 
## AnalyticsFilterTypeDef

```python
# AnalyticsFilterTypeDef definition

class AnalyticsFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    And: NotRequired[AnalyticsAndOperatorTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AnalyticsAndOperatorTypeDef](./type_defs.md#analyticsandoperatortypedef) 
## IntelligentTieringFilterTypeDef

```python
# IntelligentTieringFilterTypeDef definition

class IntelligentTieringFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    And: NotRequired[IntelligentTieringAndOperatorTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: IntelligentTieringAndOperatorTypeDef](./type_defs.md#intelligenttieringandoperatortypedef) 
## LifecycleRuleFilterBucketLifecycleConfigurationTypeDef

```python
# LifecycleRuleFilterBucketLifecycleConfigurationTypeDef definition

class LifecycleRuleFilterBucketLifecycleConfigurationTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    ObjectSizeGreaterThan: NotRequired[int],
    ObjectSizeLessThan: NotRequired[int],
    And: NotRequired[LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef](./type_defs.md#lifecycleruleandoperatorbucketlifecycleconfigurationtypedef) 
## LifecycleRuleFilterTypeDef

```python
# LifecycleRuleFilterTypeDef definition

class LifecycleRuleFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    ObjectSizeGreaterThan: NotRequired[int],
    ObjectSizeLessThan: NotRequired[int],
    And: NotRequired[LifecycleRuleAndOperatorTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: LifecycleRuleAndOperatorTypeDef](./type_defs.md#lifecycleruleandoperatortypedef) 
## MetricsFilterTypeDef

```python
# MetricsFilterTypeDef definition

class MetricsFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    AccessPointArn: NotRequired[str],
    And: NotRequired[MetricsAndOperatorTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MetricsAndOperatorTypeDef](./type_defs.md#metricsandoperatortypedef) 
## ReplicationRuleFilterTypeDef

```python
# ReplicationRuleFilterTypeDef definition

class ReplicationRuleFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[TagTypeDef],  # (1)
    And: NotRequired[ReplicationRuleAndOperatorTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicationRuleAndOperatorTypeDef](./type_defs.md#replicationruleandoperatortypedef) 
## PutBucketTaggingRequestBucketTaggingPutTypeDef

```python
# PutBucketTaggingRequestBucketTaggingPutTypeDef definition

class PutBucketTaggingRequestBucketTaggingPutTypeDef(TypedDict):
    Tagging: TaggingTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketTaggingRequestRequestTypeDef

```python
# PutBucketTaggingRequestRequestTypeDef definition

class PutBucketTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Tagging: TaggingTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutObjectTaggingRequestRequestTypeDef

```python
# PutObjectTaggingRequestRequestTypeDef definition

class PutObjectTaggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Tagging: TaggingTypeDef,  # (1)
    VersionId: NotRequired[str],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (3)
```

1. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
3. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## StorageClassAnalysisDataExportTypeDef

```python
# StorageClassAnalysisDataExportTypeDef definition

class StorageClassAnalysisDataExportTypeDef(TypedDict):
    OutputSchemaVersion: StorageClassAnalysisSchemaVersionType,  # (1)
    Destination: AnalyticsExportDestinationTypeDef,  # (2)
```

1. See [:material-code-brackets: StorageClassAnalysisSchemaVersionType](./literals.md#storageclassanalysisschemaversiontype) 
2. See [:material-code-braces: AnalyticsExportDestinationTypeDef](./type_defs.md#analyticsexportdestinationtypedef) 
## CopyObjectRequestRequestTypeDef

```python
# CopyObjectRequestRequestTypeDef definition

class CopyObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    CopySource: Union[str, CopySourceTypeDef],  # (1)
    Key: str,
    ACL: NotRequired[ObjectCannedACLType],  # (2)
    CacheControl: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ContentDisposition: NotRequired[str],
    ContentEncoding: NotRequired[str],
    ContentLanguage: NotRequired[str],
    ContentType: NotRequired[str],
    CopySourceIfMatch: NotRequired[str],
    CopySourceIfModifiedSince: NotRequired[Union[datetime, str]],
    CopySourceIfNoneMatch: NotRequired[str],
    CopySourceIfUnmodifiedSince: NotRequired[Union[datetime, str]],
    Expires: NotRequired[Union[datetime, str]],
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    Metadata: NotRequired[Mapping[str, str]],
    MetadataDirective: NotRequired[MetadataDirectiveType],  # (4)
    TaggingDirective: NotRequired[TaggingDirectiveType],  # (5)
    ServerSideEncryption: NotRequired[ServerSideEncryptionType],  # (6)
    StorageClass: NotRequired[StorageClassType],  # (7)
    WebsiteRedirectLocation: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
    SSEKMSEncryptionContext: NotRequired[str],
    BucketKeyEnabled: NotRequired[bool],
    CopySourceSSECustomerAlgorithm: NotRequired[str],
    CopySourceSSECustomerKey: NotRequired[str],
    CopySourceSSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (8)
    Tagging: NotRequired[str],
    ObjectLockMode: NotRequired[ObjectLockModeType],  # (9)
    ObjectLockRetainUntilDate: NotRequired[Union[datetime, str]],
    ObjectLockLegalHoldStatus: NotRequired[ObjectLockLegalHoldStatusType],  # (10)
    ExpectedBucketOwner: NotRequired[str],
    ExpectedSourceBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: MetadataDirectiveType](./literals.md#metadatadirectivetype) 
5. See [:material-code-brackets: TaggingDirectiveType](./literals.md#taggingdirectivetype) 
6. See [:material-code-brackets: ServerSideEncryptionType](./literals.md#serversideencryptiontype) 
7. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
8. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
9. See [:material-code-brackets: ObjectLockModeType](./literals.md#objectlockmodetype) 
10. See [:material-code-brackets: ObjectLockLegalHoldStatusType](./literals.md#objectlocklegalholdstatustype) 
## UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef

```python
# UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef definition

class UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef(TypedDict):
    CopySource: Union[str, CopySourceTypeDef],  # (1)
    CopySourceIfMatch: NotRequired[str],
    CopySourceIfModifiedSince: NotRequired[Union[datetime, str]],
    CopySourceIfNoneMatch: NotRequired[str],
    CopySourceIfUnmodifiedSince: NotRequired[Union[datetime, str]],
    CopySourceRange: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    CopySourceSSECustomerAlgorithm: NotRequired[str],
    CopySourceSSECustomerKey: NotRequired[str],
    CopySourceSSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    ExpectedSourceBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## UploadPartCopyRequestRequestTypeDef

```python
# UploadPartCopyRequestRequestTypeDef definition

class UploadPartCopyRequestRequestTypeDef(TypedDict):
    Bucket: str,
    CopySource: Union[str, CopySourceTypeDef],  # (1)
    Key: str,
    PartNumber: int,
    UploadId: str,
    CopySourceIfMatch: NotRequired[str],
    CopySourceIfModifiedSince: NotRequired[Union[datetime, str]],
    CopySourceIfNoneMatch: NotRequired[str],
    CopySourceIfUnmodifiedSince: NotRequired[Union[datetime, str]],
    CopySourceRange: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    CopySourceSSECustomerAlgorithm: NotRequired[str],
    CopySourceSSECustomerKey: NotRequired[str],
    CopySourceSSECustomerKeyMD5: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    ExpectedSourceBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: CopySourceTypeDef](./type_defs.md#copysourcetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## PutBucketCorsRequestBucketCorsPutTypeDef

```python
# PutBucketCorsRequestBucketCorsPutTypeDef definition

class PutBucketCorsRequestBucketCorsPutTypeDef(TypedDict):
    CORSConfiguration: CORSConfigurationBucketCorsTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: CORSConfigurationBucketCorsTypeDef](./type_defs.md#corsconfigurationbucketcorstypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketCorsRequestRequestTypeDef

```python
# PutBucketCorsRequestRequestTypeDef definition

class PutBucketCorsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    CORSConfiguration: CORSConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: CORSConfigurationTypeDef](./type_defs.md#corsconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef

```python
# CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef definition

class CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef(TypedDict):
    MultipartUpload: NotRequired[CompletedMultipartUploadTypeDef],  # (1)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
```

1. See [:material-code-braces: CompletedMultipartUploadTypeDef](./type_defs.md#completedmultipartuploadtypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## CompleteMultipartUploadRequestRequestTypeDef

```python
# CompleteMultipartUploadRequestRequestTypeDef definition

class CompleteMultipartUploadRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    UploadId: str,
    MultipartUpload: NotRequired[CompletedMultipartUploadTypeDef],  # (1)
    ChecksumCRC32: NotRequired[str],
    ChecksumCRC32C: NotRequired[str],
    ChecksumSHA1: NotRequired[str],
    ChecksumSHA256: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
```

1. See [:material-code-braces: CompletedMultipartUploadTypeDef](./type_defs.md#completedmultipartuploadtypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## RuleBucketLifecycleTypeDef

```python
# RuleBucketLifecycleTypeDef definition

class RuleBucketLifecycleTypeDef(TypedDict):
    Prefix: str,
    Status: ExpirationStatusType,  # (2)
    Expiration: NotRequired[LifecycleExpirationBucketLifecycleTypeDef],  # (1)
    ID: NotRequired[str],
    Transition: NotRequired[TransitionBucketLifecycleTypeDef],  # (3)
    NoncurrentVersionTransition: NotRequired[NoncurrentVersionTransitionTypeDef],  # (4)
    NoncurrentVersionExpiration: NotRequired[NoncurrentVersionExpirationTypeDef],  # (5)
    AbortIncompleteMultipartUpload: NotRequired[AbortIncompleteMultipartUploadTypeDef],  # (6)
```

1. See [:material-code-braces: LifecycleExpirationBucketLifecycleTypeDef](./type_defs.md#lifecycleexpirationbucketlifecycletypedef) 
2. See [:material-code-brackets: ExpirationStatusType](./literals.md#expirationstatustype) 
3. See [:material-code-braces: TransitionBucketLifecycleTypeDef](./type_defs.md#transitionbucketlifecycletypedef) 
4. See [:material-code-braces: NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef) 
5. See [:material-code-braces: NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef) 
6. See [:material-code-braces: AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef) 
## ObjectLockConfigurationTypeDef

```python
# ObjectLockConfigurationTypeDef definition

class ObjectLockConfigurationTypeDef(TypedDict):
    ObjectLockEnabled: NotRequired[ObjectLockEnabledType],  # (1)
    Rule: NotRequired[ObjectLockRuleTypeDef],  # (2)
```

1. See [:material-code-brackets: ObjectLockEnabledType](./literals.md#objectlockenabledtype) 
2. See [:material-code-braces: ObjectLockRuleTypeDef](./type_defs.md#objectlockruletypedef) 
## DeleteObjectsRequestBucketDeleteObjectsTypeDef

```python
# DeleteObjectsRequestBucketDeleteObjectsTypeDef definition

class DeleteObjectsRequestBucketDeleteObjectsTypeDef(TypedDict):
    Delete: DeleteTypeDef,  # (1)
    MFA: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
```

1. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## DeleteObjectsRequestRequestTypeDef

```python
# DeleteObjectsRequestRequestTypeDef definition

class DeleteObjectsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Delete: DeleteTypeDef,  # (1)
    MFA: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    BypassGovernanceRetention: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
```

1. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## NotificationConfigurationFilterBucketNotificationTypeDef

```python
# NotificationConfigurationFilterBucketNotificationTypeDef definition

class NotificationConfigurationFilterBucketNotificationTypeDef(TypedDict):
    Key: NotRequired[S3KeyFilterBucketNotificationTypeDef],  # (1)
```

1. See [:material-code-braces: S3KeyFilterBucketNotificationTypeDef](./type_defs.md#s3keyfilterbucketnotificationtypedef) 
## NotificationConfigurationFilterTypeDef

```python
# NotificationConfigurationFilterTypeDef definition

class NotificationConfigurationFilterTypeDef(TypedDict):
    Key: NotRequired[S3KeyFilterTypeDef],  # (1)
```

1. See [:material-code-braces: S3KeyFilterTypeDef](./type_defs.md#s3keyfiltertypedef) 
## GetObjectAttributesOutputTypeDef

```python
# GetObjectAttributesOutputTypeDef definition

class GetObjectAttributesOutputTypeDef(TypedDict):
    DeleteMarker: bool,
    LastModified: datetime,
    VersionId: str,
    RequestCharged: RequestChargedType,  # (1)
    ETag: str,
    Checksum: ChecksumTypeDef,  # (2)
    ObjectParts: GetObjectAttributesPartsTypeDef,  # (3)
    StorageClass: StorageClassType,  # (4)
    ObjectSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
2. See [:material-code-braces: ChecksumTypeDef](./type_defs.md#checksumtypedef) 
3. See [:material-code-braces: GetObjectAttributesPartsTypeDef](./type_defs.md#getobjectattributespartstypedef) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccessControlPolicyTypeDef

```python
# AccessControlPolicyTypeDef definition

class AccessControlPolicyTypeDef(TypedDict):
    Grants: NotRequired[Sequence[GrantTypeDef]],  # (1)
    Owner: NotRequired[OwnerTypeDef],  # (2)
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
## GetBucketAclOutputTypeDef

```python
# GetBucketAclOutputTypeDef definition

class GetBucketAclOutputTypeDef(TypedDict):
    Owner: OwnerTypeDef,  # (1)
    Grants: List[GrantTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
2. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectAclOutputTypeDef

```python
# GetObjectAclOutputTypeDef definition

class GetObjectAclOutputTypeDef(TypedDict):
    Owner: OwnerTypeDef,  # (1)
    Grants: List[GrantTypeDef],  # (2)
    RequestCharged: RequestChargedType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
2. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
3. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    BucketName: str,
    Prefix: str,
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    CannedACL: NotRequired[ObjectCannedACLType],  # (2)
    AccessControlList: NotRequired[Sequence[GrantTypeDef]],  # (3)
    Tagging: NotRequired[TaggingTypeDef],  # (4)
    UserMetadata: NotRequired[Sequence[MetadataEntryTypeDef]],  # (5)
    StorageClass: NotRequired[StorageClassType],  # (6)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
3. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
4. See [:material-code-braces: TaggingTypeDef](./type_defs.md#taggingtypedef) 
5. See [:material-code-braces: MetadataEntryTypeDef](./type_defs.md#metadataentrytypedef) 
6. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
## LoggingEnabledBucketLoggingTypeDef

```python
# LoggingEnabledBucketLoggingTypeDef definition

class LoggingEnabledBucketLoggingTypeDef(TypedDict):
    TargetBucket: str,
    TargetPrefix: str,
    TargetGrants: NotRequired[Sequence[TargetGrantTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetGrantTypeDef](./type_defs.md#targetgranttypedef) 
## LoggingEnabledResponseTypeDef

```python
# LoggingEnabledResponseTypeDef definition

class LoggingEnabledResponseTypeDef(TypedDict):
    TargetBucket: str,
    TargetGrants: List[TargetGrantTypeDef],  # (1)
    TargetPrefix: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetGrantTypeDef](./type_defs.md#targetgranttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingEnabledTypeDef

```python
# LoggingEnabledTypeDef definition

class LoggingEnabledTypeDef(TypedDict):
    TargetBucket: str,
    TargetPrefix: str,
    TargetGrants: NotRequired[List[TargetGrantTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetGrantTypeDef](./type_defs.md#targetgranttypedef) 
## InventoryS3BucketDestinationTypeDef

```python
# InventoryS3BucketDestinationTypeDef definition

class InventoryS3BucketDestinationTypeDef(TypedDict):
    Bucket: str,
    Format: InventoryFormatType,  # (1)
    AccountId: NotRequired[str],
    Prefix: NotRequired[str],
    Encryption: NotRequired[InventoryEncryptionTypeDef],  # (2)
```

1. See [:material-code-brackets: InventoryFormatType](./literals.md#inventoryformattype) 
2. See [:material-code-braces: InventoryEncryptionTypeDef](./type_defs.md#inventoryencryptiontypedef) 
## SelectObjectContentRequestRequestTypeDef

```python
# SelectObjectContentRequestRequestTypeDef definition

class SelectObjectContentRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    Expression: str,
    ExpressionType: ExpressionTypeType,  # (1)
    InputSerialization: InputSerializationTypeDef,  # (2)
    OutputSerialization: OutputSerializationTypeDef,  # (3)
    SSECustomerAlgorithm: NotRequired[str],
    SSECustomerKey: NotRequired[str],
    SSECustomerKeyMD5: NotRequired[str],
    RequestProgress: NotRequired[RequestProgressTypeDef],  # (4)
    ScanRange: NotRequired[ScanRangeTypeDef],  # (5)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
2. See [:material-code-braces: InputSerializationTypeDef](./type_defs.md#inputserializationtypedef) 
3. See [:material-code-braces: OutputSerializationTypeDef](./type_defs.md#outputserializationtypedef) 
4. See [:material-code-braces: RequestProgressTypeDef](./type_defs.md#requestprogresstypedef) 
5. See [:material-code-braces: ScanRangeTypeDef](./type_defs.md#scanrangetypedef) 
## SelectParametersTypeDef

```python
# SelectParametersTypeDef definition

class SelectParametersTypeDef(TypedDict):
    InputSerialization: InputSerializationTypeDef,  # (1)
    ExpressionType: ExpressionTypeType,  # (2)
    Expression: str,
    OutputSerialization: OutputSerializationTypeDef,  # (3)
```

1. See [:material-code-braces: InputSerializationTypeDef](./type_defs.md#inputserializationtypedef) 
2. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
3. See [:material-code-braces: OutputSerializationTypeDef](./type_defs.md#outputserializationtypedef) 
## GetBucketLifecycleOutputTypeDef

```python
# GetBucketLifecycleOutputTypeDef definition

class GetBucketLifecycleOutputTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LifecycleConfigurationTypeDef

```python
# LifecycleConfigurationTypeDef definition

class LifecycleConfigurationTypeDef(TypedDict):
    Rules: Sequence[RuleTypeDef],  # (1)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    Bucket: str,
    Account: NotRequired[str],
    StorageClass: NotRequired[StorageClassType],  # (1)
    AccessControlTranslation: NotRequired[AccessControlTranslationTypeDef],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    ReplicationTime: NotRequired[ReplicationTimeTypeDef],  # (4)
    Metrics: NotRequired[MetricsTypeDef],  # (5)
```

1. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
2. See [:material-code-braces: AccessControlTranslationTypeDef](./type_defs.md#accesscontroltranslationtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: ReplicationTimeTypeDef](./type_defs.md#replicationtimetypedef) 
5. See [:material-code-braces: MetricsTypeDef](./type_defs.md#metricstypedef) 
## PutBucketNotificationRequestRequestTypeDef

```python
# PutBucketNotificationRequestRequestTypeDef definition

class PutBucketNotificationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    NotificationConfiguration: NotificationConfigurationDeprecatedTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: NotificationConfigurationDeprecatedTypeDef](./type_defs.md#notificationconfigurationdeprecatedtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetBucketOwnershipControlsOutputTypeDef

```python
# GetBucketOwnershipControlsOutputTypeDef definition

class GetBucketOwnershipControlsOutputTypeDef(TypedDict):
    OwnershipControls: OwnershipControlsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OwnershipControlsTypeDef](./type_defs.md#ownershipcontrolstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketOwnershipControlsRequestRequestTypeDef

```python
# PutBucketOwnershipControlsRequestRequestTypeDef definition

class PutBucketOwnershipControlsRequestRequestTypeDef(TypedDict):
    Bucket: str,
    OwnershipControls: OwnershipControlsTypeDef,  # (1)
    ContentMD5: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: OwnershipControlsTypeDef](./type_defs.md#ownershipcontrolstypedef) 
## GetBucketWebsiteOutputTypeDef

```python
# GetBucketWebsiteOutputTypeDef definition

class GetBucketWebsiteOutputTypeDef(TypedDict):
    RedirectAllRequestsTo: RedirectAllRequestsToTypeDef,  # (1)
    IndexDocument: IndexDocumentTypeDef,  # (2)
    ErrorDocument: ErrorDocumentTypeDef,  # (3)
    RoutingRules: List[RoutingRuleTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RedirectAllRequestsToTypeDef](./type_defs.md#redirectallrequeststotypedef) 
2. See [:material-code-braces: IndexDocumentTypeDef](./type_defs.md#indexdocumenttypedef) 
3. See [:material-code-braces: ErrorDocumentTypeDef](./type_defs.md#errordocumenttypedef) 
4. See [:material-code-braces: RoutingRuleTypeDef](./type_defs.md#routingruletypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WebsiteConfigurationTypeDef

```python
# WebsiteConfigurationTypeDef definition

class WebsiteConfigurationTypeDef(TypedDict):
    ErrorDocument: NotRequired[ErrorDocumentTypeDef],  # (1)
    IndexDocument: NotRequired[IndexDocumentTypeDef],  # (2)
    RedirectAllRequestsTo: NotRequired[RedirectAllRequestsToTypeDef],  # (3)
    RoutingRules: NotRequired[Sequence[RoutingRuleTypeDef]],  # (4)
```

1. See [:material-code-braces: ErrorDocumentTypeDef](./type_defs.md#errordocumenttypedef) 
2. See [:material-code-braces: IndexDocumentTypeDef](./type_defs.md#indexdocumenttypedef) 
3. See [:material-code-braces: RedirectAllRequestsToTypeDef](./type_defs.md#redirectallrequeststotypedef) 
4. See [:material-code-braces: RoutingRuleTypeDef](./type_defs.md#routingruletypedef) 
## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    Rules: List[ServerSideEncryptionRuleTypeDef],  # (1)
```

1. See [:material-code-braces: ServerSideEncryptionRuleTypeDef](./type_defs.md#serversideencryptionruletypedef) 
## SelectObjectContentEventStreamTypeDef

```python
# SelectObjectContentEventStreamTypeDef definition

class SelectObjectContentEventStreamTypeDef(TypedDict):
    Records: NotRequired[RecordsEventTypeDef],  # (1)
    Stats: NotRequired[StatsEventTypeDef],  # (2)
    Progress: NotRequired[ProgressEventTypeDef],  # (3)
    Cont: NotRequired[Dict[str, Any]],
    End: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: RecordsEventTypeDef](./type_defs.md#recordseventtypedef) 
2. See [:material-code-braces: StatsEventTypeDef](./type_defs.md#statseventtypedef) 
3. See [:material-code-braces: ProgressEventTypeDef](./type_defs.md#progresseventtypedef) 
## ListMultipartUploadsOutputTypeDef

```python
# ListMultipartUploadsOutputTypeDef definition

class ListMultipartUploadsOutputTypeDef(TypedDict):
    Bucket: str,
    KeyMarker: str,
    UploadIdMarker: str,
    NextKeyMarker: str,
    Prefix: str,
    Delimiter: str,
    NextUploadIdMarker: str,
    MaxUploads: int,
    IsTruncated: bool,
    Uploads: List[MultipartUploadTypeDef],  # (1)
    CommonPrefixes: List[CommonPrefixTypeDef],  # (2)
    EncodingType: EncodingTypeType,  # (3)
    RequestCharged: RequestChargedType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: MultipartUploadTypeDef](./type_defs.md#multipartuploadtypedef) 
2. See [:material-code-braces: CommonPrefixTypeDef](./type_defs.md#commonprefixtypedef) 
3. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
4. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectsOutputTypeDef

```python
# ListObjectsOutputTypeDef definition

class ListObjectsOutputTypeDef(TypedDict):
    IsTruncated: bool,
    Marker: str,
    NextMarker: str,
    Contents: List[ObjectTypeDef],  # (1)
    Name: str,
    Prefix: str,
    Delimiter: str,
    MaxKeys: int,
    CommonPrefixes: List[CommonPrefixTypeDef],  # (2)
    EncodingType: EncodingTypeType,  # (3)
    RequestCharged: RequestChargedType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ObjectTypeDef](./type_defs.md#objecttypedef) 
2. See [:material-code-braces: CommonPrefixTypeDef](./type_defs.md#commonprefixtypedef) 
3. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
4. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectsV2OutputTypeDef

```python
# ListObjectsV2OutputTypeDef definition

class ListObjectsV2OutputTypeDef(TypedDict):
    IsTruncated: bool,
    Contents: List[ObjectTypeDef],  # (1)
    Name: str,
    Prefix: str,
    Delimiter: str,
    MaxKeys: int,
    CommonPrefixes: List[CommonPrefixTypeDef],  # (2)
    EncodingType: EncodingTypeType,  # (3)
    KeyCount: int,
    ContinuationToken: str,
    NextContinuationToken: str,
    StartAfter: str,
    RequestCharged: RequestChargedType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ObjectTypeDef](./type_defs.md#objecttypedef) 
2. See [:material-code-braces: CommonPrefixTypeDef](./type_defs.md#commonprefixtypedef) 
3. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
4. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectVersionsOutputTypeDef

```python
# ListObjectVersionsOutputTypeDef definition

class ListObjectVersionsOutputTypeDef(TypedDict):
    IsTruncated: bool,
    KeyMarker: str,
    VersionIdMarker: str,
    NextKeyMarker: str,
    NextVersionIdMarker: str,
    Versions: List[ObjectVersionTypeDef],  # (1)
    DeleteMarkers: List[DeleteMarkerEntryTypeDef],  # (2)
    Name: str,
    Prefix: str,
    Delimiter: str,
    MaxKeys: int,
    CommonPrefixes: List[CommonPrefixTypeDef],  # (3)
    EncodingType: EncodingTypeType,  # (4)
    RequestCharged: RequestChargedType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ObjectVersionTypeDef](./type_defs.md#objectversiontypedef) 
2. See [:material-code-braces: DeleteMarkerEntryTypeDef](./type_defs.md#deletemarkerentrytypedef) 
3. See [:material-code-braces: CommonPrefixTypeDef](./type_defs.md#commonprefixtypedef) 
4. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
5. See [:material-code-brackets: RequestChargedType](./literals.md#requestchargedtype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntelligentTieringConfigurationTypeDef

```python
# IntelligentTieringConfigurationTypeDef definition

class IntelligentTieringConfigurationTypeDef(TypedDict):
    Id: str,
    Status: IntelligentTieringStatusType,  # (2)
    Tierings: List[TieringTypeDef],  # (3)
    Filter: NotRequired[IntelligentTieringFilterTypeDef],  # (1)
```

1. See [:material-code-braces: IntelligentTieringFilterTypeDef](./type_defs.md#intelligenttieringfiltertypedef) 
2. See [:material-code-brackets: IntelligentTieringStatusType](./literals.md#intelligenttieringstatustype) 
3. See [:material-code-braces: TieringTypeDef](./type_defs.md#tieringtypedef) 
## LifecycleRuleBucketLifecycleConfigurationTypeDef

```python
# LifecycleRuleBucketLifecycleConfigurationTypeDef definition

class LifecycleRuleBucketLifecycleConfigurationTypeDef(TypedDict):
    Status: ExpirationStatusType,  # (3)
    Expiration: NotRequired[LifecycleExpirationBucketLifecycleConfigurationTypeDef],  # (1)
    ID: NotRequired[str],
    Prefix: NotRequired[str],
    Filter: NotRequired[LifecycleRuleFilterBucketLifecycleConfigurationTypeDef],  # (2)
    Transitions: NotRequired[Sequence[TransitionBucketLifecycleConfigurationTypeDef]],  # (4)
    NoncurrentVersionTransitions: NotRequired[Sequence[NoncurrentVersionTransitionTypeDef]],  # (5)
    NoncurrentVersionExpiration: NotRequired[NoncurrentVersionExpirationTypeDef],  # (6)
    AbortIncompleteMultipartUpload: NotRequired[AbortIncompleteMultipartUploadTypeDef],  # (7)
```

1. See [:material-code-braces: LifecycleExpirationBucketLifecycleConfigurationTypeDef](./type_defs.md#lifecycleexpirationbucketlifecycleconfigurationtypedef) 
2. See [:material-code-braces: LifecycleRuleFilterBucketLifecycleConfigurationTypeDef](./type_defs.md#lifecyclerulefilterbucketlifecycleconfigurationtypedef) 
3. See [:material-code-brackets: ExpirationStatusType](./literals.md#expirationstatustype) 
4. See [:material-code-braces: TransitionBucketLifecycleConfigurationTypeDef](./type_defs.md#transitionbucketlifecycleconfigurationtypedef) 
5. See [:material-code-braces: NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef) 
6. See [:material-code-braces: NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef) 
7. See [:material-code-braces: AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef) 
## LifecycleRuleTypeDef

```python
# LifecycleRuleTypeDef definition

class LifecycleRuleTypeDef(TypedDict):
    Status: ExpirationStatusType,  # (3)
    Expiration: NotRequired[LifecycleExpirationTypeDef],  # (1)
    ID: NotRequired[str],
    Prefix: NotRequired[str],
    Filter: NotRequired[LifecycleRuleFilterTypeDef],  # (2)
    Transitions: NotRequired[List[TransitionTypeDef]],  # (4)
    NoncurrentVersionTransitions: NotRequired[List[NoncurrentVersionTransitionTypeDef]],  # (5)
    NoncurrentVersionExpiration: NotRequired[NoncurrentVersionExpirationTypeDef],  # (6)
    AbortIncompleteMultipartUpload: NotRequired[AbortIncompleteMultipartUploadTypeDef],  # (7)
```

1. See [:material-code-braces: LifecycleExpirationTypeDef](./type_defs.md#lifecycleexpirationtypedef) 
2. See [:material-code-braces: LifecycleRuleFilterTypeDef](./type_defs.md#lifecyclerulefiltertypedef) 
3. See [:material-code-brackets: ExpirationStatusType](./literals.md#expirationstatustype) 
4. See [:material-code-braces: TransitionTypeDef](./type_defs.md#transitiontypedef) 
5. See [:material-code-braces: NoncurrentVersionTransitionTypeDef](./type_defs.md#noncurrentversiontransitiontypedef) 
6. See [:material-code-braces: NoncurrentVersionExpirationTypeDef](./type_defs.md#noncurrentversionexpirationtypedef) 
7. See [:material-code-braces: AbortIncompleteMultipartUploadTypeDef](./type_defs.md#abortincompletemultipartuploadtypedef) 
## MetricsConfigurationTypeDef

```python
# MetricsConfigurationTypeDef definition

class MetricsConfigurationTypeDef(TypedDict):
    Id: str,
    Filter: NotRequired[MetricsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsFilterTypeDef](./type_defs.md#metricsfiltertypedef) 
## StorageClassAnalysisTypeDef

```python
# StorageClassAnalysisTypeDef definition

class StorageClassAnalysisTypeDef(TypedDict):
    DataExport: NotRequired[StorageClassAnalysisDataExportTypeDef],  # (1)
```

1. See [:material-code-braces: StorageClassAnalysisDataExportTypeDef](./type_defs.md#storageclassanalysisdataexporttypedef) 
## LifecycleConfigurationBucketLifecycleTypeDef

```python
# LifecycleConfigurationBucketLifecycleTypeDef definition

class LifecycleConfigurationBucketLifecycleTypeDef(TypedDict):
    Rules: Sequence[RuleBucketLifecycleTypeDef],  # (1)
```

1. See [:material-code-braces: RuleBucketLifecycleTypeDef](./type_defs.md#rulebucketlifecycletypedef) 
## GetObjectLockConfigurationOutputTypeDef

```python
# GetObjectLockConfigurationOutputTypeDef definition

class GetObjectLockConfigurationOutputTypeDef(TypedDict):
    ObjectLockConfiguration: ObjectLockConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ObjectLockConfigurationTypeDef](./type_defs.md#objectlockconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectLockConfigurationRequestRequestTypeDef

```python
# PutObjectLockConfigurationRequestRequestTypeDef definition

class PutObjectLockConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ObjectLockConfiguration: NotRequired[ObjectLockConfigurationTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    Token: NotRequired[str],
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: ObjectLockConfigurationTypeDef](./type_defs.md#objectlockconfigurationtypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## LambdaFunctionConfigurationBucketNotificationTypeDef

```python
# LambdaFunctionConfigurationBucketNotificationTypeDef definition

class LambdaFunctionConfigurationBucketNotificationTypeDef(TypedDict):
    LambdaFunctionArn: str,
    Events: Sequence[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterBucketNotificationTypeDef](./type_defs.md#notificationconfigurationfilterbucketnotificationtypedef) 
## QueueConfigurationBucketNotificationTypeDef

```python
# QueueConfigurationBucketNotificationTypeDef definition

class QueueConfigurationBucketNotificationTypeDef(TypedDict):
    QueueArn: str,
    Events: Sequence[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterBucketNotificationTypeDef](./type_defs.md#notificationconfigurationfilterbucketnotificationtypedef) 
## TopicConfigurationBucketNotificationTypeDef

```python
# TopicConfigurationBucketNotificationTypeDef definition

class TopicConfigurationBucketNotificationTypeDef(TypedDict):
    TopicArn: str,
    Events: Sequence[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterBucketNotificationTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterBucketNotificationTypeDef](./type_defs.md#notificationconfigurationfilterbucketnotificationtypedef) 
## LambdaFunctionConfigurationTypeDef

```python
# LambdaFunctionConfigurationTypeDef definition

class LambdaFunctionConfigurationTypeDef(TypedDict):
    LambdaFunctionArn: str,
    Events: List[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterTypeDef](./type_defs.md#notificationconfigurationfiltertypedef) 
## QueueConfigurationTypeDef

```python
# QueueConfigurationTypeDef definition

class QueueConfigurationTypeDef(TypedDict):
    QueueArn: str,
    Events: List[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterTypeDef](./type_defs.md#notificationconfigurationfiltertypedef) 
## TopicConfigurationTypeDef

```python
# TopicConfigurationTypeDef definition

class TopicConfigurationTypeDef(TypedDict):
    TopicArn: str,
    Events: List[EventType],  # (1)
    Id: NotRequired[str],
    Filter: NotRequired[NotificationConfigurationFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: EventType](./literals.md#eventtype) 
2. See [:material-code-braces: NotificationConfigurationFilterTypeDef](./type_defs.md#notificationconfigurationfiltertypedef) 
## PutBucketAclRequestBucketAclPutTypeDef

```python
# PutBucketAclRequestBucketAclPutTypeDef definition

class PutBucketAclRequestBucketAclPutTypeDef(TypedDict):
    ACL: NotRequired[BucketCannedACLType],  # (1)
    AccessControlPolicy: NotRequired[AccessControlPolicyTypeDef],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketAclRequestRequestTypeDef

```python
# PutBucketAclRequestRequestTypeDef definition

class PutBucketAclRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ACL: NotRequired[BucketCannedACLType],  # (1)
    AccessControlPolicy: NotRequired[AccessControlPolicyTypeDef],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: BucketCannedACLType](./literals.md#bucketcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutObjectAclRequestObjectAclPutTypeDef

```python
# PutObjectAclRequestObjectAclPutTypeDef definition

class PutObjectAclRequestObjectAclPutTypeDef(TypedDict):
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    AccessControlPolicy: NotRequired[AccessControlPolicyTypeDef],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (4)
    VersionId: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## PutObjectAclRequestRequestTypeDef

```python
# PutObjectAclRequestRequestTypeDef definition

class PutObjectAclRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    ACL: NotRequired[ObjectCannedACLType],  # (1)
    AccessControlPolicy: NotRequired[AccessControlPolicyTypeDef],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    GrantFullControl: NotRequired[str],
    GrantRead: NotRequired[str],
    GrantReadACP: NotRequired[str],
    GrantWrite: NotRequired[str],
    GrantWriteACP: NotRequired[str],
    RequestPayer: NotRequired[RequestPayerType],  # (4)
    VersionId: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ObjectCannedACLType](./literals.md#objectcannedacltype) 
2. See [:material-code-braces: AccessControlPolicyTypeDef](./type_defs.md#accesscontrolpolicytypedef) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
4. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
## OutputLocationTypeDef

```python
# OutputLocationTypeDef definition

class OutputLocationTypeDef(TypedDict):
    S3: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## BucketLoggingStatusBucketLoggingTypeDef

```python
# BucketLoggingStatusBucketLoggingTypeDef definition

class BucketLoggingStatusBucketLoggingTypeDef(TypedDict):
    LoggingEnabled: NotRequired[LoggingEnabledBucketLoggingTypeDef],  # (1)
```

1. See [:material-code-braces: LoggingEnabledBucketLoggingTypeDef](./type_defs.md#loggingenabledbucketloggingtypedef) 
## BucketLoggingStatusTypeDef

```python
# BucketLoggingStatusTypeDef definition

class BucketLoggingStatusTypeDef(TypedDict):
    LoggingEnabled: NotRequired[LoggingEnabledTypeDef],  # (1)
```

1. See [:material-code-braces: LoggingEnabledTypeDef](./type_defs.md#loggingenabledtypedef) 
## GetBucketLoggingOutputTypeDef

```python
# GetBucketLoggingOutputTypeDef definition

class GetBucketLoggingOutputTypeDef(TypedDict):
    LoggingEnabled: LoggingEnabledTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingEnabledTypeDef](./type_defs.md#loggingenabledtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InventoryDestinationTypeDef

```python
# InventoryDestinationTypeDef definition

class InventoryDestinationTypeDef(TypedDict):
    S3BucketDestination: InventoryS3BucketDestinationTypeDef,  # (1)
```

1. See [:material-code-braces: InventoryS3BucketDestinationTypeDef](./type_defs.md#inventorys3bucketdestinationtypedef) 
## PutBucketLifecycleRequestRequestTypeDef

```python
# PutBucketLifecycleRequestRequestTypeDef definition

class PutBucketLifecycleRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    LifecycleConfiguration: NotRequired[LifecycleConfigurationTypeDef],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef) 
## ReplicationRuleTypeDef

```python
# ReplicationRuleTypeDef definition

class ReplicationRuleTypeDef(TypedDict):
    Status: ReplicationRuleStatusType,  # (2)
    Destination: DestinationTypeDef,  # (5)
    ID: NotRequired[str],
    Priority: NotRequired[int],
    Prefix: NotRequired[str],
    Filter: NotRequired[ReplicationRuleFilterTypeDef],  # (1)
    SourceSelectionCriteria: NotRequired[SourceSelectionCriteriaTypeDef],  # (3)
    ExistingObjectReplication: NotRequired[ExistingObjectReplicationTypeDef],  # (4)
    DeleteMarkerReplication: NotRequired[DeleteMarkerReplicationTypeDef],  # (6)
```

1. See [:material-code-braces: ReplicationRuleFilterTypeDef](./type_defs.md#replicationrulefiltertypedef) 
2. See [:material-code-brackets: ReplicationRuleStatusType](./literals.md#replicationrulestatustype) 
3. See [:material-code-braces: SourceSelectionCriteriaTypeDef](./type_defs.md#sourceselectioncriteriatypedef) 
4. See [:material-code-braces: ExistingObjectReplicationTypeDef](./type_defs.md#existingobjectreplicationtypedef) 
5. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
6. See [:material-code-braces: DeleteMarkerReplicationTypeDef](./type_defs.md#deletemarkerreplicationtypedef) 
## PutBucketWebsiteRequestBucketWebsitePutTypeDef

```python
# PutBucketWebsiteRequestBucketWebsitePutTypeDef definition

class PutBucketWebsiteRequestBucketWebsitePutTypeDef(TypedDict):
    WebsiteConfiguration: WebsiteConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: WebsiteConfigurationTypeDef](./type_defs.md#websiteconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketWebsiteRequestRequestTypeDef

```python
# PutBucketWebsiteRequestRequestTypeDef definition

class PutBucketWebsiteRequestRequestTypeDef(TypedDict):
    Bucket: str,
    WebsiteConfiguration: WebsiteConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: WebsiteConfigurationTypeDef](./type_defs.md#websiteconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetBucketEncryptionOutputTypeDef

```python
# GetBucketEncryptionOutputTypeDef definition

class GetBucketEncryptionOutputTypeDef(TypedDict):
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketEncryptionRequestRequestTypeDef

```python
# PutBucketEncryptionRequestRequestTypeDef definition

class PutBucketEncryptionRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (1)
    ContentMD5: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## SelectObjectContentOutputTypeDef

```python
# SelectObjectContentOutputTypeDef definition

class SelectObjectContentOutputTypeDef(TypedDict):
    Payload: AioEventStream[SelectObjectContentEventStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SelectObjectContentEventStreamTypeDef](./type_defs.md#selectobjectcontenteventstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketIntelligentTieringConfigurationOutputTypeDef

```python
# GetBucketIntelligentTieringConfigurationOutputTypeDef definition

class GetBucketIntelligentTieringConfigurationOutputTypeDef(TypedDict):
    IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntelligentTieringConfigurationTypeDef](./type_defs.md#intelligenttieringconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBucketIntelligentTieringConfigurationsOutputTypeDef

```python
# ListBucketIntelligentTieringConfigurationsOutputTypeDef definition

class ListBucketIntelligentTieringConfigurationsOutputTypeDef(TypedDict):
    IsTruncated: bool,
    ContinuationToken: str,
    NextContinuationToken: str,
    IntelligentTieringConfigurationList: List[IntelligentTieringConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntelligentTieringConfigurationTypeDef](./type_defs.md#intelligenttieringconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketIntelligentTieringConfigurationRequestRequestTypeDef

```python
# PutBucketIntelligentTieringConfigurationRequestRequestTypeDef definition

class PutBucketIntelligentTieringConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: IntelligentTieringConfigurationTypeDef](./type_defs.md#intelligenttieringconfigurationtypedef) 
## BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef

```python
# BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef definition

class BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef(TypedDict):
    Rules: Sequence[LifecycleRuleBucketLifecycleConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LifecycleRuleBucketLifecycleConfigurationTypeDef](./type_defs.md#lifecyclerulebucketlifecycleconfigurationtypedef) 
## BucketLifecycleConfigurationTypeDef

```python
# BucketLifecycleConfigurationTypeDef definition

class BucketLifecycleConfigurationTypeDef(TypedDict):
    Rules: Sequence[LifecycleRuleTypeDef],  # (1)
```

1. See [:material-code-braces: LifecycleRuleTypeDef](./type_defs.md#lifecycleruletypedef) 
## GetBucketLifecycleConfigurationOutputTypeDef

```python
# GetBucketLifecycleConfigurationOutputTypeDef definition

class GetBucketLifecycleConfigurationOutputTypeDef(TypedDict):
    Rules: List[LifecycleRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecycleRuleTypeDef](./type_defs.md#lifecycleruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketMetricsConfigurationOutputTypeDef

```python
# GetBucketMetricsConfigurationOutputTypeDef definition

class GetBucketMetricsConfigurationOutputTypeDef(TypedDict):
    MetricsConfiguration: MetricsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBucketMetricsConfigurationsOutputTypeDef

```python
# ListBucketMetricsConfigurationsOutputTypeDef definition

class ListBucketMetricsConfigurationsOutputTypeDef(TypedDict):
    IsTruncated: bool,
    ContinuationToken: str,
    NextContinuationToken: str,
    MetricsConfigurationList: List[MetricsConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketMetricsConfigurationRequestRequestTypeDef

```python
# PutBucketMetricsConfigurationRequestRequestTypeDef definition

class PutBucketMetricsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    MetricsConfiguration: MetricsConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: MetricsConfigurationTypeDef](./type_defs.md#metricsconfigurationtypedef) 
## AnalyticsConfigurationTypeDef

```python
# AnalyticsConfigurationTypeDef definition

class AnalyticsConfigurationTypeDef(TypedDict):
    Id: str,
    StorageClassAnalysis: StorageClassAnalysisTypeDef,  # (2)
    Filter: NotRequired[AnalyticsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: AnalyticsFilterTypeDef](./type_defs.md#analyticsfiltertypedef) 
2. See [:material-code-braces: StorageClassAnalysisTypeDef](./type_defs.md#storageclassanalysistypedef) 
## PutBucketLifecycleRequestBucketLifecyclePutTypeDef

```python
# PutBucketLifecycleRequestBucketLifecyclePutTypeDef definition

class PutBucketLifecycleRequestBucketLifecyclePutTypeDef(TypedDict):
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    LifecycleConfiguration: NotRequired[LifecycleConfigurationBucketLifecycleTypeDef],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: LifecycleConfigurationBucketLifecycleTypeDef](./type_defs.md#lifecycleconfigurationbucketlifecycletypedef) 
## NotificationConfigurationBucketNotificationTypeDef

```python
# NotificationConfigurationBucketNotificationTypeDef definition

class NotificationConfigurationBucketNotificationTypeDef(TypedDict):
    TopicConfigurations: NotRequired[Sequence[TopicConfigurationBucketNotificationTypeDef]],  # (1)
    QueueConfigurations: NotRequired[Sequence[QueueConfigurationBucketNotificationTypeDef]],  # (2)
    LambdaFunctionConfigurations: NotRequired[Sequence[LambdaFunctionConfigurationBucketNotificationTypeDef]],  # (3)
    EventBridgeConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: TopicConfigurationBucketNotificationTypeDef](./type_defs.md#topicconfigurationbucketnotificationtypedef) 
2. See [:material-code-braces: QueueConfigurationBucketNotificationTypeDef](./type_defs.md#queueconfigurationbucketnotificationtypedef) 
3. See [:material-code-braces: LambdaFunctionConfigurationBucketNotificationTypeDef](./type_defs.md#lambdafunctionconfigurationbucketnotificationtypedef) 
## NotificationConfigurationResponseTypeDef

```python
# NotificationConfigurationResponseTypeDef definition

class NotificationConfigurationResponseTypeDef(TypedDict):
    TopicConfigurations: List[TopicConfigurationTypeDef],  # (1)
    QueueConfigurations: List[QueueConfigurationTypeDef],  # (2)
    LambdaFunctionConfigurations: List[LambdaFunctionConfigurationTypeDef],  # (3)
    EventBridgeConfiguration: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
2. See [:material-code-braces: QueueConfigurationTypeDef](./type_defs.md#queueconfigurationtypedef) 
3. See [:material-code-braces: LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    TopicConfigurations: NotRequired[Sequence[TopicConfigurationTypeDef]],  # (1)
    QueueConfigurations: NotRequired[Sequence[QueueConfigurationTypeDef]],  # (2)
    LambdaFunctionConfigurations: NotRequired[Sequence[LambdaFunctionConfigurationTypeDef]],  # (3)
    EventBridgeConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
2. See [:material-code-braces: QueueConfigurationTypeDef](./type_defs.md#queueconfigurationtypedef) 
3. See [:material-code-braces: LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef) 
## RestoreRequestTypeDef

```python
# RestoreRequestTypeDef definition

class RestoreRequestTypeDef(TypedDict):
    Days: NotRequired[int],
    GlacierJobParameters: NotRequired[GlacierJobParametersTypeDef],  # (1)
    Type: NotRequired[RestoreRequestTypeType],  # (2)
    Tier: NotRequired[TierType],  # (3)
    Description: NotRequired[str],
    SelectParameters: NotRequired[SelectParametersTypeDef],  # (4)
    OutputLocation: NotRequired[OutputLocationTypeDef],  # (5)
```

1. See [:material-code-braces: GlacierJobParametersTypeDef](./type_defs.md#glacierjobparameterstypedef) 
2. See [:material-code-brackets: RestoreRequestTypeType](./literals.md#restorerequesttypetype) 
3. See [:material-code-brackets: TierType](./literals.md#tiertype) 
4. See [:material-code-braces: SelectParametersTypeDef](./type_defs.md#selectparameterstypedef) 
5. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
## PutBucketLoggingRequestBucketLoggingPutTypeDef

```python
# PutBucketLoggingRequestBucketLoggingPutTypeDef definition

class PutBucketLoggingRequestBucketLoggingPutTypeDef(TypedDict):
    BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: BucketLoggingStatusBucketLoggingTypeDef](./type_defs.md#bucketloggingstatusbucketloggingtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## PutBucketLoggingRequestRequestTypeDef

```python
# PutBucketLoggingRequestRequestTypeDef definition

class PutBucketLoggingRequestRequestTypeDef(TypedDict):
    Bucket: str,
    BucketLoggingStatus: BucketLoggingStatusTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: BucketLoggingStatusTypeDef](./type_defs.md#bucketloggingstatustypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## InventoryConfigurationTypeDef

```python
# InventoryConfigurationTypeDef definition

class InventoryConfigurationTypeDef(TypedDict):
    Destination: InventoryDestinationTypeDef,  # (1)
    IsEnabled: bool,
    Id: str,
    IncludedObjectVersions: InventoryIncludedObjectVersionsType,  # (3)
    Schedule: InventoryScheduleTypeDef,  # (5)
    Filter: NotRequired[InventoryFilterTypeDef],  # (2)
    OptionalFields: NotRequired[List[InventoryOptionalFieldType]],  # (4)
```

1. See [:material-code-braces: InventoryDestinationTypeDef](./type_defs.md#inventorydestinationtypedef) 
2. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
3. See [:material-code-brackets: InventoryIncludedObjectVersionsType](./literals.md#inventoryincludedobjectversionstype) 
4. See [:material-code-brackets: InventoryOptionalFieldType](./literals.md#inventoryoptionalfieldtype) 
5. See [:material-code-braces: InventoryScheduleTypeDef](./type_defs.md#inventoryscheduletypedef) 
## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    Role: str,
    Rules: List[ReplicationRuleTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef) 
## PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef

```python
# PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef definition

class PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef(TypedDict):
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    LifecycleConfiguration: NotRequired[BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef](./type_defs.md#bucketlifecycleconfigurationbucketlifecycleconfigurationtypedef) 
## PutBucketLifecycleConfigurationRequestRequestTypeDef

```python
# PutBucketLifecycleConfigurationRequestRequestTypeDef definition

class PutBucketLifecycleConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    LifecycleConfiguration: NotRequired[BucketLifecycleConfigurationTypeDef],  # (2)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: BucketLifecycleConfigurationTypeDef](./type_defs.md#bucketlifecycleconfigurationtypedef) 
## GetBucketAnalyticsConfigurationOutputTypeDef

```python
# GetBucketAnalyticsConfigurationOutputTypeDef definition

class GetBucketAnalyticsConfigurationOutputTypeDef(TypedDict):
    AnalyticsConfiguration: AnalyticsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsConfigurationTypeDef](./type_defs.md#analyticsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBucketAnalyticsConfigurationsOutputTypeDef

```python
# ListBucketAnalyticsConfigurationsOutputTypeDef definition

class ListBucketAnalyticsConfigurationsOutputTypeDef(TypedDict):
    IsTruncated: bool,
    ContinuationToken: str,
    NextContinuationToken: str,
    AnalyticsConfigurationList: List[AnalyticsConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsConfigurationTypeDef](./type_defs.md#analyticsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketAnalyticsConfigurationRequestRequestTypeDef

```python
# PutBucketAnalyticsConfigurationRequestRequestTypeDef definition

class PutBucketAnalyticsConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    AnalyticsConfiguration: AnalyticsConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: AnalyticsConfigurationTypeDef](./type_defs.md#analyticsconfigurationtypedef) 
## PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef

```python
# PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef definition

class PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef(TypedDict):
    NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
    SkipDestinationValidation: NotRequired[bool],
```

1. See [:material-code-braces: NotificationConfigurationBucketNotificationTypeDef](./type_defs.md#notificationconfigurationbucketnotificationtypedef) 
## PutBucketNotificationConfigurationRequestRequestTypeDef

```python
# PutBucketNotificationConfigurationRequestRequestTypeDef definition

class PutBucketNotificationConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    NotificationConfiguration: NotificationConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
    SkipDestinationValidation: NotRequired[bool],
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
## RestoreObjectRequestObjectRestoreObjectTypeDef

```python
# RestoreObjectRequestObjectRestoreObjectTypeDef definition

class RestoreObjectRequestObjectRestoreObjectTypeDef(TypedDict):
    VersionId: NotRequired[str],
    RestoreRequest: NotRequired[RestoreRequestTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## RestoreObjectRequestObjectSummaryRestoreObjectTypeDef

```python
# RestoreObjectRequestObjectSummaryRestoreObjectTypeDef definition

class RestoreObjectRequestObjectSummaryRestoreObjectTypeDef(TypedDict):
    VersionId: NotRequired[str],
    RestoreRequest: NotRequired[RestoreRequestTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## RestoreObjectRequestRequestTypeDef

```python
# RestoreObjectRequestRequestTypeDef definition

class RestoreObjectRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
    RestoreRequest: NotRequired[RestoreRequestTypeDef],  # (1)
    RequestPayer: NotRequired[RequestPayerType],  # (2)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (3)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: RestoreRequestTypeDef](./type_defs.md#restorerequesttypedef) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## GetBucketInventoryConfigurationOutputTypeDef

```python
# GetBucketInventoryConfigurationOutputTypeDef definition

class GetBucketInventoryConfigurationOutputTypeDef(TypedDict):
    InventoryConfiguration: InventoryConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InventoryConfigurationTypeDef](./type_defs.md#inventoryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBucketInventoryConfigurationsOutputTypeDef

```python
# ListBucketInventoryConfigurationsOutputTypeDef definition

class ListBucketInventoryConfigurationsOutputTypeDef(TypedDict):
    ContinuationToken: str,
    InventoryConfigurationList: List[InventoryConfigurationTypeDef],  # (1)
    IsTruncated: bool,
    NextContinuationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InventoryConfigurationTypeDef](./type_defs.md#inventoryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketInventoryConfigurationRequestRequestTypeDef

```python
# PutBucketInventoryConfigurationRequestRequestTypeDef definition

class PutBucketInventoryConfigurationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    Id: str,
    InventoryConfiguration: InventoryConfigurationTypeDef,  # (1)
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: InventoryConfigurationTypeDef](./type_defs.md#inventoryconfigurationtypedef) 
## GetBucketReplicationOutputTypeDef

```python
# GetBucketReplicationOutputTypeDef definition

class GetBucketReplicationOutputTypeDef(TypedDict):
    ReplicationConfiguration: ReplicationConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBucketReplicationRequestRequestTypeDef

```python
# PutBucketReplicationRequestRequestTypeDef definition

class PutBucketReplicationRequestRequestTypeDef(TypedDict):
    Bucket: str,
    ReplicationConfiguration: ReplicationConfigurationTypeDef,  # (1)
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (2)
    Token: NotRequired[str],
    ExpectedBucketOwner: NotRequired[str],
```

1. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 
2. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
