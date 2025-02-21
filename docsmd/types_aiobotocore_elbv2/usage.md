# Examples

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#elasticloadbalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[elbv2]` package installed.

Write your `ElasticLoadBalancingv2` code as usual,
type checking and code completion should work out of the box.



```python
# ElasticLoadBalancingv2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elbv2") as client:  # (1)
    result = await client.add_listener_certificates()  # (2)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. result: [:material-code-braces: AddListenerCertificatesOutputTypeDef](./type_defs.md#addlistenercertificatesoutputtypedef) 



```python
# DescribeAccountLimitsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elbv2") as client:  # (1)
    paginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



```python
# LoadBalancerAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elbv2") as client:  # (1)
    waiter = client.get_waiter("load_balancer_available")  # (2)
    await waiter.wait()
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. waiter: [LoadBalancerAvailableWaiter](./waiters.md#loadbalanceravailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[elbv2]`
or a standalone `types_aiobotocore_elbv2` package, you have to explicitly specify
`client: ElasticLoadBalancingv2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ElasticLoadBalancingv2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elbv2.client import ElasticLoadBalancingv2Client
from types_aiobotocore_elbv2.type_defs import AddListenerCertificatesOutputTypeDef
from types_aiobotocore_elbv2.type_defs import AddListenerCertificatesInputTypeDef


session = get_session()

async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    kwargs: AddListenerCertificatesInputTypeDef = {...}
    result: AddListenerCertificatesOutputTypeDef = await client.add_listener_certificates(**kwargs)
```



```python
# DescribeAccountLimitsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elbv2.client import ElasticLoadBalancingv2Client
from types_aiobotocore_elbv2.paginator import DescribeAccountLimitsPaginator
from types_aiobotocore_elbv2.type_defs import DescribeAccountLimitsOutputTypeDef


session = get_session()

async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)
```



```python
# LoadBalancerAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elbv2.client import ElasticLoadBalancingv2Client
from types_aiobotocore_elbv2.waiter import LoadBalancerAvailableWaiter


session = get_session()

async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client
    waiter: LoadBalancerAvailableWaiter = client.get_waiter("load_balancer_available")
    await waiter.wait()
```
