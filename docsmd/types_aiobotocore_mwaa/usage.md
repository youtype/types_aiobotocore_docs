# Examples

> [Index](../README.md) > [MWAA](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#mwaa)
    type annotations stubs module [types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mwaa]` package installed.

Write your `MWAA` code as usual,
type checking and code completion should work out of the box.



```python
# MWAAClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mwaa") as client:  # (1)
    result = await client.create_cli_token()  # (2)
```

1. client: [MWAAClient](./client.md)
2. result: [:material-code-braces: CreateCliTokenResponseTypeDef](./type_defs.md#createclitokenresponsetypedef) 



```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mwaa") as client:  # (1)
    paginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MWAAClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mwaa]`
or a standalone `types_aiobotocore_mwaa` package, you have to explicitly specify
`client: MWAAClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MWAAClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mwaa.client import MWAAClient
from types_aiobotocore_mwaa.type_defs import CreateCliTokenResponseTypeDef
from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestTypeDef


session = get_session()

async with session.create_client("mwaa") as client:
    client: MWAAClient
    kwargs: CreateCliTokenRequestTypeDef = {...}
    result: CreateCliTokenResponseTypeDef = await client.create_cli_token(**kwargs)
```



```python
# ListEnvironmentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mwaa.client import MWAAClient
from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator
from types_aiobotocore_mwaa.type_defs import ListEnvironmentsOutputTypeDef


session = get_session()

async with session.create_client("mwaa") as client:
    client: MWAAClient
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
    async for item in paginator.paginate(...):
        item: ListEnvironmentsOutputTypeDef
        print(item)
```


