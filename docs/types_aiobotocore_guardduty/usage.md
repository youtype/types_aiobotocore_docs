<a id="examples-for-aiobotocore-guardduty-module"></a>

# Examples for aiobotocore GuardDuty module

> [Index](../README.md) > [GuardDuty](./README.md) > Examples

- [Examples for aiobotocore GuardDuty module](#examples-for-aiobotocore-guardduty-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[guardduty]` package installed.

Write your `GuardDuty` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GuardDutyClient
# and provides type checking and code completion
async with session.create_client("guardduty") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_invitation()
    

    
    # paginator has type ListDetectorsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_detectors")
    async for item in paginator.paginate(...):
        # item has type ListDetectorsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[guardduty]` or a standalone
`types_aiobotocore_guardduty` package, you have to explicitly specify
`client: GuardDutyClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.client import GuardDutyClient
from types_aiobotocore_guardduty.type_defs import Dict[str, Any]
from types_aiobotocore_guardduty.paginator import ListDetectorsPaginator

from types_aiobotocore_guardduty.literals import PaginatorName



session = get_session()

async with session.create_client("guardduty") as client:
    client: GuardDutyClient

    
    result: Dict[str, Any] = client.accept_invitation()
    

    
    paginator_name: PaginatorName = "list_detectors"
    paginator: ListDetectorsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDetectorsResponseTypeDef
        print(item)
    

    
```
