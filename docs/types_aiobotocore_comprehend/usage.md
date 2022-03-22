<a id="examples-for-aiobotocore-comprehend-module"></a>

# Examples for aiobotocore Comprehend module

> [Index](../README.md) > [Comprehend](./README.md) > Examples

- [Examples for aiobotocore Comprehend module](#examples-for-aiobotocore-comprehend-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[comprehend]` package installed.

Write your `Comprehend` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ComprehendClient
# and provides type checking and code completion
async with session.create_client("comprehend") as client:
    
    # result has type BatchDetectDominantLanguageResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_detect_dominant_language()
    

    
    # paginator has type ListDocumentClassificationJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_document_classification_jobs")
    async for item in paginator.paginate(...):
        # item has type ListDocumentClassificationJobsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[comprehend]` or a standalone
`types_aiobotocore_comprehend` package, you have to explicitly specify
`client: ComprehendClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.client import ComprehendClient
from types_aiobotocore_comprehend.type_defs import BatchDetectDominantLanguageResponseTypeDef
from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator

from types_aiobotocore_comprehend.literals import PaginatorName



session = get_session()

async with session.create_client("comprehend") as client:
    client: ComprehendClient

    
    result: BatchDetectDominantLanguageResponseTypeDef = client.batch_detect_dominant_language()
    

    
    paginator_name: PaginatorName = "list_document_classification_jobs"
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDocumentClassificationJobsResponseTypeDef
        print(item)
    

    
```
