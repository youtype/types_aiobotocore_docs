# Examples

> [Index](../README.md) > [EntityResolution](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[entityresolution]` package installed.

Write your `EntityResolution` code as usual,
type checking and code completion should work out of the box.



```python
# EntityResolutionClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("entityresolution") as client:  # (1)
    result = await client.create_matching_workflow()  # (2)
```

1. client: [EntityResolutionClient](./client.md)
2. result: [:material-code-braces: CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef) 



```python
# ListMatchingJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("entityresolution") as client:  # (1)
    paginator = client.get_paginator("list_matching_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
3. item: [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[entityresolution]`
or a standalone `types_aiobotocore_entityresolution` package, you have to explicitly specify
`client: EntityResolutionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EntityResolutionClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.type_defs import CreateMatchingWorkflowOutputTypeDef
from types_aiobotocore_entityresolution.type_defs import CreateMatchingWorkflowInputRequestTypeDef


session = get_session()

async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
    kwargs: CreateMatchingWorkflowInputRequestTypeDef = {...}
    result: CreateMatchingWorkflowOutputTypeDef = await client.create_matching_workflow(**kwargs)
```



```python
# ListMatchingJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.paginator import ListMatchingJobsPaginator
from types_aiobotocore_entityresolution.type_defs import ListMatchingJobsOutputTypeDef


session = get_session()

async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
    paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")
    async for item in paginator.paginate(...):
        item: ListMatchingJobsOutputTypeDef
        print(item)
```


