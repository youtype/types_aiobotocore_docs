# Examples

> [Index](../README.md) > [EFS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#efs)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[efs]` package installed.

Write your `EFS` code as usual,
type checking and code completion should work out of the box.



```python
# EFSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("efs") as client:  # (1)
    result = await client.create_access_point()  # (2)
```

1. client: [EFSClient](./client.md)
2. result: [:material-code-braces: AccessPointDescriptionResponseTypeDef](./type_defs.md#accesspointdescriptionresponsetypedef) 



```python
# DescribeAccessPointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("efs") as client:  # (1)
    paginator = client.get_paginator("describe_access_points")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeAccessPointsPaginator](./paginators.md#describeaccesspointspaginator)
3. item: [:material-code-braces: DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[efs]`
or a standalone `types_aiobotocore_efs` package, you have to explicitly specify
`client: EFSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EFSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_efs.client import EFSClient
from types_aiobotocore_efs.type_defs import AccessPointDescriptionResponseTypeDef
from types_aiobotocore_efs.type_defs import CreateAccessPointRequestTypeDef


session = get_session()

async with session.create_client("efs") as client:
    client: EFSClient
    kwargs: CreateAccessPointRequestTypeDef = {...}
    result: AccessPointDescriptionResponseTypeDef = await client.create_access_point(**kwargs)
```



```python
# DescribeAccessPointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_efs.client import EFSClient
from types_aiobotocore_efs.paginator import DescribeAccessPointsPaginator
from types_aiobotocore_efs.type_defs import DescribeAccessPointsResponseTypeDef


session = get_session()

async with session.create_client("efs") as client:
    client: EFSClient
    paginator: DescribeAccessPointsPaginator = client.get_paginator("describe_access_points")
    async for item in paginator.paginate(...):
        item: DescribeAccessPointsResponseTypeDef
        print(item)
```


