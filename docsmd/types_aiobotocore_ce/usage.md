# Examples

> [Index](../README.md) > [CostExplorer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#costexplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ce]` package installed.

Write your `CostExplorer` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CostExplorerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ce") as client:  # (1)
    result = await client.create_anomaly_monitor()  # (2)
```

1. client: [CostExplorerClient](./client.md)
2. result: [:material-code-braces: CreateAnomalyMonitorResponseTypeDef](./type_defs.md#createanomalymonitorresponsetypedef)



#### Paginator usage example

```python
# GetAnomaliesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ce") as client:  # (1)
    paginator = client.get_paginator("get_anomalies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CostExplorerClient](./client.md)
2. paginator: [GetAnomaliesPaginator](./paginators.md#getanomaliespaginator)
3. item: [:material-code-braces: GetAnomaliesResponseTypeDef](./type_defs.md#getanomaliesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[ce]`
or a standalone `types_aiobotocore_ce` package, you have to explicitly specify
`client: CostExplorerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CostExplorerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ce.client import CostExplorerClient
from types_aiobotocore_ce.type_defs import CreateAnomalyMonitorResponseTypeDef
from types_aiobotocore_ce.type_defs import CreateAnomalyMonitorRequestTypeDef


session = get_session()

async with session.create_client("ce") as client:
    client: CostExplorerClient
    kwargs: CreateAnomalyMonitorRequestTypeDef = {...}
    result: CreateAnomalyMonitorResponseTypeDef = await client.create_anomaly_monitor(**kwargs)
```



#### Paginator usage example

```python
# GetAnomaliesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ce.client import CostExplorerClient
from types_aiobotocore_ce.paginator import GetAnomaliesPaginator
from types_aiobotocore_ce.type_defs import GetAnomaliesResponseTypeDef


session = get_session()

async with session.create_client("ce") as client:
    client: CostExplorerClient
    paginator: GetAnomaliesPaginator = client.get_paginator("get_anomalies")
    async for item in paginator.paginate(...):
        item: GetAnomaliesResponseTypeDef
        print(item)
```


