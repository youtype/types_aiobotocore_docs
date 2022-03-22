<a id="examples-for-aiobotocore-managedgrafana-module"></a>

# Examples for aiobotocore ManagedGrafana module

> [Index](../README.md) > [ManagedGrafana](./README.md) > Examples

- [Examples for aiobotocore ManagedGrafana module](#examples-for-aiobotocore-managedgrafana-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[grafana]` package installed.

Write your `ManagedGrafana` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ManagedGrafanaClient
# and provides type checking and code completion
async with session.create_client("grafana") as client:
    
    # result has type AssociateLicenseResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_license()
    

    
    # paginator has type ListPermissionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_permissions")
    async for item in paginator.paginate(...):
        # item has type ListPermissionsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[grafana]` or a standalone
`types_aiobotocore_grafana` package, you have to explicitly specify
`client: ManagedGrafanaClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_grafana.client import ManagedGrafanaClient
from types_aiobotocore_grafana.type_defs import AssociateLicenseResponseTypeDef
from types_aiobotocore_grafana.paginator import ListPermissionsPaginator

from types_aiobotocore_grafana.literals import PaginatorName



session = get_session()

async with session.create_client("grafana") as client:
    client: ManagedGrafanaClient

    
    result: AssociateLicenseResponseTypeDef = client.associate_license()
    

    
    paginator_name: PaginatorName = "list_permissions"
    paginator: ListPermissionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)
    

    
```
