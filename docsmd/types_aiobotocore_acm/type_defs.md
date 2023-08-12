# Type definitions

> [Index](../README.md) > [ACM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

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




## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## CertificateOptionsTypeDef

```python
# CertificateOptionsTypeDef definition

class CertificateOptionsTypeDef(TypedDict):
    CertificateTransparencyLoggingPreference: NotRequired[CertificateTransparencyLoggingPreferenceType],  # (1)
```

1. See [:material-code-brackets: CertificateTransparencyLoggingPreferenceType](./literals.md#certificatetransparencyloggingpreferencetype) 
## ExtendedKeyUsageTypeDef

```python
# ExtendedKeyUsageTypeDef definition

class ExtendedKeyUsageTypeDef(TypedDict):
    Name: NotRequired[ExtendedKeyUsageNameType],  # (1)
    OID: NotRequired[str],
```

1. See [:material-code-brackets: ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype) 
## KeyUsageTypeDef

```python
# KeyUsageTypeDef definition

class KeyUsageTypeDef(TypedDict):
    Name: NotRequired[KeyUsageNameType],  # (1)
```

1. See [:material-code-brackets: KeyUsageNameType](./literals.md#keyusagenametype) 
## CertificateSummaryTypeDef

```python
# CertificateSummaryTypeDef definition

class CertificateSummaryTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DomainName: NotRequired[str],
    SubjectAlternativeNameSummaries: NotRequired[List[str]],
    HasAdditionalSubjectAlternativeNames: NotRequired[bool],
    Status: NotRequired[CertificateStatusType],  # (1)
    Type: NotRequired[CertificateTypeType],  # (2)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (3)
    KeyUsages: NotRequired[List[KeyUsageNameType]],  # (4)
    ExtendedKeyUsages: NotRequired[List[ExtendedKeyUsageNameType]],  # (5)
    InUse: NotRequired[bool],
    Exported: NotRequired[bool],
    RenewalEligibility: NotRequired[RenewalEligibilityType],  # (6)
    NotBefore: NotRequired[datetime],
    NotAfter: NotRequired[datetime],
    CreatedAt: NotRequired[datetime],
    IssuedAt: NotRequired[datetime],
    ImportedAt: NotRequired[datetime],
    RevokedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype) 
3. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
4. See [:material-code-brackets: KeyUsageNameType](./literals.md#keyusagenametype) 
5. See [:material-code-brackets: ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype) 
6. See [:material-code-brackets: RenewalEligibilityType](./literals.md#renewaleligibilitytype) 
## DeleteCertificateRequestRequestTypeDef

```python
# DeleteCertificateRequestRequestTypeDef definition

class DeleteCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeCertificateRequestRequestTypeDef

```python
# DescribeCertificateRequestRequestTypeDef definition

class DescribeCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
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

## DomainValidationOptionTypeDef

```python
# DomainValidationOptionTypeDef definition

class DomainValidationOptionTypeDef(TypedDict):
    DomainName: str,
    ValidationDomain: str,
```

## ResourceRecordTypeDef

```python
# ResourceRecordTypeDef definition

class ResourceRecordTypeDef(TypedDict):
    Name: str,
    Type: RecordTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: RecordTypeType](./literals.md#recordtypetype) 
## ExpiryEventsConfigurationTypeDef

```python
# ExpiryEventsConfigurationTypeDef definition

class ExpiryEventsConfigurationTypeDef(TypedDict):
    DaysBeforeExpiry: NotRequired[int],
```

## FiltersTypeDef

```python
# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    extendedKeyUsage: NotRequired[Sequence[ExtendedKeyUsageNameType]],  # (1)
    keyUsage: NotRequired[Sequence[KeyUsageNameType]],  # (2)
    keyTypes: NotRequired[Sequence[KeyAlgorithmType]],  # (3)
```

1. See [:material-code-brackets: ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype) 
2. See [:material-code-brackets: KeyUsageNameType](./literals.md#keyusagenametype) 
3. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
## GetCertificateRequestRequestTypeDef

```python
# GetCertificateRequestRequestTypeDef definition

class GetCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTagsForCertificateRequestRequestTypeDef

```python
# ListTagsForCertificateRequestRequestTypeDef definition

class ListTagsForCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
```

## RenewCertificateRequestRequestTypeDef

```python
# RenewCertificateRequestRequestTypeDef definition

class RenewCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
```

## ResendValidationEmailRequestRequestTypeDef

```python
# ResendValidationEmailRequestRequestTypeDef definition

class ResendValidationEmailRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
    Domain: str,
    ValidationDomain: str,
```

## AddTagsToCertificateRequestRequestTypeDef

```python
# AddTagsToCertificateRequestRequestTypeDef definition

class AddTagsToCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RemoveTagsFromCertificateRequestRequestTypeDef

```python
# RemoveTagsFromCertificateRequestRequestTypeDef definition

class RemoveTagsFromCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ExportCertificateRequestRequestTypeDef

```python
# ExportCertificateRequestRequestTypeDef definition

class ExportCertificateRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
    Passphrase: Union[str, bytes, IO[Any], StreamingBody],
```

## ImportCertificateRequestRequestTypeDef

```python
# ImportCertificateRequestRequestTypeDef definition

class ImportCertificateRequestRequestTypeDef(TypedDict):
    Certificate: Union[str, bytes, IO[Any], StreamingBody],
    PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
    CertificateArn: NotRequired[str],
    CertificateChain: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateCertificateOptionsRequestRequestTypeDef

```python
# UpdateCertificateOptionsRequestRequestTypeDef definition

class UpdateCertificateOptionsRequestRequestTypeDef(TypedDict):
    CertificateArn: str,
    Options: CertificateOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef) 
## DescribeCertificateRequestCertificateValidatedWaitTypeDef

```python
# DescribeCertificateRequestCertificateValidatedWaitTypeDef definition

class DescribeCertificateRequestCertificateValidatedWaitTypeDef(TypedDict):
    CertificateArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportCertificateResponseTypeDef

```python
# ExportCertificateResponseTypeDef definition

class ExportCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    CertificateChain: str,
    PrivateKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCertificateResponseTypeDef

```python
# GetCertificateResponseTypeDef definition

class GetCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    CertificateChain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportCertificateResponseTypeDef

```python
# ImportCertificateResponseTypeDef definition

class ImportCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCertificatesResponseTypeDef

```python
# ListCertificatesResponseTypeDef definition

class ListCertificatesResponseTypeDef(TypedDict):
    NextToken: str,
    CertificateSummaryList: List[CertificateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForCertificateResponseTypeDef

```python
# ListTagsForCertificateResponseTypeDef definition

class ListTagsForCertificateResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestCertificateResponseTypeDef

```python
# RequestCertificateResponseTypeDef definition

class RequestCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestCertificateRequestRequestTypeDef

```python
# RequestCertificateRequestRequestTypeDef definition

class RequestCertificateRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ValidationMethod: NotRequired[ValidationMethodType],  # (1)
    SubjectAlternativeNames: NotRequired[Sequence[str]],
    IdempotencyToken: NotRequired[str],
    DomainValidationOptions: NotRequired[Sequence[DomainValidationOptionTypeDef]],  # (2)
    Options: NotRequired[CertificateOptionsTypeDef],  # (3)
    CertificateAuthorityArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (5)
```

1. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype) 
2. See [:material-code-braces: DomainValidationOptionTypeDef](./type_defs.md#domainvalidationoptiontypedef) 
3. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
## DomainValidationTypeDef

```python
# DomainValidationTypeDef definition

class DomainValidationTypeDef(TypedDict):
    DomainName: str,
    ValidationEmails: NotRequired[List[str]],
    ValidationDomain: NotRequired[str],
    ValidationStatus: NotRequired[DomainStatusType],  # (1)
    ResourceRecord: NotRequired[ResourceRecordTypeDef],  # (2)
    ValidationMethod: NotRequired[ValidationMethodType],  # (3)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef) 
3. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype) 
## GetAccountConfigurationResponseTypeDef

```python
# GetAccountConfigurationResponseTypeDef definition

class GetAccountConfigurationResponseTypeDef(TypedDict):
    ExpiryEvents: ExpiryEventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountConfigurationRequestRequestTypeDef

```python
# PutAccountConfigurationRequestRequestTypeDef definition

class PutAccountConfigurationRequestRequestTypeDef(TypedDict):
    IdempotencyToken: str,
    ExpiryEvents: NotRequired[ExpiryEventsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef) 
## ListCertificatesRequestRequestTypeDef

```python
# ListCertificatesRequestRequestTypeDef definition

class ListCertificatesRequestRequestTypeDef(TypedDict):
    CertificateStatuses: NotRequired[Sequence[CertificateStatusType]],  # (1)
    Includes: NotRequired[FiltersTypeDef],  # (2)
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
    SortBy: NotRequired[SortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListCertificatesRequestListCertificatesPaginateTypeDef

```python
# ListCertificatesRequestListCertificatesPaginateTypeDef definition

class ListCertificatesRequestListCertificatesPaginateTypeDef(TypedDict):
    CertificateStatuses: NotRequired[Sequence[CertificateStatusType]],  # (1)
    Includes: NotRequired[FiltersTypeDef],  # (2)
    SortBy: NotRequired[SortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RenewalSummaryTypeDef

```python
# RenewalSummaryTypeDef definition

class RenewalSummaryTypeDef(TypedDict):
    RenewalStatus: RenewalStatusType,  # (1)
    DomainValidationOptions: List[DomainValidationTypeDef],  # (2)
    UpdatedAt: datetime,
    RenewalStatusReason: NotRequired[FailureReasonType],  # (3)
```

1. See [:material-code-brackets: RenewalStatusType](./literals.md#renewalstatustype) 
2. See [:material-code-braces: DomainValidationTypeDef](./type_defs.md#domainvalidationtypedef) 
3. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
## CertificateDetailTypeDef

```python
# CertificateDetailTypeDef definition

class CertificateDetailTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DomainName: NotRequired[str],
    SubjectAlternativeNames: NotRequired[List[str]],
    DomainValidationOptions: NotRequired[List[DomainValidationTypeDef]],  # (1)
    Serial: NotRequired[str],
    Subject: NotRequired[str],
    Issuer: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    IssuedAt: NotRequired[datetime],
    ImportedAt: NotRequired[datetime],
    Status: NotRequired[CertificateStatusType],  # (2)
    RevokedAt: NotRequired[datetime],
    RevocationReason: NotRequired[RevocationReasonType],  # (3)
    NotBefore: NotRequired[datetime],
    NotAfter: NotRequired[datetime],
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (4)
    SignatureAlgorithm: NotRequired[str],
    InUseBy: NotRequired[List[str]],
    FailureReason: NotRequired[FailureReasonType],  # (5)
    Type: NotRequired[CertificateTypeType],  # (6)
    RenewalSummary: NotRequired[RenewalSummaryTypeDef],  # (7)
    KeyUsages: NotRequired[List[KeyUsageTypeDef]],  # (8)
    ExtendedKeyUsages: NotRequired[List[ExtendedKeyUsageTypeDef]],  # (9)
    CertificateAuthorityArn: NotRequired[str],
    RenewalEligibility: NotRequired[RenewalEligibilityType],  # (10)
    Options: NotRequired[CertificateOptionsTypeDef],  # (11)
```

1. See [:material-code-braces: DomainValidationTypeDef](./type_defs.md#domainvalidationtypedef) 
2. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
3. See [:material-code-brackets: RevocationReasonType](./literals.md#revocationreasontype) 
4. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
5. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
6. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype) 
7. See [:material-code-braces: RenewalSummaryTypeDef](./type_defs.md#renewalsummarytypedef) 
8. See [:material-code-braces: KeyUsageTypeDef](./type_defs.md#keyusagetypedef) 
9. See [:material-code-braces: ExtendedKeyUsageTypeDef](./type_defs.md#extendedkeyusagetypedef) 
10. See [:material-code-brackets: RenewalEligibilityType](./literals.md#renewaleligibilitytype) 
11. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef) 
## DescribeCertificateResponseTypeDef

```python
# DescribeCertificateResponseTypeDef definition

class DescribeCertificateResponseTypeDef(TypedDict):
    Certificate: CertificateDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateDetailTypeDef](./type_defs.md#certificatedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
