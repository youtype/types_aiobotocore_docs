# Examples

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[internetmonitor]` package installed.

Write your `CloudWatchInternetMonitor` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchInternetMonitorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("internetmonitor") as client:  # (1)
    result = await client.create_monitor()  # (2)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 



```python
# ListHealthEventsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("internetmonitor") as client:  # (1)
    paginator = client.get_paginator("list_health_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
3. item: [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[internetmonitor]`
or a standalone `types_aiobotocore_internetmonitor` package, you have to explicitly specify
`client: CloudWatchInternetMonitorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchInternetMonitorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient
from types_aiobotocore_internetmonitor.type_defs import CreateMonitorOutputTypeDef
from types_aiobotocore_internetmonitor.type_defs import CreateMonitorInputTypeDef


session = get_session()

async with session.create_client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
    kwargs: CreateMonitorInputTypeDef = {...}
    result: CreateMonitorOutputTypeDef = await client.create_monitor(**kwargs)
```



```python
# ListHealthEventsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient
from types_aiobotocore_internetmonitor.paginator import ListHealthEventsPaginator
from types_aiobotocore_internetmonitor.type_defs import ListHealthEventsOutputTypeDef


session = get_session()

async with session.create_client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
    paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")
    async for item in paginator.paginate(...):
        item: ListHealthEventsOutputTypeDef
        print(item)
```


