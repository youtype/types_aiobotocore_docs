<a id="examples-for-aiobotocore-migrationhub-module"></a>

# Examples for aiobotocore MigrationHub module

> [Index](../README.md) > [MigrationHub](./README.md) > Examples

- [Examples for aiobotocore MigrationHub module](#examples-for-aiobotocore-migrationhub-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mgh]` package installed.

Write your `MigrationHub` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MigrationHubClient
# and provides type checking and code completion
async with session.create_client("mgh") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_created_artifact()
    

    
    # paginator has type ListApplicationStatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_application_states")
    async for item in paginator.paginate(...):
        # item has type ListApplicationStatesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mgh]` or a standalone `types_aiobotocore_mgh`
package, you have to explicitly specify `client: MigrationHubClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgh.client import MigrationHubClient
from types_aiobotocore_mgh.type_defs import Dict[str, Any]
from types_aiobotocore_mgh.paginator import ListApplicationStatesPaginator

from types_aiobotocore_mgh.literals import PaginatorName



session = get_session()

async with session.create_client("mgh") as client:
    client: MigrationHubClient

    
    result: Dict[str, Any] = client.associate_created_artifact()
    

    
    paginator_name: PaginatorName = "list_application_states"
    paginator: ListApplicationStatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationStatesResultTypeDef
        print(item)
    

    
```
