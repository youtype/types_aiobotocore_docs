# Waiters

> [Index](../README.md) > [EKS](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## AddonActiveWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("addon_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/AddonActive.html#EKS.Waiter.AddonActive)

```python
# AddonActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import AddonActiveWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: AddonActiveWaiter = client.get_waiter("addon_active")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


### wait

Type annotations and code completion for `#!python AddonActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    addonName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeAddonRequestWaitTypeDef = {  # (1)
    "clusterName": ...,
    "addonName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeAddonRequestWaitTypeDef](./type_defs.md#describeaddonrequestwaittypedef) 
## AddonDeletedWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("addon_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/AddonDeleted.html#EKS.Waiter.AddonDeleted)

```python
# AddonDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import AddonDeletedWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: AddonDeletedWaiter = client.get_waiter("addon_deleted")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [AddonDeletedWaiter](./waiters.md#addondeletedwaiter)


### wait

Type annotations and code completion for `#!python AddonDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    addonName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeAddonRequestWaitExtraTypeDef = {  # (1)
    "clusterName": ...,
    "addonName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeAddonRequestWaitExtraTypeDef](./type_defs.md#describeaddonrequestwaitextratypedef) 
## ClusterActiveWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("cluster_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/ClusterActive.html#EKS.Waiter.ClusterActive)

```python
# ClusterActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import ClusterActiveWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: ClusterActiveWaiter = client.get_waiter("cluster_active")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)


### wait

Type annotations and code completion for `#!python ClusterActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeClusterRequestWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef) 
## ClusterDeletedWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("cluster_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/ClusterDeleted.html#EKS.Waiter.ClusterDeleted)

```python
# ClusterDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import ClusterDeletedWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)


### wait

Type annotations and code completion for `#!python ClusterDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeClusterRequestWaitExtraTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestWaitExtraTypeDef](./type_defs.md#describeclusterrequestwaitextratypedef) 
## FargateProfileActiveWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("fargate_profile_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/FargateProfileActive.html#EKS.Waiter.FargateProfileActive)

```python
# FargateProfileActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import FargateProfileActiveWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: FargateProfileActiveWaiter = client.get_waiter("fargate_profile_active")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [FargateProfileActiveWaiter](./waiters.md#fargateprofileactivewaiter)


### wait

Type annotations and code completion for `#!python FargateProfileActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeFargateProfileRequestWaitTypeDef = {  # (1)
    "clusterName": ...,
    "fargateProfileName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeFargateProfileRequestWaitTypeDef](./type_defs.md#describefargateprofilerequestwaittypedef) 
## FargateProfileDeletedWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("fargate_profile_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/FargateProfileDeleted.html#EKS.Waiter.FargateProfileDeleted)

```python
# FargateProfileDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import FargateProfileDeletedWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: FargateProfileDeletedWaiter = client.get_waiter("fargate_profile_deleted")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [FargateProfileDeletedWaiter](./waiters.md#fargateprofiledeletedwaiter)


### wait

Type annotations and code completion for `#!python FargateProfileDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeFargateProfileRequestWaitExtraTypeDef = {  # (1)
    "clusterName": ...,
    "fargateProfileName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeFargateProfileRequestWaitExtraTypeDef](./type_defs.md#describefargateprofilerequestwaitextratypedef) 
## NodegroupActiveWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("nodegroup_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/NodegroupActive.html#EKS.Waiter.NodegroupActive)

```python
# NodegroupActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import NodegroupActiveWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: NodegroupActiveWaiter = client.get_waiter("nodegroup_active")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [NodegroupActiveWaiter](./waiters.md#nodegroupactivewaiter)


### wait

Type annotations and code completion for `#!python NodegroupActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNodegroupRequestWaitTypeDef = {  # (1)
    "clusterName": ...,
    "nodegroupName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNodegroupRequestWaitTypeDef](./type_defs.md#describenodegrouprequestwaittypedef) 
## NodegroupDeletedWaiter

Type annotations and code completion for `#!python session.create_client("eks").get_waiter("nodegroup_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks/waiter/NodegroupDeleted.html#EKS.Waiter.NodegroupDeleted)

```python
# NodegroupDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_eks.waiter import NodegroupDeletedWaiter

session = get_session()
async with session.create_client("eks") as client:  # (1)
    waiter: NodegroupDeletedWaiter = client.get_waiter("nodegroup_deleted")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [NodegroupDeletedWaiter](./waiters.md#nodegroupdeletedwaiter)


### wait

Type annotations and code completion for `#!python NodegroupDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNodegroupRequestWaitExtraTypeDef = {  # (1)
    "clusterName": ...,
    "nodegroupName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNodegroupRequestWaitExtraTypeDef](./type_defs.md#describenodegrouprequestwaitextratypedef) 
