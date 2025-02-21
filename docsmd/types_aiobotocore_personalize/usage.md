# Examples

> [Index](../README.md) > [Personalize](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#personalize)
    type annotations stubs module [types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[personalize]` package installed.

Write your `Personalize` code as usual,
type checking and code completion should work out of the box.



```python
# PersonalizeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("personalize") as client:  # (1)
    result = await client.create_batch_inference_job()  # (2)
```

1. client: [PersonalizeClient](./client.md)
2. result: [:material-code-braces: CreateBatchInferenceJobResponseTypeDef](./type_defs.md#createbatchinferencejobresponsetypedef) 



```python
# ListBatchInferenceJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("personalize") as client:  # (1)
    paginator = client.get_paginator("list_batch_inference_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListBatchInferenceJobsPaginator](./paginators.md#listbatchinferencejobspaginator)
3. item: [:material-code-braces: ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[personalize]`
or a standalone `types_aiobotocore_personalize` package, you have to explicitly specify
`client: PersonalizeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PersonalizeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_personalize.client import PersonalizeClient
from types_aiobotocore_personalize.type_defs import CreateBatchInferenceJobResponseTypeDef
from types_aiobotocore_personalize.type_defs import CreateBatchInferenceJobRequestTypeDef


session = get_session()

async with session.create_client("personalize") as client:
    client: PersonalizeClient
    kwargs: CreateBatchInferenceJobRequestTypeDef = {...}
    result: CreateBatchInferenceJobResponseTypeDef = await client.create_batch_inference_job(**kwargs)
```



```python
# ListBatchInferenceJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_personalize.client import PersonalizeClient
from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator
from types_aiobotocore_personalize.type_defs import ListBatchInferenceJobsResponseTypeDef


session = get_session()

async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListBatchInferenceJobsPaginator = client.get_paginator("list_batch_inference_jobs")
    async for item in paginator.paginate(...):
        item: ListBatchInferenceJobsResponseTypeDef
        print(item)
```


