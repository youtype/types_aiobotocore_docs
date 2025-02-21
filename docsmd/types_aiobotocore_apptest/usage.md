# Examples

> [Index](../README.md) > [MainframeModernizationApplicationTesting](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[apptest]` package installed.

Write your `MainframeModernizationApplicationTesting` code as usual,
type checking and code completion should work out of the box.



```python
# MainframeModernizationApplicationTestingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apptest") as client:  # (1)
    result = await client.create_test_case()  # (2)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. result: [:material-code-braces: CreateTestCaseResponseTypeDef](./type_defs.md#createtestcaseresponsetypedef) 



```python
# ListTestCasesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apptest") as client:  # (1)
    paginator = client.get_paginator("list_test_cases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MainframeModernizationApplicationTestingClient](./client.md)
2. paginator: [ListTestCasesPaginator](./paginators.md#listtestcasespaginator)
3. item: [:material-code-braces: ListTestCasesResponseTypeDef](./type_defs.md#listtestcasesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[apptest]`
or a standalone `types_aiobotocore_apptest` package, you have to explicitly specify
`client: MainframeModernizationApplicationTestingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MainframeModernizationApplicationTestingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apptest.client import MainframeModernizationApplicationTestingClient
from types_aiobotocore_apptest.type_defs import CreateTestCaseResponseTypeDef
from types_aiobotocore_apptest.type_defs import CreateTestCaseRequestTypeDef


session = get_session()

async with session.create_client("apptest") as client:
    client: MainframeModernizationApplicationTestingClient
    kwargs: CreateTestCaseRequestTypeDef = {...}
    result: CreateTestCaseResponseTypeDef = await client.create_test_case(**kwargs)
```



```python
# ListTestCasesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apptest.client import MainframeModernizationApplicationTestingClient
from types_aiobotocore_apptest.paginator import ListTestCasesPaginator
from types_aiobotocore_apptest.type_defs import ListTestCasesResponseTypeDef


session = get_session()

async with session.create_client("apptest") as client:
    client: MainframeModernizationApplicationTestingClient
    paginator: ListTestCasesPaginator = client.get_paginator("list_test_cases")
    async for item in paginator.paginate(...):
        item: ListTestCasesResponseTypeDef
        print(item)
```


