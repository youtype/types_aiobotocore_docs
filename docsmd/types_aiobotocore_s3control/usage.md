# Examples

> [Index](../README.md) > [S3Control](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#s3control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3control]` package installed.

Write your `S3Control` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# S3ControlClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3control") as client:  # (1)
    result = await client.associate_access_grants_identity_center()  # (2)
```

1. client: [S3ControlClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListAccessPointsForDirectoryBucketsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3control") as client:  # (1)
    paginator = client.get_paginator("list_access_points_for_directory_buckets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForDirectoryBucketsPaginator](./paginators.md#listaccesspointsfordirectorybucketspaginator)
3. item: [:material-code-braces: ListAccessPointsForDirectoryBucketsResultTypeDef](./type_defs.md#listaccesspointsfordirectorybucketsresulttypedef)




### Explicit type annotations

With `types-aiobotocore-lite[s3control]`
or a standalone `types_aiobotocore_s3control` package, you have to explicitly specify
`client: S3ControlClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# S3ControlClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3control.client import S3ControlClient
from types_aiobotocore_s3control.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_s3control.type_defs import AssociateAccessGrantsIdentityCenterRequestTypeDef


session = get_session()

async with session.create_client("s3control") as client:
    client: S3ControlClient
    kwargs: AssociateAccessGrantsIdentityCenterRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_access_grants_identity_center(**kwargs)
```



#### Paginator usage example

```python
# ListAccessPointsForDirectoryBucketsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3control.client import S3ControlClient
from types_aiobotocore_s3control.paginator import ListAccessPointsForDirectoryBucketsPaginator
from types_aiobotocore_s3control.type_defs import ListAccessPointsForDirectoryBucketsResultTypeDef


session = get_session()

async with session.create_client("s3control") as client:
    client: S3ControlClient
    paginator: ListAccessPointsForDirectoryBucketsPaginator = client.get_paginator("list_access_points_for_directory_buckets")
    async for item in paginator.paginate(...):
        item: ListAccessPointsForDirectoryBucketsResultTypeDef
        print(item)
```


