# Examples

> [Index](../README.md) > [Imagebuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[imagebuilder]` package installed.

Write your `Imagebuilder` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ImagebuilderClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("imagebuilder") as client:  # (1)
    result = await client.cancel_image_creation()  # (2)
```

1. client: [ImagebuilderClient](./client.md)
2. result: [:material-code-braces: CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef)



#### Paginator usage example

```python
# ListComponentBuildVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("imagebuilder") as client:  # (1)
    paginator = client.get_paginator("list_component_build_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListComponentBuildVersionsPaginator](./paginators.md#listcomponentbuildversionspaginator)
3. item: [:material-code-braces: ListComponentBuildVersionsResponseTypeDef](./type_defs.md#listcomponentbuildversionsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[imagebuilder]`
or a standalone `types_aiobotocore_imagebuilder` package, you have to explicitly specify
`client: ImagebuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ImagebuilderClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.client import ImagebuilderClient
from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationResponseTypeDef
from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationRequestTypeDef


session = get_session()

async with session.create_client("imagebuilder") as client:
    client: ImagebuilderClient
    kwargs: CancelImageCreationRequestTypeDef = {...}
    result: CancelImageCreationResponseTypeDef = await client.cancel_image_creation(**kwargs)
```



#### Paginator usage example

```python
# ListComponentBuildVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.client import ImagebuilderClient
from types_aiobotocore_imagebuilder.paginator import ListComponentBuildVersionsPaginator
from types_aiobotocore_imagebuilder.type_defs import ListComponentBuildVersionsResponseTypeDef


session = get_session()

async with session.create_client("imagebuilder") as client:
    client: ImagebuilderClient
    paginator: ListComponentBuildVersionsPaginator = client.get_paginator("list_component_build_versions")
    async for item in paginator.paginate(...):
        item: ListComponentBuildVersionsResponseTypeDef
        print(item)
```


