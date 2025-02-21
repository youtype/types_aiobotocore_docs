# Examples

> [Index](../README.md) > [MediaPackage](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#mediapackage)
    type annotations stubs module [types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediapackage]` package installed.

Write your `MediaPackage` code as usual,
type checking and code completion should work out of the box.



```python
# MediaPackageClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackage") as client:  # (1)
    result = await client.configure_logs()  # (2)
```

1. client: [MediaPackageClient](./client.md)
2. result: [:material-code-braces: ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef) 



```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mediapackage") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaPackageClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mediapackage]`
or a standalone `types_aiobotocore_mediapackage` package, you have to explicitly specify
`client: MediaPackageClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaPackageClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.client import MediaPackageClient
from types_aiobotocore_mediapackage.type_defs import ConfigureLogsResponseTypeDef
from types_aiobotocore_mediapackage.type_defs import ConfigureLogsRequestTypeDef


session = get_session()

async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
    kwargs: ConfigureLogsRequestTypeDef = {...}
    result: ConfigureLogsResponseTypeDef = await client.configure_logs(**kwargs)
```



```python
# ListChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.client import MediaPackageClient
from types_aiobotocore_mediapackage.paginator import ListChannelsPaginator
from types_aiobotocore_mediapackage.type_defs import ListChannelsResponseTypeDef


session = get_session()

async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
```


