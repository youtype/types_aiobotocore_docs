# Paginators

> [Index](../README.md) > [CloudFront](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## ListCloudFrontOriginAccessIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("cloudfront").get_paginator("list_cloud_front_origin_access_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator("list_cloud_front_origin_access_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudFrontOriginAccessIdentitiesResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
3. item: [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListCloudFrontOriginAccessIdentitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesrequestlistcloudfrontoriginaccessidentitiespaginatetypedef) 
## ListDistributionsPaginator

Type annotations and code completion for `#!python session.create_client("cloudfront").get_paginator("list_distributions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListDistributionsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    paginator: ListDistributionsPaginator = client.get_paginator("list_distributions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDistributionsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListDistributionsPaginator](./paginators.md#listdistributionspaginator)
3. item: [:material-code-braces: ListDistributionsResultTypeDef](./type_defs.md#listdistributionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDistributionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDistributionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDistributionsResultTypeDef](./type_defs.md#listdistributionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDistributionsRequestListDistributionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDistributionsRequestListDistributionsPaginateTypeDef](./type_defs.md#listdistributionsrequestlistdistributionspaginatetypedef) 
## ListInvalidationsPaginator

Type annotations and code completion for `#!python session.create_client("cloudfront").get_paginator("list_invalidations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListInvalidationsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    paginator: ListInvalidationsPaginator = client.get_paginator("list_invalidations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvalidationsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListInvalidationsPaginator](./paginators.md#listinvalidationspaginator)
3. item: [:material-code-braces: ListInvalidationsResultTypeDef](./type_defs.md#listinvalidationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListInvalidationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DistributionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInvalidationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInvalidationsResultTypeDef](./type_defs.md#listinvalidationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListInvalidationsRequestListInvalidationsPaginateTypeDef = {  # (1)
    "DistributionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvalidationsRequestListInvalidationsPaginateTypeDef](./type_defs.md#listinvalidationsrequestlistinvalidationspaginatetypedef) 
## ListStreamingDistributionsPaginator

Type annotations and code completion for `#!python session.create_client("cloudfront").get_paginator("list_streaming_distributions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListStreamingDistributionsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:  # (1)
    paginator: ListStreamingDistributionsPaginator = client.get_paginator("list_streaming_distributions")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamingDistributionsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListStreamingDistributionsPaginator](./paginators.md#liststreamingdistributionspaginator)
3. item: [:material-code-braces: ListStreamingDistributionsResultTypeDef](./type_defs.md#liststreamingdistributionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamingDistributionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamingDistributionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamingDistributionsResultTypeDef](./type_defs.md#liststreamingdistributionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef](./type_defs.md#liststreamingdistributionsrequestliststreamingdistributionspaginatetypedef) 
