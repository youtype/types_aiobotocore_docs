<a id="examples-for-aiobotocore-clouddirectory-module"></a>

# Examples for aiobotocore CloudDirectory module

> [Index](../README.md) > [CloudDirectory](./README.md) > Examples

- [Examples for aiobotocore CloudDirectory module](#examples-for-aiobotocore-clouddirectory-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[clouddirectory]` package installed.

Write your `CloudDirectory` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudDirectoryClient
# and provides type checking and code completion
async with session.create_client("clouddirectory") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_facet_to_object()
    

    
    # paginator has type ListAppliedSchemaArnsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_applied_schema_arns")
    async for item in paginator.paginate(...):
        # item has type ListAppliedSchemaArnsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[clouddirectory]` or a standalone
`types_aiobotocore_clouddirectory` package, you have to explicitly specify
`client: CloudDirectoryClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.client import CloudDirectoryClient
from types_aiobotocore_clouddirectory.type_defs import Dict[str, Any]
from types_aiobotocore_clouddirectory.paginator import ListAppliedSchemaArnsPaginator

from types_aiobotocore_clouddirectory.literals import PaginatorName



session = get_session()

async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient

    
    result: Dict[str, Any] = client.add_facet_to_object()
    

    
    paginator_name: PaginatorName = "list_applied_schema_arns"
    paginator: ListAppliedSchemaArnsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAppliedSchemaArnsResponseTypeDef
        print(item)
    

    
```
