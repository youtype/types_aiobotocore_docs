# Examples

> [Index](../README.md) > [Amplify](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#amplify)
    type annotations stubs module [types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[amplify]` package installed.

Write your `Amplify` code as usual,
type checking and code completion should work out of the box.



```python
# AmplifyClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplify") as client:  # (1)
    result = await client.create_app()  # (2)
```

1. client: [AmplifyClient](./client.md)
2. result: [:material-code-braces: CreateAppResultTypeDef](./type_defs.md#createappresulttypedef) 



```python
# ListAppsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplify") as client:  # (1)
    paginator = client.get_paginator("list_apps")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AmplifyClient](./client.md)
2. paginator: [ListAppsPaginator](./paginators.md#listappspaginator)
3. item: [:material-code-braces: ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[amplify]`
or a standalone `types_aiobotocore_amplify` package, you have to explicitly specify
`client: AmplifyClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AmplifyClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplify.client import AmplifyClient
from types_aiobotocore_amplify.type_defs import CreateAppResultTypeDef
from types_aiobotocore_amplify.type_defs import CreateAppRequestTypeDef


session = get_session()

async with session.create_client("amplify") as client:
    client: AmplifyClient
    kwargs: CreateAppRequestTypeDef = {...}
    result: CreateAppResultTypeDef = await client.create_app(**kwargs)
```



```python
# ListAppsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplify.client import AmplifyClient
from types_aiobotocore_amplify.paginator import ListAppsPaginator
from types_aiobotocore_amplify.type_defs import ListAppsResultTypeDef


session = get_session()

async with session.create_client("amplify") as client:
    client: AmplifyClient
    paginator: ListAppsPaginator = client.get_paginator("list_apps")
    async for item in paginator.paginate(...):
        item: ListAppsResultTypeDef
        print(item)
```


