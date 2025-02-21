# Examples

> [Index](../README.md) > [EBS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#ebs)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ebs]` package installed.

Write your `EBS` code as usual,
type checking and code completion should work out of the box.



```python
# EBSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ebs") as client:  # (1)
    result = await client.complete_snapshot()  # (2)
```

1. client: [EBSClient](./client.md)
2. result: [:material-code-braces: CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[ebs]`
or a standalone `types_aiobotocore_ebs` package, you have to explicitly specify
`client: EBSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EBSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ebs.client import EBSClient
from types_aiobotocore_ebs.type_defs import CompleteSnapshotResponseTypeDef
from types_aiobotocore_ebs.type_defs import CompleteSnapshotRequestTypeDef


session = get_session()

async with session.create_client("ebs") as client:
    client: EBSClient
    kwargs: CompleteSnapshotRequestTypeDef = {...}
    result: CompleteSnapshotResponseTypeDef = await client.complete_snapshot(**kwargs)
```




