# Examples

> [Index](../README.md) > [IVS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#ivs)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ivs]` package installed.

Write your `IVS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IVSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ivs") as client:  # (1)
    result = await client.batch_get_channel()  # (2)
```

1. client: [IVSClient](./client.md)
2. result: [:material-code-braces: BatchGetChannelResponseTypeDef](./type_defs.md#batchgetchannelresponsetypedef)



#### Paginator usage example

```python
# ListAdConfigurationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ivs") as client:  # (1)
    paginator = client.get_paginator("list_ad_configurations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IVSClient](./client.md)
2. paginator: [ListAdConfigurationsPaginator](./paginators.md#listadconfigurationspaginator)
3. item: [:material-code-braces: ListAdConfigurationsResponseTypeDef](./type_defs.md#listadconfigurationsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[ivs]`
or a standalone `types_aiobotocore_ivs` package, you have to explicitly specify
`client: IVSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IVSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ivs.client import IVSClient
from types_aiobotocore_ivs.type_defs import BatchGetChannelResponseTypeDef
from types_aiobotocore_ivs.type_defs import BatchGetChannelRequestTypeDef


session = get_session()

async with session.create_client("ivs") as client:
    client: IVSClient
    kwargs: BatchGetChannelRequestTypeDef = {...}
    result: BatchGetChannelResponseTypeDef = await client.batch_get_channel(**kwargs)
```



#### Paginator usage example

```python
# ListAdConfigurationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ivs.client import IVSClient
from types_aiobotocore_ivs.paginator import ListAdConfigurationsPaginator
from types_aiobotocore_ivs.type_defs import ListAdConfigurationsResponseTypeDef


session = get_session()

async with session.create_client("ivs") as client:
    client: IVSClient
    paginator: ListAdConfigurationsPaginator = client.get_paginator("list_ad_configurations")
    async for item in paginator.paginate(...):
        item: ListAdConfigurationsResponseTypeDef
        print(item)
```


