<a id="paginators-for-aiobotocore-opsworks-module"></a>

# Paginators for aiobotocore OpsWorks module

> [Index](..) > [OpsWorks](.) > Paginators

Auto-generated documentation for
[OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
type annotations stubs module
[types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

- [Paginators for aiobotocore OpsWorks module](#paginators-for-aiobotocore-opsworks-module)
  - [DescribeEcsClustersPaginator](#describeecsclusterspaginator)

<a id="describeecsclusterspaginator"></a>

## DescribeEcsClustersPaginator

Type annotations for
`aiobotocore.create_client("opsworks").get_paginator("describe_ecs_clusters")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator

def get_describe_ecs_clusters_paginator() -> DescribeEcsClustersPaginator:
    return Session().create_client("opsworks").get_paginator("describe_ecs_clusters")
```

Boto3 documentation:
[OpsWorks.Paginator.DescribeEcsClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters)

Arguments for `DescribeEcsClustersPaginator.paginate` method:

- `EcsClusterArns`: `Sequence`\[`str`\]
- `StackId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEcsClustersPaginator.paginate` returns
`_PageIterator`\[[DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef)\].
