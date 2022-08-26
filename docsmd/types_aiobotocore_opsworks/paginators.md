# Paginators

> [Index](../README.md) > [OpsWorks](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## DescribeEcsClustersPaginator

Type annotations and code completion for `#!python session.create_client("opsworks").get_paginator("describe_ecs_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator

session = get_session()
async with session.create_client("opsworks") as client:  # (1)
    paginator: DescribeEcsClustersPaginator = client.get_paginator("describe_ecs_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEcsClustersResultTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. paginator: [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)
3. item: [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEcsClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EcsClusterArns: Sequence[str] = ...,
    StackId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeEcsClustersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = {  # (1)
    "EcsClusterArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef](./type_defs.md#describeecsclustersrequestdescribeecsclusterspaginatetypedef) 
