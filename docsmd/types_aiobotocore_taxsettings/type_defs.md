# Type definitions

> [Index](../README.md) > [TaxSettings](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

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
    serviceTaxCodes: List[MalaysiaServiceTaxCodeType],  # (1)
```

1. See [:material-code-brackets: MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype) 
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

## BatchPutTaxRegistrationErrorTypeDef

```python
# BatchPutTaxRegistrationErrorTypeDef definition

class BatchPutTaxRegistrationErrorTypeDef(TypedDict):
    accountId: str,
    message: str,
    code: NotRequired[str],
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
    serviceTaxCodes: Sequence[MalaysiaServiceTaxCodeType],  # (1)
```

1. See [:material-code-brackets: MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype) 
## SourceS3LocationTypeDef

```python
# SourceS3LocationTypeDef definition

class SourceS3LocationTypeDef(TypedDict):
    bucket: str,
    key: str,
```

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
## BatchDeleteTaxRegistrationResponseTypeDef

```python
# BatchDeleteTaxRegistrationResponseTypeDef definition

class BatchDeleteTaxRegistrationResponseTypeDef(TypedDict):
    errors: List[BatchDeleteTaxRegistrationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteTaxRegistrationErrorTypeDef](./type_defs.md#batchdeletetaxregistrationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTaxRegistrationDocumentResponseTypeDef

```python
# GetTaxRegistrationDocumentResponseTypeDef definition

class GetTaxRegistrationDocumentResponseTypeDef(TypedDict):
    destinationFilePath: str,
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
## GetTaxRegistrationDocumentRequestRequestTypeDef

```python
# GetTaxRegistrationDocumentRequestRequestTypeDef definition

class GetTaxRegistrationDocumentRequestRequestTypeDef(TypedDict):
    destinationS3Location: DestinationS3LocationTypeDef,  # (1)
    taxDocumentMetadata: TaxDocumentMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef) 
2. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
## ListTaxRegistrationsRequestListTaxRegistrationsPaginateTypeDef

```python
# ListTaxRegistrationsRequestListTaxRegistrationsPaginateTypeDef definition

class ListTaxRegistrationsRequestListTaxRegistrationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## TaxRegistrationDocumentTypeDef

```python
# TaxRegistrationDocumentTypeDef definition

class TaxRegistrationDocumentTypeDef(TypedDict):
    s3Location: SourceS3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef) 
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
## VerificationDetailsTypeDef

```python
# VerificationDetailsTypeDef definition

class VerificationDetailsTypeDef(TypedDict):
    dateOfBirth: NotRequired[str],
    taxRegistrationDocuments: NotRequired[Sequence[TaxRegistrationDocumentTypeDef]],  # (1)
```

1. See [:material-code-braces: TaxRegistrationDocumentTypeDef](./type_defs.md#taxregistrationdocumenttypedef) 
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
