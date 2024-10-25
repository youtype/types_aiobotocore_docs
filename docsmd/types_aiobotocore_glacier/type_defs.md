# Type definitions

> [Index](../README.md) > [Glacier](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

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


## S3LocationUnionTypeDef

```python
# S3LocationUnionTypeDef definition

S3LocationUnionTypeDef = Union[
    S3LocationTypeDef,  # (1)
    S3LocationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: S3LocationOutputTypeDef](./type_defs.md#s3locationoutputtypedef) 

## OutputLocationUnionTypeDef

```python
# OutputLocationUnionTypeDef definition

OutputLocationUnionTypeDef = Union[
    OutputLocationTypeDef,  # (1)
    OutputLocationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef) 



## AbortMultipartUploadInputRequestTypeDef

```python
# AbortMultipartUploadInputRequestTypeDef definition

class AbortMultipartUploadInputRequestTypeDef(TypedDict):
    vaultName: str,
    uploadId: str,
    accountId: NotRequired[str],
```

## AbortVaultLockInputRequestTypeDef

```python
# AbortVaultLockInputRequestTypeDef definition

class AbortVaultLockInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## AddTagsToVaultInputRequestTypeDef

```python
# AddTagsToVaultInputRequestTypeDef definition

class AddTagsToVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
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
## CompleteMultipartUploadInputMultipartUploadCompleteTypeDef

```python
# CompleteMultipartUploadInputMultipartUploadCompleteTypeDef definition

class CompleteMultipartUploadInputMultipartUploadCompleteTypeDef(TypedDict):
    archiveSize: NotRequired[str],
    checksum: NotRequired[str],
```

## CompleteMultipartUploadInputRequestTypeDef

```python
# CompleteMultipartUploadInputRequestTypeDef definition

class CompleteMultipartUploadInputRequestTypeDef(TypedDict):
    vaultName: str,
    uploadId: str,
    accountId: NotRequired[str],
    archiveSize: NotRequired[str],
    checksum: NotRequired[str],
```

## CompleteVaultLockInputRequestTypeDef

```python
# CompleteVaultLockInputRequestTypeDef definition

class CompleteVaultLockInputRequestTypeDef(TypedDict):
    vaultName: str,
    lockId: str,
    accountId: NotRequired[str],
```

## CreateVaultInputAccountCreateVaultTypeDef

```python
# CreateVaultInputAccountCreateVaultTypeDef definition

class CreateVaultInputAccountCreateVaultTypeDef(TypedDict):
    vaultName: str,
```

## CreateVaultInputRequestTypeDef

```python
# CreateVaultInputRequestTypeDef definition

class CreateVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## CreateVaultInputServiceResourceCreateVaultTypeDef

```python
# CreateVaultInputServiceResourceCreateVaultTypeDef definition

class CreateVaultInputServiceResourceCreateVaultTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## DataRetrievalRuleTypeDef

```python
# DataRetrievalRuleTypeDef definition

class DataRetrievalRuleTypeDef(TypedDict):
    Strategy: NotRequired[str],
    BytesPerHour: NotRequired[int],
```

## DeleteArchiveInputRequestTypeDef

```python
# DeleteArchiveInputRequestTypeDef definition

class DeleteArchiveInputRequestTypeDef(TypedDict):
    vaultName: str,
    archiveId: str,
    accountId: NotRequired[str],
```

## DeleteVaultAccessPolicyInputRequestTypeDef

```python
# DeleteVaultAccessPolicyInputRequestTypeDef definition

class DeleteVaultAccessPolicyInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## DeleteVaultInputRequestTypeDef

```python
# DeleteVaultInputRequestTypeDef definition

class DeleteVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## DeleteVaultNotificationsInputRequestTypeDef

```python
# DeleteVaultNotificationsInputRequestTypeDef definition

class DeleteVaultNotificationsInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## DescribeJobInputRequestTypeDef

```python
# DescribeJobInputRequestTypeDef definition

class DescribeJobInputRequestTypeDef(TypedDict):
    vaultName: str,
    jobId: str,
    accountId: NotRequired[str],
```

## DescribeVaultInputRequestTypeDef

```python
# DescribeVaultInputRequestTypeDef definition

class DescribeVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeVaultOutputTypeDef

```python
# DescribeVaultOutputTypeDef definition

class DescribeVaultOutputTypeDef(TypedDict):
    VaultARN: NotRequired[str],
    VaultName: NotRequired[str],
    CreationDate: NotRequired[str],
    LastInventoryDate: NotRequired[str],
    NumberOfArchives: NotRequired[int],
    SizeInBytes: NotRequired[int],
```

## EncryptionTypeDef

```python
# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    EncryptionType: NotRequired[EncryptionTypeType],  # (1)
    KMSKeyId: NotRequired[str],
    KMSContext: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## GetDataRetrievalPolicyInputRequestTypeDef

```python
# GetDataRetrievalPolicyInputRequestTypeDef definition

class GetDataRetrievalPolicyInputRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## GetJobOutputInputJobGetOutputTypeDef

```python
# GetJobOutputInputJobGetOutputTypeDef definition

class GetJobOutputInputJobGetOutputTypeDef(TypedDict):
    range: NotRequired[str],
```

## GetJobOutputInputRequestTypeDef

```python
# GetJobOutputInputRequestTypeDef definition

class GetJobOutputInputRequestTypeDef(TypedDict):
    vaultName: str,
    jobId: str,
    accountId: NotRequired[str],
    range: NotRequired[str],
```

## GetVaultAccessPolicyInputRequestTypeDef

```python
# GetVaultAccessPolicyInputRequestTypeDef definition

class GetVaultAccessPolicyInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## VaultAccessPolicyTypeDef

```python
# VaultAccessPolicyTypeDef definition

class VaultAccessPolicyTypeDef(TypedDict):
    Policy: NotRequired[str],
```

## GetVaultLockInputRequestTypeDef

```python
# GetVaultLockInputRequestTypeDef definition

class GetVaultLockInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## GetVaultNotificationsInputRequestTypeDef

```python
# GetVaultNotificationsInputRequestTypeDef definition

class GetVaultNotificationsInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## VaultNotificationConfigOutputTypeDef

```python
# VaultNotificationConfigOutputTypeDef definition

class VaultNotificationConfigOutputTypeDef(TypedDict):
    SNSTopic: NotRequired[str],
    Events: NotRequired[List[str]],
```

## InventoryRetrievalJobDescriptionTypeDef

```python
# InventoryRetrievalJobDescriptionTypeDef definition

class InventoryRetrievalJobDescriptionTypeDef(TypedDict):
    Format: NotRequired[str],
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    Limit: NotRequired[str],
    Marker: NotRequired[str],
```

## GranteeTypeDef

```python
# GranteeTypeDef definition

class GranteeTypeDef(TypedDict):
    Type: TypeType,  # (1)
    DisplayName: NotRequired[str],
    URI: NotRequired[str],
    ID: NotRequired[str],
    EmailAddress: NotRequired[str],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## InitiateMultipartUploadInputRequestTypeDef

```python
# InitiateMultipartUploadInputRequestTypeDef definition

class InitiateMultipartUploadInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    archiveDescription: NotRequired[str],
    partSize: NotRequired[str],
```

## InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef

```python
# InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef definition

class InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef(TypedDict):
    archiveDescription: NotRequired[str],
    partSize: NotRequired[str],
```

## VaultLockPolicyTypeDef

```python
# VaultLockPolicyTypeDef definition

class VaultLockPolicyTypeDef(TypedDict):
    Policy: NotRequired[str],
```

## InventoryRetrievalJobInputTypeDef

```python
# InventoryRetrievalJobInputTypeDef definition

class InventoryRetrievalJobInputTypeDef(TypedDict):
    StartDate: NotRequired[str],
    EndDate: NotRequired[str],
    Limit: NotRequired[str],
    Marker: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListJobsInputRequestTypeDef

```python
# ListJobsInputRequestTypeDef definition

class ListJobsInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    limit: NotRequired[str],
    marker: NotRequired[str],
    statuscode: NotRequired[str],
    completed: NotRequired[str],
```

## ListMultipartUploadsInputRequestTypeDef

```python
# ListMultipartUploadsInputRequestTypeDef definition

class ListMultipartUploadsInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    marker: NotRequired[str],
    limit: NotRequired[str],
```

## UploadListElementTypeDef

```python
# UploadListElementTypeDef definition

class UploadListElementTypeDef(TypedDict):
    MultipartUploadId: NotRequired[str],
    VaultARN: NotRequired[str],
    ArchiveDescription: NotRequired[str],
    PartSizeInBytes: NotRequired[int],
    CreationDate: NotRequired[str],
```

## ListPartsInputMultipartUploadPartsTypeDef

```python
# ListPartsInputMultipartUploadPartsTypeDef definition

class ListPartsInputMultipartUploadPartsTypeDef(TypedDict):
    marker: NotRequired[str],
    limit: NotRequired[str],
```

## ListPartsInputRequestTypeDef

```python
# ListPartsInputRequestTypeDef definition

class ListPartsInputRequestTypeDef(TypedDict):
    vaultName: str,
    uploadId: str,
    accountId: NotRequired[str],
    marker: NotRequired[str],
    limit: NotRequired[str],
```

## PartListElementTypeDef

```python
# PartListElementTypeDef definition

class PartListElementTypeDef(TypedDict):
    RangeInBytes: NotRequired[str],
    SHA256TreeHash: NotRequired[str],
```

## ListProvisionedCapacityInputRequestTypeDef

```python
# ListProvisionedCapacityInputRequestTypeDef definition

class ListProvisionedCapacityInputRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## ProvisionedCapacityDescriptionTypeDef

```python
# ProvisionedCapacityDescriptionTypeDef definition

class ProvisionedCapacityDescriptionTypeDef(TypedDict):
    CapacityId: NotRequired[str],
    StartDate: NotRequired[str],
    ExpirationDate: NotRequired[str],
```

## ListTagsForVaultInputRequestTypeDef

```python
# ListTagsForVaultInputRequestTypeDef definition

class ListTagsForVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
```

## ListVaultsInputRequestTypeDef

```python
# ListVaultsInputRequestTypeDef definition

class ListVaultsInputRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
    marker: NotRequired[str],
    limit: NotRequired[str],
```

## PurchaseProvisionedCapacityInputRequestTypeDef

```python
# PurchaseProvisionedCapacityInputRequestTypeDef definition

class PurchaseProvisionedCapacityInputRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## RemoveTagsFromVaultInputRequestTypeDef

```python
# RemoveTagsFromVaultInputRequestTypeDef definition

class RemoveTagsFromVaultInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
```

## VaultNotificationConfigTypeDef

```python
# VaultNotificationConfigTypeDef definition

class VaultNotificationConfigTypeDef(TypedDict):
    SNSTopic: NotRequired[str],
    Events: NotRequired[Sequence[str]],
```

## ArchiveCreationOutputTypeDef

```python
# ArchiveCreationOutputTypeDef definition

class ArchiveCreationOutputTypeDef(TypedDict):
    location: str,
    checksum: str,
    archiveId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVaultOutputTypeDef

```python
# CreateVaultOutputTypeDef definition

class CreateVaultOutputTypeDef(TypedDict):
    location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVaultResponseTypeDef

```python
# DescribeVaultResponseTypeDef definition

class DescribeVaultResponseTypeDef(TypedDict):
    VaultARN: str,
    VaultName: str,
    CreationDate: str,
    LastInventoryDate: str,
    NumberOfArchives: int,
    SizeInBytes: int,
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
## GetJobOutputOutputTypeDef

```python
# GetJobOutputOutputTypeDef definition

class GetJobOutputOutputTypeDef(TypedDict):
    body: StreamingBody,
    checksum: str,
    status: int,
    contentRange: str,
    acceptRanges: str,
    contentType: str,
    archiveDescription: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVaultLockOutputTypeDef

```python
# GetVaultLockOutputTypeDef definition

class GetVaultLockOutputTypeDef(TypedDict):
    Policy: str,
    State: str,
    ExpirationDate: str,
    CreationDate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateJobOutputTypeDef

```python
# InitiateJobOutputTypeDef definition

class InitiateJobOutputTypeDef(TypedDict):
    location: str,
    jobId: str,
    jobOutputPath: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateMultipartUploadOutputTypeDef

```python
# InitiateMultipartUploadOutputTypeDef definition

class InitiateMultipartUploadOutputTypeDef(TypedDict):
    location: str,
    uploadId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateVaultLockOutputTypeDef

```python
# InitiateVaultLockOutputTypeDef definition

class InitiateVaultLockOutputTypeDef(TypedDict):
    lockId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForVaultOutputTypeDef

```python
# ListTagsForVaultOutputTypeDef definition

class ListTagsForVaultOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseProvisionedCapacityOutputTypeDef

```python
# PurchaseProvisionedCapacityOutputTypeDef definition

class PurchaseProvisionedCapacityOutputTypeDef(TypedDict):
    capacityId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadMultipartPartOutputTypeDef

```python
# UploadMultipartPartOutputTypeDef definition

class UploadMultipartPartOutputTypeDef(TypedDict):
    checksum: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadArchiveInputRequestTypeDef

```python
# UploadArchiveInputRequestTypeDef definition

class UploadArchiveInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    archiveDescription: NotRequired[str],
    checksum: NotRequired[str],
    body: NotRequired[BlobTypeDef],
```

## UploadArchiveInputVaultUploadArchiveTypeDef

```python
# UploadArchiveInputVaultUploadArchiveTypeDef definition

class UploadArchiveInputVaultUploadArchiveTypeDef(TypedDict):
    archiveDescription: NotRequired[str],
    checksum: NotRequired[str],
    body: NotRequired[BlobTypeDef],
```

## UploadMultipartPartInputMultipartUploadUploadPartTypeDef

```python
# UploadMultipartPartInputMultipartUploadUploadPartTypeDef definition

class UploadMultipartPartInputMultipartUploadUploadPartTypeDef(TypedDict):
    checksum: NotRequired[str],
    range: NotRequired[str],
    body: NotRequired[BlobTypeDef],
```

## UploadMultipartPartInputRequestTypeDef

```python
# UploadMultipartPartInputRequestTypeDef definition

class UploadMultipartPartInputRequestTypeDef(TypedDict):
    vaultName: str,
    uploadId: str,
    accountId: NotRequired[str],
    checksum: NotRequired[str],
    range: NotRequired[str],
    body: NotRequired[BlobTypeDef],
```

## InputSerializationTypeDef

```python
# InputSerializationTypeDef definition

class InputSerializationTypeDef(TypedDict):
    csv: NotRequired[CSVInputTypeDef],  # (1)
```

1. See [:material-code-braces: CSVInputTypeDef](./type_defs.md#csvinputtypedef) 
## OutputSerializationTypeDef

```python
# OutputSerializationTypeDef definition

class OutputSerializationTypeDef(TypedDict):
    csv: NotRequired[CSVOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CSVOutputTypeDef](./type_defs.md#csvoutputtypedef) 
## DataRetrievalPolicyOutputTypeDef

```python
# DataRetrievalPolicyOutputTypeDef definition

class DataRetrievalPolicyOutputTypeDef(TypedDict):
    Rules: NotRequired[List[DataRetrievalRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: DataRetrievalRuleTypeDef](./type_defs.md#dataretrievalruletypedef) 
## DataRetrievalPolicyTypeDef

```python
# DataRetrievalPolicyTypeDef definition

class DataRetrievalPolicyTypeDef(TypedDict):
    Rules: NotRequired[Sequence[DataRetrievalRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: DataRetrievalRuleTypeDef](./type_defs.md#dataretrievalruletypedef) 
## DescribeVaultInputVaultExistsWaitTypeDef

```python
# DescribeVaultInputVaultExistsWaitTypeDef definition

class DescribeVaultInputVaultExistsWaitTypeDef(TypedDict):
    accountId: str,
    vaultName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeVaultInputVaultNotExistsWaitTypeDef

```python
# DescribeVaultInputVaultNotExistsWaitTypeDef definition

class DescribeVaultInputVaultNotExistsWaitTypeDef(TypedDict):
    accountId: str,
    vaultName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListVaultsOutputTypeDef

```python
# ListVaultsOutputTypeDef definition

class ListVaultsOutputTypeDef(TypedDict):
    VaultList: List[DescribeVaultOutputTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DescribeVaultOutputTypeDef](./type_defs.md#describevaultoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVaultAccessPolicyOutputTypeDef

```python
# GetVaultAccessPolicyOutputTypeDef definition

class GetVaultAccessPolicyOutputTypeDef(TypedDict):
    policy: VaultAccessPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VaultAccessPolicyTypeDef](./type_defs.md#vaultaccesspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetVaultAccessPolicyInputRequestTypeDef

```python
# SetVaultAccessPolicyInputRequestTypeDef definition

class SetVaultAccessPolicyInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    policy: NotRequired[VaultAccessPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: VaultAccessPolicyTypeDef](./type_defs.md#vaultaccesspolicytypedef) 
## GetVaultNotificationsOutputTypeDef

```python
# GetVaultNotificationsOutputTypeDef definition

class GetVaultNotificationsOutputTypeDef(TypedDict):
    vaultNotificationConfig: VaultNotificationConfigOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VaultNotificationConfigOutputTypeDef](./type_defs.md#vaultnotificationconfigoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantTypeDef

```python
# GrantTypeDef definition

class GrantTypeDef(TypedDict):
    Grantee: NotRequired[GranteeTypeDef],  # (1)
    Permission: NotRequired[PermissionType],  # (2)
```

1. See [:material-code-braces: GranteeTypeDef](./type_defs.md#granteetypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## InitiateVaultLockInputRequestTypeDef

```python
# InitiateVaultLockInputRequestTypeDef definition

class InitiateVaultLockInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    policy: NotRequired[VaultLockPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: VaultLockPolicyTypeDef](./type_defs.md#vaultlockpolicytypedef) 
## ListJobsInputListJobsPaginateTypeDef

```python
# ListJobsInputListJobsPaginateTypeDef definition

class ListJobsInputListJobsPaginateTypeDef(TypedDict):
    accountId: str,
    vaultName: str,
    statuscode: NotRequired[str],
    completed: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef

```python
# ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef definition

class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(TypedDict):
    accountId: str,
    vaultName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPartsInputListPartsPaginateTypeDef

```python
# ListPartsInputListPartsPaginateTypeDef definition

class ListPartsInputListPartsPaginateTypeDef(TypedDict):
    accountId: str,
    vaultName: str,
    uploadId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVaultsInputListVaultsPaginateTypeDef

```python
# ListVaultsInputListVaultsPaginateTypeDef definition

class ListVaultsInputListVaultsPaginateTypeDef(TypedDict):
    accountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultipartUploadsOutputTypeDef

```python
# ListMultipartUploadsOutputTypeDef definition

class ListMultipartUploadsOutputTypeDef(TypedDict):
    UploadsList: List[UploadListElementTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadListElementTypeDef](./type_defs.md#uploadlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPartsOutputTypeDef

```python
# ListPartsOutputTypeDef definition

class ListPartsOutputTypeDef(TypedDict):
    MultipartUploadId: str,
    VaultARN: str,
    ArchiveDescription: str,
    PartSizeInBytes: int,
    CreationDate: str,
    Parts: List[PartListElementTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartListElementTypeDef](./type_defs.md#partlistelementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisionedCapacityOutputTypeDef

```python
# ListProvisionedCapacityOutputTypeDef definition

class ListProvisionedCapacityOutputTypeDef(TypedDict):
    ProvisionedCapacityList: List[ProvisionedCapacityDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedCapacityDescriptionTypeDef](./type_defs.md#provisionedcapacitydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetVaultNotificationsInputNotificationSetTypeDef

```python
# SetVaultNotificationsInputNotificationSetTypeDef definition

class SetVaultNotificationsInputNotificationSetTypeDef(TypedDict):
    vaultNotificationConfig: NotRequired[VaultNotificationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VaultNotificationConfigTypeDef](./type_defs.md#vaultnotificationconfigtypedef) 
## SetVaultNotificationsInputRequestTypeDef

```python
# SetVaultNotificationsInputRequestTypeDef definition

class SetVaultNotificationsInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    vaultNotificationConfig: NotRequired[VaultNotificationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VaultNotificationConfigTypeDef](./type_defs.md#vaultnotificationconfigtypedef) 
## SelectParametersTypeDef

```python
# SelectParametersTypeDef definition

class SelectParametersTypeDef(TypedDict):
    InputSerialization: NotRequired[InputSerializationTypeDef],  # (1)
    ExpressionType: NotRequired[ExpressionTypeType],  # (2)
    Expression: NotRequired[str],
    OutputSerialization: NotRequired[OutputSerializationTypeDef],  # (3)
```

1. See [:material-code-braces: InputSerializationTypeDef](./type_defs.md#inputserializationtypedef) 
2. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
3. See [:material-code-braces: OutputSerializationTypeDef](./type_defs.md#outputserializationtypedef) 
## GetDataRetrievalPolicyOutputTypeDef

```python
# GetDataRetrievalPolicyOutputTypeDef definition

class GetDataRetrievalPolicyOutputTypeDef(TypedDict):
    Policy: DataRetrievalPolicyOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataRetrievalPolicyOutputTypeDef](./type_defs.md#dataretrievalpolicyoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDataRetrievalPolicyInputRequestTypeDef

```python
# SetDataRetrievalPolicyInputRequestTypeDef definition

class SetDataRetrievalPolicyInputRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
    Policy: NotRequired[DataRetrievalPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: DataRetrievalPolicyTypeDef](./type_defs.md#dataretrievalpolicytypedef) 
## S3LocationOutputTypeDef

```python
# S3LocationOutputTypeDef definition

class S3LocationOutputTypeDef(TypedDict):
    BucketName: NotRequired[str],
    Prefix: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    CannedACL: NotRequired[CannedACLType],  # (2)
    AccessControlList: NotRequired[List[GrantTypeDef]],  # (3)
    Tagging: NotRequired[Dict[str, str]],
    UserMetadata: NotRequired[Dict[str, str]],
    StorageClass: NotRequired[StorageClassType],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-brackets: CannedACLType](./literals.md#cannedacltype) 
3. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    BucketName: NotRequired[str],
    Prefix: NotRequired[str],
    Encryption: NotRequired[EncryptionTypeDef],  # (1)
    CannedACL: NotRequired[CannedACLType],  # (2)
    AccessControlList: NotRequired[Sequence[GrantTypeDef]],  # (3)
    Tagging: NotRequired[Mapping[str, str]],
    UserMetadata: NotRequired[Mapping[str, str]],
    StorageClass: NotRequired[StorageClassType],  # (4)
```

1. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
2. See [:material-code-brackets: CannedACLType](./literals.md#cannedacltype) 
3. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
4. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
## OutputLocationOutputTypeDef

```python
# OutputLocationOutputTypeDef definition

class OutputLocationOutputTypeDef(TypedDict):
    S3: NotRequired[S3LocationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationOutputTypeDef](./type_defs.md#s3locationoutputtypedef) 
## GlacierJobDescriptionResponseTypeDef

```python
# GlacierJobDescriptionResponseTypeDef definition

class GlacierJobDescriptionResponseTypeDef(TypedDict):
    JobId: str,
    JobDescription: str,
    Action: ActionCodeType,  # (1)
    ArchiveId: str,
    VaultARN: str,
    CreationDate: str,
    Completed: bool,
    StatusCode: StatusCodeType,  # (2)
    StatusMessage: str,
    ArchiveSizeInBytes: int,
    InventorySizeInBytes: int,
    SNSTopic: str,
    CompletionDate: str,
    SHA256TreeHash: str,
    ArchiveSHA256TreeHash: str,
    RetrievalByteRange: str,
    Tier: str,
    InventoryRetrievalParameters: InventoryRetrievalJobDescriptionTypeDef,  # (3)
    JobOutputPath: str,
    SelectParameters: SelectParametersTypeDef,  # (4)
    OutputLocation: OutputLocationOutputTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ActionCodeType](./literals.md#actioncodetype) 
2. See [:material-code-brackets: StatusCodeType](./literals.md#statuscodetype) 
3. See [:material-code-braces: InventoryRetrievalJobDescriptionTypeDef](./type_defs.md#inventoryretrievaljobdescriptiontypedef) 
4. See [:material-code-braces: SelectParametersTypeDef](./type_defs.md#selectparameterstypedef) 
5. See [:material-code-braces: OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlacierJobDescriptionTypeDef

```python
# GlacierJobDescriptionTypeDef definition

class GlacierJobDescriptionTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobDescription: NotRequired[str],
    Action: NotRequired[ActionCodeType],  # (1)
    ArchiveId: NotRequired[str],
    VaultARN: NotRequired[str],
    CreationDate: NotRequired[str],
    Completed: NotRequired[bool],
    StatusCode: NotRequired[StatusCodeType],  # (2)
    StatusMessage: NotRequired[str],
    ArchiveSizeInBytes: NotRequired[int],
    InventorySizeInBytes: NotRequired[int],
    SNSTopic: NotRequired[str],
    CompletionDate: NotRequired[str],
    SHA256TreeHash: NotRequired[str],
    ArchiveSHA256TreeHash: NotRequired[str],
    RetrievalByteRange: NotRequired[str],
    Tier: NotRequired[str],
    InventoryRetrievalParameters: NotRequired[InventoryRetrievalJobDescriptionTypeDef],  # (3)
    JobOutputPath: NotRequired[str],
    SelectParameters: NotRequired[SelectParametersTypeDef],  # (4)
    OutputLocation: NotRequired[OutputLocationOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: ActionCodeType](./literals.md#actioncodetype) 
2. See [:material-code-brackets: StatusCodeType](./literals.md#statuscodetype) 
3. See [:material-code-braces: InventoryRetrievalJobDescriptionTypeDef](./type_defs.md#inventoryretrievaljobdescriptiontypedef) 
4. See [:material-code-braces: SelectParametersTypeDef](./type_defs.md#selectparameterstypedef) 
5. See [:material-code-braces: OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef) 
## OutputLocationTypeDef

```python
# OutputLocationTypeDef definition

class OutputLocationTypeDef(TypedDict):
    S3: NotRequired[S3LocationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) [:material-code-braces: S3LocationOutputTypeDef](./type_defs.md#s3locationoutputtypedef) 
## ListJobsOutputTypeDef

```python
# ListJobsOutputTypeDef definition

class ListJobsOutputTypeDef(TypedDict):
    JobList: List[GlacierJobDescriptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlacierJobDescriptionTypeDef](./type_defs.md#glacierjobdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobParametersTypeDef

```python
# JobParametersTypeDef definition

class JobParametersTypeDef(TypedDict):
    Format: NotRequired[str],
    Type: NotRequired[str],
    ArchiveId: NotRequired[str],
    Description: NotRequired[str],
    SNSTopic: NotRequired[str],
    RetrievalByteRange: NotRequired[str],
    Tier: NotRequired[str],
    InventoryRetrievalParameters: NotRequired[InventoryRetrievalJobInputTypeDef],  # (1)
    SelectParameters: NotRequired[SelectParametersTypeDef],  # (2)
    OutputLocation: NotRequired[OutputLocationUnionTypeDef],  # (3)
```

1. See [:material-code-braces: InventoryRetrievalJobInputTypeDef](./type_defs.md#inventoryretrievaljobinputtypedef) 
2. See [:material-code-braces: SelectParametersTypeDef](./type_defs.md#selectparameterstypedef) 
3. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) [:material-code-braces: OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef) 
## InitiateJobInputRequestTypeDef

```python
# InitiateJobInputRequestTypeDef definition

class InitiateJobInputRequestTypeDef(TypedDict):
    vaultName: str,
    accountId: NotRequired[str],
    jobParameters: NotRequired[JobParametersTypeDef],  # (1)
```

1. See [:material-code-braces: JobParametersTypeDef](./type_defs.md#jobparameterstypedef) 
