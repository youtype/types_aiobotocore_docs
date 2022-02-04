<a id="paginators-for-aiobotocore-elasticloadbalancing-module"></a>

# Paginators for aiobotocore ElasticLoadBalancing module

> [Index](..) > [ElasticLoadBalancing](.) > Paginators

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
`aiobotocore.create_client("elb").get_paginator("describe_account_limits")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator

def get_describe_account_limits_paginator() -> DescribeAccountLimitsPaginator:
    return Session().create_client("elb").get_paginator("describe_account_limits")
```

Boto3 documentation:
[ElasticLoadBalancing.Paginator.DescribeAccountLimits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)

Arguments for `DescribeAccountLimitsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAccountLimitsPaginator.paginate` returns
`_PageIterator`\[[DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)\].

<a id="describeloadbalancerspaginator"></a>

## DescribeLoadBalancersPaginator

Type annotations for
`aiobotocore.create_client("elb").get_paginator("describe_load_balancers")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elb.paginator import DescribeLoadBalancersPaginator

def get_describe_load_balancers_paginator() -> DescribeLoadBalancersPaginator:
    return Session().create_client("elb").get_paginator("describe_load_balancers")
```

Boto3 documentation:
[ElasticLoadBalancing.Paginator.DescribeLoadBalancers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers)

Arguments for `DescribeLoadBalancersPaginator.paginate` method:

- `LoadBalancerNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLoadBalancersPaginator.paginate` returns
`_PageIterator`\[[DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef)\].
