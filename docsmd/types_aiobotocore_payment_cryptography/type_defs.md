# Type definitions

> [Index](../README.md) > [PaymentCryptographyControlPlane](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).



## AliasTypeDef

```python
# AliasTypeDef definition

class AliasTypeDef(TypedDict):
    AliasName: str,
    KeyArn: NotRequired[str],
```

## CreateAliasInputRequestTypeDef

```python
# CreateAliasInputRequestTypeDef definition

class CreateAliasInputRequestTypeDef(TypedDict):
    AliasName: str,
    KeyArn: NotRequired[str],
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteAliasInputRequestTypeDef

```python
# DeleteAliasInputRequestTypeDef definition

class DeleteAliasInputRequestTypeDef(TypedDict):
    AliasName: str,
```

## DeleteKeyInputRequestTypeDef

```python
# DeleteKeyInputRequestTypeDef definition

class DeleteKeyInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
    DeleteKeyInDays: NotRequired[int],
```

## ExportDukptInitialKeyTypeDef

```python
# ExportDukptInitialKeyTypeDef definition

class ExportDukptInitialKeyTypeDef(TypedDict):
    KeySerialNumber: str,
```

## ExportKeyCryptogramTypeDef

```python
# ExportKeyCryptogramTypeDef definition

class ExportKeyCryptogramTypeDef(TypedDict):
    CertificateAuthorityPublicKeyIdentifier: str,
    WrappingKeyCertificate: str,
    WrappingSpec: NotRequired[WrappingKeySpecType],  # (1)
```

1. See [:material-code-brackets: WrappingKeySpecType](./literals.md#wrappingkeyspectype) 
## WrappedKeyTypeDef

```python
# WrappedKeyTypeDef definition

class WrappedKeyTypeDef(TypedDict):
    WrappingKeyArn: str,
    WrappedKeyMaterialFormat: WrappedKeyMaterialFormatType,  # (1)
    KeyMaterial: str,
    KeyCheckValue: NotRequired[str],
    KeyCheckValueAlgorithm: NotRequired[KeyCheckValueAlgorithmType],  # (2)
```

1. See [:material-code-brackets: WrappedKeyMaterialFormatType](./literals.md#wrappedkeymaterialformattype) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
## GetAliasInputRequestTypeDef

```python
# GetAliasInputRequestTypeDef definition

class GetAliasInputRequestTypeDef(TypedDict):
    AliasName: str,
```

## GetKeyInputRequestTypeDef

```python
# GetKeyInputRequestTypeDef definition

class GetKeyInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
```

## GetParametersForExportInputRequestTypeDef

```python
# GetParametersForExportInputRequestTypeDef definition

class GetParametersForExportInputRequestTypeDef(TypedDict):
    KeyMaterialType: KeyMaterialTypeType,  # (1)
    SigningKeyAlgorithm: KeyAlgorithmType,  # (2)
```

1. See [:material-code-brackets: KeyMaterialTypeType](./literals.md#keymaterialtypetype) 
2. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
## GetParametersForImportInputRequestTypeDef

```python
# GetParametersForImportInputRequestTypeDef definition

class GetParametersForImportInputRequestTypeDef(TypedDict):
    KeyMaterialType: KeyMaterialTypeType,  # (1)
    WrappingKeyAlgorithm: KeyAlgorithmType,  # (2)
```

1. See [:material-code-brackets: KeyMaterialTypeType](./literals.md#keymaterialtypetype) 
2. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
## GetPublicKeyCertificateInputRequestTypeDef

```python
# GetPublicKeyCertificateInputRequestTypeDef definition

class GetPublicKeyCertificateInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
```

## ImportTr31KeyBlockTypeDef

```python
# ImportTr31KeyBlockTypeDef definition

class ImportTr31KeyBlockTypeDef(TypedDict):
    WrappingKeyIdentifier: str,
    WrappedKeyBlock: str,
```

## ImportTr34KeyBlockTypeDef

```python
# ImportTr34KeyBlockTypeDef definition

class ImportTr34KeyBlockTypeDef(TypedDict):
    CertificateAuthorityPublicKeyIdentifier: str,
    SigningKeyCertificate: str,
    ImportToken: str,
    WrappedKeyBlock: str,
    KeyBlockFormat: Tr34KeyBlockFormatType,  # (1)
    RandomNonce: NotRequired[str],
```

1. See [:material-code-brackets: Tr34KeyBlockFormatType](./literals.md#tr34keyblockformattype) 
## KeyModesOfUseTypeDef

```python
# KeyModesOfUseTypeDef definition

