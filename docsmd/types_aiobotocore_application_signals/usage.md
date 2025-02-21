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



```python
# CloudWatchApplicationSignalsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-signals") as client:  # (1)
    result = await client.batch_get_service_level_objective_budget_report()  # (2)
```

1. client: [CloudWatchApplicationSignalsClient](./client.md)
2. result: [:material-code-braces: BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef](./type_defs.md#batchgetservicelevelobjectivebudgetreportoutputtypedef) 



```python
# ListServiceDependenciesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-signals") as client:  # (1)
    paginator = client.get_paginator("list_service_dependencies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchApplicationSignalsClient](./client.md)
2. paginator: [ListServiceDependenciesPaginator](./paginators.md#listservicedependenciespaginator)
3. item: [:material-code-braces: ListServiceDependenciesOutputTypeDef](./type_defs.md#listservicedependenciesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[application-signals]`
or a standalone `types_aiobotocore_application_signals` package, you have to explicitly specify
`client: CloudWatchApplicationSignalsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


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



```python
# ListServiceDependenciesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_signals.client import CloudWatchApplicationSignalsClient
from types_aiobotocore_application_signals.paginator import ListServiceDependenciesPaginator
from types_aiobotocore_application_signals.type_defs import ListServiceDependenciesOutputTypeDef


session = get_session()

async with session.create_client("application-signals") as client:
    client: CloudWatchApplicationSignalsClient
    paginator: ListServiceDependenciesPaginator = client.get_paginator("list_service_dependencies")
    async for item in paginator.paginate(...):
        item: ListServiceDependenciesOutputTypeDef
        print(item)
```


