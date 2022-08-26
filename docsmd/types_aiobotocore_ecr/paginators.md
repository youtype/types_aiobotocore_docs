# Paginators

> [Index](../README.md) > [ECR](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## DescribeImageScanFindingsPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_image_scan_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: DescribeImageScanFindingsPaginator = client.get_paginator("describe_image_scan_findings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageScanFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribeImageScanFindingsPaginator](./paginators.md#describeimagescanfindingspaginator)
3. item: [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImageScanFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeImageScanFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = {  # (1)
    "repositoryName": ...,
    "imageId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef](./type_defs.md#describeimagescanfindingsrequestdescribeimagescanfindingspaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
3. item: [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    filter: DescribeImagesFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeImagesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImagesRequestDescribeImagesPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestDescribeImagesPaginateTypeDef](./type_defs.md#describeimagesrequestdescribeimagespaginatetypedef) 
## DescribePullThroughCacheRulesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_pull_through_cache_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribePullThroughCacheRulesPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: DescribePullThroughCacheRulesPaginator = client.get_paginator("describe_pull_through_cache_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePullThroughCacheRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribePullThroughCacheRulesPaginator](./paginators.md#describepullthroughcacherulespaginator)
3. item: [:material-code-braces: DescribePullThroughCacheRulesResponseTypeDef](./type_defs.md#describepullthroughcacherulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePullThroughCacheRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    registryId: str = ...,
    ecrRepositoryPrefixes: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribePullThroughCacheRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePullThroughCacheRulesResponseTypeDef](./type_defs.md#describepullthroughcacherulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = {  # (1)
    "registryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef](./type_defs.md#describepullthroughcacherulesrequestdescribepullthroughcacherulespaginatetypedef) 
## DescribeRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeRepositoriesPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: DescribeRepositoriesPaginator = client.get_paginator("describe_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRepositoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribeRepositoriesPaginator](./paginators.md#describerepositoriespaginator)
3. item: [:material-code-braces: DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRepositoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    registryId: str = ...,
    repositoryNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = {  # (1)
    "registryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef](./type_defs.md#describerepositoriesrequestdescriberepositoriespaginatetypedef) 
## GetLifecyclePolicyPreviewPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("get_lifecycle_policy_preview")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import GetLifecyclePolicyPreviewPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: GetLifecyclePolicyPreviewPaginator = client.get_paginator("get_lifecycle_policy_preview")  # (2)
    async for item in paginator.paginate(...):
        item: GetLifecyclePolicyPreviewResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [GetLifecyclePolicyPreviewPaginator](./paginators.md#getlifecyclepolicypreviewpaginator)
3. item: [:material-code-braces: GetLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#getlifecyclepolicypreviewresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetLifecyclePolicyPreviewPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    filter: LifecyclePolicyPreviewFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[GetLifecyclePolicyPreviewResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#getlifecyclepolicypreviewresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestgetlifecyclepolicypreviewpaginatetypedef) 
## ListImagesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("list_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import ListImagesPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: ListImagesPaginator = client.get_paginator("list_images")  # (2)
    async for item in paginator.paginate(...):
        item: ListImagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [ListImagesPaginator](./paginators.md#listimagespaginator)
3. item: [:material-code-braces: ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    filter: ListImagesFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListImagesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListImagesRequestListImagesPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImagesRequestListImagesPaginateTypeDef](./type_defs.md#listimagesrequestlistimagespaginatetypedef) 
