<a id="waiters-for-aiobotocore-elasticache-module"></a>

# Waiters for aiobotocore ElastiCache module

> [Index](../README.md) > [ElastiCache](./README.md) > Waiters

Auto-generated documentation for
[ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
type annotations stubs module
[types-aiobotocore-elasticache](https://pypi.org/project/types-aiobotocore-elasticache/).

- [Waiters for aiobotocore ElastiCache module](#waiters-for-aiobotocore-elasticache-module)
  - [CacheClusterAvailableWaiter](#cacheclusteravailablewaiter)
  - [CacheClusterDeletedWaiter](#cacheclusterdeletedwaiter)
  - [ReplicationGroupAvailableWaiter](#replicationgroupavailablewaiter)
  - [ReplicationGroupDeletedWaiter](#replicationgroupdeletedwaiter)

<a id="cacheclusteravailablewaiter"></a>

## CacheClusterAvailableWaiter

Type annotations for
`session.create_client("elasticache").get_waiter("cache_cluster_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticache.waiter import CacheClusterAvailableWaiter

def get_cache_cluster_available_waiter() -> CacheClusterAvailableWaiter:
    return Session().client("elasticache").get_waiter("cache_cluster_available")
```

Boto3 documentation:
[ElastiCache.Waiter.cache_cluster_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterAvailable)

Arguments for `CacheClusterAvailableWaiter.wait` method:

- `CacheClusterId`: `str`
- `MaxRecords`: `int`
- `Marker`: `str`
- `ShowCacheNodeInfo`: `bool`
- `ShowCacheClustersNotInReplicationGroups`: `bool`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="cacheclusterdeletedwaiter"></a>

## CacheClusterDeletedWaiter

Type annotations for
`session.create_client("elasticache").get_waiter("cache_cluster_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticache.waiter import CacheClusterDeletedWaiter

def get_cache_cluster_deleted_waiter() -> CacheClusterDeletedWaiter:
    return Session().client("elasticache").get_waiter("cache_cluster_deleted")
```

Boto3 documentation:
[ElastiCache.Waiter.cache_cluster_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.CacheClusterDeleted)

Arguments for `CacheClusterDeletedWaiter.wait` method:

- `CacheClusterId`: `str`
- `MaxRecords`: `int`
- `Marker`: `str`
- `ShowCacheNodeInfo`: `bool`
- `ShowCacheClustersNotInReplicationGroups`: `bool`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="replicationgroupavailablewaiter"></a>

## ReplicationGroupAvailableWaiter

Type annotations for
`session.create_client("elasticache").get_waiter("replication_group_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticache.waiter import ReplicationGroupAvailableWaiter

def get_replication_group_available_waiter() -> ReplicationGroupAvailableWaiter:
    return Session().client("elasticache").get_waiter("replication_group_available")
```

Boto3 documentation:
[ElastiCache.Waiter.replication_group_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupAvailable)

Arguments for `ReplicationGroupAvailableWaiter.wait` method:

- `ReplicationGroupId`: `str`
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="replicationgroupdeletedwaiter"></a>

## ReplicationGroupDeletedWaiter

Type annotations for
`session.create_client("elasticache").get_waiter("replication_group_deleted")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticache.waiter import ReplicationGroupDeletedWaiter

def get_replication_group_deleted_waiter() -> ReplicationGroupDeletedWaiter:
    return Session().client("elasticache").get_waiter("replication_group_deleted")
```

Boto3 documentation:
[ElastiCache.Waiter.replication_group_deleted](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Waiter.ReplicationGroupDeleted)

Arguments for `ReplicationGroupDeletedWaiter.wait` method:

- `ReplicationGroupId`: `str`
- `MaxRecords`: `int`
- `Marker`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
