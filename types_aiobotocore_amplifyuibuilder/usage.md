<a id="examples-for-aiobotocore-amplifyuibuilder-module"></a>

# Examples for aiobotocore AmplifyUIBuilder module

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Examples

- [Examples for aiobotocore AmplifyUIBuilder module](#examples-for-aiobotocore-amplifyuibuilder-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[amplifyuibuilder]` package installed.

Write your `AmplifyUIBuilder` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AmplifyUIBuilderClient
# and provides type checking and code completion
async with session.create_client("amplifyuibuilder") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ExportComponentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("export_components")
    async for item in paginator.paginate(...):
        # item has type ExportComponentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[amplifyuibuilder]` or a standalone
`types_aiobotocore_amplifyuibuilder` package, you have to explicitly specify
`client: AmplifyUIBuilderClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient
from types_aiobotocore_amplifyuibuilder.type_defs import bool
from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

from types_aiobotocore_amplifyuibuilder.literals import PaginatorName



session = get_session()

async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "export_components"
    paginator: ExportComponentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ExportComponentsResponseTypeDef
        print(item)
    

    
```
