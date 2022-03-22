<a id="examples-for-aiobotocore-connectwisdomservice-module"></a>

# Examples for aiobotocore ConnectWisdomService module

> [Index](../README.md) > [ConnectWisdomService](./README.md) > Examples

- [Examples for aiobotocore ConnectWisdomService module](#examples-for-aiobotocore-connectwisdomservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[wisdom]` package installed.

Write your `ConnectWisdomService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ConnectWisdomServiceClient
# and provides type checking and code completion
async with session.create_client("wisdom") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAssistantAssociationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_assistant_associations")
    async for item in paginator.paginate(...):
        # item has type ListAssistantAssociationsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[wisdom]` or a standalone
`types_aiobotocore_wisdom` package, you have to explicitly specify
`client: ConnectWisdomServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.client import ConnectWisdomServiceClient
from types_aiobotocore_wisdom.type_defs import bool
from types_aiobotocore_wisdom.paginator import ListAssistantAssociationsPaginator

from types_aiobotocore_wisdom.literals import PaginatorName



session = get_session()

async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_assistant_associations"
    paginator: ListAssistantAssociationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAssistantAssociationsResponseTypeDef
        print(item)
    

    
```
