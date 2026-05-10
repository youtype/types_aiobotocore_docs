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


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_acm.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime.datetime,
    str,
]
```




## AcmCertificateMetadataFilterTypeDef

```python
# AcmCertificateMetadataFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import AcmCertificateMetadataFilterTypeDef


def get_value() -> AcmCertificateMetadataFilterTypeDef:
    return {
        "Status": ...,
    }


# AcmCertificateMetadataFilterTypeDef definition

class AcmCertificateMetadataFilterTypeDef(TypedDict):
    Status: NotRequired[CertificateStatusType],  # (1)
    RenewalStatus: NotRequired[RenewalStatusType],  # (2)
    Type: NotRequired[CertificateTypeType],  # (3)
    InUse: NotRequired[bool],
    Exported: NotRequired[bool],
    ExportOption: NotRequired[CertificateExportType],  # (4)
    ManagedBy: NotRequired[CertificateManagedByType],  # (5)
    ValidationMethod: NotRequired[ValidationMethodType],  # (6)
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype)
2. See [:material-code-brackets: RenewalStatusType](./literals.md#renewalstatustype)
3. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype)
4. See [:material-code-brackets: CertificateExportType](./literals.md#certificateexporttype)
5. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)
6. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype)

## AcmCertificateMetadataTypeDef

```python
# AcmCertificateMetadataTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import AcmCertificateMetadataTypeDef


def get_value() -> AcmCertificateMetadataTypeDef:
    return {
        "CreatedAt": ...,
    }


# AcmCertificateMetadataTypeDef definition

class AcmCertificateMetadataTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime.datetime],
    Exported: NotRequired[bool],
    ImportedAt: NotRequired[datetime.datetime],
    InUse: NotRequired[bool],
    IssuedAt: NotRequired[datetime.datetime],
    RenewalEligibility: NotRequired[RenewalEligibilityType],  # (1)
    RevokedAt: NotRequired[datetime.datetime],
    Status: NotRequired[CertificateStatusType],  # (2)
    RenewalStatus: NotRequired[RenewalStatusType],  # (3)
    Type: NotRequired[CertificateTypeType],  # (4)
    ExportOption: NotRequired[CertificateExportType],  # (5)
    ManagedBy: NotRequired[CertificateManagedByType],  # (6)
    ValidationMethod: NotRequired[ValidationMethodType],  # (7)
```

