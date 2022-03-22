<a id="examples-for-aiobotocore-lakeformation-module"></a>

# Examples for aiobotocore LakeFormation module

> [Index](../README.md) > [LakeFormation](./README.md) > Examples

- [Examples for aiobotocore LakeFormation module](#examples-for-aiobotocore-lakeformation-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lakeformation]` package installed.

Write your `LakeFormation` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LakeFormationClient
# and provides type checking and code completion
async with session.create_client("lakeformation") as client:
    
    # result has type AddLFTagsToResourceResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_lf_tags_to_resource()
    

    
    # paginator has type GetWorkUnitsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_work_units")
    async for item in paginator.paginate(...):
        # item has type GetWorkUnitsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lakeformation]` or a standalone
`types_aiobotocore_lakeformation` package, you have to explicitly specify
`client: LakeFormationClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.client import LakeFormationClient
from types_aiobotocore_lakeformation.type_defs import AddLFTagsToResourceResponseTypeDef
from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

from types_aiobotocore_lakeformation.literals import PaginatorName



session = get_session()

async with session.create_client("lakeformation") as client:
    client: LakeFormationClient

    
    result: AddLFTagsToResourceResponseTypeDef = client.add_lf_tags_to_resource()
    

    
    paginator_name: PaginatorName = "get_work_units"
    paginator: GetWorkUnitsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetWorkUnitsResponseTypeDef
        print(item)
    

    
```
