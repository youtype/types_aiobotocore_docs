# Examples

> [Index](../README.md) > [EVS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#evs)
    type annotations stubs module [types-aiobotocore-evs](https://pypi.org/project/types-aiobotocore-evs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[evs]` package installed.

Write your `EVS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EVSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("evs") as client:  # (1)
    result = await client.associate_eip_to_vlan()  # (2)
```

1. client: [EVSClient](./client.md)
2. result: [:material-code-braces: AssociateEipToVlanResponseTypeDef](./type_defs.md#associateeiptovlanresponsetypedef)



#### Paginator usage example

```python
# ListEnvironmentHostsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("evs") as client:  # (1)
    paginator = client.get_paginator("list_environment_hosts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EVSClient](./client.md)
2. paginator: [ListEnvironmentHostsPaginator](./paginators.md#listenvironmenthostspaginator)
3. item: [:material-code-braces: ListEnvironmentHostsResponseTypeDef](./type_defs.md#listenvironmenthostsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[evs]`
or a standalone `types_aiobotocore_evs` package, you have to explicitly specify
`client: EVSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EVSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_evs.client import EVSClient
from types_aiobotocore_evs.type_defs import AssociateEipToVlanResponseTypeDef
from types_aiobotocore_evs.type_defs import AssociateEipToVlanRequestTypeDef


session = get_session()

async with session.create_client("evs") as client:
    client: EVSClient
    kwargs: AssociateEipToVlanRequestTypeDef = {...}
    result: AssociateEipToVlanResponseTypeDef = await client.associate_eip_to_vlan(**kwargs)
```



#### Paginator usage example

```python
# ListEnvironmentHostsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_evs.client import EVSClient
from types_aiobotocore_evs.paginator import ListEnvironmentHostsPaginator
from types_aiobotocore_evs.type_defs import ListEnvironmentHostsResponseTypeDef


session = get_session()

async with session.create_client("evs") as client:
    client: EVSClient
    paginator: ListEnvironmentHostsPaginator = client.get_paginator("list_environment_hosts")
    async for item in paginator.paginate(...):
        item: ListEnvironmentHostsResponseTypeDef
        print(item)
```


