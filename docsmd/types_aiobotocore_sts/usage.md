# Examples

> [Index](../README.md) > [STS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#sts)
    type annotations stubs module [types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sts]` package installed.

Write your `STS` code as usual,
type checking and code completion should work out of the box.



```python
# STSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sts") as client:  # (1)
    result = await client.assume_role()  # (2)
```

1. client: [STSClient](./client.md)
2. result: [:material-code-braces: AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sts]`
or a standalone `types_aiobotocore_sts` package, you have to explicitly specify
`client: STSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# STSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sts.client import STSClient
from types_aiobotocore_sts.type_defs import AssumeRoleResponseTypeDef
from types_aiobotocore_sts.type_defs import AssumeRoleRequestTypeDef


session = get_session()

async with session.create_client("sts") as client:
    client: STSClient
    kwargs: AssumeRoleRequestTypeDef = {...}
    result: AssumeRoleResponseTypeDef = await client.assume_role(**kwargs)
```