1. See [:material-code-brackets: RenewalEligibilityType](./literals.md#renewaleligibilitytype)
2. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype)
3. See [:material-code-brackets: RenewalStatusType](./literals.md#renewalstatustype)
4. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype)
5. See [:material-code-brackets: CertificateExportType](./literals.md#certificateexporttype)
6. See [:material-code-brackets: CertificateManagedByType](./literals.md#certificatemanagedbytype)
7. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype)

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

## CommonNameFilterTypeDef

```python
# CommonNameFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CommonNameFilterTypeDef


def get_value() -> CommonNameFilterTypeDef:
    return {
        "Value": ...,
    }


# CommonNameFilterTypeDef definition

class CommonNameFilterTypeDef(TypedDict):
    Value: str,
    ComparisonOperator: ComparisonOperatorType,  # (1)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype)

## CustomAttributeTypeDef

```python
# CustomAttributeTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CustomAttributeTypeDef


def get_value() -> CustomAttributeTypeDef:
    return {
        "ObjectIdentifier": ...,
    }


# CustomAttributeTypeDef definition

class CustomAttributeTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
    Value: NotRequired[str],
```


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


## DnsNameFilterTypeDef

```python
# DnsNameFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DnsNameFilterTypeDef


def get_value() -> DnsNameFilterTypeDef:
    return {
        "Value": ...,
    }


# DnsNameFilterTypeDef definition

class DnsNameFilterTypeDef(TypedDict):
    Value: str,
    ComparisonOperator: ComparisonOperatorType,  # (1)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype)

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

## OtherNameTypeDef

```python
# OtherNameTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import OtherNameTypeDef


def get_value() -> OtherNameTypeDef:
    return {
        "ObjectIdentifier": ...,
    }


# OtherNameTypeDef definition

class OtherNameTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
    Value: NotRequired[str],
```


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

## CertificateMetadataTypeDef

```python
# CertificateMetadataTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateMetadataTypeDef


def get_value() -> CertificateMetadataTypeDef:
    return {
        "AcmCertificateMetadata": ...,
    }


# CertificateMetadataTypeDef definition

class CertificateMetadataTypeDef(TypedDict):
    AcmCertificateMetadata: NotRequired[AcmCertificateMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: AcmCertificateMetadataTypeDef](./type_defs.md#acmcertificatemetadatatypedef)

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

## SubjectFilterTypeDef

```python
# SubjectFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import SubjectFilterTypeDef


def get_value() -> SubjectFilterTypeDef:
    return {
        "CommonName": ...,
    }


# SubjectFilterTypeDef definition

class SubjectFilterTypeDef(TypedDict):
    CommonName: NotRequired[CommonNameFilterTypeDef],  # (1)
```

1. See [:material-code-braces: CommonNameFilterTypeDef](./type_defs.md#commonnamefiltertypedef)

## DistinguishedNameTypeDef

```python
# DistinguishedNameTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import DistinguishedNameTypeDef


def get_value() -> DistinguishedNameTypeDef:
    return {
        "CommonName": ...,
    }


# DistinguishedNameTypeDef definition

class DistinguishedNameTypeDef(TypedDict):
    CommonName: NotRequired[str],
    DomainComponents: NotRequired[list[str]],
    Country: NotRequired[str],
    CustomAttributes: NotRequired[list[CustomAttributeTypeDef]],  # (1)
    DistinguishedNameQualifier: NotRequired[str],
    GenerationQualifier: NotRequired[str],
    GivenName: NotRequired[str],
    Initials: NotRequired[str],
    Locality: NotRequired[str],
    Organization: NotRequired[str],
    OrganizationalUnit: NotRequired[str],
    Pseudonym: NotRequired[str],
    SerialNumber: NotRequired[str],
    State: NotRequired[str],
    Surname: NotRequired[str],
    Title: NotRequired[str],
```

1. See `list[CustomAttributeTypeDef]`

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

## SubjectAlternativeNameFilterTypeDef

```python
# SubjectAlternativeNameFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import SubjectAlternativeNameFilterTypeDef


def get_value() -> SubjectAlternativeNameFilterTypeDef:
    return {
        "DnsName": ...,
    }


# SubjectAlternativeNameFilterTypeDef definition

class SubjectAlternativeNameFilterTypeDef(TypedDict):
    DnsName: NotRequired[DnsNameFilterTypeDef],  # (1)
```

1. See [:material-code-braces: DnsNameFilterTypeDef](./type_defs.md#dnsnamefiltertypedef)

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

## TimestampRangeTypeDef

```python
# TimestampRangeTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import TimestampRangeTypeDef


def get_value() -> TimestampRangeTypeDef:
    return {
        "Start": ...,
    }


# TimestampRangeTypeDef definition

class TimestampRangeTypeDef(TypedDict):
    Start: NotRequired[TimestampTypeDef],
    End: NotRequired[TimestampTypeDef],
```


## GeneralNameTypeDef

```python
# GeneralNameTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import GeneralNameTypeDef


def get_value() -> GeneralNameTypeDef:
    return {
        "DirectoryName": ...,
    }


# GeneralNameTypeDef definition

class GeneralNameTypeDef(TypedDict):
    DirectoryName: NotRequired[DistinguishedNameTypeDef],  # (1)
    DnsName: NotRequired[str],
    IpAddress: NotRequired[str],
    OtherName: NotRequired[OtherNameTypeDef],  # (2)
    RegisteredId: NotRequired[str],
    Rfc822Name: NotRequired[str],
    UniformResourceIdentifier: NotRequired[str],
```

1. See [:material-code-braces: DistinguishedNameTypeDef](./type_defs.md#distinguishednametypedef)
2. See [:material-code-braces: OtherNameTypeDef](./type_defs.md#othernametypedef)

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

## X509AttributeFilterTypeDef

```python
# X509AttributeFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import X509AttributeFilterTypeDef


def get_value() -> X509AttributeFilterTypeDef:
    return {
        "Subject": ...,
    }


# X509AttributeFilterTypeDef definition

class X509AttributeFilterTypeDef(TypedDict):
    Subject: NotRequired[SubjectFilterTypeDef],  # (1)
    SubjectAlternativeName: NotRequired[SubjectAlternativeNameFilterTypeDef],  # (2)
    ExtendedKeyUsage: NotRequired[ExtendedKeyUsageNameType],  # (3)
    KeyUsage: NotRequired[KeyUsageNameType],  # (4)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (5)
    SerialNumber: NotRequired[str],
    NotAfter: NotRequired[TimestampRangeTypeDef],  # (6)
    NotBefore: NotRequired[TimestampRangeTypeDef],  # (6)
```

1. See [:material-code-braces: SubjectFilterTypeDef](./type_defs.md#subjectfiltertypedef)
2. See [:material-code-braces: SubjectAlternativeNameFilterTypeDef](./type_defs.md#subjectalternativenamefiltertypedef)
3. See [:material-code-brackets: ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype)
4. See [:material-code-brackets: KeyUsageNameType](./literals.md#keyusagenametype)
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
6. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef)
7. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef)

## X509AttributesTypeDef

```python
# X509AttributesTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import X509AttributesTypeDef


def get_value() -> X509AttributesTypeDef:
    return {
        "Issuer": ...,
    }


# X509AttributesTypeDef definition

class X509AttributesTypeDef(TypedDict):
    Issuer: NotRequired[DistinguishedNameTypeDef],  # (1)
    Subject: NotRequired[DistinguishedNameTypeDef],  # (1)
    SubjectAlternativeNames: NotRequired[list[GeneralNameTypeDef]],  # (3)
    ExtendedKeyUsages: NotRequired[list[ExtendedKeyUsageNameType]],  # (4)
    KeyAlgorithm: NotRequired[KeyAlgorithmType],  # (5)
    KeyUsages: NotRequired[list[KeyUsageNameType]],  # (6)
    SerialNumber: NotRequired[str],
    NotAfter: NotRequired[datetime.datetime],
    NotBefore: NotRequired[datetime.datetime],
```

1. See [:material-code-braces: DistinguishedNameTypeDef](./type_defs.md#distinguishednametypedef)
2. See [:material-code-braces: DistinguishedNameTypeDef](./type_defs.md#distinguishednametypedef)
3. See `list[GeneralNameTypeDef]`
4. See `list[ExtendedKeyUsageNameType]`
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
6. See `list[KeyUsageNameType]`

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

## CertificateFilterTypeDef

```python
# CertificateFilterTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateFilterTypeDef


def get_value() -> CertificateFilterTypeDef:
    return {
        "CertificateArn": ...,
    }


# CertificateFilterTypeDef definition

class CertificateFilterTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    X509AttributeFilter: NotRequired[X509AttributeFilterTypeDef],  # (1)
    AcmCertificateMetadataFilter: NotRequired[AcmCertificateMetadataFilterTypeDef],  # (2)
```

1. See [:material-code-braces: X509AttributeFilterTypeDef](./type_defs.md#x509attributefiltertypedef)
2. See [:material-code-braces: AcmCertificateMetadataFilterTypeDef](./type_defs.md#acmcertificatemetadatafiltertypedef)

## CertificateSearchResultTypeDef

```python
# CertificateSearchResultTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateSearchResultTypeDef


def get_value() -> CertificateSearchResultTypeDef:
    return {
        "CertificateArn": ...,
    }


# CertificateSearchResultTypeDef definition

class CertificateSearchResultTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    X509Attributes: NotRequired[X509AttributesTypeDef],  # (1)
    CertificateMetadata: NotRequired[CertificateMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: X509AttributesTypeDef](./type_defs.md#x509attributestypedef)
2. See [:material-code-braces: CertificateMetadataTypeDef](./type_defs.md#certificatemetadatatypedef)

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

## CertificateFilterStatementPaginatorTypeDef

```python
# CertificateFilterStatementPaginatorTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateFilterStatementPaginatorTypeDef


def get_value() -> CertificateFilterStatementPaginatorTypeDef:
    return {
        "And": ...,
    }


# CertificateFilterStatementPaginatorTypeDef definition

class CertificateFilterStatementPaginatorTypeDef(TypedDict):
    And: NotRequired[Sequence[Mapping[str, Any]]],
    Or: NotRequired[Sequence[Mapping[str, Any]]],
    Not: NotRequired[Mapping[str, Any]],
    Filter: NotRequired[CertificateFilterTypeDef],  # (1)
```

1. See [:material-code-braces: CertificateFilterTypeDef](./type_defs.md#certificatefiltertypedef)

## CertificateFilterStatementTypeDef

```python
# CertificateFilterStatementTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import CertificateFilterStatementTypeDef


def get_value() -> CertificateFilterStatementTypeDef:
    return {
        "And": ...,
    }


# CertificateFilterStatementTypeDef definition

class CertificateFilterStatementTypeDef(TypedDict):
    And: NotRequired[Sequence[Mapping[str, Any]]],
    Or: NotRequired[Sequence[Mapping[str, Any]]],
    Not: NotRequired[Mapping[str, Any]],
    Filter: NotRequired[CertificateFilterTypeDef],  # (1)
```

1. See [:material-code-braces: CertificateFilterTypeDef](./type_defs.md#certificatefiltertypedef)

## SearchCertificatesResponseTypeDef

```python
# SearchCertificatesResponseTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import SearchCertificatesResponseTypeDef


def get_value() -> SearchCertificatesResponseTypeDef:
    return {
        "Results": ...,
    }


# SearchCertificatesResponseTypeDef definition

class SearchCertificatesResponseTypeDef(TypedDict):
    Results: list[CertificateSearchResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[CertificateSearchResultTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## SearchCertificatesRequestPaginateTypeDef

```python
# SearchCertificatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import SearchCertificatesRequestPaginateTypeDef


def get_value() -> SearchCertificatesRequestPaginateTypeDef:
    return {
        "FilterStatement": ...,
    }


# SearchCertificatesRequestPaginateTypeDef definition

class SearchCertificatesRequestPaginateTypeDef(TypedDict):
    FilterStatement: NotRequired[CertificateFilterStatementPaginatorTypeDef],  # (1)
    SortBy: NotRequired[SearchCertificatesSortByType],  # (2)
    SortOrder: NotRequired[SearchCertificatesSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: CertificateFilterStatementPaginatorTypeDef](./type_defs.md#certificatefilterstatementpaginatortypedef)
2. See [:material-code-brackets: SearchCertificatesSortByType](./literals.md#searchcertificatessortbytype)
3. See [:material-code-brackets: SearchCertificatesSortOrderType](./literals.md#searchcertificatessortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## SearchCertificatesRequestTypeDef

```python
# SearchCertificatesRequestTypeDef TypedDict usage example

from types_aiobotocore_acm.type_defs import SearchCertificatesRequestTypeDef


def get_value() -> SearchCertificatesRequestTypeDef:
    return {
        "FilterStatement": ...,
    }


# SearchCertificatesRequestTypeDef definition

class SearchCertificatesRequestTypeDef(TypedDict):
    FilterStatement: NotRequired[CertificateFilterStatementTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[SearchCertificatesSortByType],  # (2)
    SortOrder: NotRequired[SearchCertificatesSortOrderType],  # (3)
```

1. See [:material-code-braces: CertificateFilterStatementTypeDef](./type_defs.md#certificatefilterstatementtypedef)
2. See [:material-code-brackets: SearchCertificatesSortByType](./literals.md#searchcertificatessortbytype)
3. See [:material-code-brackets: SearchCertificatesSortOrderType](./literals.md#searchcertificatessortordertype)

