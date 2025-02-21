# Examples

> [Index](../README.md) > [ManagedGrafana](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[grafana]` package installed.

Write your `ManagedGrafana` code as usual,
type checking and code completion should work out of the box.



```python
# ManagedGrafanaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("grafana") as client:  # (1)
    result = await client.associate_license()  # (2)
```

1. client: [ManagedGrafanaClient](./client.md)
2. result: [:material-code-braces: AssociateLicenseResponseTypeDef](./type_defs.md#associatelicenseresponsetypedef) 



```python
# ListPermissionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("grafana") as client:  # (1)
    paginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[grafana]`
or a standalone `types_aiobotocore_grafana` package, you have to explicitly specify
`client: ManagedGrafanaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ManagedGrafanaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_grafana.client import ManagedGrafanaClient
from types_aiobotocore_grafana.type_defs import AssociateLicenseResponseTypeDef
from types_aiobotocore_grafana.type_defs import AssociateLicenseRequestTypeDef


session = get_session()

async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient
    kwargs: AssociateLicenseRequestTypeDef = {...}
    result: AssociateLicenseResponseTypeDef = await client.associate_license(**kwargs)
```



```python
# ListPermissionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_grafana.client import ManagedGrafanaClient
from types_aiobotocore_grafana.paginator import ListPermissionsPaginator
from types_aiobotocore_grafana.type_defs import ListPermissionsResponseTypeDef


session = get_session()

async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)
```


