# Examples

> [Index](../README.md) > [LocationServiceMapsV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2)
    type annotations stubs module [types-aiobotocore-geo-maps](https://pypi.org/project/types-aiobotocore-geo-maps/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[geo-maps]` package installed.

Write your `LocationServiceMapsV2` code as usual,
type checking and code completion should work out of the box.



```python
# LocationServiceMapsV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("geo-maps") as client:  # (1)
    result = await client.get_glyphs()  # (2)
```

1. client: [LocationServiceMapsV2Client](./client.md)
2. result: [:material-code-braces: GetGlyphsResponseTypeDef](./type_defs.md#getglyphsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[geo-maps]`
or a standalone `types_aiobotocore_geo_maps` package, you have to explicitly specify
`client: LocationServiceMapsV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LocationServiceMapsV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_geo_maps.client import LocationServiceMapsV2Client
from types_aiobotocore_geo_maps.type_defs import GetGlyphsResponseTypeDef
from types_aiobotocore_geo_maps.type_defs import GetGlyphsRequestTypeDef


session = get_session()

async with session.create_client("geo-maps") as client:
    client: LocationServiceMapsV2Client
    kwargs: GetGlyphsRequestTypeDef = {...}
    result: GetGlyphsResponseTypeDef = await client.get_glyphs(**kwargs)
```




