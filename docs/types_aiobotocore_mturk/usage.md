<a id="examples-for-aiobotocore-mturk-module"></a>

# Examples for aiobotocore MTurk module

> [Index](../README.md) > [MTurk](./README.md) > Examples

- [Examples for aiobotocore MTurk module](#examples-for-aiobotocore-mturk-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mturk]` package installed.

Write your `MTurk` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MTurkClient
# and provides type checking and code completion
async with session.create_client("mturk") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_qualification_request()
    

    
    # paginator has type ListAssignmentsForHITPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_assignments_for_hit")
    async for item in paginator.paginate(...):
        # item has type ListAssignmentsForHITResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mturk]` or a standalone `types_aiobotocore_mturk`
package, you have to explicitly specify `client: MTurkClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mturk.client import MTurkClient
from types_aiobotocore_mturk.type_defs import Dict[str, Any]
from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator

from types_aiobotocore_mturk.literals import PaginatorName



session = get_session()

async with session.create_client("mturk") as client:
    client: MTurkClient

    
    result: Dict[str, Any] = client.accept_qualification_request()
    

    
    paginator_name: PaginatorName = "list_assignments_for_hit"
    paginator: ListAssignmentsForHITPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAssignmentsForHITResponseTypeDef
        print(item)
    

    
```
