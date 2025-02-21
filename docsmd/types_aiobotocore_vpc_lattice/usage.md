# Examples

> [Index](../README.md) > [VPCLattice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#vpclattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[vpc-lattice]` package installed.

Write your `VPCLattice` code as usual,
type checking and code completion should work out of the box.



```python
# VPCLatticeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("vpc-lattice") as client:  # (1)
    result = await client.batch_update_rule()  # (2)
```

1. client: [VPCLatticeClient](./client.md)
2. result: [:material-code-braces: BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef) 



```python
# ListAccessLogSubscriptionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("vpc-lattice") as client:  # (1)
    paginator = client.get_paginator("list_access_log_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [VPCLatticeClient](./client.md)
2. paginator: [ListAccessLogSubscriptionsPaginator](./paginators.md#listaccesslogsubscriptionspaginator)
3. item: [:material-code-braces: ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[vpc-lattice]`
or a standalone `types_aiobotocore_vpc_lattice` package, you have to explicitly specify
`client: VPCLatticeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# VPCLatticeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_vpc_lattice.client import VPCLatticeClient
from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleResponseTypeDef
from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleRequestTypeDef


session = get_session()

async with session.create_client("vpc-lattice") as client:
    client: VPCLatticeClient
    kwargs: BatchUpdateRuleRequestTypeDef = {...}
    result: BatchUpdateRuleResponseTypeDef = await client.batch_update_rule(**kwargs)
```



```python
# ListAccessLogSubscriptionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_vpc_lattice.client import VPCLatticeClient
from types_aiobotocore_vpc_lattice.paginator import ListAccessLogSubscriptionsPaginator
from types_aiobotocore_vpc_lattice.type_defs import ListAccessLogSubscriptionsResponseTypeDef


session = get_session()

async with session.create_client("vpc-lattice") as client:
    client: VPCLatticeClient
    paginator: ListAccessLogSubscriptionsPaginator = client.get_paginator("list_access_log_subscriptions")
    async for item in paginator.paginate(...):
        item: ListAccessLogSubscriptionsResponseTypeDef
        print(item)
```


