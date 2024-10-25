# Account module

> [Index](../README.md) > Account


!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Account` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[account]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[account]'


# standalone installation
python -m pip install types-aiobotocore-account
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-account
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AccountClient

Type annotations and code completion for  `#!python session.create_client("account")` as [AccountClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# AccountClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_account.client import AccountClient


session = get_session()
async with session.create_client("account") as client:
    client: AccountClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("account").get_paginator("...")`.

```python
# ListRegionsPaginator usage example

from types_aiobotocore_account.paginator import ListRegionsPaginator

def get_list_regions_paginator() -> ListRegionsPaginator:
    return client.get_paginator("list_regions"))
```

- [ListRegionsPaginator](./paginators.md#listregionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlternateContactTypeType usage example

from types_aiobotocore_account.literals import AlternateContactTypeType

def get_value() -> AlternateContactTypeType:
    return "BILLING"
```

- [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
- [ListRegionsPaginatorName](./literals.md#listregionspaginatorname)
- [PrimaryEmailUpdateStatusType](./literals.md#primaryemailupdatestatustype)
- [RegionOptStatusType](./literals.md#regionoptstatustype)
- [AccountServiceName](./literals.md#accountservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptPrimaryEmailUpdateRequestRequestTypeDef](./type_defs.md#acceptprimaryemailupdaterequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- [ContactInformationTypeDef](./type_defs.md#contactinformationtypedef)
- [DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef)
- [DisableRegionRequestRequestTypeDef](./type_defs.md#disableregionrequestrequesttypedef)
- [EnableRegionRequestRequestTypeDef](./type_defs.md#enableregionrequestrequesttypedef)
- [GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef)
- [GetContactInformationRequestRequestTypeDef](./type_defs.md#getcontactinformationrequestrequesttypedef)
- [GetPrimaryEmailRequestRequestTypeDef](./type_defs.md#getprimaryemailrequestrequesttypedef)
- [GetRegionOptStatusRequestRequestTypeDef](./type_defs.md#getregionoptstatusrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRegionsRequestRequestTypeDef](./type_defs.md#listregionsrequestrequesttypedef)
- [RegionTypeDef](./type_defs.md#regiontypedef)
- [PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef)
- [StartPrimaryEmailUpdateRequestRequestTypeDef](./type_defs.md#startprimaryemailupdaterequestrequesttypedef)
- [AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetPrimaryEmailResponseTypeDef](./type_defs.md#getprimaryemailresponsetypedef)
- [GetRegionOptStatusResponseTypeDef](./type_defs.md#getregionoptstatusresponsetypedef)
- [StartPrimaryEmailUpdateResponseTypeDef](./type_defs.md#startprimaryemailupdateresponsetypedef)
- [GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef)
- [GetContactInformationResponseTypeDef](./type_defs.md#getcontactinformationresponsetypedef)
- [PutContactInformationRequestRequestTypeDef](./type_defs.md#putcontactinformationrequestrequesttypedef)
- [ListRegionsRequestListRegionsPaginateTypeDef](./type_defs.md#listregionsrequestlistregionspaginatetypedef)
- [ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef)

