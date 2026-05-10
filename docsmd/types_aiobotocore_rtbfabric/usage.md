# Examples

> [Index](../README.md) > [RTBFabric](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[rtbfabric]` package installed.

Write your `RTBFabric` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RTBFabricClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rtbfabric") as client:  # (1)
    result = await client.accept_link()  # (2)
```

1. client: [RTBFabricClient](./client.md)
2. result: [:material-code-braces: AcceptLinkResponseTypeDef](./type_defs.md#acceptlinkresponsetypedef)



#### Paginator usage example

```python
# ListLinksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rtbfabric") as client:  # (1)
    paginator = client.get_paginator("list_links")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RTBFabricClient](./client.md)
2. paginator: [ListLinksPaginator](./paginators.md#listlinkspaginator)
3. item: [:material-code-braces: ListLinksResponseTypeDef](./type_defs.md#listlinksresponsetypedef)



#### Waiter usage example

```python
# InboundExternalLinkActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rtbfabric") as client:  # (1)
    waiter = client.get_waiter("inbound_external_link_active")  # (2)
    await waiter.wait(...)
```

1. client: [RTBFabricClient](./client.md)
2. waiter: [InboundExternalLinkActiveWaiter](./waiters.md#inboundexternallinkactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[rtbfabric]`
or a standalone `types_aiobotocore_rtbfabric` package, you have to explicitly specify
`client: RTBFabricClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RTBFabricClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.client import RTBFabricClient
from types_aiobotocore_rtbfabric.type_defs import AcceptLinkResponseTypeDef
from types_aiobotocore_rtbfabric.type_defs import AcceptLinkRequestTypeDef


session = get_session()

async with session.create_client("rtbfabric") as client:
    client: RTBFabricClient
    kwargs: AcceptLinkRequestTypeDef = {...}
    result: AcceptLinkResponseTypeDef = await client.accept_link(**kwargs)
```



#### Paginator usage example

```python
# ListLinksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.client import RTBFabricClient
from types_aiobotocore_rtbfabric.paginator import ListLinksPaginator
from types_aiobotocore_rtbfabric.type_defs import ListLinksResponseTypeDef


session = get_session()

async with session.create_client("rtbfabric") as client:
    client: RTBFabricClient
    paginator: ListLinksPaginator = client.get_paginator("list_links")
    async for item in paginator.paginate(...):
        item: ListLinksResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# InboundExternalLinkActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.client import RTBFabricClient
from types_aiobotocore_rtbfabric.waiter import InboundExternalLinkActiveWaiter


session = get_session()

async with session.create_client("rtbfabric") as client:
    client: RTBFabricClient
    waiter: InboundExternalLinkActiveWaiter = client.get_waiter("inbound_external_link_active")
    await waiter.wait(...)
```
