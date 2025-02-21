# Examples

> [Index](../README.md) > [Lightsail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#lightsail)
    type annotations stubs module [types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lightsail]` package installed.

Write your `Lightsail` code as usual,
type checking and code completion should work out of the box.



```python
# LightsailClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lightsail") as client:  # (1)
    result = await client.allocate_static_ip()  # (2)
```

1. client: [LightsailClient](./client.md)
2. result: [:material-code-braces: AllocateStaticIpResultTypeDef](./type_defs.md#allocatestaticipresulttypedef) 



```python
# GetActiveNamesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lightsail") as client:  # (1)
    paginator = client.get_paginator("get_active_names")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetActiveNamesPaginator](./paginators.md#getactivenamespaginator)
3. item: [:material-code-braces: GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[lightsail]`
or a standalone `types_aiobotocore_lightsail` package, you have to explicitly specify
`client: LightsailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LightsailClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.client import LightsailClient
from types_aiobotocore_lightsail.type_defs import AllocateStaticIpResultTypeDef
from types_aiobotocore_lightsail.type_defs import AllocateStaticIpRequestTypeDef


session = get_session()

async with session.create_client("lightsail") as client:
    client: LightsailClient
    kwargs: AllocateStaticIpRequestTypeDef = {...}
    result: AllocateStaticIpResultTypeDef = await client.allocate_static_ip(**kwargs)
```



```python
# GetActiveNamesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.client import LightsailClient
from types_aiobotocore_lightsail.paginator import GetActiveNamesPaginator
from types_aiobotocore_lightsail.type_defs import GetActiveNamesResultTypeDef


session = get_session()

async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetActiveNamesPaginator = client.get_paginator("get_active_names")
    async for item in paginator.paginate(...):
        item: GetActiveNamesResultTypeDef
        print(item)
```


