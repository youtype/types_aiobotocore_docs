# Paginators

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.create_client("elb").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("elb") as client:  # (1)
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingClient](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsinputdescribeaccountlimitspaginatetypedef) 
## DescribeLoadBalancersPaginator

Type annotations and code completion for `#!python session.create_client("elb").get_paginator("describe_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elb.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("elb") as client:  # (1)
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccessPointsOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingClient](./client.md)
2. paginator: [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)
3. item: [:material-code-braces: DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccessPointsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = {  # (1)
    "LoadBalancerNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef](./type_defs.md#describeaccesspointsinputdescribeloadbalancerspaginatetypedef) 
