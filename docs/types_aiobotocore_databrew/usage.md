<a id="examples-for-aiobotocore-gluedatabrew-module"></a>

# Examples for aiobotocore GlueDataBrew module

> [Index](../README.md) > [GlueDataBrew](./README.md) > Examples

- [Examples for aiobotocore GlueDataBrew module](#examples-for-aiobotocore-gluedatabrew-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[databrew]` package installed.

Write your `GlueDataBrew` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GlueDataBrewClient
# and provides type checking and code completion
async with session.create_client("databrew") as client:
    
    # result has type BatchDeleteRecipeVersionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_delete_recipe_version()
    

    
    # paginator has type ListDatasetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_datasets")
    async for item in paginator.paginate(...):
        # item has type ListDatasetsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[databrew]` or a standalone
`types_aiobotocore_databrew` package, you have to explicitly specify
`client: GlueDataBrewClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.client import GlueDataBrewClient
from types_aiobotocore_databrew.type_defs import BatchDeleteRecipeVersionResponseTypeDef
from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

from types_aiobotocore_databrew.literals import PaginatorName



session = get_session()

async with session.create_client("databrew") as client:
    client: GlueDataBrewClient

    
    result: BatchDeleteRecipeVersionResponseTypeDef = client.batch_delete_recipe_version()
    

    
    paginator_name: PaginatorName = "list_datasets"
    paginator: ListDatasetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)
    

    
```
