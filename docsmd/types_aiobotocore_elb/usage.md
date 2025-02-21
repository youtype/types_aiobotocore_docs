# Examples

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#elasticloadbalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[elb]` package installed.

Write your `ElasticLoadBalancing` code as usual,
type checking and code completion should work out of the box.



```python
# ElasticLoadBalancingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elb") as client:  # (1)
    result = await client.apply_security_groups_to_load_balancer()  # (2)
```

1. client: [ElasticLoadBalancingClient](./client.md)
2. result: [:material-code-braces: ApplySecurityGroupsToLoadBalancerOutputTypeDef](./type_defs.md#applysecuritygroupstoloadbalanceroutputtypedef) 



```python
# DescribeAccountLimitsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elb") as client:  # (1)
    paginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingClient](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



```python
# AnyInstanceInServiceWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elb") as client:  # (1)
    waiter = client.get_waiter("any_instance_in_service")  # (2)
    await waiter.wait()
```

1. client: [ElasticLoadBalancingClient](./client.md)
2. waiter: [AnyInstanceInServiceWaiter](./waiters.md#anyinstanceinservicewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[elb]`
or a standalone `types_aiobotocore_elb` package, you have to explicitly specify
`client: ElasticLoadBalancingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ElasticLoadBalancingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elb.client import ElasticLoadBalancingClient
from types_aiobotocore_elb.type_defs import ApplySecurityGroupsToLoadBalancerOutputTypeDef
from types_aiobotocore_elb.type_defs import ApplySecurityGroupsToLoadBalancerInputTypeDef


session = get_session()

async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
    kwargs: ApplySecurityGroupsToLoadBalancerInputTypeDef = {...}
    result: ApplySecurityGroupsToLoadBalancerOutputTypeDef = await client.apply_security_groups_to_load_balancer(**kwargs)
```



```python
# DescribeAccountLimitsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elb.client import ElasticLoadBalancingClient
from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator
from types_aiobotocore_elb.type_defs import DescribeAccountLimitsOutputTypeDef


session = get_session()

async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)
```



```python
# AnyInstanceInServiceWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elb.client import ElasticLoadBalancingClient
from types_aiobotocore_elb.waiter import AnyInstanceInServiceWaiter


session = get_session()

async with session.create_client("elb") as client:
    client: ElasticLoadBalancingClient
    waiter: AnyInstanceInServiceWaiter = client.get_waiter("any_instance_in_service")
    await waiter.wait()
```
