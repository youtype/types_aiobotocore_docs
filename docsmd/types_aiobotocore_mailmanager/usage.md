# Examples

> [Index](../README.md) > [MailManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mailmanager]` package installed.

Write your `MailManager` code as usual,
type checking and code completion should work out of the box.



```python
# MailManagerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mailmanager") as client:  # (1)
    result = await client.create_addon_instance()  # (2)
```

1. client: [MailManagerClient](./client.md)
2. result: [:material-code-braces: CreateAddonInstanceResponseTypeDef](./type_defs.md#createaddoninstanceresponsetypedef) 



```python
# ListAddonInstancesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mailmanager") as client:  # (1)
    paginator = client.get_paginator("list_addon_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
3. item: [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mailmanager]`
or a standalone `types_aiobotocore_mailmanager` package, you have to explicitly specify
`client: MailManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MailManagerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.client import MailManagerClient
from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceResponseTypeDef
from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceRequestTypeDef


session = get_session()

async with session.create_client("mailmanager") as client:
    client: MailManagerClient
    kwargs: CreateAddonInstanceRequestTypeDef = {...}
    result: CreateAddonInstanceResponseTypeDef = await client.create_addon_instance(**kwargs)
```



```python
# ListAddonInstancesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.client import MailManagerClient
from types_aiobotocore_mailmanager.paginator import ListAddonInstancesPaginator
from types_aiobotocore_mailmanager.type_defs import ListAddonInstancesResponseTypeDef


session = get_session()

async with session.create_client("mailmanager") as client:
    client: MailManagerClient
    paginator: ListAddonInstancesPaginator = client.get_paginator("list_addon_instances")
    async for item in paginator.paginate(...):
        item: ListAddonInstancesResponseTypeDef
        print(item)
```


