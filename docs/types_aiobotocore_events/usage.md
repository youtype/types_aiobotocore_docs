<a id="examples-for-aiobotocore-eventbridge-module"></a>

# Examples for aiobotocore EventBridge module

> [Index](../README.md) > [EventBridge](./README.md) > Examples

- [Examples for aiobotocore EventBridge module](#examples-for-aiobotocore-eventbridge-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[events]` package installed.

Write your `EventBridge` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EventBridgeClient
# and provides type checking and code completion
async with session.create_client("events") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_event_source()
    

    
    # paginator has type ListRuleNamesByTargetPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_rule_names_by_target")
    async for item in paginator.paginate(...):
        # item has type ListRuleNamesByTargetResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[events]` or a standalone
`types_aiobotocore_events` package, you have to explicitly specify
`client: EventBridgeClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_events.client import EventBridgeClient
from types_aiobotocore_events.type_defs import None
from types_aiobotocore_events.paginator import ListRuleNamesByTargetPaginator

from types_aiobotocore_events.literals import PaginatorName



session = get_session()

async with session.create_client("events") as client:
    client: EventBridgeClient

    
    result: None = client.activate_event_source()
    

    
    paginator_name: PaginatorName = "list_rule_names_by_target"
    paginator: ListRuleNamesByTargetPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListRuleNamesByTargetResponseTypeDef
        print(item)
    

    
```
