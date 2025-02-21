# Examples

> [Index](../README.md) > [SimSpaceWeaver](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SimSpaceWeaver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#simspaceweaver)
    type annotations stubs module [types-aiobotocore-simspaceweaver](https://pypi.org/project/types-aiobotocore-simspaceweaver/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[simspaceweaver]` package installed.

Write your `SimSpaceWeaver` code as usual,
type checking and code completion should work out of the box.



```python
# SimSpaceWeaverClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("simspaceweaver") as client:  # (1)
    result = await client.describe_app()  # (2)
```

1. client: [SimSpaceWeaverClient](./client.md)
2. result: [:material-code-braces: DescribeAppOutputTypeDef](./type_defs.md#describeappoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[simspaceweaver]`
or a standalone `types_aiobotocore_simspaceweaver` package, you have to explicitly specify
`client: SimSpaceWeaverClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SimSpaceWeaverClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_simspaceweaver.client import SimSpaceWeaverClient
from types_aiobotocore_simspaceweaver.type_defs import DescribeAppOutputTypeDef
from types_aiobotocore_simspaceweaver.type_defs import DescribeAppInputTypeDef


session = get_session()

async with session.create_client("simspaceweaver") as client:
    client: SimSpaceWeaverClient
    kwargs: DescribeAppInputTypeDef = {...}
    result: DescribeAppOutputTypeDef = await client.describe_app(**kwargs)
```




