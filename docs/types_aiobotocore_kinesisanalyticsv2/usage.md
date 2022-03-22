<a id="examples-for-aiobotocore-kinesisanalyticsv2-module"></a>

# Examples for aiobotocore KinesisAnalyticsV2 module

> [Index](../README.md) > [KinesisAnalyticsV2](./README.md) > Examples

- [Examples for aiobotocore KinesisAnalyticsV2 module](#examples-for-aiobotocore-kinesisanalyticsv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisanalyticsv2]` package installed.

Write your `KinesisAnalyticsV2` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisAnalyticsV2Client
# and provides type checking and code completion
async with session.create_client("kinesisanalyticsv2") as client:
    
    # result has type AddApplicationCloudWatchLoggingOptionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_application_cloud_watch_logging_option()
    

    
    # paginator has type ListApplicationSnapshotsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_application_snapshots")
    async for item in paginator.paginate(...):
        # item has type ListApplicationSnapshotsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesisanalyticsv2]` or a standalone
`types_aiobotocore_kinesisanalyticsv2` package, you have to explicitly specify
`client: KinesisAnalyticsV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesisanalyticsv2.client import KinesisAnalyticsV2Client
from types_aiobotocore_kinesisanalyticsv2.type_defs import AddApplicationCloudWatchLoggingOptionResponseTypeDef
from types_aiobotocore_kinesisanalyticsv2.paginator import ListApplicationSnapshotsPaginator

from types_aiobotocore_kinesisanalyticsv2.literals import PaginatorName



session = get_session()

async with session.create_client("kinesisanalyticsv2") as client:
    client: KinesisAnalyticsV2Client

    
    result: AddApplicationCloudWatchLoggingOptionResponseTypeDef = client.add_application_cloud_watch_logging_option()
    

    
    paginator_name: PaginatorName = "list_application_snapshots"
    paginator: ListApplicationSnapshotsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationSnapshotsResponseTypeDef
        print(item)
    

    
```
