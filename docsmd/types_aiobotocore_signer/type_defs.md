# Type definitions

> [Index](../README.md) > [signer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

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




## AddProfilePermissionRequestRequestTypeDef

```python
# AddProfilePermissionRequestRequestTypeDef definition

class AddProfilePermissionRequestRequestTypeDef(TypedDict):
    profileName: str,
    action: str,
    principal: str,
    statementId: str,
    profileVersion: NotRequired[str],
    revisionId: NotRequired[str],
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

## CancelSigningProfileRequestRequestTypeDef

```python
# CancelSigningProfileRequestRequestTypeDef definition

class CancelSigningProfileRequestRequestTypeDef(TypedDict):
    profileName: str,
```

## DescribeSigningJobRequestRequestTypeDef

```python
# DescribeSigningJobRequestRequestTypeDef definition

class DescribeSigningJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## SigningJobRevocationRecordTypeDef

```python
# SigningJobRevocationRecordTypeDef definition

class SigningJobRevocationRecordTypeDef(TypedDict):
    reason: NotRequired[str],
    revokedAt: NotRequired[datetime],
    revokedBy: NotRequired[str],
```

## SigningMaterialTypeDef

```python
# SigningMaterialTypeDef definition

class SigningMaterialTypeDef(TypedDict):
    certificateArn: str,
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    prefix: NotRequired[str],
```

## EncryptionAlgorithmOptionsTypeDef

```python
# EncryptionAlgorithmOptionsTypeDef definition

class EncryptionAlgorithmOptionsTypeDef(TypedDict):
    allowedValues: List[EncryptionAlgorithmType],  # (1)
    defaultValue: EncryptionAlgorithmType,  # (2)
```

1. See [:material-code-brackets: EncryptionAlgorithmType](./literals.md#encryptionalgorithmtype) 
2. See [:material-code-brackets: EncryptionAlgorithmType](./literals.md#encryptionalgorithmtype) 
## GetSigningPlatformRequestRequestTypeDef

```python
# GetSigningPlatformRequestRequestTypeDef definition

class GetSigningPlatformRequestRequestTypeDef(TypedDict):
    platformId: str,
```

## SigningImageFormatTypeDef

```python
# SigningImageFormatTypeDef definition

class SigningImageFormatTypeDef(TypedDict):
    supportedFormats: List[ImageFormatType],  # (1)
    defaultFormat: ImageFormatType,  # (2)
```

1. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype) 
2. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype) 
## GetSigningProfileRequestRequestTypeDef

```python
# GetSigningProfileRequestRequestTypeDef definition

class GetSigningProfileRequestRequestTypeDef(TypedDict):
    profileName: str,
    profileOwner: NotRequired[str],
```

## SignatureValidityPeriodTypeDef

```python
# SignatureValidityPeriodTypeDef definition

class SignatureValidityPeriodTypeDef(TypedDict):
    value: NotRequired[int],
    type: NotRequired[ValidityTypeType],  # (1)
```

1. See [:material-code-brackets: ValidityTypeType](./literals.md#validitytypetype) 
## SigningProfileRevocationRecordTypeDef

```python
# SigningProfileRevocationRecordTypeDef definition

class SigningProfileRevocationRecordTypeDef(TypedDict):
    revocationEffectiveFrom: NotRequired[datetime],
    revokedAt: NotRequired[datetime],
    revokedBy: NotRequired[str],
```

## HashAlgorithmOptionsTypeDef

```python
# HashAlgorithmOptionsTypeDef definition

class HashAlgorithmOptionsTypeDef(TypedDict):
    allowedValues: List[HashAlgorithmType],  # (1)
    defaultValue: HashAlgorithmType,  # (2)
```

1. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
2. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
## ListProfilePermissionsRequestRequestTypeDef

```python
# ListProfilePermissionsRequestRequestTypeDef definition

class ListProfilePermissionsRequestRequestTypeDef(TypedDict):
    profileName: str,
    nextToken: NotRequired[str],
```

## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    action: NotRequired[str],
    principal: NotRequired[str],
    statementId: NotRequired[str],
    profileVersion: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSigningPlatformsRequestRequestTypeDef

```python
# ListSigningPlatformsRequestRequestTypeDef definition

class ListSigningPlatformsRequestRequestTypeDef(TypedDict):
    category: NotRequired[str],
    partner: NotRequired[str],
    target: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListSigningProfilesRequestRequestTypeDef

```python
# ListSigningProfilesRequestRequestTypeDef definition

class ListSigningProfilesRequestRequestTypeDef(TypedDict):
    includeCanceled: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    platformId: NotRequired[str],
    statuses: NotRequired[Sequence[SigningProfileStatusType]],  # (1)
```

1. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RemoveProfilePermissionRequestRequestTypeDef

```python
# RemoveProfilePermissionRequestRequestTypeDef definition

class RemoveProfilePermissionRequestRequestTypeDef(TypedDict):
    profileName: str,
    revisionId: str,
    statementId: str,
```

## RevokeSignatureRequestRequestTypeDef

```python
# RevokeSignatureRequestRequestTypeDef definition

class RevokeSignatureRequestRequestTypeDef(TypedDict):
    jobId: str,
    reason: str,
    jobOwner: NotRequired[str],
```

## S3SignedObjectTypeDef

```python
# S3SignedObjectTypeDef definition

class S3SignedObjectTypeDef(TypedDict):
    bucketName: NotRequired[str],
    key: NotRequired[str],
```

## S3SourceTypeDef

```python
# S3SourceTypeDef definition

class S3SourceTypeDef(TypedDict):
    bucketName: str,
    key: str,
    version: str,
```

## SigningConfigurationOverridesTypeDef

```python
# SigningConfigurationOverridesTypeDef definition

class SigningConfigurationOverridesTypeDef(TypedDict):
    encryptionAlgorithm: NotRequired[EncryptionAlgorithmType],  # (1)
    hashAlgorithm: NotRequired[HashAlgorithmType],  # (2)
```

1. See [:material-code-brackets: EncryptionAlgorithmType](./literals.md#encryptionalgorithmtype) 
2. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AddProfilePermissionResponseTypeDef

```python
# AddProfilePermissionResponseTypeDef definition

class AddProfilePermissionResponseTypeDef(TypedDict):
    revisionId: str,
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
## GetRevocationStatusResponseTypeDef

```python
# GetRevocationStatusResponseTypeDef definition

class GetRevocationStatusResponseTypeDef(TypedDict):
    revokedEntities: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSigningProfileResponseTypeDef

```python
# PutSigningProfileResponseTypeDef definition

class PutSigningProfileResponseTypeDef(TypedDict):
    arn: str,
    profileVersion: str,
    profileVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveProfilePermissionResponseTypeDef

```python
# RemoveProfilePermissionResponseTypeDef definition

class RemoveProfilePermissionResponseTypeDef(TypedDict):
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignPayloadResponseTypeDef

```python
# SignPayloadResponseTypeDef definition

class SignPayloadResponseTypeDef(TypedDict):
    jobId: str,
    jobOwner: str,
    metadata: Dict[str, str],
    signature: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSigningJobResponseTypeDef

```python
# StartSigningJobResponseTypeDef definition

class StartSigningJobResponseTypeDef(TypedDict):
    jobId: str,
    jobOwner: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignPayloadRequestRequestTypeDef

```python
# SignPayloadRequestRequestTypeDef definition

class SignPayloadRequestRequestTypeDef(TypedDict):
    profileName: str,
    payload: Union[str, bytes, IO[Any], StreamingBody],
    payloadFormat: str,
    profileOwner: NotRequired[str],
```

## DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef

```python
# DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef definition

class DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef(TypedDict):
    jobId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## GetRevocationStatusRequestRequestTypeDef

```python
# GetRevocationStatusRequestRequestTypeDef definition

class GetRevocationStatusRequestRequestTypeDef(TypedDict):
    signatureTimestamp: Union[datetime, str],
    platformId: str,
    profileVersionArn: str,
    jobArn: str,
    certificateHashes: Sequence[str],
```

## ListSigningJobsRequestRequestTypeDef

```python
# ListSigningJobsRequestRequestTypeDef definition

class ListSigningJobsRequestRequestTypeDef(TypedDict):
    status: NotRequired[SigningStatusType],  # (1)
    platformId: NotRequired[str],
    requestedBy: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    isRevoked: NotRequired[bool],
    signatureExpiresBefore: NotRequired[Union[datetime, str]],
    signatureExpiresAfter: NotRequired[Union[datetime, str]],
    jobInvoker: NotRequired[str],
```

1. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
## RevokeSigningProfileRequestRequestTypeDef

```python
# RevokeSigningProfileRequestRequestTypeDef definition

class RevokeSigningProfileRequestRequestTypeDef(TypedDict):
    profileName: str,
    profileVersion: str,
    reason: str,
    effectiveTime: Union[datetime, str],
```

## SigningProfileTypeDef

```python
# SigningProfileTypeDef definition

class SigningProfileTypeDef(TypedDict):
    profileName: NotRequired[str],
    profileVersion: NotRequired[str],
    profileVersionArn: NotRequired[str],
    signingMaterial: NotRequired[SigningMaterialTypeDef],  # (1)
    signatureValidityPeriod: NotRequired[SignatureValidityPeriodTypeDef],  # (2)
    platformId: NotRequired[str],
    platformDisplayName: NotRequired[str],
    signingParameters: NotRequired[Dict[str, str]],
    status: NotRequired[SigningProfileStatusType],  # (3)
    arn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
2. See [:material-code-braces: SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef) 
3. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
## SigningConfigurationTypeDef

```python
# SigningConfigurationTypeDef definition

class SigningConfigurationTypeDef(TypedDict):
    encryptionAlgorithmOptions: EncryptionAlgorithmOptionsTypeDef,  # (1)
    hashAlgorithmOptions: HashAlgorithmOptionsTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionAlgorithmOptionsTypeDef](./type_defs.md#encryptionalgorithmoptionstypedef) 
2. See [:material-code-braces: HashAlgorithmOptionsTypeDef](./type_defs.md#hashalgorithmoptionstypedef) 
## ListProfilePermissionsResponseTypeDef

```python
# ListProfilePermissionsResponseTypeDef definition

class ListProfilePermissionsResponseTypeDef(TypedDict):
    revisionId: str,
    policySizeBytes: int,
    permissions: List[PermissionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSigningJobsRequestListSigningJobsPaginateTypeDef

```python
# ListSigningJobsRequestListSigningJobsPaginateTypeDef definition

class ListSigningJobsRequestListSigningJobsPaginateTypeDef(TypedDict):
    status: NotRequired[SigningStatusType],  # (1)
    platformId: NotRequired[str],
    requestedBy: NotRequired[str],
    isRevoked: NotRequired[bool],
    signatureExpiresBefore: NotRequired[Union[datetime, str]],
    signatureExpiresAfter: NotRequired[Union[datetime, str]],
    jobInvoker: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef

```python
# ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef definition

class ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef(TypedDict):
    category: NotRequired[str],
    partner: NotRequired[str],
    target: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSigningProfilesRequestListSigningProfilesPaginateTypeDef

```python
# ListSigningProfilesRequestListSigningProfilesPaginateTypeDef definition

class ListSigningProfilesRequestListSigningProfilesPaginateTypeDef(TypedDict):
    includeCanceled: NotRequired[bool],
    platformId: NotRequired[str],
    statuses: NotRequired[Sequence[SigningProfileStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SignedObjectTypeDef

```python
# SignedObjectTypeDef definition

class SignedObjectTypeDef(TypedDict):
    s3: NotRequired[S3SignedObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3SignedObjectTypeDef](./type_defs.md#s3signedobjecttypedef) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    s3: NotRequired[S3SourceTypeDef],  # (1)
```

1. See [:material-code-braces: S3SourceTypeDef](./type_defs.md#s3sourcetypedef) 
## SigningPlatformOverridesTypeDef

```python
# SigningPlatformOverridesTypeDef definition

class SigningPlatformOverridesTypeDef(TypedDict):
    signingConfiguration: NotRequired[SigningConfigurationOverridesTypeDef],  # (1)
    signingImageFormat: NotRequired[ImageFormatType],  # (2)
```

1. See [:material-code-braces: SigningConfigurationOverridesTypeDef](./type_defs.md#signingconfigurationoverridestypedef) 
2. See [:material-code-brackets: ImageFormatType](./literals.md#imageformattype) 
## ListSigningProfilesResponseTypeDef

```python
# ListSigningProfilesResponseTypeDef definition

class ListSigningProfilesResponseTypeDef(TypedDict):
    profiles: List[SigningProfileTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SigningProfileTypeDef](./type_defs.md#signingprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSigningPlatformResponseTypeDef

```python
# GetSigningPlatformResponseTypeDef definition

class GetSigningPlatformResponseTypeDef(TypedDict):
    platformId: str,
    displayName: str,
    partner: str,
    target: str,
    category: CategoryType,  # (1)
    signingConfiguration: SigningConfigurationTypeDef,  # (2)
    signingImageFormat: SigningImageFormatTypeDef,  # (3)
    maxSizeInMB: int,
    revocationSupported: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CategoryType](./literals.md#categorytype) 
2. See [:material-code-braces: SigningConfigurationTypeDef](./type_defs.md#signingconfigurationtypedef) 
3. See [:material-code-braces: SigningImageFormatTypeDef](./type_defs.md#signingimageformattypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SigningPlatformTypeDef

```python
# SigningPlatformTypeDef definition

class SigningPlatformTypeDef(TypedDict):
    platformId: NotRequired[str],
    displayName: NotRequired[str],
    partner: NotRequired[str],
    target: NotRequired[str],
    category: NotRequired[CategoryType],  # (1)
    signingConfiguration: NotRequired[SigningConfigurationTypeDef],  # (2)
    signingImageFormat: NotRequired[SigningImageFormatTypeDef],  # (3)
    maxSizeInMB: NotRequired[int],
    revocationSupported: NotRequired[bool],
```

1. See [:material-code-brackets: CategoryType](./literals.md#categorytype) 
2. See [:material-code-braces: SigningConfigurationTypeDef](./type_defs.md#signingconfigurationtypedef) 
3. See [:material-code-braces: SigningImageFormatTypeDef](./type_defs.md#signingimageformattypedef) 
## SigningJobTypeDef

```python
# SigningJobTypeDef definition

class SigningJobTypeDef(TypedDict):
    jobId: NotRequired[str],
    source: NotRequired[SourceTypeDef],  # (1)
    signedObject: NotRequired[SignedObjectTypeDef],  # (2)
    signingMaterial: NotRequired[SigningMaterialTypeDef],  # (3)
    createdAt: NotRequired[datetime],
    status: NotRequired[SigningStatusType],  # (4)
    isRevoked: NotRequired[bool],
    profileName: NotRequired[str],
    profileVersion: NotRequired[str],
    platformId: NotRequired[str],
    platformDisplayName: NotRequired[str],
    signatureExpiresAt: NotRequired[datetime],
    jobOwner: NotRequired[str],
    jobInvoker: NotRequired[str],
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SignedObjectTypeDef](./type_defs.md#signedobjecttypedef) 
3. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
4. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
## StartSigningJobRequestRequestTypeDef

```python
# StartSigningJobRequestRequestTypeDef definition

class StartSigningJobRequestRequestTypeDef(TypedDict):
    source: SourceTypeDef,  # (1)
    destination: DestinationTypeDef,  # (2)
    profileName: str,
    clientRequestToken: str,
    profileOwner: NotRequired[str],
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## DescribeSigningJobResponseTypeDef

```python
# DescribeSigningJobResponseTypeDef definition

class DescribeSigningJobResponseTypeDef(TypedDict):
    jobId: str,
    source: SourceTypeDef,  # (1)
    signingMaterial: SigningMaterialTypeDef,  # (2)
    platformId: str,
    platformDisplayName: str,
    profileName: str,
    profileVersion: str,
    overrides: SigningPlatformOverridesTypeDef,  # (3)
    signingParameters: Dict[str, str],
    createdAt: datetime,
    completedAt: datetime,
    signatureExpiresAt: datetime,
    requestedBy: str,
    status: SigningStatusType,  # (4)
    statusReason: str,
    revocationRecord: SigningJobRevocationRecordTypeDef,  # (5)
    signedObject: SignedObjectTypeDef,  # (6)
    jobOwner: str,
    jobInvoker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
3. See [:material-code-braces: SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef) 
4. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
5. See [:material-code-braces: SigningJobRevocationRecordTypeDef](./type_defs.md#signingjobrevocationrecordtypedef) 
6. See [:material-code-braces: SignedObjectTypeDef](./type_defs.md#signedobjecttypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSigningProfileResponseTypeDef

```python
# GetSigningProfileResponseTypeDef definition

class GetSigningProfileResponseTypeDef(TypedDict):
    profileName: str,
    profileVersion: str,
    profileVersionArn: str,
    revocationRecord: SigningProfileRevocationRecordTypeDef,  # (1)
    signingMaterial: SigningMaterialTypeDef,  # (2)
    platformId: str,
    platformDisplayName: str,
    signatureValidityPeriod: SignatureValidityPeriodTypeDef,  # (3)
    overrides: SigningPlatformOverridesTypeDef,  # (4)
    signingParameters: Dict[str, str],
    status: SigningProfileStatusType,  # (5)
    statusReason: str,
    arn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SigningProfileRevocationRecordTypeDef](./type_defs.md#signingprofilerevocationrecordtypedef) 
2. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
3. See [:material-code-braces: SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef) 
4. See [:material-code-braces: SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef) 
5. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSigningProfileRequestRequestTypeDef

```python
# PutSigningProfileRequestRequestTypeDef definition

class PutSigningProfileRequestRequestTypeDef(TypedDict):
    profileName: str,
    platformId: str,
    signingMaterial: NotRequired[SigningMaterialTypeDef],  # (1)
    signatureValidityPeriod: NotRequired[SignatureValidityPeriodTypeDef],  # (2)
    overrides: NotRequired[SigningPlatformOverridesTypeDef],  # (3)
    signingParameters: NotRequired[Mapping[str, str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef) 
2. See [:material-code-braces: SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef) 
3. See [:material-code-braces: SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef) 
## ListSigningPlatformsResponseTypeDef

```python
# ListSigningPlatformsResponseTypeDef definition

class ListSigningPlatformsResponseTypeDef(TypedDict):
    platforms: List[SigningPlatformTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SigningPlatformTypeDef](./type_defs.md#signingplatformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSigningJobsResponseTypeDef

```python
# ListSigningJobsResponseTypeDef definition

class ListSigningJobsResponseTypeDef(TypedDict):
    jobs: List[SigningJobTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SigningJobTypeDef](./type_defs.md#signingjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
