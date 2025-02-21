# Examples

> [Index](../README.md) > [Translate](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[translate]` package installed.

Write your `Translate` code as usual,
type checking and code completion should work out of the box.



```python
# TranslateClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("translate") as client:  # (1)
    result = await client.create_parallel_data()  # (2)
```

1. client: [TranslateClient](./client.md)
2. result: [:material-code-braces: CreateParallelDataResponseTypeDef](./type_defs.md#createparalleldataresponsetypedef) 



```python
# ListTerminologiesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("translate") as client:  # (1)
    paginator = client.get_paginator("list_terminologies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TranslateClient](./client.md)
2. paginator: [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)
3. item: [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[translate]`
or a standalone `types_aiobotocore_translate` package, you have to explicitly specify
`client: TranslateClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TranslateClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_translate.client import TranslateClient
from types_aiobotocore_translate.type_defs import CreateParallelDataResponseTypeDef
from types_aiobotocore_translate.type_defs import CreateParallelDataRequestTypeDef


session = get_session()

async with session.create_client("translate") as client:
    client: TranslateClient
    kwargs: CreateParallelDataRequestTypeDef = {...}
    result: CreateParallelDataResponseTypeDef = await client.create_parallel_data(**kwargs)
```



```python
# ListTerminologiesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_translate.client import TranslateClient
from types_aiobotocore_translate.paginator import ListTerminologiesPaginator
from types_aiobotocore_translate.type_defs import ListTerminologiesResponseTypeDef


session = get_session()

async with session.create_client("translate") as client:
    client: TranslateClient
    paginator: ListTerminologiesPaginator = client.get_paginator("list_terminologies")
    async for item in paginator.paginate(...):
        item: ListTerminologiesResponseTypeDef
        print(item)
```


