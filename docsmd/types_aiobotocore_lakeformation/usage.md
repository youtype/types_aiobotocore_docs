# Examples

> [Index](../README.md) > [LakeFormation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lakeformation]` package installed.

Write your `LakeFormation` code as usual,
type checking and code completion should work out of the box.



```python
# LakeFormationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lakeformation") as client:  # (1)
    result = await client.add_lf_tags_to_resource()  # (2)
```

1. client: [LakeFormationClient](./client.md)
2. result: [:material-code-braces: AddLFTagsToResourceResponseTypeDef](./type_defs.md#addlftagstoresourceresponsetypedef) 



```python
# GetWorkUnitsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lakeformation") as client:  # (1)
    paginator = client.get_paginator("get_work_units")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [GetWorkUnitsPaginator](./paginators.md#getworkunitspaginator)
3. item: [:material-code-braces: GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[lakeformation]`
or a standalone `types_aiobotocore_lakeformation` package, you have to explicitly specify
`client: LakeFormationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LakeFormationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.client import LakeFormationClient
from types_aiobotocore_lakeformation.type_defs import AddLFTagsToResourceResponseTypeDef
from types_aiobotocore_lakeformation.type_defs import AddLFTagsToResourceRequestTypeDef


session = get_session()

async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    kwargs: AddLFTagsToResourceRequestTypeDef = {...}
    result: AddLFTagsToResourceResponseTypeDef = await client.add_lf_tags_to_resource(**kwargs)
```



```python
# GetWorkUnitsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.client import LakeFormationClient
from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator
from types_aiobotocore_lakeformation.type_defs import GetWorkUnitsResponseTypeDef


session = get_session()

async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: GetWorkUnitsPaginator = client.get_paginator("get_work_units")
    async for item in paginator.paginate(...):
        item: GetWorkUnitsResponseTypeDef
        print(item)
```


