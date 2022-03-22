<a id="examples-for-aiobotocore-translate-module"></a>

# Examples for aiobotocore Translate module

> [Index](../README.md) > [Translate](./README.md) > Examples

- [Examples for aiobotocore Translate module](#examples-for-aiobotocore-translate-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[translate]` package installed.

Write your `Translate` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type TranslateClient
# and provides type checking and code completion
async with session.create_client("translate") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListTerminologiesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_terminologies")
    async for item in paginator.paginate(...):
        # item has type ListTerminologiesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[translate]` or a standalone
`types_aiobotocore_translate` package, you have to explicitly specify
`client: TranslateClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_translate.client import TranslateClient
from types_aiobotocore_translate.type_defs import bool
from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

from types_aiobotocore_translate.literals import PaginatorName



session = get_session()

async with session.create_client("translate") as client:
    client: TranslateClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_terminologies"
    paginator: ListTerminologiesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListTerminologiesResponseTypeDef
        print(item)
    

    
```
