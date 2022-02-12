<a id="paginators-for-aiobotocore-ecr-module"></a>

# Paginators for aiobotocore ECR module

> [Index](..) > [ECR](.) > Paginators

Auto-generated documentation for
[ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
type annotations stubs module
[types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

- [Paginators for aiobotocore ECR module](#paginators-for-aiobotocore-ecr-module)
  - [DescribeImageScanFindingsPaginator](#describeimagescanfindingspaginator)
  - [DescribeImagesPaginator](#describeimagespaginator)
  - [DescribePullThroughCacheRulesPaginator](#describepullthroughcacherulespaginator)
  - [DescribeRepositoriesPaginator](#describerepositoriespaginator)
  - [GetLifecyclePolicyPreviewPaginator](#getlifecyclepolicypreviewpaginator)
  - [ListImagesPaginator](#listimagespaginator)

<a id="describeimagescanfindingspaginator"></a>

## DescribeImageScanFindingsPaginator

Type annotations for
`session.create_client("ecr").get_paginator("describe_image_scan_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: DescribeImageScanFindingsPaginator = client.get_paginator("describe_image_scan_findings")
```

Boto3 documentation:
[ECR.Paginator.DescribeImageScanFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings)

Arguments for `DescribeImageScanFindingsPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `imageId`: [ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)
  *(required)*
- `registryId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeImageScanFindingsPaginator.paginate` returns
`AsyncIterable`\[[DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef)\].

<a id="describeimagespaginator"></a>

## DescribeImagesPaginator

Type annotations for
`session.create_client("ecr").get_paginator("describe_images")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")
```

Boto3 documentation:
[ECR.Paginator.DescribeImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages)

Arguments for `DescribeImagesPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
- `filter`:
  [DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeImagesPaginator.paginate` returns
`AsyncIterable`\[[DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef)\].

<a id="describepullthroughcacherulespaginator"></a>

## DescribePullThroughCacheRulesPaginator

Type annotations for
`session.create_client("ecr").get_paginator("describe_pull_through_cache_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribePullThroughCacheRulesPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: DescribePullThroughCacheRulesPaginator = client.get_paginator("describe_pull_through_cache_rules")
```

Boto3 documentation:
[ECR.Paginator.DescribePullThroughCacheRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules)

Arguments for `DescribePullThroughCacheRulesPaginator.paginate` method:

- `registryId`: `str`
- `ecrRepositoryPrefixes`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribePullThroughCacheRulesPaginator.paginate` returns
`AsyncIterable`\[[DescribePullThroughCacheRulesResponseTypeDef](./type_defs.md#describepullthroughcacherulesresponsetypedef)\].

<a id="describerepositoriespaginator"></a>

## DescribeRepositoriesPaginator

Type annotations for
`session.create_client("ecr").get_paginator("describe_repositories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeRepositoriesPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: DescribeRepositoriesPaginator = client.get_paginator("describe_repositories")
```

Boto3 documentation:
[ECR.Paginator.DescribeRepositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories)

Arguments for `DescribeRepositoriesPaginator.paginate` method:

- `registryId`: `str`
- `repositoryNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRepositoriesPaginator.paginate` returns
`AsyncIterable`\[[DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef)\].

<a id="getlifecyclepolicypreviewpaginator"></a>

## GetLifecyclePolicyPreviewPaginator

Type annotations for
`session.create_client("ecr").get_paginator("get_lifecycle_policy_preview")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import GetLifecyclePolicyPreviewPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: GetLifecyclePolicyPreviewPaginator = client.get_paginator("get_lifecycle_policy_preview")
```

Boto3 documentation:
[ECR.Paginator.GetLifecyclePolicyPreview](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview)

Arguments for `GetLifecyclePolicyPreviewPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
- `filter`:
  [LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetLifecyclePolicyPreviewPaginator.paginate` returns
`AsyncIterable`\[[GetLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#getlifecyclepolicypreviewresponsetypedef)\].

<a id="listimagespaginator"></a>

## ListImagesPaginator

Type annotations for
`session.create_client("ecr").get_paginator("list_images")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import ListImagesPaginator

session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
    paginator: ListImagesPaginator = client.get_paginator("list_images")
```

Boto3 documentation:
[ECR.Paginator.ListImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages)

Arguments for `ListImagesPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `filter`: [ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListImagesPaginator.paginate` returns
`AsyncIterable`\[[ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef)\].
