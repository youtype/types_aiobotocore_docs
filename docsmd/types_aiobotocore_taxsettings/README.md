# TaxSettings module

> [Index](../README.md) > TaxSettings


!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `TaxSettings` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `TaxSettings` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[taxsettings]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[taxsettings]'

# standalone installation
python -m pip install types-aiobotocore-taxsettings
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-taxsettings
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TaxSettingsClient

Type annotations and code completion for  `#!python session.create_client("taxsettings")` as [TaxSettingsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client)

```python
# TaxSettingsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_taxsettings.client import TaxSettingsClient


session = get_session()
async with session.create_client("taxsettings") as client:
    client: TaxSettingsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("taxsettings").get_paginator("...")`.

```python
# ListSupplementalTaxRegistrationsPaginator usage example

from types_aiobotocore_taxsettings.paginator import ListSupplementalTaxRegistrationsPaginator

def get_list_supplemental_tax_registrations_paginator() -> ListSupplementalTaxRegistrationsPaginator:
    return client.get_paginator("list_supplemental_tax_registrations"))
```

- [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
- [ListTaxExemptionsPaginator](./paginators.md#listtaxexemptionspaginator)
- [ListTaxRegistrationsPaginator](./paginators.md#listtaxregistrationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AddressRoleTypeType usage example

from types_aiobotocore_taxsettings.literals import AddressRoleTypeType

def get_value() -> AddressRoleTypeType:
    return "BillingAddress"
```

- [AddressRoleTypeType](./literals.md#addressroletypetype)
- [EntityExemptionAccountStatusType](./literals.md#entityexemptionaccountstatustype)
- [HeritageStatusType](./literals.md#heritagestatustype)
- [IndonesiaTaxRegistrationNumberTypeType](./literals.md#indonesiataxregistrationnumbertypetype)
- [IndustriesType](./literals.md#industriestype)
- [IsraelCustomerTypeType](./literals.md#israelcustomertypetype)
- [IsraelDealerTypeType](./literals.md#israeldealertypetype)
- [ListSupplementalTaxRegistrationsPaginatorName](./literals.md#listsupplementaltaxregistrationspaginatorname)
- [ListTaxExemptionsPaginatorName](./literals.md#listtaxexemptionspaginatorname)
- [ListTaxRegistrationsPaginatorName](./literals.md#listtaxregistrationspaginatorname)
- [MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype)
- [PersonTypeType](./literals.md#persontypetype)
- [RegistrationTypeType](./literals.md#registrationtypetype)
- [SaudiArabiaTaxRegistrationNumberTypeType](./literals.md#saudiarabiataxregistrationnumbertypetype)
- [SectorType](./literals.md#sectortype)
- [SupplementalTaxRegistrationTypeType](./literals.md#supplementaltaxregistrationtypetype)
- [TaxRegistrationNumberTypeType](./literals.md#taxregistrationnumbertypetype)
- [TaxRegistrationStatusType](./literals.md#taxregistrationstatustype)
- [TaxRegistrationTypeType](./literals.md#taxregistrationtypetype)
- [UkraineTrnTypeType](./literals.md#ukrainetrntypetype)
- [UzbekistanTaxRegistrationNumberTypeType](./literals.md#uzbekistantaxregistrationnumbertypetype)
- [TaxSettingsServiceName](./literals.md#taxsettingsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TaxInheritanceDetailsTypeDef](./type_defs.md#taxinheritancedetailstypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [JurisdictionTypeDef](./type_defs.md#jurisdictiontypedef)
- [CanadaAdditionalInfoTypeDef](./type_defs.md#canadaadditionalinfotypedef)
- [EgyptAdditionalInfoTypeDef](./type_defs.md#egyptadditionalinfotypedef)
- [EstoniaAdditionalInfoTypeDef](./type_defs.md#estoniaadditionalinfotypedef)
- [GeorgiaAdditionalInfoTypeDef](./type_defs.md#georgiaadditionalinfotypedef)
- [GreeceAdditionalInfoTypeDef](./type_defs.md#greeceadditionalinfotypedef)
- [IndonesiaAdditionalInfoTypeDef](./type_defs.md#indonesiaadditionalinfotypedef)
- [IsraelAdditionalInfoTypeDef](./type_defs.md#israeladditionalinfotypedef)
- [ItalyAdditionalInfoTypeDef](./type_defs.md#italyadditionalinfotypedef)
- [KenyaAdditionalInfoTypeDef](./type_defs.md#kenyaadditionalinfotypedef)
- [PolandAdditionalInfoTypeDef](./type_defs.md#polandadditionalinfotypedef)
- [RomaniaAdditionalInfoTypeDef](./type_defs.md#romaniaadditionalinfotypedef)
- [SaudiArabiaAdditionalInfoTypeDef](./type_defs.md#saudiarabiaadditionalinfotypedef)
- [SouthKoreaAdditionalInfoTypeDef](./type_defs.md#southkoreaadditionalinfotypedef)
- [SpainAdditionalInfoTypeDef](./type_defs.md#spainadditionalinfotypedef)
- [TurkeyAdditionalInfoTypeDef](./type_defs.md#turkeyadditionalinfotypedef)
- [UkraineAdditionalInfoTypeDef](./type_defs.md#ukraineadditionalinfotypedef)
- [UzbekistanAdditionalInfoTypeDef](./type_defs.md#uzbekistanadditionalinfotypedef)
- [VietnamAdditionalInfoTypeDef](./type_defs.md#vietnamadditionalinfotypedef)
- [BrazilAdditionalInfoTypeDef](./type_defs.md#braziladditionalinfotypedef)
- [IndiaAdditionalInfoTypeDef](./type_defs.md#indiaadditionalinfotypedef)
- [MalaysiaAdditionalInfoOutputTypeDef](./type_defs.md#malaysiaadditionalinfooutputtypedef)
- [AuthorityTypeDef](./type_defs.md#authoritytypedef)
- [BatchDeleteTaxRegistrationErrorTypeDef](./type_defs.md#batchdeletetaxregistrationerrortypedef)
- [BatchDeleteTaxRegistrationRequestTypeDef](./type_defs.md#batchdeletetaxregistrationrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetTaxExemptionsRequestTypeDef](./type_defs.md#batchgettaxexemptionsrequesttypedef)
- [BatchPutTaxRegistrationErrorTypeDef](./type_defs.md#batchputtaxregistrationerrortypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DeleteSupplementalTaxRegistrationRequestTypeDef](./type_defs.md#deletesupplementaltaxregistrationrequesttypedef)
- [DeleteTaxRegistrationRequestTypeDef](./type_defs.md#deletetaxregistrationrequesttypedef)
- [DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef)
- [TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef)
- [GetTaxRegistrationRequestTypeDef](./type_defs.md#gettaxregistrationrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListSupplementalTaxRegistrationsRequestTypeDef](./type_defs.md#listsupplementaltaxregistrationsrequesttypedef)
- [ListTaxExemptionsRequestTypeDef](./type_defs.md#listtaxexemptionsrequesttypedef)
- [ListTaxRegistrationsRequestTypeDef](./type_defs.md#listtaxregistrationsrequesttypedef)
- [MalaysiaAdditionalInfoTypeDef](./type_defs.md#malaysiaadditionalinfotypedef)
- [PutTaxInheritanceRequestTypeDef](./type_defs.md#puttaxinheritancerequesttypedef)
- [SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef)
- [SupplementalTaxRegistrationEntryTypeDef](./type_defs.md#supplementaltaxregistrationentrytypedef)
- [SupplementalTaxRegistrationTypeDef](./type_defs.md#supplementaltaxregistrationtypedef)
- [AccountMetaDataTypeDef](./type_defs.md#accountmetadatatypedef)
- [AdditionalInfoResponseTypeDef](./type_defs.md#additionalinforesponsetypedef)
- [TaxExemptionTypeTypeDef](./type_defs.md#taxexemptiontypetypedef)
- [BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef)
- [GetTaxInheritanceResponseTypeDef](./type_defs.md#gettaxinheritanceresponsetypedef)
- [GetTaxRegistrationDocumentResponseTypeDef](./type_defs.md#gettaxregistrationdocumentresponsetypedef)
- [PutSupplementalTaxRegistrationResponseTypeDef](./type_defs.md#putsupplementaltaxregistrationresponsetypedef)
- [PutTaxExemptionResponseTypeDef](./type_defs.md#puttaxexemptionresponsetypedef)
- [PutTaxRegistrationResponseTypeDef](./type_defs.md#puttaxregistrationresponsetypedef)
- [BatchPutTaxRegistrationResponseTypeDef](./type_defs.md#batchputtaxregistrationresponsetypedef)
- [ExemptionCertificateTypeDef](./type_defs.md#exemptioncertificatetypedef)
- [TaxRegistrationDocFileTypeDef](./type_defs.md#taxregistrationdocfiletypedef)
- [GetTaxRegistrationDocumentRequestTypeDef](./type_defs.md#gettaxregistrationdocumentrequesttypedef)
- [ListSupplementalTaxRegistrationsRequestPaginateTypeDef](./type_defs.md#listsupplementaltaxregistrationsrequestpaginatetypedef)
- [ListTaxExemptionsRequestPaginateTypeDef](./type_defs.md#listtaxexemptionsrequestpaginatetypedef)
- [ListTaxRegistrationsRequestPaginateTypeDef](./type_defs.md#listtaxregistrationsrequestpaginatetypedef)
- [MalaysiaAdditionalInfoUnionTypeDef](./type_defs.md#malaysiaadditionalinfouniontypedef)
- [PutSupplementalTaxRegistrationRequestTypeDef](./type_defs.md#putsupplementaltaxregistrationrequesttypedef)
- [ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef)
- [TaxRegistrationTypeDef](./type_defs.md#taxregistrationtypedef)
- [TaxRegistrationWithJurisdictionTypeDef](./type_defs.md#taxregistrationwithjurisdictiontypedef)
- [GetTaxExemptionTypesResponseTypeDef](./type_defs.md#gettaxexemptiontypesresponsetypedef)
- [TaxExemptionTypeDef](./type_defs.md#taxexemptiontypedef)
- [PutTaxExemptionRequestTypeDef](./type_defs.md#puttaxexemptionrequesttypedef)
- [TaxRegistrationDocumentTypeDef](./type_defs.md#taxregistrationdocumenttypedef)
- [AdditionalInfoRequestTypeDef](./type_defs.md#additionalinforequesttypedef)
- [GetTaxRegistrationResponseTypeDef](./type_defs.md#gettaxregistrationresponsetypedef)
- [AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef)
- [TaxExemptionDetailsTypeDef](./type_defs.md#taxexemptiondetailstypedef)
- [VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)
- [ListTaxRegistrationsResponseTypeDef](./type_defs.md#listtaxregistrationsresponsetypedef)
- [BatchGetTaxExemptionsResponseTypeDef](./type_defs.md#batchgettaxexemptionsresponsetypedef)
- [ListTaxExemptionsResponseTypeDef](./type_defs.md#listtaxexemptionsresponsetypedef)
- [TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef)
- [BatchPutTaxRegistrationRequestTypeDef](./type_defs.md#batchputtaxregistrationrequesttypedef)
- [PutTaxRegistrationRequestTypeDef](./type_defs.md#puttaxregistrationrequesttypedef)

