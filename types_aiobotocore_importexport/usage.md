<a id="examples-for-aiobotocore-importexport-module"></a>

# Examples for aiobotocore ImportExport module

> [Index](../README.md) > [ImportExport](./README.md) > Examples

- [Examples for aiobotocore ImportExport module](#examples-for-aiobotocore-importexport-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[importexport]` package installed.

Write your `ImportExport` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ImportExportClient
# and provides type checking and code completion
async with session.create_client("importexport") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_jobs")
    async for item in paginator.paginate(...):
        # item has type ListJobsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[importexport]` or a standalone
`types_aiobotocore_importexport` package, you have to explicitly specify
`client: ImportExportClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_importexport.client import ImportExportClient
from types_aiobotocore_importexport.type_defs import bool
from types_aiobotocore_importexport.paginator import ListJobsPaginator

from types_aiobotocore_importexport.literals import PaginatorName



session = get_session()

async with session.create_client("importexport") as client:
    client: ImportExportClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_jobs"
    paginator: ListJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)
    

    
```
