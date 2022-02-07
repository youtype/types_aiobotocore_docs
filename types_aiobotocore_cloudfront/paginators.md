<a id="paginators-for-aiobotocore-cloudfront-module"></a>

# Paginators for aiobotocore CloudFront module

> [Index](..) > [CloudFront](.) > Paginators

Auto-generated documentation for
[CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
type annotations stubs module
[types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

- [Paginators for aiobotocore CloudFront module](#paginators-for-aiobotocore-cloudfront-module)
  - [ListCloudFrontOriginAccessIdentitiesPaginator](#listcloudfrontoriginaccessidentitiespaginator)
  - [ListDistributionsPaginator](#listdistributionspaginator)
  - [ListInvalidationsPaginator](#listinvalidationspaginator)
  - [ListStreamingDistributionsPaginator](#liststreamingdistributionspaginator)

<a id="listcloudfrontoriginaccessidentitiespaginator"></a>

## ListCloudFrontOriginAccessIdentitiesPaginator

Type annotations for
`session.create_client("cloudfront").get_paginator("list_cloud_front_origin_access_identities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator

session = get_session()
async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator("list_cloud_front_origin_access_identities")
```

Boto3 documentation:
[CloudFront.Paginator.ListCloudFrontOriginAccessIdentities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)

Arguments for `ListCloudFrontOriginAccessIdentitiesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCloudFrontOriginAccessIdentitiesPaginator.paginate` returns
`_PageIterator`\[[ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef)\].

<a id="listdistributionspaginator"></a>

## ListDistributionsPaginator

Type annotations for
`session.create_client("cloudfront").get_paginator("list_distributions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListDistributionsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    paginator: ListDistributionsPaginator = client.get_paginator("list_distributions")
```

Boto3 documentation:
[CloudFront.Paginator.ListDistributions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)

Arguments for `ListDistributionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDistributionsPaginator.paginate` returns
`_PageIterator`\[[ListDistributionsResultTypeDef](./type_defs.md#listdistributionsresulttypedef)\].

<a id="listinvalidationspaginator"></a>

## ListInvalidationsPaginator

Type annotations for
`session.create_client("cloudfront").get_paginator("list_invalidations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListInvalidationsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    paginator: ListInvalidationsPaginator = client.get_paginator("list_invalidations")
```

Boto3 documentation:
[CloudFront.Paginator.ListInvalidations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)

Arguments for `ListInvalidationsPaginator.paginate` method:

- `DistributionId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInvalidationsPaginator.paginate` returns
`_PageIterator`\[[ListInvalidationsResultTypeDef](./type_defs.md#listinvalidationsresulttypedef)\].

<a id="liststreamingdistributionspaginator"></a>

## ListStreamingDistributionsPaginator

Type annotations for
`session.create_client("cloudfront").get_paginator("list_streaming_distributions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudfront.paginator import ListStreamingDistributionsPaginator

session = get_session()
async with session.create_client("cloudfront") as client:
    client: CloudFrontClient
    paginator: ListStreamingDistributionsPaginator = client.get_paginator("list_streaming_distributions")
```

Boto3 documentation:
[CloudFront.Paginator.ListStreamingDistributions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)

Arguments for `ListStreamingDistributionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamingDistributionsPaginator.paginate` returns
`_PageIterator`\[[ListStreamingDistributionsResultTypeDef](./type_defs.md#liststreamingdistributionsresulttypedef)\].
