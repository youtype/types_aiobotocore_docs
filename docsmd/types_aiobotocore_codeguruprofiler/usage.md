# Examples

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#codeguruprofiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codeguruprofiler]` package installed.

Write your `CodeGuruProfiler` code as usual,
type checking and code completion should work out of the box.



```python
# CodeGuruProfilerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeguruprofiler") as client:  # (1)
    result = await client.add_notification_channels()  # (2)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. result: [:material-code-braces: AddNotificationChannelsResponseTypeDef](./type_defs.md#addnotificationchannelsresponsetypedef) 



```python
# ListProfileTimesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeguruprofiler") as client:  # (1)
    paginator = client.get_paginator("list_profile_times")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. paginator: [ListProfileTimesPaginator](./paginators.md#listprofiletimespaginator)
3. item: [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[codeguruprofiler]`
or a standalone `types_aiobotocore_codeguruprofiler` package, you have to explicitly specify
`client: CodeGuruProfilerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeGuruProfilerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient
from types_aiobotocore_codeguruprofiler.type_defs import AddNotificationChannelsResponseTypeDef
from types_aiobotocore_codeguruprofiler.type_defs import AddNotificationChannelsRequestTypeDef


session = get_session()

async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient
    kwargs: AddNotificationChannelsRequestTypeDef = {...}
    result: AddNotificationChannelsResponseTypeDef = await client.add_notification_channels(**kwargs)
```



```python
# ListProfileTimesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient
from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator
from types_aiobotocore_codeguruprofiler.type_defs import ListProfileTimesResponseTypeDef


session = get_session()

async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient
    paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
    async for item in paginator.paginate(...):
        item: ListProfileTimesResponseTypeDef
        print(item)
```


