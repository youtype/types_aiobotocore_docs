# Examples

> [Index](../README.md) > [NetworkManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#networkmanager)
    type annotations stubs module [types-aiobotocore-networkmanager](https://pypi.org/project/types-aiobotocore-networkmanager/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[networkmanager]` package installed.

Write your `NetworkManager` code as usual,
type checking and code completion should work out of the box.



```python
# NetworkManagerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkmanager") as client:  # (1)
    result = await client.accept_attachment()  # (2)
```

1. client: [NetworkManagerClient](./client.md)
2. result: [:material-code-braces: AcceptAttachmentResponseTypeDef](./type_defs.md#acceptattachmentresponsetypedef) 



```python
# DescribeGlobalNetworksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("networkmanager") as client:  # (1)
    paginator = client.get_paginator("describe_global_networks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NetworkManagerClient](./client.md)
2. paginator: [DescribeGlobalNetworksPaginator](./paginators.md#describeglobalnetworkspaginator)
3. item: [:material-code-braces: DescribeGlobalNetworksResponseTypeDef](./type_defs.md#describeglobalnetworksresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[networkmanager]`
or a standalone `types_aiobotocore_networkmanager` package, you have to explicitly specify
`client: NetworkManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NetworkManagerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.client import NetworkManagerClient
from types_aiobotocore_networkmanager.type_defs import AcceptAttachmentResponseTypeDef
from types_aiobotocore_networkmanager.type_defs import AcceptAttachmentRequestTypeDef


session = get_session()

async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    kwargs: AcceptAttachmentRequestTypeDef = {...}
    result: AcceptAttachmentResponseTypeDef = await client.accept_attachment(**kwargs)
```



```python
# DescribeGlobalNetworksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.client import NetworkManagerClient
from types_aiobotocore_networkmanager.paginator import DescribeGlobalNetworksPaginator
from types_aiobotocore_networkmanager.type_defs import DescribeGlobalNetworksResponseTypeDef


session = get_session()

async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: DescribeGlobalNetworksPaginator = client.get_paginator("describe_global_networks")
    async for item in paginator.paginate(...):
        item: DescribeGlobalNetworksResponseTypeDef
        print(item)
```


