# Examples

> [Index](../README.md) > [Comprehend](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[comprehend]` package installed.

Write your `Comprehend` code as usual,
type checking and code completion should work out of the box.



```python
# ComprehendClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("comprehend") as client:  # (1)
    result = await client.batch_detect_dominant_language()  # (2)
```

1. client: [ComprehendClient](./client.md)
2. result: [:material-code-braces: BatchDetectDominantLanguageResponseTypeDef](./type_defs.md#batchdetectdominantlanguageresponsetypedef) 



```python
# ListDocumentClassificationJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("comprehend") as client:  # (1)
    paginator = client.get_paginator("list_document_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
3. item: [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[comprehend]`
or a standalone `types_aiobotocore_comprehend` package, you have to explicitly specify
`client: ComprehendClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ComprehendClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_comprehend.client import ComprehendClient
from types_aiobotocore_comprehend.type_defs import BatchDetectDominantLanguageResponseTypeDef
from types_aiobotocore_comprehend.type_defs import BatchDetectDominantLanguageRequestTypeDef


session = get_session()

async with session.create_client("comprehend") as client:
    client: ComprehendClient
    kwargs: BatchDetectDominantLanguageRequestTypeDef = {...}
    result: BatchDetectDominantLanguageResponseTypeDef = await client.batch_detect_dominant_language(**kwargs)
```



```python
# ListDocumentClassificationJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_comprehend.client import ComprehendClient
from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator
from types_aiobotocore_comprehend.type_defs import ListDocumentClassificationJobsResponseTypeDef


session = get_session()

async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator("list_document_classification_jobs")
    async for item in paginator.paginate(...):
        item: ListDocumentClassificationJobsResponseTypeDef
        print(item)
```


