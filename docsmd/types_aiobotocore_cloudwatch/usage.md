# Examples

> [Index](../README.md) > [CloudWatch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudwatch]` package installed.

Write your `CloudWatch` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudwatch") as client:  # (1)
    result = await client.delete_alarms()  # (2)
```

1. client: [CloudWatchClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeAlarmHistoryPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudwatch") as client:  # (1)
    paginator = client.get_paginator("describe_alarm_history")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
3. item: [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 



```python
# AlarmExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudwatch") as client:  # (1)
    waiter = client.get_waiter("alarm_exists")  # (2)
    await waiter.wait()
```

1. client: [CloudWatchClient](./client.md)
2. waiter: [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[cloudwatch]`
or a standalone `types_aiobotocore_cloudwatch` package, you have to explicitly specify
`client: CloudWatchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.client import CloudWatchClient
from types_aiobotocore_cloudwatch.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_cloudwatch.type_defs import DeleteAlarmsInputTypeDef


session = get_session()

async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    kwargs: DeleteAlarmsInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.delete_alarms(**kwargs)
```



```python
# DescribeAlarmHistoryPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.client import CloudWatchClient
from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator
from types_aiobotocore_cloudwatch.type_defs import DescribeAlarmHistoryOutputTypeDef


session = get_session()

async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    paginator: DescribeAlarmHistoryPaginator = client.get_paginator("describe_alarm_history")
    async for item in paginator.paginate(...):
        item: DescribeAlarmHistoryOutputTypeDef
        print(item)
```



```python
# AlarmExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.client import CloudWatchClient
from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter


session = get_session()

async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
    waiter: AlarmExistsWaiter = client.get_waiter("alarm_exists")
    await waiter.wait()
```
