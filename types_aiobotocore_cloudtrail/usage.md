<a id="examples-for-aiobotocore-cloudtrail-module"></a>

# Examples for aiobotocore CloudTrail module

> [Index](../README.md) > [CloudTrail](./README.md) > Examples

- [Examples for aiobotocore CloudTrail module](#examples-for-aiobotocore-cloudtrail-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudtrail]` package installed.

Write your `CloudTrail` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudTrailClient
# and provides type checking and code completion
async with session.create_client("cloudtrail") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags()
    

    
    # paginator has type ListPublicKeysPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_public_keys")
    async for item in paginator.paginate(...):
        # item has type ListPublicKeysResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudtrail]` or a standalone
`types_aiobotocore_cloudtrail` package, you have to explicitly specify
`client: CloudTrailClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.client import CloudTrailClient
from types_aiobotocore_cloudtrail.type_defs import Dict[str, Any]
from types_aiobotocore_cloudtrail.paginator import ListPublicKeysPaginator

from types_aiobotocore_cloudtrail.literals import PaginatorName



session = get_session()

async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient

    
    result: Dict[str, Any] = client.add_tags()
    

    
    paginator_name: PaginatorName = "list_public_keys"
    paginator: ListPublicKeysPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListPublicKeysResponseTypeDef
        print(item)
    

    
```
