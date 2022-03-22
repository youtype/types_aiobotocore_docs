<a id="paginators-for-aiobotocore-elasticloadbalancing-module"></a>

# Paginators for aiobotocore ElasticLoadBalancing module

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > Paginators

Auto-generated documentation for
[ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
type annotations stubs module
[types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

- [Paginators for aiobotocore ElasticLoadBalancing module](#paginators-for-aiobotocore-elasticloadbalancing-module)
  - [DescribeAccountLimitsPaginator](#describeaccountlimitspaginator)
  - [DescribeLoadBalancersPaginator](#describeloadbalancerspaginator)

<a id="describeaccountlimitspaginator"></a>

## DescribeAccountLimitsPaginator

Type annotations for
`session.create_client("elb").get_paginator("describe_account_limits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
```

Boto3 documentation:
[ElasticLoadBalancing.Paginator.DescribeAccountLimits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)

Arguments for `DescribeAccountLimitsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAccountLimitsPaginator.paginate` returns
`AsyncIterator`\[[DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)\].

<a id="describeloadbalancerspaginator"></a>

## DescribeLoadBalancersPaginator

Type annotations for
`session.create_client("elb").get_paginator("describe_load_balancers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elb.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
```

Boto3 documentation:
[ElasticLoadBalancing.Paginator.DescribeLoadBalancers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers)

Arguments for `DescribeLoadBalancersPaginator.paginate` method:

- `LoadBalancerNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLoadBalancersPaginator.paginate` returns
`AsyncIterator`\[[DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef)\].
