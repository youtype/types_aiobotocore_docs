# Examples

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#amplifyuibuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[amplifyuibuilder]` package installed.

Write your `AmplifyUIBuilder` code as usual,
type checking and code completion should work out of the box.



```python
# AmplifyUIBuilderClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplifyuibuilder") as client:  # (1)
    result = await client.create_component()  # (2)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. result: [:material-code-braces: CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef) 



```python
# ExportComponentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator = client.get_paginator("export_components")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
3. item: [:material-code-braces: ExportComponentsResponsePaginatorTypeDef](./type_defs.md#exportcomponentsresponsepaginatortypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[amplifyuibuilder]`
or a standalone `types_aiobotocore_amplifyuibuilder` package, you have to explicitly specify
`client: AmplifyUIBuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AmplifyUIBuilderClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient
from types_aiobotocore_amplifyuibuilder.type_defs import CreateComponentResponseTypeDef
from types_aiobotocore_amplifyuibuilder.type_defs import CreateComponentRequestTypeDef


session = get_session()

async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    kwargs: CreateComponentRequestTypeDef = {...}
    result: CreateComponentResponseTypeDef = await client.create_component(**kwargs)
```



```python
# ExportComponentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient
from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator
from types_aiobotocore_amplifyuibuilder.type_defs import ExportComponentsResponsePaginatorTypeDef


session = get_session()

async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")
    async for item in paginator.paginate(...):
        item: ExportComponentsResponsePaginatorTypeDef
        print(item)
```


