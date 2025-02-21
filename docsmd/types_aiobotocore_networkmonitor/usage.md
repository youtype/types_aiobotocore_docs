# Examples

> [Index](../README.md) > [CloudWatchNetworkMonitor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchNetworkMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#cloudwatchnetworkmonitor)
    type annotations stubs module [types-aiobotocore-networkmonitor](https://pypi.org/project/types-aiobotocore-networkmonitor/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[networkmonitor]` package installed.

Write your `CloudWatchNetworkMonitor` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchNetworkMonitorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkmonitor") as client:  # (1)
    result = await client.create_monitor()  # (2)
```

1. client: [CloudWatchNetworkMonitorClient](./client.md)
2. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 



```python
# ListMonitorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkmonitor") as client:  # (1)
    paginator = client.get_paginator("list_monitors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchNetworkMonitorClient](./client.md)
2. paginator: [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
3. item: [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[networkmonitor]`
or a standalone `types_aiobotocore_networkmonitor` package, you have to explicitly specify
`client: CloudWatchNetworkMonitorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchNetworkMonitorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkmonitor.client import CloudWatchNetworkMonitorClient
from types_aiobotocore_networkmonitor.type_defs import CreateMonitorOutputTypeDef
from types_aiobotocore_networkmonitor.type_defs import CreateMonitorInputTypeDef


session = get_session()

async with session.create_client("networkmonitor") as client:
    client: CloudWatchNetworkMonitorClient
    kwargs: CreateMonitorInputTypeDef = {...}
    result: CreateMonitorOutputTypeDef = await client.create_monitor(**kwargs)
```



```python
# ListMonitorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkmonitor.client import CloudWatchNetworkMonitorClient
from types_aiobotocore_networkmonitor.paginator import ListMonitorsPaginator
from types_aiobotocore_networkmonitor.type_defs import ListMonitorsOutputTypeDef


session = get_session()

async with session.create_client("networkmonitor") as client:
    client: CloudWatchNetworkMonitorClient
    paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")
    async for item in paginator.paginate(...):
        item: ListMonitorsOutputTypeDef
        print(item)
```


