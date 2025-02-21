# Examples

> [Index](../README.md) > [MemoryDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#memorydb)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[memorydb]` package installed.

Write your `MemoryDB` code as usual,
type checking and code completion should work out of the box.



```python
# MemoryDBClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("memorydb") as client:  # (1)
    result = await client.batch_update_cluster()  # (2)
```

1. client: [MemoryDBClient](./client.md)
2. result: [:material-code-braces: BatchUpdateClusterResponseTypeDef](./type_defs.md#batchupdateclusterresponsetypedef) 



```python
# DescribeACLsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("memorydb") as client:  # (1)
    paginator = client.get_paginator("describe_acls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeACLsPaginator](./paginators.md#describeaclspaginator)
3. item: [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[memorydb]`
or a standalone `types_aiobotocore_memorydb` package, you have to explicitly specify
`client: MemoryDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MemoryDBClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.client import MemoryDBClient
from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterResponseTypeDef
from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterRequestTypeDef


session = get_session()

async with session.create_client("memorydb") as client:
    client: MemoryDBClient
    kwargs: BatchUpdateClusterRequestTypeDef = {...}
    result: BatchUpdateClusterResponseTypeDef = await client.batch_update_cluster(**kwargs)
```



```python
# DescribeACLsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.client import MemoryDBClient
from types_aiobotocore_memorydb.paginator import DescribeACLsPaginator
from types_aiobotocore_memorydb.type_defs import DescribeACLsResponseTypeDef


session = get_session()

async with session.create_client("memorydb") as client:
    client: MemoryDBClient
    paginator: DescribeACLsPaginator = client.get_paginator("describe_acls")
    async for item in paginator.paginate(...):
        item: DescribeACLsResponseTypeDef
        print(item)
```


