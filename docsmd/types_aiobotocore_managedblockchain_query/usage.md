# Examples

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[managedblockchain-query]` package installed.

Write your `ManagedBlockchainQuery` code as usual,
type checking and code completion should work out of the box.



```python
# ManagedBlockchainQueryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("managedblockchain-query") as client:  # (1)
    result = await client.batch_get_token_balance()  # (2)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. result: [:material-code-braces: BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef) 



```python
# ListAssetContractsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator = client.get_paginator("list_asset_contracts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
3. item: [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[managedblockchain-query]`
or a standalone `types_aiobotocore_managedblockchain_query` package, you have to explicitly specify
`client: ManagedBlockchainQueryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ManagedBlockchainQueryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient
from types_aiobotocore_managedblockchain_query.type_defs import BatchGetTokenBalanceOutputTypeDef
from types_aiobotocore_managedblockchain_query.type_defs import BatchGetTokenBalanceInputTypeDef


session = get_session()

async with session.create_client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
    kwargs: BatchGetTokenBalanceInputTypeDef = {...}
    result: BatchGetTokenBalanceOutputTypeDef = await client.batch_get_token_balance(**kwargs)
```



```python
# ListAssetContractsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient
from types_aiobotocore_managedblockchain_query.paginator import ListAssetContractsPaginator
from types_aiobotocore_managedblockchain_query.type_defs import ListAssetContractsOutputTypeDef


session = get_session()

async with session.create_client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
    paginator: ListAssetContractsPaginator = client.get_paginator("list_asset_contracts")
    async for item in paginator.paginate(...):
        item: ListAssetContractsOutputTypeDef
        print(item)
```


