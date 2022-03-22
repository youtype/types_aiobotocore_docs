<a id="examples-for-aiobotocore-alexaforbusiness-module"></a>

# Examples for aiobotocore AlexaForBusiness module

> [Index](../README.md) > [AlexaForBusiness](./README.md) > Examples

- [Examples for aiobotocore AlexaForBusiness module](#examples-for-aiobotocore-alexaforbusiness-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[alexaforbusiness]` package installed.

Write your `AlexaForBusiness` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AlexaForBusinessClient
# and provides type checking and code completion
async with session.create_client("alexaforbusiness") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.approve_skill()
    

    
    # paginator has type ListBusinessReportSchedulesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_business_report_schedules")
    async for item in paginator.paginate(...):
        # item has type ListBusinessReportSchedulesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[alexaforbusiness]` or a standalone
`types_aiobotocore_alexaforbusiness` package, you have to explicitly specify
`client: AlexaForBusinessClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.client import AlexaForBusinessClient
from types_aiobotocore_alexaforbusiness.type_defs import Dict[str, Any]
from types_aiobotocore_alexaforbusiness.paginator import ListBusinessReportSchedulesPaginator

from types_aiobotocore_alexaforbusiness.literals import PaginatorName



session = get_session()

async with session.create_client("alexaforbusiness") as client:
    client: AlexaForBusinessClient

    
    result: Dict[str, Any] = client.approve_skill()
    

    
    paginator_name: PaginatorName = "list_business_report_schedules"
    paginator: ListBusinessReportSchedulesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBusinessReportSchedulesResponseTypeDef
        print(item)
    

    
```
