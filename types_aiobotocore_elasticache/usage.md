<a id="examples-for-aiobotocore-elasticache-module"></a>

# Examples for aiobotocore ElastiCache module

> [Index](../README.md) > [ElastiCache](./README.md) > Examples

- [Examples for aiobotocore ElastiCache module](#examples-for-aiobotocore-elasticache-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[elasticache]` package installed.

Write your `ElastiCache` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElastiCacheClient
# and provides type checking and code completion
async with session.create_client("elasticache") as client:
    
    # result has type TagListMessageTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_resource()
    

    
    # paginator has type DescribeCacheClustersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_cache_clusters")
    async for item in paginator.paginate(...):
        # item has type CacheClusterMessageTypeDef
        print(item)
    

    
    # waiter has type CacheClusterAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("cache_cluster_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[elasticache]` or a standalone
`types_aiobotocore_elasticache` package, you have to explicitly specify
`client: ElastiCacheClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_elasticache.client import ElastiCacheClient
from types_aiobotocore_elasticache.type_defs import TagListMessageTypeDef
from types_aiobotocore_elasticache.paginator import DescribeCacheClustersPaginator
from types_aiobotocore_elasticache.waiter import CacheClusterAvailableWaiter
from types_aiobotocore_elasticache.literals import PaginatorName
from types_aiobotocore_elasticache.literals import WaiterName


session = get_session()

async with session.create_client("elasticache") as client:
    client: ElastiCacheClient

    
    result: TagListMessageTypeDef = client.add_tags_to_resource()
    

    
    paginator_name: PaginatorName = "describe_cache_clusters"
    paginator: DescribeCacheClustersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: CacheClusterMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "cache_cluster_available"
    waiter: CacheClusterAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
