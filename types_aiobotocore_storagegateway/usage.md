<a id="examples-for-aiobotocore-storagegateway-module"></a>

# Examples for aiobotocore StorageGateway module

> [Index](../README.md) > [StorageGateway](./README.md) > Examples

- [Examples for aiobotocore StorageGateway module](#examples-for-aiobotocore-storagegateway-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[storagegateway]` package installed.

Write your `StorageGateway` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type StorageGatewayClient
# and provides type checking and code completion
async with session.create_client("storagegateway") as client:
    
    # result has type ActivateGatewayOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_gateway()
    

    
    # paginator has type DescribeTapeArchivesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_tape_archives")
    async for item in paginator.paginate(...):
        # item has type DescribeTapeArchivesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[storagegateway]` or a standalone
`types_aiobotocore_storagegateway` package, you have to explicitly specify
`client: StorageGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.client import StorageGatewayClient
from types_aiobotocore_storagegateway.type_defs import ActivateGatewayOutputTypeDef
from types_aiobotocore_storagegateway.paginator import DescribeTapeArchivesPaginator

from types_aiobotocore_storagegateway.literals import PaginatorName



session = get_session()

async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient

    
    result: ActivateGatewayOutputTypeDef = client.activate_gateway()
    

    
    paginator_name: PaginatorName = "describe_tape_archives"
    paginator: DescribeTapeArchivesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeTapeArchivesOutputTypeDef
        print(item)
    

    
```
