# Type definitions

> [Index](../README.md) > [KMS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#kms)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

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




## AliasListEntryTypeDef

```python
# AliasListEntryTypeDef definition

class AliasListEntryTypeDef(TypedDict):
    AliasName: NotRequired[str],
    AliasArn: NotRequired[str],
    TargetKeyId: NotRequired[str],
    CreationDate: NotRequired[datetime],
    LastUpdatedDate: NotRequired[datetime],
```

## CancelKeyDeletionRequestRequestTypeDef

```python
# CancelKeyDeletionRequestRequestTypeDef definition

class CancelKeyDeletionRequestRequestTypeDef(TypedDict):
    KeyId: str,
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

## ConnectCustomKeyStoreRequestRequestTypeDef

```python
# ConnectCustomKeyStoreRequestRequestTypeDef definition

class ConnectCustomKeyStoreRequestRequestTypeDef(TypedDict):
    CustomKeyStoreId: str,
```

## CreateAliasRequestRequestTypeDef

```python
# CreateAliasRequestRequestTypeDef definition

class CreateAliasRequestRequestTypeDef(TypedDict):
    AliasName: str,
    TargetKeyId: str,
```

## XksProxyAuthenticationCredentialTypeTypeDef

```python
# XksProxyAuthenticationCredentialTypeTypeDef definition

class XksProxyAuthenticationCredentialTypeTypeDef(TypedDict):
    AccessKeyId: str,
    RawSecretAccessKey: str,
```

## GrantConstraintsTypeDef

```python
# GrantConstraintsTypeDef definition

class GrantConstraintsTypeDef(TypedDict):
    EncryptionContextSubset: NotRequired[Mapping[str, str]],
    EncryptionContextEquals: NotRequired[Mapping[str, str]],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    TagKey: str,
    TagValue: str,
```

## XksProxyConfigurationTypeTypeDef

```python
# XksProxyConfigurationTypeTypeDef definition

class XksProxyConfigurationTypeTypeDef(TypedDict):
    Connectivity: NotRequired[XksProxyConnectivityTypeType],  # (1)
    AccessKeyId: NotRequired[str],
    UriEndpoint: NotRequired[str],
    UriPath: NotRequired[str],
    VpcEndpointServiceName: NotRequired[str],
```

1. See [:material-code-brackets: XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype) 
## DeleteAliasRequestRequestTypeDef

```python
# DeleteAliasRequestRequestTypeDef definition

class DeleteAliasRequestRequestTypeDef(TypedDict):
    AliasName: str,
```

## DeleteCustomKeyStoreRequestRequestTypeDef

```python
# DeleteCustomKeyStoreRequestRequestTypeDef definition

class DeleteCustomKeyStoreRequestRequestTypeDef(TypedDict):
    CustomKeyStoreId: str,
```

## DeleteImportedKeyMaterialRequestRequestTypeDef

```python
# DeleteImportedKeyMaterialRequestRequestTypeDef definition

class DeleteImportedKeyMaterialRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeCustomKeyStoresRequestRequestTypeDef

```python
# DescribeCustomKeyStoresRequestRequestTypeDef definition

class DescribeCustomKeyStoresRequestRequestTypeDef(TypedDict):
    CustomKeyStoreId: NotRequired[str],
    CustomKeyStoreName: NotRequired[str],
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeKeyRequestRequestTypeDef

```python
# DescribeKeyRequestRequestTypeDef definition

class DescribeKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    GrantTokens: NotRequired[Sequence[str]],
```

## DisableKeyRequestRequestTypeDef

```python
# DisableKeyRequestRequestTypeDef definition

class DisableKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## DisableKeyRotationRequestRequestTypeDef

```python
# DisableKeyRotationRequestRequestTypeDef definition

class DisableKeyRotationRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## DisconnectCustomKeyStoreRequestRequestTypeDef

```python
# DisconnectCustomKeyStoreRequestRequestTypeDef definition

class DisconnectCustomKeyStoreRequestRequestTypeDef(TypedDict):
    CustomKeyStoreId: str,
```

## EnableKeyRequestRequestTypeDef

```python
# EnableKeyRequestRequestTypeDef definition

class EnableKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## EnableKeyRotationRequestRequestTypeDef

```python
# EnableKeyRotationRequestRequestTypeDef definition

class EnableKeyRotationRequestRequestTypeDef(TypedDict):
    KeyId: str,
    RotationPeriodInDays: NotRequired[int],
```

## GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef

```python
# GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef definition

class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(TypedDict):
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    EncryptionContext: NotRequired[Mapping[str, str]],
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
## GenerateDataKeyWithoutPlaintextRequestRequestTypeDef

```python
# GenerateDataKeyWithoutPlaintextRequestRequestTypeDef definition

class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(TypedDict):
    KeyId: str,
    EncryptionContext: NotRequired[Mapping[str, str]],
    KeySpec: NotRequired[DataKeySpecType],  # (1)
    NumberOfBytes: NotRequired[int],
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: DataKeySpecType](./literals.md#datakeyspectype) 
## GetKeyPolicyRequestRequestTypeDef

```python
# GetKeyPolicyRequestRequestTypeDef definition

class GetKeyPolicyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    PolicyName: NotRequired[str],
```

## GetKeyRotationStatusRequestRequestTypeDef

```python
# GetKeyRotationStatusRequestRequestTypeDef definition

class GetKeyRotationStatusRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## GetParametersForImportRequestRequestTypeDef

```python
# GetParametersForImportRequestRequestTypeDef definition

class GetParametersForImportRequestRequestTypeDef(TypedDict):
    KeyId: str,
    WrappingAlgorithm: AlgorithmSpecType,  # (1)
    WrappingKeySpec: WrappingKeySpecType,  # (2)
```

1. See [:material-code-brackets: AlgorithmSpecType](./literals.md#algorithmspectype) 
2. See [:material-code-brackets: WrappingKeySpecType](./literals.md#wrappingkeyspectype) 
## GetPublicKeyRequestRequestTypeDef

```python
# GetPublicKeyRequestRequestTypeDef definition

class GetPublicKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    GrantTokens: NotRequired[Sequence[str]],
```

## GrantConstraintsOutputTypeDef

```python
# GrantConstraintsOutputTypeDef definition

class GrantConstraintsOutputTypeDef(TypedDict):
    EncryptionContextSubset: NotRequired[Dict[str, str]],
    EncryptionContextEquals: NotRequired[Dict[str, str]],
```

## KeyListEntryTypeDef

```python
# KeyListEntryTypeDef definition

class KeyListEntryTypeDef(TypedDict):
    KeyId: NotRequired[str],
    KeyArn: NotRequired[str],
```

## XksKeyConfigurationTypeTypeDef

```python
# XksKeyConfigurationTypeTypeDef definition

class XksKeyConfigurationTypeTypeDef(TypedDict):
    Id: NotRequired[str],
```

## ListAliasesRequestRequestTypeDef

```python
# ListAliasesRequestRequestTypeDef definition

class ListAliasesRequestRequestTypeDef(TypedDict):
    KeyId: NotRequired[str],
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## ListGrantsRequestRequestTypeDef

```python
# ListGrantsRequestRequestTypeDef definition

class ListGrantsRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
    GrantId: NotRequired[str],
    GranteePrincipal: NotRequired[str],
```

## ListKeyPoliciesRequestRequestTypeDef

```python
# ListKeyPoliciesRequestRequestTypeDef definition

class ListKeyPoliciesRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## ListKeyRotationsRequestRequestTypeDef

```python
# ListKeyRotationsRequestRequestTypeDef definition

class ListKeyRotationsRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## RotationsListEntryTypeDef

```python
# RotationsListEntryTypeDef definition

class RotationsListEntryTypeDef(TypedDict):
    KeyId: NotRequired[str],
    RotationDate: NotRequired[datetime],
    RotationType: NotRequired[RotationTypeType],  # (1)
```

1. See [:material-code-brackets: RotationTypeType](./literals.md#rotationtypetype) 
## ListKeysRequestRequestTypeDef

```python
# ListKeysRequestRequestTypeDef definition

class ListKeysRequestRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## ListResourceTagsRequestRequestTypeDef

```python
# ListResourceTagsRequestRequestTypeDef definition

class ListResourceTagsRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## ListRetirableGrantsRequestRequestTypeDef

```python
# ListRetirableGrantsRequestRequestTypeDef definition

class ListRetirableGrantsRequestRequestTypeDef(TypedDict):
    RetiringPrincipal: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## MultiRegionKeyTypeDef

```python
# MultiRegionKeyTypeDef definition

class MultiRegionKeyTypeDef(TypedDict):
    Arn: NotRequired[str],
    Region: NotRequired[str],
```

## PutKeyPolicyRequestRequestTypeDef

```python
# PutKeyPolicyRequestRequestTypeDef definition

class PutKeyPolicyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Policy: str,
    PolicyName: NotRequired[str],
    BypassPolicyLockoutSafetyCheck: NotRequired[bool],
```

## RetireGrantRequestRequestTypeDef

```python
# RetireGrantRequestRequestTypeDef definition

class RetireGrantRequestRequestTypeDef(TypedDict):
    GrantToken: NotRequired[str],
    KeyId: NotRequired[str],
    GrantId: NotRequired[str],
    DryRun: NotRequired[bool],
```

## RevokeGrantRequestRequestTypeDef

```python
# RevokeGrantRequestRequestTypeDef definition

class RevokeGrantRequestRequestTypeDef(TypedDict):
    KeyId: str,
    GrantId: str,
    DryRun: NotRequired[bool],
```

## RotateKeyOnDemandRequestRequestTypeDef

```python
# RotateKeyOnDemandRequestRequestTypeDef definition

class RotateKeyOnDemandRequestRequestTypeDef(TypedDict):
    KeyId: str,
```

## ScheduleKeyDeletionRequestRequestTypeDef

```python
# ScheduleKeyDeletionRequestRequestTypeDef definition

class ScheduleKeyDeletionRequestRequestTypeDef(TypedDict):
    KeyId: str,
    PendingWindowInDays: NotRequired[int],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    KeyId: str,
    TagKeys: Sequence[str],
```

## UpdateAliasRequestRequestTypeDef

```python
# UpdateAliasRequestRequestTypeDef definition

class UpdateAliasRequestRequestTypeDef(TypedDict):
    AliasName: str,
    TargetKeyId: str,
```

## UpdateKeyDescriptionRequestRequestTypeDef

```python
# UpdateKeyDescriptionRequestRequestTypeDef definition

class UpdateKeyDescriptionRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Description: str,
```

## UpdatePrimaryRegionRequestRequestTypeDef

```python
# UpdatePrimaryRegionRequestRequestTypeDef definition

class UpdatePrimaryRegionRequestRequestTypeDef(TypedDict):
    KeyId: str,
    PrimaryRegion: str,
```

## EncryptRequestRequestTypeDef

```python
# EncryptRequestRequestTypeDef definition

class EncryptRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Plaintext: BlobTypeDef,
    EncryptionContext: NotRequired[Mapping[str, str]],
    GrantTokens: NotRequired[Sequence[str]],
    EncryptionAlgorithm: NotRequired[EncryptionAlgorithmSpecType],  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
## GenerateMacRequestRequestTypeDef

```python
# GenerateMacRequestRequestTypeDef definition

class GenerateMacRequestRequestTypeDef(TypedDict):
    Message: BlobTypeDef,
    KeyId: str,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
## ReEncryptRequestRequestTypeDef

```python
# ReEncryptRequestRequestTypeDef definition

class ReEncryptRequestRequestTypeDef(TypedDict):
    CiphertextBlob: BlobTypeDef,
    DestinationKeyId: str,
    SourceEncryptionContext: NotRequired[Mapping[str, str]],
    SourceKeyId: NotRequired[str],
    DestinationEncryptionContext: NotRequired[Mapping[str, str]],
    SourceEncryptionAlgorithm: NotRequired[EncryptionAlgorithmSpecType],  # (1)
    DestinationEncryptionAlgorithm: NotRequired[EncryptionAlgorithmSpecType],  # (1)
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
## RecipientInfoTypeDef

```python
# RecipientInfoTypeDef definition

class RecipientInfoTypeDef(TypedDict):
    KeyEncryptionAlgorithm: NotRequired[KeyEncryptionMechanismType],  # (1)
    AttestationDocument: NotRequired[BlobTypeDef],
```

1. See [:material-code-brackets: KeyEncryptionMechanismType](./literals.md#keyencryptionmechanismtype) 
## SignRequestRequestTypeDef

```python
# SignRequestRequestTypeDef definition

class SignRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Message: BlobTypeDef,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    MessageType: NotRequired[MessageTypeType],  # (2)
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## VerifyMacRequestRequestTypeDef

```python
# VerifyMacRequestRequestTypeDef definition

class VerifyMacRequestRequestTypeDef(TypedDict):
    Message: BlobTypeDef,
    KeyId: str,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    Mac: BlobTypeDef,
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
## VerifyRequestRequestTypeDef

```python
# VerifyRequestRequestTypeDef definition

class VerifyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Message: BlobTypeDef,
    Signature: BlobTypeDef,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    MessageType: NotRequired[MessageTypeType],  # (2)
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## CancelKeyDeletionResponseTypeDef

```python
# CancelKeyDeletionResponseTypeDef definition

class CancelKeyDeletionResponseTypeDef(TypedDict):
    KeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomKeyStoreResponseTypeDef

```python
# CreateCustomKeyStoreResponseTypeDef definition

class CreateCustomKeyStoreResponseTypeDef(TypedDict):
    CustomKeyStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGrantResponseTypeDef

```python
# CreateGrantResponseTypeDef definition

class CreateGrantResponseTypeDef(TypedDict):
    GrantToken: str,
    GrantId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecryptResponseTypeDef

```python
# DecryptResponseTypeDef definition

class DecryptResponseTypeDef(TypedDict):
    KeyId: str,
    Plaintext: bytes,
    EncryptionAlgorithm: EncryptionAlgorithmSpecType,  # (1)
    CiphertextForRecipient: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeriveSharedSecretResponseTypeDef

```python
# DeriveSharedSecretResponseTypeDef definition

class DeriveSharedSecretResponseTypeDef(TypedDict):
    KeyId: str,
    SharedSecret: bytes,
    CiphertextForRecipient: bytes,
    KeyAgreementAlgorithm: KeyAgreementAlgorithmSpecType,  # (1)
    KeyOrigin: OriginTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype) 
2. See [:material-code-brackets: OriginTypeType](./literals.md#origintypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptResponseTypeDef

```python
# EncryptResponseTypeDef definition

class EncryptResponseTypeDef(TypedDict):
    CiphertextBlob: bytes,
    KeyId: str,
    EncryptionAlgorithm: EncryptionAlgorithmSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateDataKeyPairResponseTypeDef

```python
# GenerateDataKeyPairResponseTypeDef definition

class GenerateDataKeyPairResponseTypeDef(TypedDict):
    PrivateKeyCiphertextBlob: bytes,
    PrivateKeyPlaintext: bytes,
    PublicKey: bytes,
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    CiphertextForRecipient: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateDataKeyPairWithoutPlaintextResponseTypeDef

```python
# GenerateDataKeyPairWithoutPlaintextResponseTypeDef definition

class GenerateDataKeyPairWithoutPlaintextResponseTypeDef(TypedDict):
    PrivateKeyCiphertextBlob: bytes,
    PublicKey: bytes,
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateDataKeyResponseTypeDef

```python
# GenerateDataKeyResponseTypeDef definition

class GenerateDataKeyResponseTypeDef(TypedDict):
    CiphertextBlob: bytes,
    Plaintext: bytes,
    KeyId: str,
    CiphertextForRecipient: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateDataKeyWithoutPlaintextResponseTypeDef

```python
# GenerateDataKeyWithoutPlaintextResponseTypeDef definition

class GenerateDataKeyWithoutPlaintextResponseTypeDef(TypedDict):
    CiphertextBlob: bytes,
    KeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateMacResponseTypeDef

```python
# GenerateMacResponseTypeDef definition

class GenerateMacResponseTypeDef(TypedDict):
    Mac: bytes,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    KeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateRandomResponseTypeDef

```python
# GenerateRandomResponseTypeDef definition

class GenerateRandomResponseTypeDef(TypedDict):
    Plaintext: bytes,
    CiphertextForRecipient: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyPolicyResponseTypeDef

```python
# GetKeyPolicyResponseTypeDef definition

class GetKeyPolicyResponseTypeDef(TypedDict):
    Policy: str,
    PolicyName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyRotationStatusResponseTypeDef

```python
# GetKeyRotationStatusResponseTypeDef definition

class GetKeyRotationStatusResponseTypeDef(TypedDict):
    KeyRotationEnabled: bool,
    KeyId: str,
    RotationPeriodInDays: int,
    NextRotationDate: datetime,
    OnDemandRotationStartDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersForImportResponseTypeDef

```python
# GetParametersForImportResponseTypeDef definition

class GetParametersForImportResponseTypeDef(TypedDict):
    KeyId: str,
    ImportToken: bytes,
    PublicKey: bytes,
    ParametersValidTo: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPublicKeyResponseTypeDef

```python
# GetPublicKeyResponseTypeDef definition

class GetPublicKeyResponseTypeDef(TypedDict):
    KeyId: str,
    PublicKey: bytes,
    CustomerMasterKeySpec: CustomerMasterKeySpecType,  # (1)
    KeySpec: KeySpecType,  # (2)
    KeyUsage: KeyUsageTypeType,  # (3)
    EncryptionAlgorithms: List[EncryptionAlgorithmSpecType],  # (4)
    SigningAlgorithms: List[SigningAlgorithmSpecType],  # (5)
    KeyAgreementAlgorithms: List[KeyAgreementAlgorithmSpecType],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: CustomerMasterKeySpecType](./literals.md#customermasterkeyspectype) 
2. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
3. See [:material-code-brackets: KeyUsageTypeType](./literals.md#keyusagetypetype) 
4. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
5. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
6. See [:material-code-brackets: KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesResponseTypeDef

```python
# ListAliasesResponseTypeDef definition

class ListAliasesResponseTypeDef(TypedDict):
    Aliases: List[AliasListEntryTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasListEntryTypeDef](./type_defs.md#aliaslistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyPoliciesResponseTypeDef

```python
# ListKeyPoliciesResponseTypeDef definition

class ListKeyPoliciesResponseTypeDef(TypedDict):
    PolicyNames: List[str],
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReEncryptResponseTypeDef

```python
# ReEncryptResponseTypeDef definition

class ReEncryptResponseTypeDef(TypedDict):
    CiphertextBlob: bytes,
    SourceKeyId: str,
    KeyId: str,
    SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType,  # (1)
    DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateKeyOnDemandResponseTypeDef

```python
# RotateKeyOnDemandResponseTypeDef definition

class RotateKeyOnDemandResponseTypeDef(TypedDict):
    KeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduleKeyDeletionResponseTypeDef

```python
# ScheduleKeyDeletionResponseTypeDef definition

class ScheduleKeyDeletionResponseTypeDef(TypedDict):
    KeyId: str,
    DeletionDate: datetime,
    KeyState: KeyStateType,  # (1)
    PendingWindowInDays: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignResponseTypeDef

```python
# SignResponseTypeDef definition

class SignResponseTypeDef(TypedDict):
    KeyId: str,
    Signature: bytes,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyMacResponseTypeDef

```python
# VerifyMacResponseTypeDef definition

class VerifyMacResponseTypeDef(TypedDict):
    KeyId: str,
    MacValid: bool,
    MacAlgorithm: MacAlgorithmSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyResponseTypeDef

```python
# VerifyResponseTypeDef definition

class VerifyResponseTypeDef(TypedDict):
    KeyId: str,
    SignatureValid: bool,
    SigningAlgorithm: SigningAlgorithmSpecType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomKeyStoreRequestRequestTypeDef

```python
# CreateCustomKeyStoreRequestRequestTypeDef definition

class CreateCustomKeyStoreRequestRequestTypeDef(TypedDict):
    CustomKeyStoreName: str,
    CloudHsmClusterId: NotRequired[str],
    TrustAnchorCertificate: NotRequired[str],
    KeyStorePassword: NotRequired[str],
    CustomKeyStoreType: NotRequired[CustomKeyStoreTypeType],  # (1)
    XksProxyUriEndpoint: NotRequired[str],
    XksProxyUriPath: NotRequired[str],
    XksProxyVpcEndpointServiceName: NotRequired[str],
    XksProxyAuthenticationCredential: NotRequired[XksProxyAuthenticationCredentialTypeTypeDef],  # (2)
    XksProxyConnectivity: NotRequired[XksProxyConnectivityTypeType],  # (3)
```

1. See [:material-code-brackets: CustomKeyStoreTypeType](./literals.md#customkeystoretypetype) 
2. See [:material-code-braces: XksProxyAuthenticationCredentialTypeTypeDef](./type_defs.md#xksproxyauthenticationcredentialtypetypedef) 
3. See [:material-code-brackets: XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype) 
## UpdateCustomKeyStoreRequestRequestTypeDef

```python
# UpdateCustomKeyStoreRequestRequestTypeDef definition

class UpdateCustomKeyStoreRequestRequestTypeDef(TypedDict):
    CustomKeyStoreId: str,
    NewCustomKeyStoreName: NotRequired[str],
    KeyStorePassword: NotRequired[str],
    CloudHsmClusterId: NotRequired[str],
    XksProxyUriEndpoint: NotRequired[str],
    XksProxyUriPath: NotRequired[str],
    XksProxyVpcEndpointServiceName: NotRequired[str],
    XksProxyAuthenticationCredential: NotRequired[XksProxyAuthenticationCredentialTypeTypeDef],  # (1)
    XksProxyConnectivity: NotRequired[XksProxyConnectivityTypeType],  # (2)
```

1. See [:material-code-braces: XksProxyAuthenticationCredentialTypeTypeDef](./type_defs.md#xksproxyauthenticationcredentialtypetypedef) 
2. See [:material-code-brackets: XksProxyConnectivityTypeType](./literals.md#xksproxyconnectivitytypetype) 
## CreateGrantRequestRequestTypeDef

```python
# CreateGrantRequestRequestTypeDef definition

class CreateGrantRequestRequestTypeDef(TypedDict):
    KeyId: str,
    GranteePrincipal: str,
    Operations: Sequence[GrantOperationType],  # (1)
    RetiringPrincipal: NotRequired[str],
    Constraints: NotRequired[GrantConstraintsTypeDef],  # (2)
    GrantTokens: NotRequired[Sequence[str]],
    Name: NotRequired[str],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: GrantOperationType](./literals.md#grantoperationtype) 
2. See [:material-code-braces: GrantConstraintsTypeDef](./type_defs.md#grantconstraintstypedef) 
## CreateKeyRequestRequestTypeDef

```python
# CreateKeyRequestRequestTypeDef definition

class CreateKeyRequestRequestTypeDef(TypedDict):
    Policy: NotRequired[str],
    Description: NotRequired[str],
    KeyUsage: NotRequired[KeyUsageTypeType],  # (1)
    CustomerMasterKeySpec: NotRequired[CustomerMasterKeySpecType],  # (2)
    KeySpec: NotRequired[KeySpecType],  # (3)
    Origin: NotRequired[OriginTypeType],  # (4)
    CustomKeyStoreId: NotRequired[str],
    BypassPolicyLockoutSafetyCheck: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    MultiRegion: NotRequired[bool],
    XksKeyId: NotRequired[str],
```

1. See [:material-code-brackets: KeyUsageTypeType](./literals.md#keyusagetypetype) 
2. See [:material-code-brackets: CustomerMasterKeySpecType](./literals.md#customermasterkeyspectype) 
3. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
4. See [:material-code-brackets: OriginTypeType](./literals.md#origintypetype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListResourceTagsResponseTypeDef

```python
# ListResourceTagsResponseTypeDef definition

class ListResourceTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicateKeyRequestRequestTypeDef

```python
# ReplicateKeyRequestRequestTypeDef definition

class ReplicateKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    ReplicaRegion: str,
    Policy: NotRequired[str],
    BypassPolicyLockoutSafetyCheck: NotRequired[bool],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    KeyId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CustomKeyStoresListEntryTypeDef

```python
# CustomKeyStoresListEntryTypeDef definition

class CustomKeyStoresListEntryTypeDef(TypedDict):
    CustomKeyStoreId: NotRequired[str],
    CustomKeyStoreName: NotRequired[str],
    CloudHsmClusterId: NotRequired[str],
    TrustAnchorCertificate: NotRequired[str],
    ConnectionState: NotRequired[ConnectionStateTypeType],  # (1)
    ConnectionErrorCode: NotRequired[ConnectionErrorCodeTypeType],  # (2)
    CreationDate: NotRequired[datetime],
    CustomKeyStoreType: NotRequired[CustomKeyStoreTypeType],  # (3)
    XksProxyConfiguration: NotRequired[XksProxyConfigurationTypeTypeDef],  # (4)
```

1. See [:material-code-brackets: ConnectionStateTypeType](./literals.md#connectionstatetypetype) 
2. See [:material-code-brackets: ConnectionErrorCodeTypeType](./literals.md#connectionerrorcodetypetype) 
3. See [:material-code-brackets: CustomKeyStoreTypeType](./literals.md#customkeystoretypetype) 
4. See [:material-code-braces: XksProxyConfigurationTypeTypeDef](./type_defs.md#xksproxyconfigurationtypetypedef) 
## DescribeCustomKeyStoresRequestPaginateTypeDef

```python
# DescribeCustomKeyStoresRequestPaginateTypeDef definition

class DescribeCustomKeyStoresRequestPaginateTypeDef(TypedDict):
    CustomKeyStoreId: NotRequired[str],
    CustomKeyStoreName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAliasesRequestPaginateTypeDef

```python
# ListAliasesRequestPaginateTypeDef definition

class ListAliasesRequestPaginateTypeDef(TypedDict):
    KeyId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGrantsRequestPaginateTypeDef

```python
# ListGrantsRequestPaginateTypeDef definition

class ListGrantsRequestPaginateTypeDef(TypedDict):
    KeyId: str,
    GrantId: NotRequired[str],
    GranteePrincipal: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeyPoliciesRequestPaginateTypeDef

```python
# ListKeyPoliciesRequestPaginateTypeDef definition

class ListKeyPoliciesRequestPaginateTypeDef(TypedDict):
    KeyId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeyRotationsRequestPaginateTypeDef

```python
# ListKeyRotationsRequestPaginateTypeDef definition

class ListKeyRotationsRequestPaginateTypeDef(TypedDict):
    KeyId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeysRequestPaginateTypeDef

```python
# ListKeysRequestPaginateTypeDef definition

class ListKeysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceTagsRequestPaginateTypeDef

```python
# ListResourceTagsRequestPaginateTypeDef definition

class ListResourceTagsRequestPaginateTypeDef(TypedDict):
    KeyId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRetirableGrantsRequestPaginateTypeDef

```python
# ListRetirableGrantsRequestPaginateTypeDef definition

class ListRetirableGrantsRequestPaginateTypeDef(TypedDict):
    RetiringPrincipal: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GrantListEntryTypeDef

```python
# GrantListEntryTypeDef definition

class GrantListEntryTypeDef(TypedDict):
    KeyId: NotRequired[str],
    GrantId: NotRequired[str],
    Name: NotRequired[str],
    CreationDate: NotRequired[datetime],
    GranteePrincipal: NotRequired[str],
    RetiringPrincipal: NotRequired[str],
    IssuingAccount: NotRequired[str],
    Operations: NotRequired[List[GrantOperationType]],  # (1)
    Constraints: NotRequired[GrantConstraintsOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: GrantOperationType](./literals.md#grantoperationtype) 
2. See [:material-code-braces: GrantConstraintsOutputTypeDef](./type_defs.md#grantconstraintsoutputtypedef) 
## ImportKeyMaterialRequestRequestTypeDef

```python
# ImportKeyMaterialRequestRequestTypeDef definition

class ImportKeyMaterialRequestRequestTypeDef(TypedDict):
    KeyId: str,
    ImportToken: BlobTypeDef,
    EncryptedKeyMaterial: BlobTypeDef,
    ValidTo: NotRequired[TimestampTypeDef],
    ExpirationModel: NotRequired[ExpirationModelTypeType],  # (1)
```

1. See [:material-code-brackets: ExpirationModelTypeType](./literals.md#expirationmodeltypetype) 
## ListKeysResponseTypeDef

```python
# ListKeysResponseTypeDef definition

class ListKeysResponseTypeDef(TypedDict):
    Keys: List[KeyListEntryTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyListEntryTypeDef](./type_defs.md#keylistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyRotationsResponseTypeDef

```python
# ListKeyRotationsResponseTypeDef definition

class ListKeyRotationsResponseTypeDef(TypedDict):
    Rotations: List[RotationsListEntryTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RotationsListEntryTypeDef](./type_defs.md#rotationslistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MultiRegionConfigurationTypeDef

```python
# MultiRegionConfigurationTypeDef definition

class MultiRegionConfigurationTypeDef(TypedDict):
    MultiRegionKeyType: NotRequired[MultiRegionKeyTypeType],  # (1)
    PrimaryKey: NotRequired[MultiRegionKeyTypeDef],  # (2)
    ReplicaKeys: NotRequired[List[MultiRegionKeyTypeDef]],  # (3)
```

1. See [:material-code-brackets: MultiRegionKeyTypeType](./literals.md#multiregionkeytypetype) 
2. See [:material-code-braces: MultiRegionKeyTypeDef](./type_defs.md#multiregionkeytypedef) 
3. See [:material-code-braces: MultiRegionKeyTypeDef](./type_defs.md#multiregionkeytypedef) 
## DecryptRequestRequestTypeDef

```python
# DecryptRequestRequestTypeDef definition

class DecryptRequestRequestTypeDef(TypedDict):
    CiphertextBlob: BlobTypeDef,
    EncryptionContext: NotRequired[Mapping[str, str]],
    GrantTokens: NotRequired[Sequence[str]],
    KeyId: NotRequired[str],
    EncryptionAlgorithm: NotRequired[EncryptionAlgorithmSpecType],  # (1)
    Recipient: NotRequired[RecipientInfoTypeDef],  # (2)
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
## DeriveSharedSecretRequestRequestTypeDef

```python
# DeriveSharedSecretRequestRequestTypeDef definition

class DeriveSharedSecretRequestRequestTypeDef(TypedDict):
    KeyId: str,
    KeyAgreementAlgorithm: KeyAgreementAlgorithmSpecType,  # (1)
    PublicKey: BlobTypeDef,
    GrantTokens: NotRequired[Sequence[str]],
    DryRun: NotRequired[bool],
    Recipient: NotRequired[RecipientInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
## GenerateDataKeyPairRequestRequestTypeDef

```python
# GenerateDataKeyPairRequestRequestTypeDef definition

class GenerateDataKeyPairRequestRequestTypeDef(TypedDict):
    KeyId: str,
    KeyPairSpec: DataKeyPairSpecType,  # (1)
    EncryptionContext: NotRequired[Mapping[str, str]],
    GrantTokens: NotRequired[Sequence[str]],
    Recipient: NotRequired[RecipientInfoTypeDef],  # (2)
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: DataKeyPairSpecType](./literals.md#datakeypairspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
## GenerateDataKeyRequestRequestTypeDef

```python
# GenerateDataKeyRequestRequestTypeDef definition

class GenerateDataKeyRequestRequestTypeDef(TypedDict):
    KeyId: str,
    EncryptionContext: NotRequired[Mapping[str, str]],
    NumberOfBytes: NotRequired[int],
    KeySpec: NotRequired[DataKeySpecType],  # (1)
    GrantTokens: NotRequired[Sequence[str]],
    Recipient: NotRequired[RecipientInfoTypeDef],  # (2)
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: DataKeySpecType](./literals.md#datakeyspectype) 
2. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
## GenerateRandomRequestRequestTypeDef

```python
# GenerateRandomRequestRequestTypeDef definition

class GenerateRandomRequestRequestTypeDef(TypedDict):
    NumberOfBytes: NotRequired[int],
    CustomKeyStoreId: NotRequired[str],
    Recipient: NotRequired[RecipientInfoTypeDef],  # (1)
```

1. See [:material-code-braces: RecipientInfoTypeDef](./type_defs.md#recipientinfotypedef) 
## DescribeCustomKeyStoresResponseTypeDef

```python
# DescribeCustomKeyStoresResponseTypeDef definition

class DescribeCustomKeyStoresResponseTypeDef(TypedDict):
    CustomKeyStores: List[CustomKeyStoresListEntryTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomKeyStoresListEntryTypeDef](./type_defs.md#customkeystoreslistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGrantsResponseTypeDef

```python
# ListGrantsResponseTypeDef definition

class ListGrantsResponseTypeDef(TypedDict):
    Grants: List[GrantListEntryTypeDef],  # (1)
    NextMarker: str,
    Truncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GrantListEntryTypeDef](./type_defs.md#grantlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KeyMetadataTypeDef

```python
# KeyMetadataTypeDef definition

class KeyMetadataTypeDef(TypedDict):
    KeyId: str,
    AWSAccountId: NotRequired[str],
    Arn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    Enabled: NotRequired[bool],
    Description: NotRequired[str],
    KeyUsage: NotRequired[KeyUsageTypeType],  # (1)
    KeyState: NotRequired[KeyStateType],  # (2)
    DeletionDate: NotRequired[datetime],
    ValidTo: NotRequired[datetime],
    Origin: NotRequired[OriginTypeType],  # (3)
    CustomKeyStoreId: NotRequired[str],
    CloudHsmClusterId: NotRequired[str],
    ExpirationModel: NotRequired[ExpirationModelTypeType],  # (4)
    KeyManager: NotRequired[KeyManagerTypeType],  # (5)
    CustomerMasterKeySpec: NotRequired[CustomerMasterKeySpecType],  # (6)
    KeySpec: NotRequired[KeySpecType],  # (7)
    EncryptionAlgorithms: NotRequired[List[EncryptionAlgorithmSpecType]],  # (8)
    SigningAlgorithms: NotRequired[List[SigningAlgorithmSpecType]],  # (9)
    KeyAgreementAlgorithms: NotRequired[List[KeyAgreementAlgorithmSpecType]],  # (10)
    MultiRegion: NotRequired[bool],
    MultiRegionConfiguration: NotRequired[MultiRegionConfigurationTypeDef],  # (11)
    PendingDeletionWindowInDays: NotRequired[int],
    MacAlgorithms: NotRequired[List[MacAlgorithmSpecType]],  # (12)
    XksKeyConfiguration: NotRequired[XksKeyConfigurationTypeTypeDef],  # (13)
```

1. See [:material-code-brackets: KeyUsageTypeType](./literals.md#keyusagetypetype) 
2. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
3. See [:material-code-brackets: OriginTypeType](./literals.md#origintypetype) 
4. See [:material-code-brackets: ExpirationModelTypeType](./literals.md#expirationmodeltypetype) 
5. See [:material-code-brackets: KeyManagerTypeType](./literals.md#keymanagertypetype) 
6. See [:material-code-brackets: CustomerMasterKeySpecType](./literals.md#customermasterkeyspectype) 
7. See [:material-code-brackets: KeySpecType](./literals.md#keyspectype) 
8. See [:material-code-brackets: EncryptionAlgorithmSpecType](./literals.md#encryptionalgorithmspectype) 
9. See [:material-code-brackets: SigningAlgorithmSpecType](./literals.md#signingalgorithmspectype) 
10. See [:material-code-brackets: KeyAgreementAlgorithmSpecType](./literals.md#keyagreementalgorithmspectype) 
11. See [:material-code-braces: MultiRegionConfigurationTypeDef](./type_defs.md#multiregionconfigurationtypedef) 
12. See [:material-code-brackets: MacAlgorithmSpecType](./literals.md#macalgorithmspectype) 
13. See [:material-code-braces: XksKeyConfigurationTypeTypeDef](./type_defs.md#xkskeyconfigurationtypetypedef) 
## CreateKeyResponseTypeDef

```python
# CreateKeyResponseTypeDef definition

class CreateKeyResponseTypeDef(TypedDict):
    KeyMetadata: KeyMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyMetadataTypeDef](./type_defs.md#keymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKeyResponseTypeDef

```python
# DescribeKeyResponseTypeDef definition

class DescribeKeyResponseTypeDef(TypedDict):
    KeyMetadata: KeyMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyMetadataTypeDef](./type_defs.md#keymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicateKeyResponseTypeDef

```python
# ReplicateKeyResponseTypeDef definition

class ReplicateKeyResponseTypeDef(TypedDict):
    ReplicaKeyMetadata: KeyMetadataTypeDef,  # (1)
    ReplicaPolicy: str,
    ReplicaTags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: KeyMetadataTypeDef](./type_defs.md#keymetadatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
