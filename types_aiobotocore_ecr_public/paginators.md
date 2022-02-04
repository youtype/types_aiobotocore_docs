<a id="paginators-for-aiobotocore-ecrpublic-module"></a>

# Paginators for aiobotocore ECRPublic module

> [Index](..) > [ECRPublic](.) > Paginators

Auto-generated documentation for
[ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
type annotations stubs module
[types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

- [Paginators for aiobotocore ECRPublic module](#paginators-for-aiobotocore-ecrpublic-module)
  - [DescribeImageTagsPaginator](#describeimagetagspaginator)
  - [DescribeImagesPaginator](#describeimagespaginator)
  - [DescribeRegistriesPaginator](#describeregistriespaginator)
  - [DescribeRepositoriesPaginator](#describerepositoriespaginator)

<a id="describeimagetagspaginator"></a>

## DescribeImageTagsPaginator

Type annotations for
`aiobotocore.create_client("ecr-public").get_paginator("describe_image_tags")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator

def get_describe_image_tags_paginator() -> DescribeImageTagsPaginator:
    return Session().create_client("ecr-public").get_paginator("describe_image_tags")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeImageTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags)

Arguments for `DescribeImageTagsPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeImageTagsPaginator.paginate` returns
`_PageIterator`\[[DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef)\].

<a id="describeimagespaginator"></a>

## DescribeImagesPaginator

Type annotations for
`aiobotocore.create_client("ecr-public").get_paginator("describe_images")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeImagesPaginator

def get_describe_images_paginator() -> DescribeImagesPaginator:
    return Session().create_client("ecr-public").get_paginator("describe_images")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages)

Arguments for `DescribeImagesPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeImagesPaginator.paginate` returns
`_PageIterator`\[[DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef)\].

<a id="describeregistriespaginator"></a>

## DescribeRegistriesPaginator

Type annotations for
`aiobotocore.create_client("ecr-public").get_paginator("describe_registries")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeRegistriesPaginator

def get_describe_registries_paginator() -> DescribeRegistriesPaginator:
    return Session().create_client("ecr-public").get_paginator("describe_registries")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeRegistries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)

Arguments for `DescribeRegistriesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRegistriesPaginator.paginate` returns
`_PageIterator`\[[DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef)\].

<a id="describerepositoriespaginator"></a>

## DescribeRepositoriesPaginator

Type annotations for
`aiobotocore.create_client("ecr-public").get_paginator("describe_repositories")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeRepositoriesPaginator

def get_describe_repositories_paginator() -> DescribeRepositoriesPaginator:
    return Session().create_client("ecr-public").get_paginator("describe_repositories")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeRepositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories)

Arguments for `DescribeRepositoriesPaginator.paginate` method:

- `registryId`: `str`
- `repositoryNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRepositoriesPaginator.paginate` returns
`_PageIterator`\[[DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef)\].
