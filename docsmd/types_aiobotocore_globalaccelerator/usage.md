# Examples

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#globalaccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[globalaccelerator]` package installed.

Write your `GlobalAccelerator` code as usual,
type checking and code completion should work out of the box.



```python
# GlobalAcceleratorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("globalaccelerator") as client:  # (1)
    result = await client.add_custom_routing_endpoints()  # (2)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. result: [:material-code-braces: AddCustomRoutingEndpointsResponseTypeDef](./type_defs.md#addcustomroutingendpointsresponsetypedef) 



```python
# ListAcceleratorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("globalaccelerator") as client:  # (1)
    paginator = client.get_paginator("list_accelerators")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListAcceleratorsPaginator](./paginators.md#listacceleratorspaginator)
3. item: [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[globalaccelerator]`
or a standalone `types_aiobotocore_globalaccelerator` package, you have to explicitly specify
`client: GlobalAcceleratorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GlobalAcceleratorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.client import GlobalAcceleratorClient
from types_aiobotocore_globalaccelerator.type_defs import AddCustomRoutingEndpointsResponseTypeDef
from types_aiobotocore_globalaccelerator.type_defs import AddCustomRoutingEndpointsRequestTypeDef


session = get_session()

async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    kwargs: AddCustomRoutingEndpointsRequestTypeDef = {...}
    result: AddCustomRoutingEndpointsResponseTypeDef = await client.add_custom_routing_endpoints(**kwargs)
```



```python
# ListAcceleratorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.client import GlobalAcceleratorClient
from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator
from types_aiobotocore_globalaccelerator.type_defs import ListAcceleratorsResponseTypeDef


session = get_session()

async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListAcceleratorsPaginator = client.get_paginator("list_accelerators")
    async for item in paginator.paginate(...):
        item: ListAcceleratorsResponseTypeDef
        print(item)
```


