<a id="examples-for-aiobotocore-elasticloadbalancingv2-module"></a>

# Examples for aiobotocore ElasticLoadBalancingv2 module

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Examples

- [Examples for aiobotocore ElasticLoadBalancingv2 module](#examples-for-aiobotocore-elasticloadbalancingv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[elbv2]` package installed.

Write your `ElasticLoadBalancingv2` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElasticLoadBalancingv2Client
# and provides type checking and code completion
async with session.create_client("elbv2") as client:
    
    # result has type AddListenerCertificatesOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_listener_certificates()
    

    
    # paginator has type DescribeAccountLimitsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_account_limits")
    async for item in paginator.paginate(...):
        # item has type DescribeAccountLimitsOutputTypeDef
        print(item)
    

    
    # waiter has type LoadBalancerAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("load_balancer_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[elbv2]` or a standalone `types_aiobotocore_elbv2`
package, you have to explicitly specify `client: ElasticLoadBalancingv2Client`
type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_elbv2.client import ElasticLoadBalancingv2Client
from types_aiobotocore_elbv2.type_defs import AddListenerCertificatesOutputTypeDef
from types_aiobotocore_elbv2.paginator import DescribeAccountLimitsPaginator
from types_aiobotocore_elbv2.waiter import LoadBalancerAvailableWaiter
from types_aiobotocore_elbv2.literals import PaginatorName
from types_aiobotocore_elbv2.literals import WaiterName


session = get_session()

async with session.create_client("elbv2") as client:
    client: ElasticLoadBalancingv2Client

    
    result: AddListenerCertificatesOutputTypeDef = client.add_listener_certificates()
    

    
    paginator_name: PaginatorName = "describe_account_limits"
    paginator: DescribeAccountLimitsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "load_balancer_available"
    waiter: LoadBalancerAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
