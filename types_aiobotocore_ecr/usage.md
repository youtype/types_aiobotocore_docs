<a id="examples-for-aiobotocore-ecr-module"></a>

# Examples for aiobotocore ECR module

> [Index](../README.md) > [ECR](./README.md) > Examples

- [Examples for aiobotocore ECR module](#examples-for-aiobotocore-ecr-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ecr]` package installed.

Write your `ECR` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ECRClient
# and provides type checking and code completion
async with session.create_client("ecr") as client:
    
    # result has type BatchCheckLayerAvailabilityResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_check_layer_availability()
    

    
    # paginator has type DescribeImageScanFindingsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_image_scan_findings")
    async for item in paginator.paginate(...):
        # item has type DescribeImageScanFindingsResponseTypeDef
        print(item)
    

    
    # waiter has type ImageScanCompleteWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("image_scan_complete")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ecr]` or a standalone `types_aiobotocore_ecr`
package, you have to explicitly specify `client: ECRClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.client import ECRClient
from types_aiobotocore_ecr.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator
from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter
from types_aiobotocore_ecr.literals import PaginatorName
from types_aiobotocore_ecr.literals import WaiterName


session = get_session()

async with session.create_client("ecr") as client:
    client: ECRClient

    
    result: BatchCheckLayerAvailabilityResponseTypeDef = client.batch_check_layer_availability()
    

    
    paginator_name: PaginatorName = "describe_image_scan_findings"
    paginator: DescribeImageScanFindingsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeImageScanFindingsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "image_scan_complete"
    waiter: ImageScanCompleteWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
