# Examples

> [Index](../README.md) > [NetworkFlowMonitor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor)
    type annotations stubs module [types-aiobotocore-networkflowmonitor](https://pypi.org/project/types-aiobotocore-networkflowmonitor/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[networkflowmonitor]` package installed.

Write your `NetworkFlowMonitor` code as usual,
type checking and code completion should work out of the box.



```python
# NetworkFlowMonitorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkflowmonitor") as client:  # (1)
    result = await client.create_monitor()  # (2)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 



```python
# GetQueryResultsMonitorTopContributorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkflowmonitor") as client:  # (1)
    paginator = client.get_paginator("get_query_results_monitor_top_contributors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. paginator: [GetQueryResultsMonitorTopContributorsPaginator](./paginators.md#getqueryresultsmonitortopcontributorspaginator)
3. item: [:material-code-braces: GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[networkflowmonitor]`
or a standalone `types_aiobotocore_networkflowmonitor` package, you have to explicitly specify
`client: NetworkFlowMonitorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NetworkFlowMonitorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient
from types_aiobotocore_networkflowmonitor.type_defs import CreateMonitorOutputTypeDef
from types_aiobotocore_networkflowmonitor.type_defs import CreateMonitorInputTypeDef


session = get_session()

async with session.create_client("networkflowmonitor") as client:
    client: NetworkFlowMonitorClient
    kwargs: CreateMonitorInputTypeDef = {...}
    result: CreateMonitorOutputTypeDef = await client.create_monitor(**kwargs)
```



```python
# GetQueryResultsMonitorTopContributorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient
from types_aiobotocore_networkflowmonitor.paginator import GetQueryResultsMonitorTopContributorsPaginator
from types_aiobotocore_networkflowmonitor.type_defs import GetQueryResultsMonitorTopContributorsOutputTypeDef


session = get_session()

async with session.create_client("networkflowmonitor") as client:
    client: NetworkFlowMonitorClient
    paginator: GetQueryResultsMonitorTopContributorsPaginator = client.get_paginator("get_query_results_monitor_top_contributors")
    async for item in paginator.paginate(...):
        item: GetQueryResultsMonitorTopContributorsOutputTypeDef
        print(item)
```


