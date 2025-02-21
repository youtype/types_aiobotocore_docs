# Waiters

> [Index](../README.md) > [AuroraDSQL](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## ClusterActiveWaiter

Type annotations and code completion for `#!python session.create_client("dsql").get_waiter("cluster_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/waiter/ClusterActive.html#AuroraDSQL.Waiter.ClusterActive)

```python
# ClusterActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dsql.waiter import ClusterActiveWaiter

session = get_session()
async with session.create_client("dsql") as client:  # (1)
    waiter: ClusterActiveWaiter = client.get_waiter("cluster_active")  # (2)
    await waiter.wait()
```

1. client: [AuroraDSQLClient](./client.md)
2. waiter: [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)


### wait

Type annotations and code completion for `#!python ClusterActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetClusterInputWaitTypeDef = {  # (1)
    "identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetClusterInputWaitTypeDef](./type_defs.md#getclusterinputwaittypedef) 
## ClusterNotExistsWaiter

Type annotations and code completion for `#!python session.create_client("dsql").get_waiter("cluster_not_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/waiter/ClusterNotExists.html#AuroraDSQL.Waiter.ClusterNotExists)

```python
# ClusterNotExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dsql.waiter import ClusterNotExistsWaiter

session = get_session()
async with session.create_client("dsql") as client:  # (1)
    waiter: ClusterNotExistsWaiter = client.get_waiter("cluster_not_exists")  # (2)
    await waiter.wait()
```

1. client: [AuroraDSQLClient](./client.md)
2. waiter: [ClusterNotExistsWaiter](./waiters.md#clusternotexistswaiter)


### wait

Type annotations and code completion for `#!python ClusterNotExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetClusterInputWaitExtraTypeDef = {  # (1)
    "identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetClusterInputWaitExtraTypeDef](./type_defs.md#getclusterinputwaitextratypedef) 
