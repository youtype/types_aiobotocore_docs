<a id="examples-for-aiobotocore-route53recoverycluster-module"></a>

# Examples for aiobotocore Route53RecoveryCluster module

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Examples

- [Examples for aiobotocore Route53RecoveryCluster module](#examples-for-aiobotocore-route53recoverycluster-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53-recovery-cluster]` package
installed.

Write your `Route53RecoveryCluster` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53RecoveryClusterClient
# and provides type checking and code completion
async with session.create_client("route53-recovery-cluster") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53-recovery-cluster]` or a standalone
`types_aiobotocore_route53_recovery_cluster` package, you have to explicitly
specify `client: Route53RecoveryClusterClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient
from types_aiobotocore_route53_recovery_cluster.type_defs import bool






session = get_session()

async with session.create_client("route53-recovery-cluster") as client:
    client: Route53RecoveryClusterClient

    
    result: bool = client.can_paginate()
    

    

    
```
