# Examples

> [Index](../README.md) > [SignerDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SignerDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data.html#signerdataplane)
    type annotations stubs module [types-aiobotocore-signer-data](https://pypi.org/project/types-aiobotocore-signer-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[signer-data]` package installed.

Write your `SignerDataPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SignerDataPlaneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("signer-data") as client:  # (1)
    result = await client.get_revocation_status()  # (2)
```

1. client: [SignerDataPlaneClient](./client.md)
2. result: [:material-code-braces: GetRevocationStatusResponseTypeDef](./type_defs.md#getrevocationstatusresponsetypedef)






### Explicit type annotations

With `types-aiobotocore-lite[signer-data]`
or a standalone `types_aiobotocore_signer_data` package, you have to explicitly specify
`client: SignerDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SignerDataPlaneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_signer_data.client import SignerDataPlaneClient
from types_aiobotocore_signer_data.type_defs import GetRevocationStatusResponseTypeDef
from types_aiobotocore_signer_data.type_defs import GetRevocationStatusRequestTypeDef


session = get_session()

async with session.create_client("signer-data") as client:
    client: SignerDataPlaneClient
    kwargs: GetRevocationStatusRequestTypeDef = {...}
    result: GetRevocationStatusResponseTypeDef = await client.get_revocation_status(**kwargs)
```