class KeyModesOfUseTypeDef(TypedDict):
    Encrypt: NotRequired[bool],
    Decrypt: NotRequired[bool],
    Wrap: NotRequired[bool],
    Unwrap: NotRequired[bool],
    Generate: NotRequired[bool],
    Sign: NotRequired[bool],
    Verify: NotRequired[bool],
    DeriveKey: NotRequired[bool],
    NoRestrictions: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAliasesInputRequestTypeDef

```python
# ListAliasesInputRequestTypeDef definition

class ListAliasesInputRequestTypeDef(TypedDict):
    KeyArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListKeysInputRequestTypeDef

```python
# ListKeysInputRequestTypeDef definition

class ListKeysInputRequestTypeDef(TypedDict):
    KeyState: NotRequired[KeyStateType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RestoreKeyInputRequestTypeDef

```python
# RestoreKeyInputRequestTypeDef definition

class RestoreKeyInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
```

## StartKeyUsageInputRequestTypeDef

```python
# StartKeyUsageInputRequestTypeDef definition

class StartKeyUsageInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
```

## StopKeyUsageInputRequestTypeDef

```python
# StopKeyUsageInputRequestTypeDef definition

class StopKeyUsageInputRequestTypeDef(TypedDict):
    KeyIdentifier: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateAliasInputRequestTypeDef

```python
# UpdateAliasInputRequestTypeDef definition

class UpdateAliasInputRequestTypeDef(TypedDict):
    AliasName: str,
    KeyArn: NotRequired[str],
```

## CreateAliasOutputTypeDef

```python
# CreateAliasOutputTypeDef definition

class CreateAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAliasOutputTypeDef

```python
# GetAliasOutputTypeDef definition

class GetAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersForExportOutputTypeDef

```python
# GetParametersForExportOutputTypeDef definition

class GetParametersForExportOutputTypeDef(TypedDict):
    SigningKeyCertificate: str,
    SigningKeyCertificateChain: str,
    SigningKeyAlgorithm: KeyAlgorithmType,  # (1)
    ExportToken: str,
    ParametersValidUntilTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParametersForImportOutputTypeDef

```python
# GetParametersForImportOutputTypeDef definition

class GetParametersForImportOutputTypeDef(TypedDict):
    WrappingKeyCertificate: str,
    WrappingKeyCertificateChain: str,
    WrappingKeyAlgorithm: KeyAlgorithmType,  # (1)
    ImportToken: str,
    ParametersValidUntilTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPublicKeyCertificateOutputTypeDef

```python
# GetPublicKeyCertificateOutputTypeDef definition

class GetPublicKeyCertificateOutputTypeDef(TypedDict):
    KeyCertificate: str,
    KeyCertificateChain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesOutputTypeDef

```python
# ListAliasesOutputTypeDef definition

class ListAliasesOutputTypeDef(TypedDict):
    Aliases: List[AliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAliasOutputTypeDef

```python
# UpdateAliasOutputTypeDef definition

class UpdateAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ExportAttributesTypeDef

```python
# ExportAttributesTypeDef definition

class ExportAttributesTypeDef(TypedDict):
    ExportDukptInitialKey: NotRequired[ExportDukptInitialKeyTypeDef],  # (1)
    KeyCheckValueAlgorithm: NotRequired[KeyCheckValueAlgorithmType],  # (2)
```

1. See [:material-code-braces: ExportDukptInitialKeyTypeDef](./type_defs.md#exportdukptinitialkeytypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
## ExportKeyOutputTypeDef

```python
# ExportKeyOutputTypeDef definition

class ExportKeyOutputTypeDef(TypedDict):
    WrappedKey: WrappedKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KeyAttributesTypeDef

```python
# KeyAttributesTypeDef definition

class KeyAttributesTypeDef(TypedDict):
    KeyUsage: KeyUsageType,  # (1)
    KeyClass: KeyClassType,  # (2)
    KeyAlgorithm: KeyAlgorithmType,  # (3)
    KeyModesOfUse: KeyModesOfUseTypeDef,  # (4)
```

1. See [:material-code-brackets: KeyUsageType](./literals.md#keyusagetype) 
2. See [:material-code-brackets: KeyClassType](./literals.md#keyclasstype) 
3. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
4. See [:material-code-braces: KeyModesOfUseTypeDef](./type_defs.md#keymodesofusetypedef) 
## KeyBlockHeadersTypeDef

```python
# KeyBlockHeadersTypeDef definition

class KeyBlockHeadersTypeDef(TypedDict):
    KeyModesOfUse: NotRequired[KeyModesOfUseTypeDef],  # (1)
    KeyExportability: NotRequired[KeyExportabilityType],  # (2)
    KeyVersion: NotRequired[str],
    OptionalBlocks: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KeyModesOfUseTypeDef](./type_defs.md#keymodesofusetypedef) 
2. See [:material-code-brackets: KeyExportabilityType](./literals.md#keyexportabilitytype) 
## ListAliasesInputPaginateTypeDef

```python
# ListAliasesInputPaginateTypeDef definition

class ListAliasesInputPaginateTypeDef(TypedDict):
    KeyArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeysInputPaginateTypeDef

```python
# ListKeysInputPaginateTypeDef definition

class ListKeysInputPaginateTypeDef(TypedDict):
    KeyState: NotRequired[KeyStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceInputPaginateTypeDef

```python
# ListTagsForResourceInputPaginateTypeDef definition

class ListTagsForResourceInputPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## CreateKeyInputRequestTypeDef

```python
# CreateKeyInputRequestTypeDef definition

class CreateKeyInputRequestTypeDef(TypedDict):
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    Exportable: bool,
    KeyCheckValueAlgorithm: NotRequired[KeyCheckValueAlgorithmType],  # (2)
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportKeyCryptogramTypeDef

```python
# ImportKeyCryptogramTypeDef definition

class ImportKeyCryptogramTypeDef(TypedDict):
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    Exportable: bool,
    WrappedKeyCryptogram: str,
    ImportToken: str,
    WrappingSpec: NotRequired[WrappingKeySpecType],  # (2)
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
2. See [:material-code-brackets: WrappingKeySpecType](./literals.md#wrappingkeyspectype) 
## KeySummaryTypeDef

```python
# KeySummaryTypeDef definition

class KeySummaryTypeDef(TypedDict):
    KeyArn: str,
    KeyState: KeyStateType,  # (1)
    KeyAttributes: KeyAttributesTypeDef,  # (2)
    KeyCheckValue: str,
    Exportable: bool,
    Enabled: bool,
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
2. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
## KeyTypeDef

```python
# KeyTypeDef definition

class KeyTypeDef(TypedDict):
    KeyArn: str,
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    KeyCheckValue: str,
    KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType,  # (2)
    Enabled: bool,
    Exportable: bool,
    KeyState: KeyStateType,  # (3)
    KeyOrigin: KeyOriginType,  # (4)
    CreateTimestamp: datetime,
    UsageStartTimestamp: NotRequired[datetime],
    UsageStopTimestamp: NotRequired[datetime],
    DeletePendingTimestamp: NotRequired[datetime],
    DeleteTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
3. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
4. See [:material-code-brackets: KeyOriginType](./literals.md#keyorigintype) 
## RootCertificatePublicKeyTypeDef

```python
# RootCertificatePublicKeyTypeDef definition

class RootCertificatePublicKeyTypeDef(TypedDict):
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    PublicKeyCertificate: str,
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
## TrustedCertificatePublicKeyTypeDef

```python
# TrustedCertificatePublicKeyTypeDef definition

class TrustedCertificatePublicKeyTypeDef(TypedDict):
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    PublicKeyCertificate: str,
    CertificateAuthorityPublicKeyIdentifier: str,
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
## ExportTr31KeyBlockTypeDef

```python
# ExportTr31KeyBlockTypeDef definition

class ExportTr31KeyBlockTypeDef(TypedDict):
    WrappingKeyIdentifier: str,
    KeyBlockHeaders: NotRequired[KeyBlockHeadersTypeDef],  # (1)
```

1. See [:material-code-braces: KeyBlockHeadersTypeDef](./type_defs.md#keyblockheaderstypedef) 
## ExportTr34KeyBlockTypeDef

```python
# ExportTr34KeyBlockTypeDef definition

class ExportTr34KeyBlockTypeDef(TypedDict):
    CertificateAuthorityPublicKeyIdentifier: str,
    WrappingKeyCertificate: str,
    ExportToken: str,
    KeyBlockFormat: Tr34KeyBlockFormatType,  # (1)
    RandomNonce: NotRequired[str],
    KeyBlockHeaders: NotRequired[KeyBlockHeadersTypeDef],  # (2)
```

1. See [:material-code-brackets: Tr34KeyBlockFormatType](./literals.md#tr34keyblockformattype) 
2. See [:material-code-braces: KeyBlockHeadersTypeDef](./type_defs.md#keyblockheaderstypedef) 
## ListKeysOutputTypeDef

```python
# ListKeysOutputTypeDef definition

class ListKeysOutputTypeDef(TypedDict):
    Keys: List[KeySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: KeySummaryTypeDef](./type_defs.md#keysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKeyOutputTypeDef

```python
# CreateKeyOutputTypeDef definition

class CreateKeyOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKeyOutputTypeDef

```python
# DeleteKeyOutputTypeDef definition

class DeleteKeyOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyOutputTypeDef

```python
# GetKeyOutputTypeDef definition

class GetKeyOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportKeyOutputTypeDef

```python
# ImportKeyOutputTypeDef definition

class ImportKeyOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreKeyOutputTypeDef

```python
# RestoreKeyOutputTypeDef definition

class RestoreKeyOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartKeyUsageOutputTypeDef

```python
# StartKeyUsageOutputTypeDef definition

class StartKeyUsageOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopKeyUsageOutputTypeDef

```python
# StopKeyUsageOutputTypeDef definition

class StopKeyUsageOutputTypeDef(TypedDict):
    Key: KeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyTypeDef](./type_defs.md#keytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportKeyMaterialTypeDef

```python
# ImportKeyMaterialTypeDef definition

class ImportKeyMaterialTypeDef(TypedDict):
    RootCertificatePublicKey: NotRequired[RootCertificatePublicKeyTypeDef],  # (1)
    TrustedCertificatePublicKey: NotRequired[TrustedCertificatePublicKeyTypeDef],  # (2)
    Tr31KeyBlock: NotRequired[ImportTr31KeyBlockTypeDef],  # (3)
    Tr34KeyBlock: NotRequired[ImportTr34KeyBlockTypeDef],  # (4)
    KeyCryptogram: NotRequired[ImportKeyCryptogramTypeDef],  # (5)
```

1. See [:material-code-braces: RootCertificatePublicKeyTypeDef](./type_defs.md#rootcertificatepublickeytypedef) 
2. See [:material-code-braces: TrustedCertificatePublicKeyTypeDef](./type_defs.md#trustedcertificatepublickeytypedef) 
3. See [:material-code-braces: ImportTr31KeyBlockTypeDef](./type_defs.md#importtr31keyblocktypedef) 
4. See [:material-code-braces: ImportTr34KeyBlockTypeDef](./type_defs.md#importtr34keyblocktypedef) 
5. See [:material-code-braces: ImportKeyCryptogramTypeDef](./type_defs.md#importkeycryptogramtypedef) 
## ExportKeyMaterialTypeDef

```python
# ExportKeyMaterialTypeDef definition

class ExportKeyMaterialTypeDef(TypedDict):
    Tr31KeyBlock: NotRequired[ExportTr31KeyBlockTypeDef],  # (1)
    Tr34KeyBlock: NotRequired[ExportTr34KeyBlockTypeDef],  # (2)
    KeyCryptogram: NotRequired[ExportKeyCryptogramTypeDef],  # (3)
```

1. See [:material-code-braces: ExportTr31KeyBlockTypeDef](./type_defs.md#exporttr31keyblocktypedef) 
2. See [:material-code-braces: ExportTr34KeyBlockTypeDef](./type_defs.md#exporttr34keyblocktypedef) 
3. See [:material-code-braces: ExportKeyCryptogramTypeDef](./type_defs.md#exportkeycryptogramtypedef) 
## ImportKeyInputRequestTypeDef

```python
# ImportKeyInputRequestTypeDef definition

class ImportKeyInputRequestTypeDef(TypedDict):
    KeyMaterial: ImportKeyMaterialTypeDef,  # (1)
    KeyCheckValueAlgorithm: NotRequired[KeyCheckValueAlgorithmType],  # (2)
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ImportKeyMaterialTypeDef](./type_defs.md#importkeymaterialtypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ExportKeyInputRequestTypeDef

```python
# ExportKeyInputRequestTypeDef definition

class ExportKeyInputRequestTypeDef(TypedDict):
    KeyMaterial: ExportKeyMaterialTypeDef,  # (1)
    ExportKeyIdentifier: str,
    ExportAttributes: NotRequired[ExportAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: ExportKeyMaterialTypeDef](./type_defs.md#exportkeymaterialtypedef) 
2. See [:material-code-braces: ExportAttributesTypeDef](./type_defs.md#exportattributestypedef) 
