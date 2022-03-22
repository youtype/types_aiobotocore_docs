<a id="examples-for-aiobotocore-cloudwatchlogs-module"></a>

# Examples for aiobotocore CloudWatchLogs module

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Examples

- [Examples for aiobotocore CloudWatchLogs module](#examples-for-aiobotocore-cloudwatchlogs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[logs]` package installed.

Write your `CloudWatchLogs` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudWatchLogsClient
# and provides type checking and code completion
async with session.create_client("logs") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_kms_key()
    

    
    # paginator has type DescribeDestinationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_destinations")
    async for item in paginator.paginate(...):
        # item has type DescribeDestinationsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[logs]` or a standalone `types_aiobotocore_logs`
package, you have to explicitly specify `client: CloudWatchLogsClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_logs.client import CloudWatchLogsClient
from types_aiobotocore_logs.type_defs import None
from types_aiobotocore_logs.paginator import DescribeDestinationsPaginator

from types_aiobotocore_logs.literals import PaginatorName



session = get_session()

async with session.create_client("logs") as client:
    client: CloudWatchLogsClient

    
    result: None = client.associate_kms_key()
    

    
    paginator_name: PaginatorName = "describe_destinations"
    paginator: DescribeDestinationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeDestinationsResponseTypeDef
        print(item)
    

    
```
