# Examples

> [Index](../README.md) > [Inspectorscan](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[inspector-scan]` package installed.

Write your `Inspectorscan` code as usual,
type checking and code completion should work out of the box.



```python
# InspectorscanClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("inspector-scan") as client:  # (1)
    result = await client.scan_sbom()  # (2)
```

1. client: [InspectorscanClient](./client.md)
2. result: [:material-code-braces: ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[inspector-scan]`
or a standalone `types_aiobotocore_inspector_scan` package, you have to explicitly specify
`client: InspectorscanClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# InspectorscanClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_inspector_scan.client import InspectorscanClient
from types_aiobotocore_inspector_scan.type_defs import ScanSbomResponseTypeDef
from types_aiobotocore_inspector_scan.type_defs import ScanSbomRequestTypeDef


session = get_session()

async with session.create_client("inspector-scan") as client:
    client: InspectorscanClient
    kwargs: ScanSbomRequestTypeDef = {...}
    result: ScanSbomResponseTypeDef = await client.scan_sbom(**kwargs)
```




