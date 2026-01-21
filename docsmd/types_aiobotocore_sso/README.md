# SSO module

> [Index](../README.md) > SSO


!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SSO` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SSO` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sso]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sso]'

# standalone installation
python -m pip install types-aiobotocore-sso
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sso
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSOClient

Type annotations and code completion for  `#!python session.create_client("sso")` as [SSOClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client)

```python
# SSOClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sso.client import SSOClient


session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("sso").get_paginator("...")`.

```python
# ListAccountRolesPaginator usage example

from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

def get_list_account_roles_paginator() -> ListAccountRolesPaginator:
    return client.get_paginator("list_account_roles"))
```

- [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
- [ListAccountsPaginator](./paginators.md#listaccountspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListAccountRolesPaginatorName usage example

from types_aiobotocore_sso.literals import ListAccountRolesPaginatorName

def get_value() -> ListAccountRolesPaginatorName:
    return "list_account_roles"
```

- [ListAccountRolesPaginatorName](./literals.md#listaccountrolespaginatorname)
- [ListAccountsPaginatorName](./literals.md#listaccountspaginatorname)
- [SSOServiceName](./literals.md#ssoservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountInfoTypeDef](./type_defs.md#accountinfotypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRoleCredentialsRequestTypeDef](./type_defs.md#getrolecredentialsrequesttypedef)
- [RoleCredentialsTypeDef](./type_defs.md#rolecredentialstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccountRolesRequestTypeDef](./type_defs.md#listaccountrolesrequesttypedef)
- [RoleInfoTypeDef](./type_defs.md#roleinfotypedef)
- [ListAccountsRequestTypeDef](./type_defs.md#listaccountsrequesttypedef)
- [LogoutRequestTypeDef](./type_defs.md#logoutrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)
- [GetRoleCredentialsResponseTypeDef](./type_defs.md#getrolecredentialsresponsetypedef)
- [ListAccountRolesRequestPaginateTypeDef](./type_defs.md#listaccountrolesrequestpaginatetypedef)
- [ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef)
- [ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef)

