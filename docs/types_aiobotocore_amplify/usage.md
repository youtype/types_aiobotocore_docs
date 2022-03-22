<a id="examples-for-aiobotocore-amplify-module"></a>

# Examples for aiobotocore Amplify module

> [Index](../README.md) > [Amplify](./README.md) > Examples

- [Examples for aiobotocore Amplify module](#examples-for-aiobotocore-amplify-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[amplify]` package installed.

Write your `Amplify` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AmplifyClient
# and provides type checking and code completion
async with session.create_client("amplify") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAppsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_apps")
    async for item in paginator.paginate(...):
        # item has type ListAppsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[amplify]` or a standalone
`types_aiobotocore_amplify` package, you have to explicitly specify
`client: AmplifyClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplify.client import AmplifyClient
from types_aiobotocore_amplify.type_defs import bool
from types_aiobotocore_amplify.paginator import ListAppsPaginator

from types_aiobotocore_amplify.literals import PaginatorName



session = get_session()

async with session.create_client("amplify") as client:
    client: AmplifyClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_apps"
    paginator: ListAppsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAppsResultTypeDef
        print(item)
    

    
```
