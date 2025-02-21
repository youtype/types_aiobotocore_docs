# Examples

> [Index](../README.md) > [ElastiCache](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#elasticache)
    type annotations stubs module [types-aiobotocore-elasticache](https://pypi.org/project/types-aiobotocore-elasticache/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[elasticache]` package installed.

Write your `ElastiCache` code as usual,
type checking and code completion should work out of the box.



```python
# ElastiCacheClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticache") as client:  # (1)
    result = await client.add_tags_to_resource()  # (2)
```

1. client: [ElastiCacheClient](./client.md)
2. result: [:material-code-braces: TagListMessageTypeDef](./type_defs.md#taglistmessagetypedef) 



```python
# DescribeCacheClustersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticache") as client:  # (1)
    paginator = client.get_paginator("describe_cache_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheClustersPaginator](./paginators.md#describecacheclusterspaginator)
3. item: [:material-code-braces: CacheClusterMessageTypeDef](./type_defs.md#cacheclustermessagetypedef) 



```python
# CacheClusterAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticache") as client:  # (1)
    waiter = client.get_waiter("cache_cluster_available")  # (2)
    await waiter.wait()
```

1. client: [ElastiCacheClient](./client.md)
2. waiter: [CacheClusterAvailableWaiter](./waiters.md#cacheclusteravailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[elasticache]`
or a standalone `types_aiobotocore_elasticache` package, you have to explicitly specify
`client: ElastiCacheClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ElastiCacheClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.client import ElastiCacheClient
from types_aiobotocore_elasticache.type_defs import TagListMessageTypeDef
from types_aiobotocore_elasticache.type_defs import AddTagsToResourceMessageTypeDef


session = get_session()

async with session.create_client("elasticache") as client:
    client: ElastiCacheClient
    kwargs: AddTagsToResourceMessageTypeDef = {...}
    result: TagListMessageTypeDef = await client.add_tags_to_resource(**kwargs)
```



```python
# DescribeCacheClustersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.client import ElastiCacheClient
from types_aiobotocore_elasticache.paginator import DescribeCacheClustersPaginator
from types_aiobotocore_elasticache.type_defs import CacheClusterMessageTypeDef


session = get_session()

async with session.create_client("elasticache") as client:
    client: ElastiCacheClient
    paginator: DescribeCacheClustersPaginator = client.get_paginator("describe_cache_clusters")
    async for item in paginator.paginate(...):
        item: CacheClusterMessageTypeDef
        print(item)
```



```python
# CacheClusterAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.client import ElastiCacheClient
from types_aiobotocore_elasticache.waiter import CacheClusterAvailableWaiter


session = get_session()

async with session.create_client("elasticache") as client:
    client: ElastiCacheClient
    waiter: CacheClusterAvailableWaiter = client.get_waiter("cache_cluster_available")
    await waiter.wait()
```
