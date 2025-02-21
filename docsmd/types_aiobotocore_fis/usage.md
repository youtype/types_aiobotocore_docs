# Examples

> [Index](../README.md) > [FIS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#fis)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[fis]` package installed.

Write your `FIS` code as usual,
type checking and code completion should work out of the box.



```python
# FISClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fis") as client:  # (1)
    result = await client.create_experiment_template()  # (2)
```

1. client: [FISClient](./client.md)
2. result: [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef) 



```python
# ListActionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fis") as client:  # (1)
    paginator = client.get_paginator("list_actions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FISClient](./client.md)
2. paginator: [ListActionsPaginator](./paginators.md#listactionspaginator)
3. item: [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[fis]`
or a standalone `types_aiobotocore_fis` package, you have to explicitly specify
`client: FISClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FISClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fis.client import FISClient
from types_aiobotocore_fis.type_defs import CreateExperimentTemplateResponseTypeDef
from types_aiobotocore_fis.type_defs import CreateExperimentTemplateRequestTypeDef


session = get_session()

async with session.create_client("fis") as client:
    client: FISClient
    kwargs: CreateExperimentTemplateRequestTypeDef = {...}
    result: CreateExperimentTemplateResponseTypeDef = await client.create_experiment_template(**kwargs)
```



```python
# ListActionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fis.client import FISClient
from types_aiobotocore_fis.paginator import ListActionsPaginator
from types_aiobotocore_fis.type_defs import ListActionsResponseTypeDef


session = get_session()

async with session.create_client("fis") as client:
    client: FISClient
    paginator: ListActionsPaginator = client.get_paginator("list_actions")
    async for item in paginator.paginate(...):
        item: ListActionsResponseTypeDef
        print(item)
```


