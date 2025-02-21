# Examples

> [Index](../README.md) > [MainframeModernization](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#mainframemodernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[m2]` package installed.

Write your `MainframeModernization` code as usual,
type checking and code completion should work out of the box.



```python
# MainframeModernizationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("m2") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [MainframeModernizationClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



```python
# ListApplicationVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("m2") as client:  # (1)
    paginator = client.get_paginator("list_application_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MainframeModernizationClient](./client.md)
2. paginator: [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
3. item: [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[m2]`
or a standalone `types_aiobotocore_m2` package, you have to explicitly specify
`client: MainframeModernizationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MainframeModernizationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_m2.client import MainframeModernizationClient
from types_aiobotocore_m2.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_m2.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("m2") as client:
    client: MainframeModernizationClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```



```python
# ListApplicationVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_m2.client import MainframeModernizationClient
from types_aiobotocore_m2.paginator import ListApplicationVersionsPaginator
from types_aiobotocore_m2.type_defs import ListApplicationVersionsResponseTypeDef


session = get_session()

async with session.create_client("m2") as client:
    client: MainframeModernizationClient
    paginator: ListApplicationVersionsPaginator = client.get_paginator("list_application_versions")
    async for item in paginator.paginate(...):
        item: ListApplicationVersionsResponseTypeDef
        print(item)
```


