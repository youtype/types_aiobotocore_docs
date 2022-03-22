<a id="examples-for-aiobotocore-s3-module"></a>

# Examples for aiobotocore S3 module

> [Index](../README.md) > [S3](./README.md) > Examples

- [Examples for aiobotocore S3 module](#examples-for-aiobotocore-s3-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[s3]` package installed.

Write your `S3` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type S3Client
# and provides type checking and code completion
async with session.create_client("s3") as client:
    
    # result has type AbortMultipartUploadOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.abort_multipart_upload()
    

    
    # paginator has type ListMultipartUploadsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_multipart_uploads")
    async for item in paginator.paginate(...):
        # item has type ListMultipartUploadsOutputTypeDef
        print(item)
    

    
    # waiter has type BucketExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("bucket_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[s3]` or a standalone `types_aiobotocore_s3`
package, you have to explicitly specify `client: S3Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.type_defs import AbortMultipartUploadOutputTypeDef
from types_aiobotocore_s3.paginator import ListMultipartUploadsPaginator
from types_aiobotocore_s3.waiter import BucketExistsWaiter
from types_aiobotocore_s3.literals import PaginatorName
from types_aiobotocore_s3.literals import WaiterName


session = get_session()

async with session.create_client("s3") as client:
    client: S3Client

    
    result: AbortMultipartUploadOutputTypeDef = client.abort_multipart_upload()
    

    
    paginator_name: PaginatorName = "list_multipart_uploads"
    paginator: ListMultipartUploadsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListMultipartUploadsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "bucket_exists"
    waiter: BucketExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
