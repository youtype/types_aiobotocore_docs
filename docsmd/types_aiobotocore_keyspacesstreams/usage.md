# Examples

> [Index](../README.md) > [KeyspacesStreams](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KeyspacesStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams.html#keyspacesstreams)
    type annotations stubs module [types-aiobotocore-keyspacesstreams](https://pypi.org/project/types-aiobotocore-keyspacesstreams/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[keyspacesstreams]` package installed.

Write your `KeyspacesStreams` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# KeyspacesStreamsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("keyspacesstreams") as client:  # (1)
    result = await client.get_records()  # (2)
```

1. client: [KeyspacesStreamsClient](./client.md)
2. result: [:material-code-braces: GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)



#### Paginator usage example

```python
# GetStreamPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("keyspacesstreams") as client:  # (1)
    paginator = client.get_paginator("get_stream")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KeyspacesStreamsClient](./client.md)
2. paginator: [GetStreamPaginator](./paginators.md#getstreampaginator)
3. item: [:material-code-braces: GetStreamOutputTypeDef](./type_defs.md#getstreamoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[keyspacesstreams]`
or a standalone `types_aiobotocore_keyspacesstreams` package, you have to explicitly specify
`client: KeyspacesStreamsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# KeyspacesStreamsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_keyspacesstreams.client import KeyspacesStreamsClient
from types_aiobotocore_keyspacesstreams.type_defs import GetRecordsOutputTypeDef
from types_aiobotocore_keyspacesstreams.type_defs import GetRecordsInputTypeDef


session = get_session()

async with session.create_client("keyspacesstreams") as client:
    client: KeyspacesStreamsClient
    kwargs: GetRecordsInputTypeDef = {...}
    result: GetRecordsOutputTypeDef = await client.get_records(**kwargs)
```



#### Paginator usage example

```python
# GetStreamPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_keyspacesstreams.client import KeyspacesStreamsClient
from types_aiobotocore_keyspacesstreams.paginator import GetStreamPaginator
from types_aiobotocore_keyspacesstreams.type_defs import GetStreamOutputTypeDef


session = get_session()

async with session.create_client("keyspacesstreams") as client:
    client: KeyspacesStreamsClient
    paginator: GetStreamPaginator = client.get_paginator("get_stream")
    async for item in paginator.paginate(...):
        item: GetStreamOutputTypeDef
        print(item)
```


