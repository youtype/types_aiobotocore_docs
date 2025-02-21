# Examples

> [Index](../README.md) > [CloudFront](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudfront]` package installed.

Write your `CloudFront` code as usual,
type checking and code completion should work out of the box.



```python
# CloudFrontClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudfront") as client:  # (1)
    result = await client.associate_alias()  # (2)
```

1. client: [CloudFrontClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListCloudFrontOriginAccessIdentitiesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudfront") as client:  # (1)
    paginator = client.get_paginator("list_cloud_front_origin_access_identities")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
3. item: [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef) 



```python
# DistributionDeployedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudfront") as client:  # (1)
    waiter = client.get_waiter("distribution_deployed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[cloudfront]`
or a standalone `types_aiobotocore_cloudfront` package, you have to explicitly specify
`client: CloudFrontClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudFrontClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.client import CloudFrontClient
from types_aiobotocore_cloudfront.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_cloudfront.type_defs import AssociateAliasRequestTypeDef


session = get_session()

async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    kwargs: AssociateAliasRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_alias(**kwargs)
```



```python
# ListCloudFrontOriginAccessIdentitiesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.client import CloudFrontClient
from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator
from types_aiobotocore_cloudfront.type_defs import ListCloudFrontOriginAccessIdentitiesResultTypeDef


session = get_session()

async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator("list_cloud_front_origin_access_identities")
    async for item in paginator.paginate(...):
        item: ListCloudFrontOriginAccessIdentitiesResultTypeDef
        print(item)
```



```python
# DistributionDeployedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.client import CloudFrontClient
from types_aiobotocore_cloudfront.waiter import DistributionDeployedWaiter


session = get_session()

async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    waiter: DistributionDeployedWaiter = client.get_waiter("distribution_deployed")
    await waiter.wait()
```
