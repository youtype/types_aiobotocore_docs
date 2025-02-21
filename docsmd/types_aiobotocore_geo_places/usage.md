# Examples

> [Index](../README.md) > [LocationServicePlacesV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2)
    type annotations stubs module [types-aiobotocore-geo-places](https://pypi.org/project/types-aiobotocore-geo-places/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[geo-places]` package installed.

Write your `LocationServicePlacesV2` code as usual,
type checking and code completion should work out of the box.



```python
# LocationServicePlacesV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("geo-places") as client:  # (1)
    result = await client.autocomplete()  # (2)
```

1. client: [LocationServicePlacesV2Client](./client.md)
2. result: [:material-code-braces: AutocompleteResponseTypeDef](./type_defs.md#autocompleteresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[geo-places]`
or a standalone `types_aiobotocore_geo_places` package, you have to explicitly specify
`client: LocationServicePlacesV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LocationServicePlacesV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_geo_places.client import LocationServicePlacesV2Client
from types_aiobotocore_geo_places.type_defs import AutocompleteResponseTypeDef
from types_aiobotocore_geo_places.type_defs import AutocompleteRequestTypeDef


session = get_session()

async with session.create_client("geo-places") as client:
    client: LocationServicePlacesV2Client
    kwargs: AutocompleteRequestTypeDef = {...}
    result: AutocompleteResponseTypeDef = await client.autocomplete(**kwargs)
```




