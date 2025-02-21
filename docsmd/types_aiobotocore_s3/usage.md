# Examples

> [Index](../README.md) > [S3](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#s3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3]` package installed.

Write your `S3` code as usual,
type checking and code completion should work out of the box.



```python
# S3Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3") as client:  # (1)
    result = await client.abort_multipart_upload()  # (2)
```

1. client: [S3Client](./client.md)
2. result: [:material-code-braces: AbortMultipartUploadOutputTypeDef](./type_defs.md#abortmultipartuploadoutputtypedef) 



```python
# ListBucketsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3") as client:  # (1)
    paginator = client.get_paginator("list_buckets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListBucketsPaginator](./paginators.md#listbucketspaginator)
3. item: [:material-code-braces: ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef) 



```python
# BucketExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("s3") as client:  # (1)
    waiter = client.get_waiter("bucket_exists")  # (2)
    await waiter.wait()
```

1. client: [S3Client](./client.md)
2. waiter: [BucketExistsWaiter](./waiters.md#bucketexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[s3]`
or a standalone `types_aiobotocore_s3` package, you have to explicitly specify
`client: S3Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# S3Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.type_defs import AbortMultipartUploadOutputTypeDef
from types_aiobotocore_s3.type_defs import AbortMultipartUploadRequestTypeDef


session = get_session()

async with session.create_client("s3") as client:
    client: S3Client
    kwargs: AbortMultipartUploadRequestTypeDef = {...}
    result: AbortMultipartUploadOutputTypeDef = await client.abort_multipart_upload(**kwargs)
```



```python
# ListBucketsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.paginator import ListBucketsPaginator
from types_aiobotocore_s3.type_defs import ListBucketsOutputTypeDef


session = get_session()

async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListBucketsPaginator = client.get_paginator("list_buckets")
    async for item in paginator.paginate(...):
        item: ListBucketsOutputTypeDef
        print(item)
```



```python
# BucketExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.waiter import BucketExistsWaiter


session = get_session()

async with session.create_client("s3") as client:
    client: S3Client
    waiter: BucketExistsWaiter = client.get_waiter("bucket_exists")
    await waiter.wait()
```
