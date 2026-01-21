# Type definitions

> [Index](../README.md) > [ACM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_acm.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    aiobotocore.response.StreamingBody,
]
```




## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```


## CertificateOptionsTypeDef

```python
# CertificateOptionsTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateOptionsTypeDef


def get_value() -> CertificateOptionsTypeDef:
    return {
        "CertificateTransparencyLoggingPreference": ...,
    }


# CertificateOptionsTypeDef definition

class CertificateOptionsTypeDef(TypedDict):
    CertificateTransparencyLoggingPreference: NotRequired[CertificateTransparencyLoggingPreferenceType],  # (1)
    Export: NotRequired[CertificateExportType],  # (2)
```

1. See [:material-code-brackets: CertificateTransparencyLoggingPreferenceType](./literals.md#certificatetransparencyloggingpreferencetype)
2. See [:material-code-brackets: CertificateExportType](./literals.md#certificateexporttype)

## ExtendedKeyUsageTypeDef

```python
# ExtendedKeyUsageTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ExtendedKeyUsageTypeDef


def get_value() -> ExtendedKeyUsageTypeDef:
    return {
        "Name": ...,
    }


# ExtendedKeyUsageTypeDef definition

class ExtendedKeyUsageTypeDef(TypedDict):
    Name: NotRequired[ExtendedKeyUsageNameType],  # (1)
    OID: NotRequired[str],
```

1. See [:material-code-brackets: ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype)

## KeyUsageTypeDef

```python
# KeyUsageTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import KeyUsageTypeDef


def get_value() -> KeyUsageTypeDef:
    return {
        "Name": ...,
    }


# KeyUsageTypeDef definition

class KeyUsageTypeDef(TypedDict):
    Name: NotRequired[KeyUsageNameType],  # (1)
```

1. See [:material-code-brackets: KeyUsageNameType](./literals.md#keyusagenametype)

## CertificateSummaryTypeDef

```python
# CertificateSummaryTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateSummaryTypeDef


def get_value() -> CertificateSummaryTypeDef:
    return {
        "CertificateArn": ...,
    }


# CertificateSummaryTypeDef definition

class CertificateSummaryTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DomainName: NotRequired[str],
    SubjectAlternativeNameSummaries: NotRequired[list[str]],
    HasAdditionalSubjectAlternativeNames: NotRequired[bool],
    Status: NotRequired[CertificateStatusType],  # (1)
    Type: NotRequired[CertificateTypeType],  # (2)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (3)
    KeyUsages: NotRequired[list[KeyUsageNameType]],  # (4)
    ExtendedKeyUsages: NotRequired[list[ExtendedKeyUsageNameType]],  # (5)
    ExportOption: NotRequired[CertificateExportType],  # (6)
    InUse: NotRequired[bool],
    Exported: NotRequired[bool],
    RenewalEligibility: NotRequired[RenewalEligibilityType],  # (7)
    NotBefore: NotRequired[datetime.datetime],
    NotAfter: NotRequired[datetime.datetime],
    CreatedAt: NotRequired[datetime.datetime],
    IssuedAt: NotRequired[datetime.datetime],
    ImportedAt: NotRequired[datetime.datetime],
    RevokedAt: NotRequired[datetime.datetime],
    ManagedBy: NotRequired[CertificateManagedByType],  # (8)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype)
2. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype)
3. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
4. See `list[KeyUsageNameType]`
5. See `list[ExtendedKeyUsageNameType]`
6. See [:material-code-brackets: CertificateExportType](./literals.md#certificateexporttype)
7. See [:material-code-brackets: RenewalEligibilityType](./literals.md#renewaleligibilitytype)
8. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)

## DeleteCertificateRequestTypeDef

```python
# DeleteCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DeleteCertificateRequestTypeDef


def get_value() -> DeleteCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# DeleteCertificateRequestTypeDef definition

class DeleteCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
```


## DescribeCertificateRequestTypeDef

```python
# DescribeCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DescribeCertificateRequestTypeDef


def get_value() -> DescribeCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# DescribeCertificateRequestTypeDef definition

class DescribeCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
```


## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## DomainValidationOptionTypeDef

```python
# DomainValidationOptionTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DomainValidationOptionTypeDef


def get_value() -> DomainValidationOptionTypeDef:
    return {
        "DomainName": ...,
    }


# DomainValidationOptionTypeDef definition

class DomainValidationOptionTypeDef(TypedDict):
    DomainName: str,
    ValidationDomain: str,
```


## HttpRedirectTypeDef

```python
# HttpRedirectTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import HttpRedirectTypeDef


def get_value() -> HttpRedirectTypeDef:
    return {
        "RedirectFrom": ...,
    }


# HttpRedirectTypeDef definition

class HttpRedirectTypeDef(TypedDict):
    RedirectFrom: NotRequired[str],
    RedirectTo: NotRequired[str],
```


## ResourceRecordTypeDef

```python
# ResourceRecordTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ResourceRecordTypeDef


def get_value() -> ResourceRecordTypeDef:
    return {
        "Name": ...,
    }


# ResourceRecordTypeDef definition

class ResourceRecordTypeDef(TypedDict):
    Name: str,
    Type: RecordTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: RecordTypeType](./literals.md#recordtypetype)

## ExpiryEventsConfigurationTypeDef

```python
# ExpiryEventsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ExpiryEventsConfigurationTypeDef


def get_value() -> ExpiryEventsConfigurationTypeDef:
    return {
        "DaysBeforeExpiry": ...,
    }


# ExpiryEventsConfigurationTypeDef definition

class ExpiryEventsConfigurationTypeDef(TypedDict):
    DaysBeforeExpiry: NotRequired[int],
```


## FiltersTypeDef

```python
# FiltersTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import FiltersTypeDef


def get_value() -> FiltersTypeDef:
    return {
        "extendedKeyUsage": ...,
    }


# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    extendedKeyUsage: NotRequired[Sequence[ExtendedKeyUsageNameType]],  # (1)
    keyUsage: NotRequired[Sequence[KeyUsageNameType]],  # (2)
    keyTypes: NotRequired[Sequence[KeyAlgorithmType]],  # (3)
    exportOption: NotRequired[CertificateExportType],  # (4)
    managedBy: NotRequired[CertificateManagedByType],  # (5)
```

1. See `Sequence[ExtendedKeyUsageNameType]`
2. See `Sequence[KeyUsageNameType]`
3. See `Sequence[KeyAlgorithmType]`
4. See [:material-code-brackets: CertificateExportType](./literals.md#certificateexporttype)
5. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)

## GetCertificateRequestTypeDef

```python
# GetCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import GetCertificateRequestTypeDef


def get_value() -> GetCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# GetCertificateRequestTypeDef definition

class GetCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import PaginatorConfigTypeDef


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


## ListTagsForCertificateRequestTypeDef

```python
# ListTagsForCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ListTagsForCertificateRequestTypeDef


def get_value() -> ListTagsForCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# ListTagsForCertificateRequestTypeDef definition

class ListTagsForCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
```


## RenewCertificateRequestTypeDef

```python
# RenewCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RenewCertificateRequestTypeDef


def get_value() -> RenewCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# RenewCertificateRequestTypeDef definition

class RenewCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
```


## ResendValidationEmailRequestTypeDef

```python
# ResendValidationEmailRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ResendValidationEmailRequestTypeDef


def get_value() -> ResendValidationEmailRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# ResendValidationEmailRequestTypeDef definition

class ResendValidationEmailRequestTypeDef(TypedDict):
    CertificateArn: str,
    Domain: str,
    ValidationDomain: str,
```


## RevokeCertificateRequestTypeDef

```python
# RevokeCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RevokeCertificateRequestTypeDef


def get_value() -> RevokeCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# RevokeCertificateRequestTypeDef definition

class RevokeCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
    RevocationReason: RevocationReasonType,  # (1)
```

1. See [:material-code-brackets: RevocationReasonType](./literals.md#revocationreasontype)

## AddTagsToCertificateRequestTypeDef

```python
# AddTagsToCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import AddTagsToCertificateRequestTypeDef


def get_value() -> AddTagsToCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# AddTagsToCertificateRequestTypeDef definition

class AddTagsToCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See `Sequence[TagTypeDef]`

## RemoveTagsFromCertificateRequestTypeDef

```python
# RemoveTagsFromCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RemoveTagsFromCertificateRequestTypeDef


def get_value() -> RemoveTagsFromCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# RemoveTagsFromCertificateRequestTypeDef definition

class RemoveTagsFromCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See `Sequence[TagTypeDef]`

## ExportCertificateRequestTypeDef

```python
# ExportCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ExportCertificateRequestTypeDef


def get_value() -> ExportCertificateRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# ExportCertificateRequestTypeDef definition

class ExportCertificateRequestTypeDef(TypedDict):
    CertificateArn: str,
    Passphrase: BlobTypeDef,
```


## ImportCertificateRequestTypeDef

```python
# ImportCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ImportCertificateRequestTypeDef


def get_value() -> ImportCertificateRequestTypeDef:
    return {
        "Certificate": ...,
    }


# ImportCertificateRequestTypeDef definition

class ImportCertificateRequestTypeDef(TypedDict):
    Certificate: BlobTypeDef,
    PrivateKey: BlobTypeDef,
    CertificateArn: NotRequired[str],
    CertificateChain: NotRequired[BlobTypeDef],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See `Sequence[TagTypeDef]`

## UpdateCertificateOptionsRequestTypeDef

```python
# UpdateCertificateOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import UpdateCertificateOptionsRequestTypeDef


def get_value() -> UpdateCertificateOptionsRequestTypeDef:
    return {
        "CertificateArn": ...,
    }


# UpdateCertificateOptionsRequestTypeDef definition

class UpdateCertificateOptionsRequestTypeDef(TypedDict):
    CertificateArn: str,
    Options: CertificateOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)

## DescribeCertificateRequestWaitTypeDef

```python
# DescribeCertificateRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DescribeCertificateRequestWaitTypeDef


def get_value() -> DescribeCertificateRequestWaitTypeDef:
    return {
        "CertificateArn": ...,
    }


# DescribeCertificateRequestWaitTypeDef definition

class DescribeCertificateRequestWaitTypeDef(TypedDict):
    CertificateArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ExportCertificateResponseTypeDef

```python
# ExportCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ExportCertificateResponseTypeDef


def get_value() -> ExportCertificateResponseTypeDef:
    return {
        "Certificate": ...,
    }


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
# GetCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import GetCertificateResponseTypeDef


def get_value() -> GetCertificateResponseTypeDef:
    return {
        "Certificate": ...,
    }


# GetCertificateResponseTypeDef definition

class GetCertificateResponseTypeDef(TypedDict):
    Certificate: str,
    CertificateChain: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ImportCertificateResponseTypeDef

```python
# ImportCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ImportCertificateResponseTypeDef


def get_value() -> ImportCertificateResponseTypeDef:
    return {
        "CertificateArn": ...,
    }


# ImportCertificateResponseTypeDef definition

class ImportCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListCertificatesResponseTypeDef

```python
# ListCertificatesResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ListCertificatesResponseTypeDef


def get_value() -> ListCertificatesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListCertificatesResponseTypeDef definition

class ListCertificatesResponseTypeDef(TypedDict):
    CertificateSummaryList: list[CertificateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[CertificateSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForCertificateResponseTypeDef

```python
# ListTagsForCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ListTagsForCertificateResponseTypeDef


def get_value() -> ListTagsForCertificateResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForCertificateResponseTypeDef definition

class ListTagsForCertificateResponseTypeDef(TypedDict):
    Tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[TagTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RequestCertificateResponseTypeDef

```python
# RequestCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RequestCertificateResponseTypeDef


def get_value() -> RequestCertificateResponseTypeDef:
    return {
        "CertificateArn": ...,
    }


# RequestCertificateResponseTypeDef definition

class RequestCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RevokeCertificateResponseTypeDef

```python
# RevokeCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RevokeCertificateResponseTypeDef


def get_value() -> RevokeCertificateResponseTypeDef:
    return {
        "CertificateArn": ...,
    }


# RevokeCertificateResponseTypeDef definition

class RevokeCertificateResponseTypeDef(TypedDict):
    CertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RequestCertificateRequestTypeDef

```python
# RequestCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RequestCertificateRequestTypeDef


def get_value() -> RequestCertificateRequestTypeDef:
    return {
        "DomainName": ...,
    }


# RequestCertificateRequestTypeDef definition

class RequestCertificateRequestTypeDef(TypedDict):
    DomainName: str,
    ValidationMethod: NotRequired[ValidationMethodType],  # (1)
    SubjectAlternativeNames: NotRequired[Sequence[str]],
    IdempotencyToken: NotRequired[str],
    DomainValidationOptions: NotRequired[Sequence[DomainValidationOptionTypeDef]],  # (2)
    Options: NotRequired[CertificateOptionsTypeDef],  # (3)
    CertificateAuthorityArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (5)
    ManagedBy: NotRequired[CertificateManagedByType],  # (6)
```

1. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype)
2. See `Sequence[DomainValidationOptionTypeDef]`
3. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)
4. See `Sequence[TagTypeDef]`
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
6. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)

## DomainValidationTypeDef

```python
# DomainValidationTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DomainValidationTypeDef


def get_value() -> DomainValidationTypeDef:
    return {
        "DomainName": ...,
    }


# DomainValidationTypeDef definition

class DomainValidationTypeDef(TypedDict):
    DomainName: str,
    ValidationEmails: NotRequired[list[str]],
    ValidationDomain: NotRequired[str],
    ValidationStatus: NotRequired[DomainStatusType],  # (1)
    ResourceRecord: NotRequired[ResourceRecordTypeDef],  # (2)
    HttpRedirect: NotRequired[HttpRedirectTypeDef],  # (3)
    ValidationMethod: NotRequired[ValidationMethodType],  # (4)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype)
2. See [:material-code-braces: ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef)
3. See [:material-code-braces: HttpRedirectTypeDef](./type_defs.md#httpredirecttypedef)
4. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype)

## GetAccountConfigurationResponseTypeDef

```python
# GetAccountConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import GetAccountConfigurationResponseTypeDef


def get_value() -> GetAccountConfigurationResponseTypeDef:
    return {
        "ExpiryEvents": ...,
    }


# GetAccountConfigurationResponseTypeDef definition

class GetAccountConfigurationResponseTypeDef(TypedDict):
    ExpiryEvents: ExpiryEventsConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutAccountConfigurationRequestTypeDef

```python
# PutAccountConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import PutAccountConfigurationRequestTypeDef


def get_value() -> PutAccountConfigurationRequestTypeDef:
    return {
        "IdempotencyToken": ...,
    }


# PutAccountConfigurationRequestTypeDef definition

class PutAccountConfigurationRequestTypeDef(TypedDict):
    IdempotencyToken: str,
    ExpiryEvents: NotRequired[ExpiryEventsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef)

## ListCertificatesRequestTypeDef

```python
# ListCertificatesRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ListCertificatesRequestTypeDef


def get_value() -> ListCertificatesRequestTypeDef:
    return {
        "CertificateStatuses": ...,
    }


# ListCertificatesRequestTypeDef definition

class ListCertificatesRequestTypeDef(TypedDict):
    CertificateStatuses: NotRequired[Sequence[CertificateStatusType]],  # (1)
    Includes: NotRequired[FiltersTypeDef],  # (2)
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
    SortBy: NotRequired[SortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
```

1. See `Sequence[CertificateStatusType]`
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype)
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)

## ListCertificatesRequestPaginateTypeDef

```python
# ListCertificatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import ListCertificatesRequestPaginateTypeDef


def get_value() -> ListCertificatesRequestPaginateTypeDef:
    return {
        "CertificateStatuses": ...,
    }


# ListCertificatesRequestPaginateTypeDef definition

class ListCertificatesRequestPaginateTypeDef(TypedDict):
    CertificateStatuses: NotRequired[Sequence[CertificateStatusType]],  # (1)
    Includes: NotRequired[FiltersTypeDef],  # (2)
    SortBy: NotRequired[SortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See `Sequence[CertificateStatusType]`
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype)
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## RenewalSummaryTypeDef

```python
# RenewalSummaryTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import RenewalSummaryTypeDef


def get_value() -> RenewalSummaryTypeDef:
    return {
        "RenewalStatus": ...,
    }


# RenewalSummaryTypeDef definition

class RenewalSummaryTypeDef(TypedDict):
    RenewalStatus: RenewalStatusType,  # (1)
    DomainValidationOptions: list[DomainValidationTypeDef],  # (2)
    UpdatedAt: datetime.datetime,
    RenewalStatusReason: NotRequired[FailureReasonType],  # (3)
```

1. See [:material-code-brackets: RenewalStatusType](./literals.md#renewalstatustype)
2. See `list[DomainValidationTypeDef]`
3. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype)

## CertificateDetailTypeDef

```python
# CertificateDetailTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateDetailTypeDef


def get_value() -> CertificateDetailTypeDef:
    return {
        "CertificateArn": ...,
    }


# CertificateDetailTypeDef definition

class CertificateDetailTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DomainName: NotRequired[str],
    SubjectAlternativeNames: NotRequired[list[str]],
    ManagedBy: NotRequired[CertificateManagedByType],  # (1)
    DomainValidationOptions: NotRequired[list[DomainValidationTypeDef]],  # (2)
    Serial: NotRequired[str],
    Subject: NotRequired[str],
    Issuer: NotRequired[str],
    CreatedAt: NotRequired[datetime.datetime],
    IssuedAt: NotRequired[datetime.datetime],
    ImportedAt: NotRequired[datetime.datetime],
    Status: NotRequired[CertificateStatusType],  # (3)
    RevokedAt: NotRequired[datetime.datetime],
    RevocationReason: NotRequired[RevocationReasonType],  # (4)
    NotBefore: NotRequired[datetime.datetime],
    NotAfter: NotRequired[datetime.datetime],
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (5)
    SignatureAlgorithm: NotRequired[str],
    InUseBy: NotRequired[list[str]],
    FailureReason: NotRequired[FailureReasonType],  # (6)
    Type: NotRequired[CertificateTypeType],  # (7)
    RenewalSummary: NotRequired[RenewalSummaryTypeDef],  # (8)
    KeyUsages: NotRequired[list[KeyUsageTypeDef]],  # (9)
    ExtendedKeyUsages: NotRequired[list[ExtendedKeyUsageTypeDef]],  # (10)
    CertificateAuthorityArn: NotRequired[str],
    RenewalEligibility: NotRequired[RenewalEligibilityType],  # (11)
    Options: NotRequired[CertificateOptionsTypeDef],  # (12)
```

1. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)
2. See `list[DomainValidationTypeDef]`
3. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype)
4. See [:material-code-brackets: RevocationReasonType](./literals.md#revocationreasontype)
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
6. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype)
7. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype)
8. See [:material-code-braces: RenewalSummaryTypeDef](./type_defs.md#renewalsummarytypedef)
9. See `list[KeyUsageTypeDef]`
10. See `list[ExtendedKeyUsageTypeDef]`
11. See [:material-code-brackets: RenewalEligibilityType](./literals.md#renewaleligibilitytype)
12. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)

## DescribeCertificateResponseTypeDef

```python
# DescribeCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DescribeCertificateResponseTypeDef


def get_value() -> DescribeCertificateResponseTypeDef:
    return {
        "Certificate": ...,
    }


# DescribeCertificateResponseTypeDef definition

class DescribeCertificateResponseTypeDef(TypedDict):
    Certificate: CertificateDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateDetailTypeDef](./type_defs.md#certificatedetailtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

