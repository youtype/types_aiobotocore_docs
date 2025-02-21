# Examples

> [Index](../README.md) > [GlueDataBrew](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#gluedatabrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[databrew]` package installed.

Write your `GlueDataBrew` code as usual,
type checking and code completion should work out of the box.



```python
# GlueDataBrewClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("databrew") as client:  # (1)
    result = await client.batch_delete_recipe_version()  # (2)
```

1. client: [GlueDataBrewClient](./client.md)
2. result: [:material-code-braces: BatchDeleteRecipeVersionResponseTypeDef](./type_defs.md#batchdeleterecipeversionresponsetypedef) 



```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("databrew") as client:  # (1)
    paginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[databrew]`
or a standalone `types_aiobotocore_databrew` package, you have to explicitly specify
`client: GlueDataBrewClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GlueDataBrewClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_databrew.client import GlueDataBrewClient
from types_aiobotocore_databrew.type_defs import BatchDeleteRecipeVersionResponseTypeDef
from types_aiobotocore_databrew.type_defs import BatchDeleteRecipeVersionRequestTypeDef


session = get_session()

async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    kwargs: BatchDeleteRecipeVersionRequestTypeDef = {...}
    result: BatchDeleteRecipeVersionResponseTypeDef = await client.batch_delete_recipe_version(**kwargs)
```



```python
# ListDatasetsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_databrew.client import GlueDataBrewClient
from types_aiobotocore_databrew.paginator import ListDatasetsPaginator
from types_aiobotocore_databrew.type_defs import ListDatasetsResponseTypeDef


session = get_session()

async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)
```


