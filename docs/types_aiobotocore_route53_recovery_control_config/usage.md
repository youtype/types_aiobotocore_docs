<a id="examples-for-aiobotocore-route53recoverycontrolconfig-module"></a>

# Examples for aiobotocore Route53RecoveryControlConfig module

> [Index](../README.md) > [Route53RecoveryControlConfig](./README.md) >
> Examples

- [Examples for aiobotocore Route53RecoveryControlConfig module](#examples-for-aiobotocore-route53recoverycontrolconfig-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53-recovery-control-config]` package
installed.

Write your `Route53RecoveryControlConfig` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53RecoveryControlConfigClient
# and provides type checking and code completion
async with session.create_client("route53-recovery-control-config") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
    # waiter has type ClusterCreatedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("cluster_created")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53-recovery-control-config]` or a standalone
`types_aiobotocore_route53_recovery_control_config` package, you have to
explicitly specify `client: Route53RecoveryControlConfigClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
from types_aiobotocore_route53_recovery_control_config.type_defs import bool

from types_aiobotocore_route53_recovery_control_config.waiter import ClusterCreatedWaiter

from types_aiobotocore_route53_recovery_control_config.literals import WaiterName


session = get_session()

async with session.create_client("route53-recovery-control-config") as client:
    client: Route53RecoveryControlConfigClient

    
    result: bool = client.can_paginate()
    

    

    
    waiter_name: WaiterName = "cluster_created"
    waiter: ClusterCreatedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
