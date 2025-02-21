# Examples

> [Index](../README.md) > [WellArchitected](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[wellarchitected]` package installed.

Write your `WellArchitected` code as usual,
type checking and code completion should work out of the box.



```python
# WellArchitectedClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("wellarchitected") as client:  # (1)
    result = await client.associate_lenses()  # (2)
```

1. client: [WellArchitectedClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[wellarchitected]`
or a standalone `types_aiobotocore_wellarchitected` package, you have to explicitly specify
`client: WellArchitectedClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WellArchitectedClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_wellarchitected.client import WellArchitectedClient
from types_aiobotocore_wellarchitected.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_wellarchitected.type_defs import AssociateLensesInputTypeDef


session = get_session()

async with session.create_client("wellarchitected") as client:
    client: WellArchitectedClient
    kwargs: AssociateLensesInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_lenses(**kwargs)
```




