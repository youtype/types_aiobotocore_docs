# Examples

> [Index](../README.md) > [Interconnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Interconnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect.html#interconnect)
    type annotations stubs module [types-aiobotocore-interconnect](https://pypi.org/project/types-aiobotocore-interconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[interconnect]` package installed.

Write your `Interconnect` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# InterconnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("interconnect") as client:  # (1)
    result = await client.accept_connection_proposal()  # (2)
```

1. client: [InterconnectClient](./client.md)
2. result: [:material-code-braces: AcceptConnectionProposalResponseTypeDef](./type_defs.md#acceptconnectionproposalresponsetypedef)



#### Paginator usage example

```python
# ListAttachPointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("interconnect") as client:  # (1)
    paginator = client.get_paginator("list_attach_points")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [InterconnectClient](./client.md)
2. paginator: [ListAttachPointsPaginator](./paginators.md#listattachpointspaginator)
3. item: [:material-code-braces: ListAttachPointsResponseTypeDef](./type_defs.md#listattachpointsresponsetypedef)



#### Waiter usage example

```python
# ConnectionAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("interconnect") as client:  # (1)
    waiter = client.get_waiter("connection_available")  # (2)
    await waiter.wait(...)
```

1. client: [InterconnectClient](./client.md)
2. waiter: [ConnectionAvailableWaiter](./waiters.md#connectionavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[interconnect]`
or a standalone `types_aiobotocore_interconnect` package, you have to explicitly specify
`client: InterconnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# InterconnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.client import InterconnectClient
from types_aiobotocore_interconnect.type_defs import AcceptConnectionProposalResponseTypeDef
from types_aiobotocore_interconnect.type_defs import AcceptConnectionProposalRequestTypeDef


session = get_session()

async with session.create_client("interconnect") as client:
    client: InterconnectClient
    kwargs: AcceptConnectionProposalRequestTypeDef = {...}
    result: AcceptConnectionProposalResponseTypeDef = await client.accept_connection_proposal(**kwargs)
```



#### Paginator usage example

```python
# ListAttachPointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.client import InterconnectClient
from types_aiobotocore_interconnect.paginator import ListAttachPointsPaginator
from types_aiobotocore_interconnect.type_defs import ListAttachPointsResponseTypeDef


session = get_session()

async with session.create_client("interconnect") as client:
    client: InterconnectClient
    paginator: ListAttachPointsPaginator = client.get_paginator("list_attach_points")
    async for item in paginator.paginate(...):
        item: ListAttachPointsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# ConnectionAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.client import InterconnectClient
from types_aiobotocore_interconnect.waiter import ConnectionAvailableWaiter


session = get_session()

async with session.create_client("interconnect") as client:
    client: InterconnectClient
    waiter: ConnectionAvailableWaiter = client.get_waiter("connection_available")
    await waiter.wait(...)
```
