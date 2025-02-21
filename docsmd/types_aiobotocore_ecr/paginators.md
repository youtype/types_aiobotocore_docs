# Paginators

> [Index](../README.md) > [ECR](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## DescribeImageScanFindingsPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_image_scan_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/DescribeImageScanFindings.html#ECR.Paginator.DescribeImageScanFindings)

```python
# DescribeImageScanFindingsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeImageScanFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageScanFindingsRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
    "imageId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageScanFindingsRequestPaginateTypeDef](./type_defs.md#describeimagescanfindingsrequestpaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/DescribeImages.html#ECR.Paginator.DescribeImages)

```python
# DescribeImagesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    filter: DescribeImagesFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeImagesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImagesRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestPaginateTypeDef](./type_defs.md#describeimagesrequestpaginatetypedef) 
## DescribePullThroughCacheRulesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_pull_through_cache_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/DescribePullThroughCacheRules.html#ECR.Paginator.DescribePullThroughCacheRules)

```python
# DescribePullThroughCacheRulesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    registryId: str = ...,
    ecrRepositoryPrefixes: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribePullThroughCacheRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePullThroughCacheRulesResponseTypeDef](./type_defs.md#describepullthroughcacherulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePullThroughCacheRulesRequestPaginateTypeDef = {  # (1)
    "registryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePullThroughCacheRulesRequestPaginateTypeDef](./type_defs.md#describepullthroughcacherulesrequestpaginatetypedef) 
## DescribeRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/DescribeRepositories.html#ECR.Paginator.DescribeRepositories)

```python
# DescribeRepositoriesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    registryId: str = ...,
    repositoryNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRepositoriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRepositoriesRequestPaginateTypeDef = {  # (1)
    "registryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRepositoriesRequestPaginateTypeDef](./type_defs.md#describerepositoriesrequestpaginatetypedef) 
## DescribeRepositoryCreationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("describe_repository_creation_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/DescribeRepositoryCreationTemplates.html#ECR.Paginator.DescribeRepositoryCreationTemplates)

```python
# DescribeRepositoryCreationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr.paginator import DescribeRepositoryCreationTemplatesPaginator

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    paginator: DescribeRepositoryCreationTemplatesPaginator = client.get_paginator("describe_repository_creation_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRepositoryCreationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRClient](./client.md)
2. paginator: [DescribeRepositoryCreationTemplatesPaginator](./paginators.md#describerepositorycreationtemplatespaginator)
3. item: [:material-code-braces: DescribeRepositoryCreationTemplatesResponseTypeDef](./type_defs.md#describerepositorycreationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRepositoryCreationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    prefixes: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRepositoryCreationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRepositoryCreationTemplatesResponseTypeDef](./type_defs.md#describerepositorycreationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRepositoryCreationTemplatesRequestPaginateTypeDef = {  # (1)
    "prefixes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRepositoryCreationTemplatesRequestPaginateTypeDef](./type_defs.md#describerepositorycreationtemplatesrequestpaginatetypedef) 
## GetLifecyclePolicyPreviewPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("get_lifecycle_policy_preview")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/GetLifecyclePolicyPreview.html#ECR.Paginator.GetLifecyclePolicyPreview)

```python
# GetLifecyclePolicyPreviewPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    filter: LifecyclePolicyPreviewFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetLifecyclePolicyPreviewResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#getlifecyclepolicypreviewresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetLifecyclePolicyPreviewRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyPreviewRequestPaginateTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestpaginatetypedef) 
## ListImagesPaginator

Type annotations and code completion for `#!python session.create_client("ecr").get_paginator("list_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/paginator/ListImages.html#ECR.Paginator.ListImages)

```python
# ListImagesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    filter: ListImagesFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListImagesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImagesRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImagesRequestPaginateTypeDef](./type_defs.md#listimagesrequestpaginatetypedef) 
