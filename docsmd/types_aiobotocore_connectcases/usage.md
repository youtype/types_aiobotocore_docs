# Examples

> [Index](../README.md) > [ConnectCases](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[connectcases]` package installed.

Write your `ConnectCases` code as usual,
type checking and code completion should work out of the box.



```python
# ConnectCasesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("connectcases") as client:  # (1)
    result = await client.batch_get_case_rule()  # (2)
```

1. client: [ConnectCasesClient](./client.md)
2. result: [:material-code-braces: BatchGetCaseRuleResponseTypeDef](./type_defs.md#batchgetcaseruleresponsetypedef) 



```python
# ListCaseRulesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("connectcases") as client:  # (1)
    paginator = client.get_paginator("list_case_rules")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [ListCaseRulesPaginator](./paginators.md#listcaserulespaginator)
3. item: [:material-code-braces: ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[connectcases]`
or a standalone `types_aiobotocore_connectcases` package, you have to explicitly specify
`client: ConnectCasesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ConnectCasesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleResponseTypeDef
from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleRequestTypeDef


session = get_session()

async with session.create_client("connectcases") as client:
    client: ConnectCasesClient
    kwargs: BatchGetCaseRuleRequestTypeDef = {...}
    result: BatchGetCaseRuleResponseTypeDef = await client.batch_get_case_rule(**kwargs)
```



```python
# ListCaseRulesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.paginator import ListCaseRulesPaginator
from types_aiobotocore_connectcases.type_defs import ListCaseRulesResponseTypeDef


session = get_session()

async with session.create_client("connectcases") as client:
    client: ConnectCasesClient
    paginator: ListCaseRulesPaginator = client.get_paginator("list_case_rules")
    async for item in paginator.paginate(...):
        item: ListCaseRulesResponseTypeDef
        print(item)
```


