# Examples

> [Index](../README.md) > [AIOps](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AIOps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#aiops)
    type annotations stubs module [types-aiobotocore-aiops](https://pypi.org/project/types-aiobotocore-aiops/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[aiops]` package installed.

Write your `AIOps` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AIOpsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("aiops") as client:  # (1)
    result = await client.create_investigation_group()  # (2)
```

1. client: [AIOpsClient](./client.md)
2. result: [:material-code-braces: CreateInvestigationGroupOutputTypeDef](./type_defs.md#createinvestigationgroupoutputtypedef)



#### Paginator usage example

```python
# ListInvestigationGroupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("aiops") as client:  # (1)
    paginator = client.get_paginator("list_investigation_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AIOpsClient](./client.md)
2. paginator: [ListInvestigationGroupsPaginator](./paginators.md#listinvestigationgroupspaginator)
3. item: [:material-code-braces: ListInvestigationGroupsOutputTypeDef](./type_defs.md#listinvestigationgroupsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[aiops]`
or a standalone `types_aiobotocore_aiops` package, you have to explicitly specify
`client: AIOpsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AIOpsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_aiops.client import AIOpsClient
from types_aiobotocore_aiops.type_defs import CreateInvestigationGroupOutputTypeDef
from types_aiobotocore_aiops.type_defs import CreateInvestigationGroupInputTypeDef


session = get_session()

async with session.create_client("aiops") as client:
    client: AIOpsClient
    kwargs: CreateInvestigationGroupInputTypeDef = {...}
    result: CreateInvestigationGroupOutputTypeDef = await client.create_investigation_group(**kwargs)
```



#### Paginator usage example

```python
# ListInvestigationGroupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_aiops.client import AIOpsClient
from types_aiobotocore_aiops.paginator import ListInvestigationGroupsPaginator
from types_aiobotocore_aiops.type_defs import ListInvestigationGroupsOutputTypeDef


session = get_session()

async with session.create_client("aiops") as client:
    client: AIOpsClient
    paginator: ListInvestigationGroupsPaginator = client.get_paginator("list_investigation_groups")
    async for item in paginator.paginate(...):
        item: ListInvestigationGroupsOutputTypeDef
        print(item)
```


