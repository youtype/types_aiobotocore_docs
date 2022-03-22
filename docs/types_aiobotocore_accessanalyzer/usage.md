<a id="examples-for-aiobotocore-accessanalyzer-module"></a>

# Examples for aiobotocore AccessAnalyzer module

> [Index](../README.md) > [AccessAnalyzer](./README.md) > Examples

- [Examples for aiobotocore AccessAnalyzer module](#examples-for-aiobotocore-accessanalyzer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[accessanalyzer]` package installed.

Write your `AccessAnalyzer` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AccessAnalyzerClient
# and provides type checking and code completion
async with session.create_client("accessanalyzer") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.apply_archive_rule()
    

    
    # paginator has type ListAccessPreviewFindingsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_access_preview_findings")
    async for item in paginator.paginate(...):
        # item has type ListAccessPreviewFindingsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[accessanalyzer]` or a standalone
`types_aiobotocore_accessanalyzer` package, you have to explicitly specify
`client: AccessAnalyzerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient
from types_aiobotocore_accessanalyzer.type_defs import None
from types_aiobotocore_accessanalyzer.paginator import ListAccessPreviewFindingsPaginator

from types_aiobotocore_accessanalyzer.literals import PaginatorName



session = get_session()

async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient

    
    result: None = client.apply_archive_rule()
    

    
    paginator_name: PaginatorName = "list_access_preview_findings"
    paginator: ListAccessPreviewFindingsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccessPreviewFindingsResponseTypeDef
        print(item)
    

    
```
