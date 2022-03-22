<a id="examples-for-aiobotocore-cloudwatch-module"></a>

# Examples for aiobotocore CloudWatch module

> [Index](../README.md) > [CloudWatch](./README.md) > Examples

- [Examples for aiobotocore CloudWatch module](#examples-for-aiobotocore-cloudwatch-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudwatch]` package installed.

Write your `CloudWatch` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudWatchClient
# and provides type checking and code completion
async with session.create_client("cloudwatch") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeAlarmHistoryPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_alarm_history")
    async for item in paginator.paginate(...):
        # item has type DescribeAlarmHistoryOutputTypeDef
        print(item)
    

    
    # waiter has type AlarmExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("alarm_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudwatch]` or a standalone
`types_aiobotocore_cloudwatch` package, you have to explicitly specify
`client: CloudWatchClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.client import CloudWatchClient
from types_aiobotocore_cloudwatch.type_defs import bool
from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator
from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter
from types_aiobotocore_cloudwatch.literals import PaginatorName
from types_aiobotocore_cloudwatch.literals import WaiterName


session = get_session()

async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_alarm_history"
    paginator: DescribeAlarmHistoryPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAlarmHistoryOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "alarm_exists"
    waiter: AlarmExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
