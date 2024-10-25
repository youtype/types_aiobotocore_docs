# TaxSettings module

> [Index](../README.md) > TaxSettings


!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## How to install



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
# ListTaxRegistrationsPaginator usage example

from types_aiobotocore_taxsettings.paginator import ListTaxRegistrationsPaginator

def get_list_tax_registrations_paginator() -> ListTaxRegistrationsPaginator:
    return client.get_paginator("list_tax_registrations"))
```

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
- [IndustriesType](./literals.md#industriestype)
- [IsraelCustomerTypeType](./literals.md#israelcustomertypetype)
- [IsraelDealerTypeType](./literals.md#israeldealertypetype)
- [ListTaxRegistrationsPaginatorName](./literals.md#listtaxregistrationspaginatorname)
- [MalaysiaServiceTaxCodeType](./literals.md#malaysiaservicetaxcodetype)
- [PersonTypeType](./literals.md#persontypetype)
- [RegistrationTypeType](./literals.md#registrationtypetype)
- [SaudiArabiaTaxRegistrationNumberTypeType](./literals.md#saudiarabiataxregistrationnumbertypetype)
- [SectorType](./literals.md#sectortype)
- [TaxRegistrationNumberTypeType](./literals.md#taxregistrationnumbertypetype)
- [TaxRegistrationStatusType](./literals.md#taxregistrationstatustype)
- [TaxRegistrationTypeType](./literals.md#taxregistrationtypetype)
- [UkraineTrnTypeType](./literals.md#ukrainetrntypetype)
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
- [EstoniaAdditionalInfoTypeDef](./type_defs.md#estoniaadditionalinfotypedef)
- [GeorgiaAdditionalInfoTypeDef](./type_defs.md#georgiaadditionalinfotypedef)
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
- [BrazilAdditionalInfoTypeDef](./type_defs.md#braziladditionalinfotypedef)
- [IndiaAdditionalInfoTypeDef](./type_defs.md#indiaadditionalinfotypedef)
- [MalaysiaAdditionalInfoOutputTypeDef](./type_defs.md#malaysiaadditionalinfooutputtypedef)
- [BatchDeleteTaxRegistrationErrorTypeDef](./type_defs.md#batchdeletetaxregistrationerrortypedef)
- [BatchDeleteTaxRegistrationRequestRequestTypeDef](./type_defs.md#batchdeletetaxregistrationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchPutTaxRegistrationErrorTypeDef](./type_defs.md#batchputtaxregistrationerrortypedef)
- [DeleteTaxRegistrationRequestRequestTypeDef](./type_defs.md#deletetaxregistrationrequestrequesttypedef)
- [DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef)
- [TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef)
- [GetTaxRegistrationRequestRequestTypeDef](./type_defs.md#gettaxregistrationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTaxRegistrationsRequestRequestTypeDef](./type_defs.md#listtaxregistrationsrequestrequesttypedef)
- [MalaysiaAdditionalInfoTypeDef](./type_defs.md#malaysiaadditionalinfotypedef)
- [SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef)
- [AccountMetaDataTypeDef](./type_defs.md#accountmetadatatypedef)
- [AdditionalInfoResponseTypeDef](./type_defs.md#additionalinforesponsetypedef)
- [BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef)
- [GetTaxRegistrationDocumentResponseTypeDef](./type_defs.md#gettaxregistrationdocumentresponsetypedef)
- [PutTaxRegistrationResponseTypeDef](./type_defs.md#puttaxregistrationresponsetypedef)
- [BatchPutTaxRegistrationResponseTypeDef](./type_defs.md#batchputtaxregistrationresponsetypedef)
- [GetTaxRegistrationDocumentRequestRequestTypeDef](./type_defs.md#gettaxregistrationdocumentrequestrequesttypedef)
- [ListTaxRegistrationsRequestListTaxRegistrationsPaginateTypeDef](./type_defs.md#listtaxregistrationsrequestlisttaxregistrationspaginatetypedef)
- [MalaysiaAdditionalInfoUnionTypeDef](./type_defs.md#malaysiaadditionalinfouniontypedef)
- [TaxRegistrationDocumentTypeDef](./type_defs.md#taxregistrationdocumenttypedef)
- [TaxRegistrationTypeDef](./type_defs.md#taxregistrationtypedef)
- [TaxRegistrationWithJurisdictionTypeDef](./type_defs.md#taxregistrationwithjurisdictiontypedef)
- [AdditionalInfoRequestTypeDef](./type_defs.md#additionalinforequesttypedef)
- [VerificationDetailsTypeDef](./type_defs.md#verificationdetailstypedef)
- [GetTaxRegistrationResponseTypeDef](./type_defs.md#gettaxregistrationresponsetypedef)
- [AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef)
- [TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef)
- [ListTaxRegistrationsResponseTypeDef](./type_defs.md#listtaxregistrationsresponsetypedef)
- [BatchPutTaxRegistrationRequestRequestTypeDef](./type_defs.md#batchputtaxregistrationrequestrequesttypedef)
- [PutTaxRegistrationRequestRequestTypeDef](./type_defs.md#puttaxregistrationrequestrequesttypedef)

