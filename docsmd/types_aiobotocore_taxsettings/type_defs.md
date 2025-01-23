# Type definitions

> [Index](../README.md) > [TaxSettings](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

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


## MalaysiaAdditionalInfoUnionTypeDef

```python
# MalaysiaAdditionalInfoUnionTypeDef definition

MalaysiaAdditionalInfoUnionTypeDef = Union[
    MalaysiaAdditionalInfoTypeDef,  # (1)
    MalaysiaAdditionalInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MalaysiaAdditionalInfoTypeDef](./type_defs.md#malaysiaadditionalinfotypedef) 
2. See [:material-code-braces: MalaysiaAdditionalInfoOutputTypeDef](./type_defs.md#malaysiaadditionalinfooutputtypedef) 



## TaxInheritanceDetailsTypeDef

```python
# TaxInheritanceDetailsTypeDef definition

class TaxInheritanceDetailsTypeDef(TypedDict):
    inheritanceObtainedReason: NotRequired[str],
    parentEntityId: NotRequired[str],
```

## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    addressLine1: str,
    city: str,
    countryCode: str,
    postalCode: str,
    addressLine2: NotRequired[str],
    addressLine3: NotRequired[str],
    districtOrCounty: NotRequired[str],
    stateOrRegion: NotRequired[str],
```

## JurisdictionTypeDef

```python
# JurisdictionTypeDef definition

class JurisdictionTypeDef(TypedDict):
    countryCode: str,
    stateOrRegion: NotRequired[str],
```

## CanadaAdditionalInfoTypeDef

```python
# CanadaAdditionalInfoTypeDef definition

class CanadaAdditionalInfoTypeDef(TypedDict):
    canadaQuebecSalesTaxNumber: NotRequired[str],
    canadaRetailSalesTaxNumber: NotRequired[str],
    isResellerAccount: NotRequired[bool],
    provincialSalesTaxId: NotRequired[str],
```

## EstoniaAdditionalInfoTypeDef

```python
# EstoniaAdditionalInfoTypeDef definition

class EstoniaAdditionalInfoTypeDef(TypedDict):
    registryCommercialCode: str,
```

## GeorgiaAdditionalInfoTypeDef

```python
# GeorgiaAdditionalInfoTypeDef definition

class GeorgiaAdditionalInfoTypeDef(TypedDict):
    personType: PersonTypeType,  # (1)
```

1. See [:material-code-brackets: PersonTypeType](./literals.md#persontypetype) 
## IsraelAdditionalInfoTypeDef

```python
# IsraelAdditionalInfoTypeDef definition

class IsraelAdditionalInfoTypeDef(TypedDict):
    customerType: IsraelCustomerTypeType,  # (1)
    dealerType: IsraelDealerTypeType,  # (2)
```

1. See [:material-code-brackets: IsraelCustomerTypeType](./literals.md#israelcustomertypetype) 
2. See [:material-code-brackets: IsraelDealerTypeType](./literals.md#israeldealertypetype) 
## ItalyAdditionalInfoTypeDef

```python
# ItalyAdditionalInfoTypeDef definition

class ItalyAdditionalInfoTypeDef(TypedDict):
    cigNumber: NotRequired[str],
    cupNumber: NotRequired[str],
    sdiAccountId: NotRequired[str],
    taxCode: NotRequired[str],
```

## KenyaAdditionalInfoTypeDef

```python
# KenyaAdditionalInfoTypeDef definition

class KenyaAdditionalInfoTypeDef(TypedDict):
    personType: PersonTypeType,  # (1)
```

1. See [:material-code-brackets: PersonTypeType](./literals.md#persontypetype) 
## PolandAdditionalInfoTypeDef

```python
# PolandAdditionalInfoTypeDef definition

class PolandAdditionalInfoTypeDef(TypedDict):
    individualRegistrationNumber: NotRequired[str],
    isGroupVatEnabled: NotRequired[bool],
```

## RomaniaAdditionalInfoTypeDef

```python
# RomaniaAdditionalInfoTypeDef definition

class RomaniaAdditionalInfoTypeDef(TypedDict):
    taxRegistrationNumberType: TaxRegistrationNumberTypeType,  # (1)
```

1. See [:material-code-brackets: TaxRegistrationNumberTypeType](./literals.md#taxregistrationnumbertypetype) 
## SaudiArabiaAdditionalInfoTypeDef

```python
# SaudiArabiaAdditionalInfoTypeDef definition

class SaudiArabiaAdditionalInfoTypeDef(TypedDict):
    taxRegistrationNumberType: NotRequired[SaudiArabiaTaxRegistrationNumberTypeType],  # (1)
```

1. See [:material-code-brackets: SaudiArabiaTaxRegistrationNumberTypeType](./literals.md#saudiarabiataxregistrationnumbertypetype) 
## SouthKoreaAdditionalInfoTypeDef

```python
# SouthKoreaAdditionalInfoTypeDef definition

class SouthKoreaAdditionalInfoTypeDef(TypedDict):
    businessRepresentativeName: str,
    itemOfBusiness: str,
    lineOfBusiness: str,
```

## SpainAdditionalInfoTypeDef

```python
# SpainAdditionalInfoTypeDef definition

class SpainAdditionalInfoTypeDef(TypedDict):
    registrationType: RegistrationTypeType,  # (1)
```

1. See [:material-code-brackets: RegistrationTypeType](./literals.md#registrationtypetype) 
## TurkeyAdditionalInfoTypeDef

```python
# TurkeyAdditionalInfoTypeDef definition

class TurkeyAdditionalInfoTypeDef(TypedDict):
    industries: NotRequired[IndustriesType],  # (1)
    kepEmailId: NotRequired[str],
    secondaryTaxId: NotRequired[str],
    taxOffice: NotRequired[str],
```

1. See [:material-code-brackets: IndustriesType](./literals.md#industriestype) 
## UkraineAdditionalInfoTypeDef

```python
# UkraineAdditionalInfoTypeDef definition

class UkraineAdditionalInfoTypeDef(TypedDict):
    ukraineTrnType: UkraineTrnTypeType,  # (1)
```

1. See [:material-code-brackets: UkraineTrnTypeType](./literals.md#ukrainetrntypetype) 
## BrazilAdditionalInfoTypeDef

```python
# BrazilAdditionalInfoTypeDef definition

class BrazilAdditionalInfoTypeDef(TypedDict):
    ccmCode: NotRequired[str],
    legalNatureCode: NotRequired[str],
```

## IndiaAdditionalInfoTypeDef

```python
# IndiaAdditionalInfoTypeDef definition

class IndiaAdditionalInfoTypeDef(TypedDict):
    pan: NotRequired[str],
```

## MalaysiaAdditionalInfoOutputTypeDef

```python
# MalaysiaAdditionalInfoOutputTypeDef definition

class MalaysiaAdditionalInfoOutputTypeDef(TypedDict):
    businessRegistrationNumber: NotRequired[str],
    serviceTaxCodes: NotRequired[List[MalaysiaServiceTaxCodeType]],  # (1)
    taxInformationNumber: NotRequired[str],
```

1. See [:material-code-brackets: MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype) 
## AuthorityTypeDef

```python
# AuthorityTypeDef definition

class AuthorityTypeDef(TypedDict):
    country: str,
    state: NotRequired[str],
```

## BatchDeleteTaxRegistrationErrorTypeDef

```python
# BatchDeleteTaxRegistrationErrorTypeDef definition

class BatchDeleteTaxRegistrationErrorTypeDef(TypedDict):
    accountId: str,
    message: str,
    code: NotRequired[str],
```

## BatchDeleteTaxRegistrationRequestRequestTypeDef

```python
# BatchDeleteTaxRegistrationRequestRequestTypeDef definition

class BatchDeleteTaxRegistrationRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
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

## BatchGetTaxExemptionsRequestRequestTypeDef

```python
# BatchGetTaxExemptionsRequestRequestTypeDef definition

class BatchGetTaxExemptionsRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
```

## BatchPutTaxRegistrationErrorTypeDef

```python
# BatchPutTaxRegistrationErrorTypeDef definition

class BatchPutTaxRegistrationErrorTypeDef(TypedDict):
    accountId: str,
    message: str,
    code: NotRequired[str],
```

## DeleteSupplementalTaxRegistrationRequestRequestTypeDef

```python
# DeleteSupplementalTaxRegistrationRequestRequestTypeDef definition

class DeleteSupplementalTaxRegistrationRequestRequestTypeDef(TypedDict):
    authorityId: str,
```

## DeleteTaxRegistrationRequestRequestTypeDef

```python
# DeleteTaxRegistrationRequestRequestTypeDef definition

class DeleteTaxRegistrationRequestRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## DestinationS3LocationTypeDef

```python
# DestinationS3LocationTypeDef definition

class DestinationS3LocationTypeDef(TypedDict):
    bucket: str,
    prefix: NotRequired[str],
```

## TaxDocumentMetadataTypeDef

```python
# TaxDocumentMetadataTypeDef definition

class TaxDocumentMetadataTypeDef(TypedDict):
    taxDocumentAccessToken: str,
    taxDocumentName: str,
```

## GetTaxRegistrationRequestRequestTypeDef

```python
# GetTaxRegistrationRequestRequestTypeDef definition

class GetTaxRegistrationRequestRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSupplementalTaxRegistrationsRequestRequestTypeDef

```python
# ListSupplementalTaxRegistrationsRequestRequestTypeDef definition

class ListSupplementalTaxRegistrationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTaxExemptionsRequestRequestTypeDef

```python
# ListTaxExemptionsRequestRequestTypeDef definition

class ListTaxExemptionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTaxRegistrationsRequestRequestTypeDef

```python
# ListTaxRegistrationsRequestRequestTypeDef definition

class ListTaxRegistrationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MalaysiaAdditionalInfoTypeDef

```python
# MalaysiaAdditionalInfoTypeDef definition

class MalaysiaAdditionalInfoTypeDef(TypedDict):
    businessRegistrationNumber: NotRequired[str],
    serviceTaxCodes: NotRequired[Sequence[MalaysiaServiceTaxCodeType]],  # (1)
    taxInformationNumber: NotRequired[str],
```

1. See [:material-code-brackets: MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype) 
## PutTaxInheritanceRequestRequestTypeDef

```python
# PutTaxInheritanceRequestRequestTypeDef definition

class PutTaxInheritanceRequestRequestTypeDef(TypedDict):
    heritageStatus: NotRequired[HeritageStatusType],  # (1)
```

1. See [:material-code-brackets: HeritageStatusType](./literals.md#heritagestatustype) 
## SourceS3LocationTypeDef

```python
# SourceS3LocationTypeDef definition

class SourceS3LocationTypeDef(TypedDict):
    bucket: str,
    key: str,
```

## SupplementalTaxRegistrationEntryTypeDef

```python
# SupplementalTaxRegistrationEntryTypeDef definition

class SupplementalTaxRegistrationEntryTypeDef(TypedDict):
    address: AddressTypeDef,  # (1)
    legalName: str,
    registrationId: str,
    registrationType: SupplementalTaxRegistrationTypeType,  # (2)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-brackets: SupplementalTaxRegistrationTypeType](./literals.md#supplementaltaxregistrationtypetype) 
## SupplementalTaxRegistrationTypeDef

```python
# SupplementalTaxRegistrationTypeDef definition

class SupplementalTaxRegistrationTypeDef(TypedDict):
    address: AddressTypeDef,  # (1)
    authorityId: str,
    legalName: str,
    registrationId: str,
    registrationType: SupplementalTaxRegistrationTypeType,  # (2)
    status: TaxRegistrationStatusType,  # (3)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-brackets: SupplementalTaxRegistrationTypeType](./literals.md#supplementaltaxregistrationtypetype) 
3. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
## AccountMetaDataTypeDef

```python
# AccountMetaDataTypeDef definition

class AccountMetaDataTypeDef(TypedDict):
    accountName: NotRequired[str],
    address: NotRequired[AddressTypeDef],  # (1)
    addressRoleMap: NotRequired[Dict[AddressRoleTypeType, JurisdictionTypeDef]],  # (2)
    addressType: NotRequired[AddressRoleTypeType],  # (3)
    seller: NotRequired[str],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-brackets: AddressRoleTypeType](./literals.md#addressroletypetype) [:material-code-braces: JurisdictionTypeDef](./type_defs.md#jurisdictiontypedef) 
3. See [:material-code-brackets: AddressRoleTypeType](./literals.md#addressroletypetype) 
## AdditionalInfoResponseTypeDef

```python
# AdditionalInfoResponseTypeDef definition

class AdditionalInfoResponseTypeDef(TypedDict):
    brazilAdditionalInfo: NotRequired[BrazilAdditionalInfoTypeDef],  # (1)
    canadaAdditionalInfo: NotRequired[CanadaAdditionalInfoTypeDef],  # (2)
    estoniaAdditionalInfo: NotRequired[EstoniaAdditionalInfoTypeDef],  # (3)
    georgiaAdditionalInfo: NotRequired[GeorgiaAdditionalInfoTypeDef],  # (4)
    indiaAdditionalInfo: NotRequired[IndiaAdditionalInfoTypeDef],  # (5)
    israelAdditionalInfo: NotRequired[IsraelAdditionalInfoTypeDef],  # (6)
    italyAdditionalInfo: NotRequired[ItalyAdditionalInfoTypeDef],  # (7)
    kenyaAdditionalInfo: NotRequired[KenyaAdditionalInfoTypeDef],  # (8)
    malaysiaAdditionalInfo: NotRequired[MalaysiaAdditionalInfoOutputTypeDef],  # (9)
    polandAdditionalInfo: NotRequired[PolandAdditionalInfoTypeDef],  # (10)
    romaniaAdditionalInfo: NotRequired[RomaniaAdditionalInfoTypeDef],  # (11)
    saudiArabiaAdditionalInfo: NotRequired[SaudiArabiaAdditionalInfoTypeDef],  # (12)
    southKoreaAdditionalInfo: NotRequired[SouthKoreaAdditionalInfoTypeDef],  # (13)
    spainAdditionalInfo: NotRequired[SpainAdditionalInfoTypeDef],  # (14)
    turkeyAdditionalInfo: NotRequired[TurkeyAdditionalInfoTypeDef],  # (15)
    ukraineAdditionalInfo: NotRequired[UkraineAdditionalInfoTypeDef],  # (16)
```

1. See [:material-code-braces: BrazilAdditionalInfoTypeDef](./type_defs.md#braziladditionalinfotypedef) 
2. See [:material-code-braces: CanadaAdditionalInfoTypeDef](./type_defs.md#canadaadditionalinfotypedef) 
3. See [:material-code-braces: EstoniaAdditionalInfoTypeDef](./type_defs.md#estoniaadditionalinfotypedef) 
4. See [:material-code-braces: GeorgiaAdditionalInfoTypeDef](./type_defs.md#georgiaadditionalinfotypedef) 
5. See [:material-code-braces: IndiaAdditionalInfoTypeDef](./type_defs.md#indiaadditionalinfotypedef) 
6. See [:material-code-braces: IsraelAdditionalInfoTypeDef](./type_defs.md#israeladditionalinfotypedef) 
7. See [:material-code-braces: ItalyAdditionalInfoTypeDef](./type_defs.md#italyadditionalinfotypedef) 
8. See [:material-code-braces: KenyaAdditionalInfoTypeDef](./type_defs.md#kenyaadditionalinfotypedef) 
9. See [:material-code-braces: MalaysiaAdditionalInfoOutputTypeDef](./type_defs.md#malaysiaadditionalinfooutputtypedef) 
10. See [:material-code-braces: PolandAdditionalInfoTypeDef](./type_defs.md#polandadditionalinfotypedef) 
11. See [:material-code-braces: RomaniaAdditionalInfoTypeDef](./type_defs.md#romaniaadditionalinfotypedef) 
12. See [:material-code-braces: SaudiArabiaAdditionalInfoTypeDef](./type_defs.md#saudiarabiaadditionalinfotypedef) 
13. See [:material-code-braces: SouthKoreaAdditionalInfoTypeDef](./type_defs.md#southkoreaadditionalinfotypedef) 
14. See [:material-code-braces: SpainAdditionalInfoTypeDef](./type_defs.md#spainadditionalinfotypedef) 
15. See [:material-code-braces: TurkeyAdditionalInfoTypeDef](./type_defs.md#turkeyadditionalinfotypedef) 
16. See [:material-code-braces: UkraineAdditionalInfoTypeDef](./type_defs.md#ukraineadditionalinfotypedef) 
## TaxExemptionTypeTypeDef

```python
# TaxExemptionTypeTypeDef definition

class TaxExemptionTypeTypeDef(TypedDict):
    applicableJurisdictions: NotRequired[List[AuthorityTypeDef]],  # (1)
    description: NotRequired[str],
    displayName: NotRequired[str],
```

1. See [:material-code-braces: AuthorityTypeDef](./type_defs.md#authoritytypedef) 
## BatchDeleteTaxRegistrationResponseTypeDef

```python
# BatchDeleteTaxRegistrationResponseTypeDef definition

class BatchDeleteTaxRegistrationResponseTypeDef(TypedDict):
    errors: List[BatchDeleteTaxRegistrationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteTaxRegistrationErrorTypeDef](./type_defs.md#batchdeletetaxregistrationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTaxInheritanceResponseTypeDef

```python
# GetTaxInheritanceResponseTypeDef definition

class GetTaxInheritanceResponseTypeDef(TypedDict):
    heritageStatus: HeritageStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: HeritageStatusType](./literals.md#heritagestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTaxRegistrationDocumentResponseTypeDef

```python
# GetTaxRegistrationDocumentResponseTypeDef definition

class GetTaxRegistrationDocumentResponseTypeDef(TypedDict):
    destinationFilePath: str,
    presignedS3Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSupplementalTaxRegistrationResponseTypeDef

```python
# PutSupplementalTaxRegistrationResponseTypeDef definition

class PutSupplementalTaxRegistrationResponseTypeDef(TypedDict):
    authorityId: str,
    status: TaxRegistrationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTaxExemptionResponseTypeDef

```python
# PutTaxExemptionResponseTypeDef definition

class PutTaxExemptionResponseTypeDef(TypedDict):
    caseId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTaxRegistrationResponseTypeDef

```python
# PutTaxRegistrationResponseTypeDef definition

class PutTaxRegistrationResponseTypeDef(TypedDict):
    status: TaxRegistrationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutTaxRegistrationResponseTypeDef

```python
# BatchPutTaxRegistrationResponseTypeDef definition

class BatchPutTaxRegistrationResponseTypeDef(TypedDict):
    errors: List[BatchPutTaxRegistrationErrorTypeDef],  # (1)
    status: TaxRegistrationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchPutTaxRegistrationErrorTypeDef](./type_defs.md#batchputtaxregistrationerrortypedef) 
2. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExemptionCertificateTypeDef

```python
# ExemptionCertificateTypeDef definition

class ExemptionCertificateTypeDef(TypedDict):
    documentFile: BlobTypeDef,
    documentName: str,
```

## TaxRegistrationDocFileTypeDef

```python
# TaxRegistrationDocFileTypeDef definition

class TaxRegistrationDocFileTypeDef(TypedDict):
    fileContent: BlobTypeDef,
    fileName: str,
```

## GetTaxRegistrationDocumentRequestRequestTypeDef

```python
# GetTaxRegistrationDocumentRequestRequestTypeDef definition

class GetTaxRegistrationDocumentRequestRequestTypeDef(TypedDict):
    taxDocumentMetadata: TaxDocumentMetadataTypeDef,  # (1)
    destinationS3Location: NotRequired[DestinationS3LocationTypeDef],  # (2)
```

1. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
2. See [:material-code-braces: DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef) 
## ListSupplementalTaxRegistrationsRequestPaginateTypeDef

```python
# ListSupplementalTaxRegistrationsRequestPaginateTypeDef definition

class ListSupplementalTaxRegistrationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaxExemptionsRequestPaginateTypeDef

```python
# ListTaxExemptionsRequestPaginateTypeDef definition

class ListTaxExemptionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaxRegistrationsRequestPaginateTypeDef

```python
# ListTaxRegistrationsRequestPaginateTypeDef definition

class ListTaxRegistrationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PutSupplementalTaxRegistrationRequestRequestTypeDef

```python
# PutSupplementalTaxRegistrationRequestRequestTypeDef definition

class PutSupplementalTaxRegistrationRequestRequestTypeDef(TypedDict):
    taxRegistrationEntry: SupplementalTaxRegistrationEntryTypeDef,  # (1)
```

1. See [:material-code-braces: SupplementalTaxRegistrationEntryTypeDef](./type_defs.md#supplementaltaxregistrationentrytypedef) 
## ListSupplementalTaxRegistrationsResponseTypeDef

```python
# ListSupplementalTaxRegistrationsResponseTypeDef definition

class ListSupplementalTaxRegistrationsResponseTypeDef(TypedDict):
    taxRegistrations: List[SupplementalTaxRegistrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SupplementalTaxRegistrationTypeDef](./type_defs.md#supplementaltaxregistrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaxRegistrationTypeDef

```python
# TaxRegistrationTypeDef definition

class TaxRegistrationTypeDef(TypedDict):
    legalAddress: AddressTypeDef,  # (2)
    legalName: str,
    registrationId: str,
    registrationType: TaxRegistrationTypeType,  # (3)
    status: TaxRegistrationStatusType,  # (5)
    additionalTaxInformation: NotRequired[AdditionalInfoResponseTypeDef],  # (1)
    certifiedEmailId: NotRequired[str],
    sector: NotRequired[SectorType],  # (4)
    taxDocumentMetadatas: NotRequired[List[TaxDocumentMetadataTypeDef]],  # (6)
```

1. See [:material-code-braces: AdditionalInfoResponseTypeDef](./type_defs.md#additionalinforesponsetypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-brackets: TaxRegistrationTypeType](./literals.md#taxregistrationtypetype) 
4. See [:material-code-brackets: SectorType](./literals.md#sectortype) 
5. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
6. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
## TaxRegistrationWithJurisdictionTypeDef

```python
# TaxRegistrationWithJurisdictionTypeDef definition

class TaxRegistrationWithJurisdictionTypeDef(TypedDict):
    jurisdiction: JurisdictionTypeDef,  # (2)
    legalName: str,
    registrationId: str,
    registrationType: TaxRegistrationTypeType,  # (3)
    status: TaxRegistrationStatusType,  # (5)
    additionalTaxInformation: NotRequired[AdditionalInfoResponseTypeDef],  # (1)
    certifiedEmailId: NotRequired[str],
    sector: NotRequired[SectorType],  # (4)
    taxDocumentMetadatas: NotRequired[List[TaxDocumentMetadataTypeDef]],  # (6)
```

1. See [:material-code-braces: AdditionalInfoResponseTypeDef](./type_defs.md#additionalinforesponsetypedef) 
2. See [:material-code-braces: JurisdictionTypeDef](./type_defs.md#jurisdictiontypedef) 
3. See [:material-code-brackets: TaxRegistrationTypeType](./literals.md#taxregistrationtypetype) 
4. See [:material-code-brackets: SectorType](./literals.md#sectortype) 
5. See [:material-code-brackets: TaxRegistrationStatusType](./literals.md#taxregistrationstatustype) 
6. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
## GetTaxExemptionTypesResponseTypeDef

```python
# GetTaxExemptionTypesResponseTypeDef definition

class GetTaxExemptionTypesResponseTypeDef(TypedDict):
    taxExemptionTypes: List[TaxExemptionTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaxExemptionTypeTypeDef](./type_defs.md#taxexemptiontypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaxExemptionTypeDef

```python
# TaxExemptionTypeDef definition

class TaxExemptionTypeDef(TypedDict):
    authority: AuthorityTypeDef,  # (1)
    taxExemptionType: TaxExemptionTypeTypeDef,  # (3)
    effectiveDate: NotRequired[datetime],
    expirationDate: NotRequired[datetime],
    status: NotRequired[EntityExemptionAccountStatusType],  # (2)
    systemEffectiveDate: NotRequired[datetime],
```

1. See [:material-code-braces: AuthorityTypeDef](./type_defs.md#authoritytypedef) 
2. See [:material-code-brackets: EntityExemptionAccountStatusType](./literals.md#entityexemptionaccountstatustype) 
3. See [:material-code-braces: TaxExemptionTypeTypeDef](./type_defs.md#taxexemptiontypetypedef) 
## PutTaxExemptionRequestRequestTypeDef

```python
# PutTaxExemptionRequestRequestTypeDef definition

class PutTaxExemptionRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
    authority: AuthorityTypeDef,  # (1)
    exemptionCertificate: ExemptionCertificateTypeDef,  # (2)
    exemptionType: str,
```

1. See [:material-code-braces: AuthorityTypeDef](./type_defs.md#authoritytypedef) 
2. See [:material-code-braces: ExemptionCertificateTypeDef](./type_defs.md#exemptioncertificatetypedef) 
## TaxRegistrationDocumentTypeDef

```python
# TaxRegistrationDocumentTypeDef definition

class TaxRegistrationDocumentTypeDef(TypedDict):
    file: NotRequired[TaxRegistrationDocFileTypeDef],  # (1)
    s3Location: NotRequired[SourceS3LocationTypeDef],  # (2)
```

1. See [:material-code-braces: TaxRegistrationDocFileTypeDef](./type_defs.md#taxregistrationdocfiletypedef) 
2. See [:material-code-braces: SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef) 
## AdditionalInfoRequestTypeDef

```python
# AdditionalInfoRequestTypeDef definition

class AdditionalInfoRequestTypeDef(TypedDict):
    canadaAdditionalInfo: NotRequired[CanadaAdditionalInfoTypeDef],  # (1)
    estoniaAdditionalInfo: NotRequired[EstoniaAdditionalInfoTypeDef],  # (2)
    georgiaAdditionalInfo: NotRequired[GeorgiaAdditionalInfoTypeDef],  # (3)
    israelAdditionalInfo: NotRequired[IsraelAdditionalInfoTypeDef],  # (4)
    italyAdditionalInfo: NotRequired[ItalyAdditionalInfoTypeDef],  # (5)
    kenyaAdditionalInfo: NotRequired[KenyaAdditionalInfoTypeDef],  # (6)
    malaysiaAdditionalInfo: NotRequired[MalaysiaAdditionalInfoUnionTypeDef],  # (7)
    polandAdditionalInfo: NotRequired[PolandAdditionalInfoTypeDef],  # (8)
    romaniaAdditionalInfo: NotRequired[RomaniaAdditionalInfoTypeDef],  # (9)
    saudiArabiaAdditionalInfo: NotRequired[SaudiArabiaAdditionalInfoTypeDef],  # (10)
    southKoreaAdditionalInfo: NotRequired[SouthKoreaAdditionalInfoTypeDef],  # (11)
    spainAdditionalInfo: NotRequired[SpainAdditionalInfoTypeDef],  # (12)
    turkeyAdditionalInfo: NotRequired[TurkeyAdditionalInfoTypeDef],  # (13)
    ukraineAdditionalInfo: NotRequired[UkraineAdditionalInfoTypeDef],  # (14)
```

1. See [:material-code-braces: CanadaAdditionalInfoTypeDef](./type_defs.md#canadaadditionalinfotypedef) 
2. See [:material-code-braces: EstoniaAdditionalInfoTypeDef](./type_defs.md#estoniaadditionalinfotypedef) 
3. See [:material-code-braces: GeorgiaAdditionalInfoTypeDef](./type_defs.md#georgiaadditionalinfotypedef) 
4. See [:material-code-braces: IsraelAdditionalInfoTypeDef](./type_defs.md#israeladditionalinfotypedef) 
5. See [:material-code-braces: ItalyAdditionalInfoTypeDef](./type_defs.md#italyadditionalinfotypedef) 
6. See [:material-code-braces: KenyaAdditionalInfoTypeDef](./type_defs.md#kenyaadditionalinfotypedef) 
7. See [:material-code-braces: MalaysiaAdditionalInfoTypeDef](./type_defs.md#malaysiaadditionalinfotypedef) [:material-code-braces: MalaysiaAdditionalInfoOutputTypeDef](./type_defs.md#malaysiaadditionalinfooutputtypedef) 
8. See [:material-code-braces: PolandAdditionalInfoTypeDef](./type_defs.md#polandadditionalinfotypedef) 
9. See [:material-code-braces: RomaniaAdditionalInfoTypeDef](./type_defs.md#romaniaadditionalinfotypedef) 
10. See [:material-code-braces: SaudiArabiaAdditionalInfoTypeDef](./type_defs.md#saudiarabiaadditionalinfotypedef) 
11. See [:material-code-braces: SouthKoreaAdditionalInfoTypeDef](./type_defs.md#southkoreaadditionalinfotypedef) 
12. See [:material-code-braces: SpainAdditionalInfoTypeDef](./type_defs.md#spainadditionalinfotypedef) 
13. See [:material-code-braces: TurkeyAdditionalInfoTypeDef](./type_defs.md#turkeyadditionalinfotypedef) 
14. See [:material-code-braces: UkraineAdditionalInfoTypeDef](./type_defs.md#ukraineadditionalinfotypedef) 
## GetTaxRegistrationResponseTypeDef

```python
# GetTaxRegistrationResponseTypeDef definition

class GetTaxRegistrationResponseTypeDef(TypedDict):
    taxRegistration: TaxRegistrationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaxRegistrationTypeDef](./type_defs.md#taxregistrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccountDetailsTypeDef

```python
# AccountDetailsTypeDef definition

class AccountDetailsTypeDef(TypedDict):
    accountId: NotRequired[str],
    accountMetaData: NotRequired[AccountMetaDataTypeDef],  # (1)
    taxInheritanceDetails: NotRequired[TaxInheritanceDetailsTypeDef],  # (2)
    taxRegistration: NotRequired[TaxRegistrationWithJurisdictionTypeDef],  # (3)
```

1. See [:material-code-braces: AccountMetaDataTypeDef](./type_defs.md#accountmetadatatypedef) 
2. See [:material-code-braces: TaxInheritanceDetailsTypeDef](./type_defs.md#taxinheritancedetailstypedef) 
3. See [:material-code-braces: TaxRegistrationWithJurisdictionTypeDef](./type_defs.md#taxregistrationwithjurisdictiontypedef) 
## TaxExemptionDetailsTypeDef

```python
# TaxExemptionDetailsTypeDef definition

class TaxExemptionDetailsTypeDef(TypedDict):
    heritageObtainedDetails: NotRequired[bool],
    heritageObtainedParentEntity: NotRequired[str],
    heritageObtainedReason: NotRequired[str],
    taxExemptions: NotRequired[List[TaxExemptionTypeDef]],  # (1)
```

1. See [:material-code-braces: TaxExemptionTypeDef](./type_defs.md#taxexemptiontypedef) 
## VerificationDetailsTypeDef

```python
# VerificationDetailsTypeDef definition

class VerificationDetailsTypeDef(TypedDict):
    dateOfBirth: NotRequired[str],
    taxRegistrationDocuments: NotRequired[Sequence[TaxRegistrationDocumentTypeDef]],  # (1)
```

1. See [:material-code-braces: TaxRegistrationDocumentTypeDef](./type_defs.md#taxregistrationdocumenttypedef) 
## ListTaxRegistrationsResponseTypeDef

```python
# ListTaxRegistrationsResponseTypeDef definition

class ListTaxRegistrationsResponseTypeDef(TypedDict):
    accountDetails: List[AccountDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetTaxExemptionsResponseTypeDef

```python
# BatchGetTaxExemptionsResponseTypeDef definition

class BatchGetTaxExemptionsResponseTypeDef(TypedDict):
    failedAccounts: List[str],
    taxExemptionDetailsMap: Dict[str, TaxExemptionDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaxExemptionDetailsTypeDef](./type_defs.md#taxexemptiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaxExemptionsResponseTypeDef

```python
# ListTaxExemptionsResponseTypeDef definition

class ListTaxExemptionsResponseTypeDef(TypedDict):
    taxExemptionDetailsMap: Dict[str, TaxExemptionDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TaxExemptionDetailsTypeDef](./type_defs.md#taxexemptiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaxRegistrationEntryTypeDef

```python
# TaxRegistrationEntryTypeDef definition

class TaxRegistrationEntryTypeDef(TypedDict):
    registrationId: str,
    registrationType: TaxRegistrationTypeType,  # (3)
    additionalTaxInformation: NotRequired[AdditionalInfoRequestTypeDef],  # (1)
    certifiedEmailId: NotRequired[str],
    legalAddress: NotRequired[AddressTypeDef],  # (2)
    legalName: NotRequired[str],
    sector: NotRequired[SectorType],  # (4)
    verificationDetails: NotRequired[VerificationDetailsTypeDef],  # (5)
```

1. See [:material-code-braces: AdditionalInfoRequestTypeDef](./type_defs.md#additionalinforequesttypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-brackets: TaxRegistrationTypeType](./literals.md#taxregistrationtypetype) 
4. See [:material-code-brackets: SectorType](./literals.md#sectortype) 
5. See [:material-code-braces: VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef) 
## BatchPutTaxRegistrationRequestRequestTypeDef

```python
# BatchPutTaxRegistrationRequestRequestTypeDef definition

class BatchPutTaxRegistrationRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
    taxRegistrationEntry: TaxRegistrationEntryTypeDef,  # (1)
```

1. See [:material-code-braces: TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef) 
## PutTaxRegistrationRequestRequestTypeDef

```python
# PutTaxRegistrationRequestRequestTypeDef definition

class PutTaxRegistrationRequestRequestTypeDef(TypedDict):
    taxRegistrationEntry: TaxRegistrationEntryTypeDef,  # (1)
    accountId: NotRequired[str],
```

1. See [:material-code-braces: TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef) 
