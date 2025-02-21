# Examples

> [Index](../README.md) > [FMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#fms)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[fms]` package installed.

Write your `FMS` code as usual,
type checking and code completion should work out of the box.



```python
# FMSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fms") as client:  # (1)
    result = await client.associate_admin_account()  # (2)
```

1. client: [FMSClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListAdminAccountsForOrganizationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fms") as client:  # (1)
    paginator = client.get_paginator("list_admin_accounts_for_organization")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListAdminAccountsForOrganizationPaginator](./paginators.md#listadminaccountsfororganizationpaginator)
3. item: [:material-code-braces: ListAdminAccountsForOrganizationResponseTypeDef](./type_defs.md#listadminaccountsfororganizationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[fms]`
or a standalone `types_aiobotocore_fms` package, you have to explicitly specify
`client: FMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FMSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fms.client import FMSClient
from types_aiobotocore_fms.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_fms.type_defs import AssociateAdminAccountRequestTypeDef


session = get_session()

async with session.create_client("fms") as client:
    client: FMSClient
    kwargs: AssociateAdminAccountRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_admin_account(**kwargs)
```



```python
# ListAdminAccountsForOrganizationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fms.client import FMSClient
from types_aiobotocore_fms.paginator import ListAdminAccountsForOrganizationPaginator
from types_aiobotocore_fms.type_defs import ListAdminAccountsForOrganizationResponseTypeDef


session = get_session()

async with session.create_client("fms") as client:
    client: FMSClient
    paginator: ListAdminAccountsForOrganizationPaginator = client.get_paginator("list_admin_accounts_for_organization")
    async for item in paginator.paginate(...):
        item: ListAdminAccountsForOrganizationResponseTypeDef
        print(item)
```


