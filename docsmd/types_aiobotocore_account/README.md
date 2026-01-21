# Account module

> [Index](../README.md) > Account


!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Account` service.
1. Use provided commands to install generated packages.



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
- [AwsAccountStateType](./literals.md#awsaccountstatetype)
- [ListRegionsPaginatorName](./literals.md#listregionspaginatorname)
- [PrimaryEmailUpdateStatusType](./literals.md#primaryemailupdatestatustype)
- [RegionOptStatusType](./literals.md#regionoptstatustype)
- [AccountServiceName](./literals.md#accountservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptPrimaryEmailUpdateRequestTypeDef](./type_defs.md#acceptprimaryemailupdaterequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- [ContactInformationTypeDef](./type_defs.md#contactinformationtypedef)
- [DeleteAlternateContactRequestTypeDef](./type_defs.md#deletealternatecontactrequesttypedef)
- [DisableRegionRequestTypeDef](./type_defs.md#disableregionrequesttypedef)
- [EnableRegionRequestTypeDef](./type_defs.md#enableregionrequesttypedef)
- [GetAccountInformationRequestTypeDef](./type_defs.md#getaccountinformationrequesttypedef)
- [GetAlternateContactRequestTypeDef](./type_defs.md#getalternatecontactrequesttypedef)
- [GetContactInformationRequestTypeDef](./type_defs.md#getcontactinformationrequesttypedef)
- [GetGovCloudAccountInformationRequestTypeDef](./type_defs.md#getgovcloudaccountinformationrequesttypedef)
- [GetPrimaryEmailRequestTypeDef](./type_defs.md#getprimaryemailrequesttypedef)
- [GetRegionOptStatusRequestTypeDef](./type_defs.md#getregionoptstatusrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRegionsRequestTypeDef](./type_defs.md#listregionsrequesttypedef)
- [RegionTypeDef](./type_defs.md#regiontypedef)
- [PutAccountNameRequestTypeDef](./type_defs.md#putaccountnamerequesttypedef)
- [PutAlternateContactRequestTypeDef](./type_defs.md#putalternatecontactrequesttypedef)
- [StartPrimaryEmailUpdateRequestTypeDef](./type_defs.md#startprimaryemailupdaterequesttypedef)
- [AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAccountInformationResponseTypeDef](./type_defs.md#getaccountinformationresponsetypedef)
- [GetGovCloudAccountInformationResponseTypeDef](./type_defs.md#getgovcloudaccountinformationresponsetypedef)
- [GetPrimaryEmailResponseTypeDef](./type_defs.md#getprimaryemailresponsetypedef)
- [GetRegionOptStatusResponseTypeDef](./type_defs.md#getregionoptstatusresponsetypedef)
- [StartPrimaryEmailUpdateResponseTypeDef](./type_defs.md#startprimaryemailupdateresponsetypedef)
- [GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef)
- [GetContactInformationResponseTypeDef](./type_defs.md#getcontactinformationresponsetypedef)
- [PutContactInformationRequestTypeDef](./type_defs.md#putcontactinformationrequesttypedef)
- [ListRegionsRequestPaginateTypeDef](./type_defs.md#listregionsrequestpaginatetypedef)
- [ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef)

