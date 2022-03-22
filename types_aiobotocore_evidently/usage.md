<a id="examples-for-aiobotocore-cloudwatchevidently-module"></a>

# Examples for aiobotocore CloudWatchEvidently module

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Examples

- [Examples for aiobotocore CloudWatchEvidently module](#examples-for-aiobotocore-cloudwatchevidently-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[evidently]` package installed.

Write your `CloudWatchEvidently` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudWatchEvidentlyClient
# and provides type checking and code completion
async with session.create_client("evidently") as client:
    
    # result has type BatchEvaluateFeatureResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_evaluate_feature()
    

    
    # paginator has type ListExperimentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_experiments")
    async for item in paginator.paginate(...):
        # item has type ListExperimentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[evidently]` or a standalone
`types_aiobotocore_evidently` package, you have to explicitly specify
`client: CloudWatchEvidentlyClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient
from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureResponseTypeDef
from types_aiobotocore_evidently.paginator import ListExperimentsPaginator

from types_aiobotocore_evidently.literals import PaginatorName



session = get_session()

async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient

    
    result: BatchEvaluateFeatureResponseTypeDef = client.batch_evaluate_feature()
    

    
    paginator_name: PaginatorName = "list_experiments"
    paginator: ListExperimentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListExperimentsResponseTypeDef
        print(item)
    

    
```
