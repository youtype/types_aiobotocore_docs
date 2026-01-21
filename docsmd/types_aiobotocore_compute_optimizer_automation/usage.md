# Examples

> [Index](../README.md) > [ComputeOptimizerAutomation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ComputeOptimizerAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation.html#computeoptimizerautomation)
    type annotations stubs module [types-aiobotocore-compute-optimizer-automation](https://pypi.org/project/types-aiobotocore-compute-optimizer-automation/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[compute-optimizer-automation]` package installed.

Write your `ComputeOptimizerAutomation` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ComputeOptimizerAutomationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("compute-optimizer-automation") as client:  # (1)
    result = await client.associate_accounts()  # (2)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. result: [:material-code-braces: AssociateAccountsResponseTypeDef](./type_defs.md#associateaccountsresponsetypedef)



#### Paginator usage example

```python
# ListAccountsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[compute-optimizer-automation]`
or a standalone `types_aiobotocore_compute_optimizer_automation` package, you have to explicitly specify
`client: ComputeOptimizerAutomationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ComputeOptimizerAutomationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.client import ComputeOptimizerAutomationClient
from types_aiobotocore_compute_optimizer_automation.type_defs import AssociateAccountsResponseTypeDef
from types_aiobotocore_compute_optimizer_automation.type_defs import AssociateAccountsRequestTypeDef


session = get_session()

async with session.create_client("compute-optimizer-automation") as client:
    client: ComputeOptimizerAutomationClient
    kwargs: AssociateAccountsRequestTypeDef = {...}
    result: AssociateAccountsResponseTypeDef = await client.associate_accounts(**kwargs)
```



#### Paginator usage example

```python
# ListAccountsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.client import ComputeOptimizerAutomationClient
from types_aiobotocore_compute_optimizer_automation.paginator import ListAccountsPaginator
from types_aiobotocore_compute_optimizer_automation.type_defs import ListAccountsResponseTypeDef


session = get_session()

async with session.create_client("compute-optimizer-automation") as client:
    client: ComputeOptimizerAutomationClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)
```


