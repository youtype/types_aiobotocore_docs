# Examples

> [Index](../README.md) > [Budgets](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[budgets]` package installed.

Write your `Budgets` code as usual,
type checking and code completion should work out of the box.



```python
# BudgetsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("budgets") as client:  # (1)
    result = await client.create_budget_action()  # (2)
```

1. client: [BudgetsClient](./client.md)
2. result: [:material-code-braces: CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef) 



```python
# DescribeBudgetActionHistoriesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("budgets") as client:  # (1)
    paginator = client.get_paginator("describe_budget_action_histories")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BudgetsClient](./client.md)
2. paginator: [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
3. item: [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[budgets]`
or a standalone `types_aiobotocore_budgets` package, you have to explicitly specify
`client: BudgetsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BudgetsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_budgets.client import BudgetsClient
from types_aiobotocore_budgets.type_defs import CreateBudgetActionResponseTypeDef
from types_aiobotocore_budgets.type_defs import CreateBudgetActionRequestTypeDef


session = get_session()

async with session.create_client("budgets") as client:
    client: BudgetsClient
    kwargs: CreateBudgetActionRequestTypeDef = {...}
    result: CreateBudgetActionResponseTypeDef = await client.create_budget_action(**kwargs)
```



```python
# DescribeBudgetActionHistoriesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_budgets.client import BudgetsClient
from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator
from types_aiobotocore_budgets.type_defs import DescribeBudgetActionHistoriesResponseTypeDef


session = get_session()

async with session.create_client("budgets") as client:
    client: BudgetsClient
    paginator: DescribeBudgetActionHistoriesPaginator = client.get_paginator("describe_budget_action_histories")
    async for item in paginator.paginate(...):
        item: DescribeBudgetActionHistoriesResponseTypeDef
        print(item)
```


