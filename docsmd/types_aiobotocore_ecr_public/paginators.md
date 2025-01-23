# Paginators

> [Index](../README.md) > [ECRPublic](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ecrpublic)
    type annotations stubs module [types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

## DescribeImageTagsPaginator

Type annotations and code completion for `#!python session.create_client("ecr-public").get_paginator("describe_image_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public/paginator/DescribeImageTags.html#ECRPublic.Paginator.DescribeImageTags)

```python
# DescribeImageTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator

session = get_session()
async with session.create_client("ecr-public") as client:  # (1)
    paginator: DescribeImageTagsPaginator = client.get_paginator("describe_image_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
3. item: [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImageTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeImageTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageTagsRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageTagsRequestPaginateTypeDef](./type_defs.md#describeimagetagsrequestpaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.create_client("ecr-public").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public/paginator/DescribeImages.html#ECRPublic.Paginator.DescribeImages)

```python
# DescribeImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeImagesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImagesRequestPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestPaginateTypeDef](./type_defs.md#describeimagesrequestpaginatetypedef) 
## DescribeRegistriesPaginator

Type annotations and code completion for `#!python session.create_client("ecr-public").get_paginator("describe_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public/paginator/DescribeRegistries.html#ECRPublic.Paginator.DescribeRegistries)

```python
# DescribeRegistriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeRegistriesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:  # (1)
    paginator: DescribeRegistriesPaginator = client.get_paginator("describe_registries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistriesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeRegistriesPaginator](./paginators.md#describeregistriespaginator)
3. item: [:material-code-braces: DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRegistriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistriesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistriesRequestPaginateTypeDef](./type_defs.md#describeregistriesrequestpaginatetypedef) 
## DescribeRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("ecr-public").get_paginator("describe_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public/paginator/DescribeRepositories.html#ECRPublic.Paginator.DescribeRepositories)

```python
# DescribeRepositoriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeRepositoriesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:  # (1)
    paginator: DescribeRepositoriesPaginator = client.get_paginator("describe_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRepositoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
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
