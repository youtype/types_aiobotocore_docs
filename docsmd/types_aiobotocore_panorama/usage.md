# Examples

> [Index](../README.md) > [Panorama](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[panorama]` package installed.

Write your `Panorama` code as usual,
type checking and code completion should work out of the box.



```python
# PanoramaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("panorama") as client:  # (1)
    result = await client.create_application_instance()  # (2)
```

1. client: [PanoramaClient](./client.md)
2. result: [:material-code-braces: CreateApplicationInstanceResponseTypeDef](./type_defs.md#createapplicationinstanceresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[panorama]`
or a standalone `types_aiobotocore_panorama` package, you have to explicitly specify
`client: PanoramaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PanoramaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_panorama.client import PanoramaClient
from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceResponseTypeDef
from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceRequestTypeDef


session = get_session()

async with session.create_client("panorama") as client:
    client: PanoramaClient
    kwargs: CreateApplicationInstanceRequestTypeDef = {...}
    result: CreateApplicationInstanceResponseTypeDef = await client.create_application_instance(**kwargs)
```




