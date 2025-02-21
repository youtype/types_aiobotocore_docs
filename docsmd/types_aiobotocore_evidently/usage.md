# Examples

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[evidently]` package installed.

Write your `CloudWatchEvidently` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchEvidentlyClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("evidently") as client:  # (1)
    result = await client.batch_evaluate_feature()  # (2)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. result: [:material-code-braces: BatchEvaluateFeatureResponseTypeDef](./type_defs.md#batchevaluatefeatureresponsetypedef) 



```python
# ListExperimentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("evidently") as client:  # (1)
    paginator = client.get_paginator("list_experiments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
3. item: [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[evidently]`
or a standalone `types_aiobotocore_evidently` package, you have to explicitly specify
`client: CloudWatchEvidentlyClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchEvidentlyClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient
from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureResponseTypeDef
from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureRequestTypeDef


session = get_session()

async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    kwargs: BatchEvaluateFeatureRequestTypeDef = {...}
    result: BatchEvaluateFeatureResponseTypeDef = await client.batch_evaluate_feature(**kwargs)
```



```python
# ListExperimentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient
from types_aiobotocore_evidently.paginator import ListExperimentsPaginator
from types_aiobotocore_evidently.type_defs import ListExperimentsResponseTypeDef


session = get_session()

async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    paginator: ListExperimentsPaginator = client.get_paginator("list_experiments")
    async for item in paginator.paginate(...):
        item: ListExperimentsResponseTypeDef
        print(item)
```


