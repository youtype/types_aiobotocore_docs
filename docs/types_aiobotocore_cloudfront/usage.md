<a id="examples-for-aiobotocore-cloudfront-module"></a>

# Examples for aiobotocore CloudFront module

> [Index](../README.md) > [CloudFront](./README.md) > Examples

- [Examples for aiobotocore CloudFront module](#examples-for-aiobotocore-cloudfront-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudfront]` package installed.

Write your `CloudFront` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudFrontClient
# and provides type checking and code completion
async with session.create_client("cloudfront") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_alias()
    

    
    # paginator has type ListCloudFrontOriginAccessIdentitiesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_cloud_front_origin_access_identities")
    async for item in paginator.paginate(...):
        # item has type ListCloudFrontOriginAccessIdentitiesResultTypeDef
        print(item)
    

    
    # waiter has type DistributionDeployedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("distribution_deployed")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudfront]` or a standalone
`types_aiobotocore_cloudfront` package, you have to explicitly specify
`client: CloudFrontClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.client import CloudFrontClient
from types_aiobotocore_cloudfront.type_defs import None
from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator
from types_aiobotocore_cloudfront.waiter import DistributionDeployedWaiter
from types_aiobotocore_cloudfront.literals import PaginatorName
from types_aiobotocore_cloudfront.literals import WaiterName


session = get_session()

async with session.create_client("cloudfront") as client:
    client: CloudFrontClient

    
    result: None = client.associate_alias()
    

    
    paginator_name: PaginatorName = "list_cloud_front_origin_access_identities"
    paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListCloudFrontOriginAccessIdentitiesResultTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "distribution_deployed"
    waiter: DistributionDeployedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```