# Examples

> [Index](../README.md) > [StorageGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#storagegateway)
    type annotations stubs module [types-aiobotocore-storagegateway](https://pypi.org/project/types-aiobotocore-storagegateway/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[storagegateway]` package installed.

Write your `StorageGateway` code as usual,
type checking and code completion should work out of the box.



```python
# StorageGatewayClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("storagegateway") as client:  # (1)
    result = await client.activate_gateway()  # (2)
```

1. client: [StorageGatewayClient](./client.md)
2. result: [:material-code-braces: ActivateGatewayOutputTypeDef](./type_defs.md#activategatewayoutputtypedef) 



```python
# DescribeTapeArchivesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("storagegateway") as client:  # (1)
    paginator = client.get_paginator("describe_tape_archives")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [DescribeTapeArchivesPaginator](./paginators.md#describetapearchivespaginator)
3. item: [:material-code-braces: DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[storagegateway]`
or a standalone `types_aiobotocore_storagegateway` package, you have to explicitly specify
`client: StorageGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# StorageGatewayClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.client import StorageGatewayClient
from types_aiobotocore_storagegateway.type_defs import ActivateGatewayOutputTypeDef
from types_aiobotocore_storagegateway.type_defs import ActivateGatewayInputTypeDef


session = get_session()

async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    kwargs: ActivateGatewayInputTypeDef = {...}
    result: ActivateGatewayOutputTypeDef = await client.activate_gateway(**kwargs)
```



```python
# DescribeTapeArchivesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.client import StorageGatewayClient
from types_aiobotocore_storagegateway.paginator import DescribeTapeArchivesPaginator
from types_aiobotocore_storagegateway.type_defs import DescribeTapeArchivesOutputTypeDef


session = get_session()

async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: DescribeTapeArchivesPaginator = client.get_paginator("describe_tape_archives")
    async for item in paginator.paginate(...):
        item: DescribeTapeArchivesOutputTypeDef
        print(item)
```


