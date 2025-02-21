# Examples

> [Index](../README.md) > [ApplicationInsights](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#applicationinsights)
    type annotations stubs module [types-aiobotocore-application-insights](https://pypi.org/project/types-aiobotocore-application-insights/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[application-insights]` package installed.

Write your `ApplicationInsights` code as usual,
type checking and code completion should work out of the box.



```python
# ApplicationInsightsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-insights") as client:  # (1)
    result = await client.add_workload()  # (2)
```

1. client: [ApplicationInsightsClient](./client.md)
2. result: [:material-code-braces: AddWorkloadResponseTypeDef](./type_defs.md#addworkloadresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[application-insights]`
or a standalone `types_aiobotocore_application_insights` package, you have to explicitly specify
`client: ApplicationInsightsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ApplicationInsightsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_insights.client import ApplicationInsightsClient
from types_aiobotocore_application_insights.type_defs import AddWorkloadResponseTypeDef
from types_aiobotocore_application_insights.type_defs import AddWorkloadRequestTypeDef


session = get_session()

async with session.create_client("application-insights") as client:
    client: ApplicationInsightsClient
    kwargs: AddWorkloadRequestTypeDef = {...}
    result: AddWorkloadResponseTypeDef = await client.add_workload(**kwargs)
```




