# Examples

> [Index](../README.md) > [CleanRoomsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cleanrooms]` package installed.

Write your `CleanRoomsService` code as usual,
type checking and code completion should work out of the box.



```python
# CleanRoomsServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cleanrooms") as client:  # (1)
    result = await client.batch_get_collaboration_analysis_template()  # (2)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. result: [:material-code-braces: BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef) 



```python
# ListAnalysisTemplatesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cleanrooms") as client:  # (1)
    paginator = client.get_paginator("list_analysis_templates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
3. item: [:material-code-braces: ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cleanrooms]`
or a standalone `types_aiobotocore_cleanrooms` package, you have to explicitly specify
`client: CleanRoomsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CleanRoomsServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateOutputTypeDef
from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateInputTypeDef


session = get_session()

async with session.create_client("cleanrooms") as client:
    client: CleanRoomsServiceClient
    kwargs: BatchGetCollaborationAnalysisTemplateInputTypeDef = {...}
    result: BatchGetCollaborationAnalysisTemplateOutputTypeDef = await client.batch_get_collaboration_analysis_template(**kwargs)
```



```python
# ListAnalysisTemplatesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
from types_aiobotocore_cleanrooms.paginator import ListAnalysisTemplatesPaginator
from types_aiobotocore_cleanrooms.type_defs import ListAnalysisTemplatesOutputTypeDef


session = get_session()

async with session.create_client("cleanrooms") as client:
    client: CleanRoomsServiceClient
    paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")
    async for item in paginator.paginate(...):
        item: ListAnalysisTemplatesOutputTypeDef
        print(item)
```


