# Examples

> [Index](../README.md) > [LocationServiceRoutesV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationServiceRoutesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#locationserviceroutesv2)
    type annotations stubs module [types-aiobotocore-geo-routes](https://pypi.org/project/types-aiobotocore-geo-routes/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[geo-routes]` package installed.

Write your `LocationServiceRoutesV2` code as usual,
type checking and code completion should work out of the box.



```python
# LocationServiceRoutesV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("geo-routes") as client:  # (1)
    result = await client.calculate_isolines()  # (2)
```

1. client: [LocationServiceRoutesV2Client](./client.md)
2. result: [:material-code-braces: CalculateIsolinesResponseTypeDef](./type_defs.md#calculateisolinesresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[geo-routes]`
or a standalone `types_aiobotocore_geo_routes` package, you have to explicitly specify
`client: LocationServiceRoutesV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LocationServiceRoutesV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_geo_routes.client import LocationServiceRoutesV2Client
from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesResponseTypeDef
from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesRequestTypeDef


session = get_session()

async with session.create_client("geo-routes") as client:
    client: LocationServiceRoutesV2Client
    kwargs: CalculateIsolinesRequestTypeDef = {...}
    result: CalculateIsolinesResponseTypeDef = await client.calculate_isolines(**kwargs)
```




