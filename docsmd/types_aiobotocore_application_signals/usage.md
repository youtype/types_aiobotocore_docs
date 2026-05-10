# Examples

> [Index](../README.md) > [CloudWatchApplicationSignals](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals)
    type annotations stubs module [types-aiobotocore-application-signals](https://pypi.org/project/types-aiobotocore-application-signals/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[application-signals]` package installed.

Write your `CloudWatchApplicationSignals` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchApplicationSignalsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-signals") as client:  # (1)
    result = await client.batch_get_service_level_objective_budget_report()  # (2)
```

1. client: [CloudWatchApplicationSignalsClient](./client.md)
2. result: [:material-code-braces: BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef](./type_defs.md#batchgetservicelevelobjectivebudgetreportoutputtypedef)



#### Paginator usage example

```python
# ListEntityEventsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-signals") as client:  # (1)
    paginator = client.get_paginator("list_entity_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchApplicationSignalsClient](./client.md)
2. paginator: [ListEntityEventsPaginator](./paginators.md#listentityeventspaginator)
3. item: [:material-code-braces: ListEntityEventsOutputTypeDef](./type_defs.md#listentityeventsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[application-signals]`
or a standalone `types_aiobotocore_application_signals` package, you have to explicitly specify
`client: CloudWatchApplicationSignalsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchApplicationSignalsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_signals.client import CloudWatchApplicationSignalsClient
from types_aiobotocore_application_signals.type_defs import BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef
from types_aiobotocore_application_signals.type_defs import BatchGetServiceLevelObjectiveBudgetReportInputTypeDef


session = get_session()

async with session.create_client("application-signals") as client:
    client: CloudWatchApplicationSignalsClient
    kwargs: BatchGetServiceLevelObjectiveBudgetReportInputTypeDef = {...}
    result: BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef = await client.batch_get_service_level_objective_budget_report(**kwargs)
```



#### Paginator usage example

```python
# ListEntityEventsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_signals.client import CloudWatchApplicationSignalsClient
from types_aiobotocore_application_signals.paginator import ListEntityEventsPaginator
from types_aiobotocore_application_signals.type_defs import ListEntityEventsOutputTypeDef


session = get_session()

async with session.create_client("application-signals") as client:
    client: CloudWatchApplicationSignalsClient
    paginator: ListEntityEventsPaginator = client.get_paginator("list_entity_events")
    async for item in paginator.paginate(...):
        item: ListEntityEventsOutputTypeDef
        print(item)
```


