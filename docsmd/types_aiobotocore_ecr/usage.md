# Examples

> [Index](../README.md) > [ECR](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ecr]` package installed.

Write your `ECR` code as usual,
type checking and code completion should work out of the box.



```python
# ECRClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecr") as client:  # (1)
    result = await client.batch_check_layer_availability()  # (2)
```

1. client: [ECRClient](./client.md)
2. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef) 



```python
# DescribeImageScanFindingsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecr") as client:  # (1)
    paginator = client.get_paginator("describe_image_scan_findings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribeImageScanFindingsPaginator](./paginators.md#describeimagescanfindingspaginator)
3. item: [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 



```python
# ImageScanCompleteWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecr") as client:  # (1)
    waiter = client.get_waiter("image_scan_complete")  # (2)
    await waiter.wait()
```

1. client: [ECRClient](./client.md)
2. waiter: [ImageScanCompleteWaiter](./waiters.md#imagescancompletewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ecr]`
or a standalone `types_aiobotocore_ecr` package, you have to explicitly specify
`client: ECRClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ECRClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecr.client import ECRClient
from types_aiobotocore_ecr.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
from types_aiobotocore_ecr.type_defs import BatchCheckLayerAvailabilityRequestTypeDef


session = get_session()

async with session.create_client("ecr") as client:
    client: ECRClient
    kwargs: BatchCheckLayerAvailabilityRequestTypeDef = {...}
    result: BatchCheckLayerAvailabilityResponseTypeDef = await client.batch_check_layer_availability(**kwargs)
```



```python
# DescribeImageScanFindingsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecr.client import ECRClient
from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator
from types_aiobotocore_ecr.type_defs import DescribeImageScanFindingsResponseTypeDef


session = get_session()

async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: DescribeImageScanFindingsPaginator = client.get_paginator("describe_image_scan_findings")
    async for item in paginator.paginate(...):
        item: DescribeImageScanFindingsResponseTypeDef
        print(item)
```



```python
# ImageScanCompleteWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecr.client import ECRClient
from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter


session = get_session()

async with session.create_client("ecr") as client:
    client: ECRClient
    waiter: ImageScanCompleteWaiter = client.get_waiter("image_scan_complete")
    await waiter.wait()
```
