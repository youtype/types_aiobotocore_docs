# Examples

> [Index](../README.md) > [SavingsPlans](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#savingsplans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[savingsplans]` package installed.

Write your `SavingsPlans` code as usual,
type checking and code completion should work out of the box.



```python
# SavingsPlansClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("savingsplans") as client:  # (1)
    result = await client.create_savings_plan()  # (2)
```

1. client: [SavingsPlansClient](./client.md)
2. result: [:material-code-braces: CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[savingsplans]`
or a standalone `types_aiobotocore_savingsplans` package, you have to explicitly specify
`client: SavingsPlansClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SavingsPlansClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_savingsplans.client import SavingsPlansClient
from types_aiobotocore_savingsplans.type_defs import CreateSavingsPlanResponseTypeDef
from types_aiobotocore_savingsplans.type_defs import CreateSavingsPlanRequestTypeDef


session = get_session()

async with session.create_client("savingsplans") as client:
    client: SavingsPlansClient
    kwargs: CreateSavingsPlanRequestTypeDef = {...}
    result: CreateSavingsPlanResponseTypeDef = await client.create_savings_plan(**kwargs)
```




