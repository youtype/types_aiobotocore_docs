# Examples

> [Index](../README.md) > [IoTSecureTunneling](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#iotsecuretunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotsecuretunneling]` package installed.

Write your `IoTSecureTunneling` code as usual,
type checking and code completion should work out of the box.



```python
# IoTSecureTunnelingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotsecuretunneling") as client:  # (1)
    result = await client.describe_tunnel()  # (2)
```

1. client: [IoTSecureTunnelingClient](./client.md)
2. result: [:material-code-braces: DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[iotsecuretunneling]`
or a standalone `types_aiobotocore_iotsecuretunneling` package, you have to explicitly specify
`client: IoTSecureTunnelingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTSecureTunnelingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient
from types_aiobotocore_iotsecuretunneling.type_defs import DescribeTunnelResponseTypeDef
from types_aiobotocore_iotsecuretunneling.type_defs import DescribeTunnelRequestTypeDef


session = get_session()

async with session.create_client("iotsecuretunneling") as client:
    client: IoTSecureTunnelingClient
    kwargs: DescribeTunnelRequestTypeDef = {...}
    result: DescribeTunnelResponseTypeDef = await client.describe_tunnel(**kwargs)
```




