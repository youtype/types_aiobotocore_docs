<a id="paginators-for-aiobotocore-ecrpublic-module"></a>

# Paginators for aiobotocore ECRPublic module

> [Index](../README.md) > [ECRPublic](./README.md) > Paginators

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
`session.create_client("ecr-public").get_paginator("describe_image_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator

session = get_session()
async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    paginator: DescribeImageTagsPaginator = client.get_paginator("describe_image_tags")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeImageTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags)

Arguments for `DescribeImageTagsPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeImageTagsPaginator.paginate` returns
`AsyncIterator`\[[DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef)\].

<a id="describeimagespaginator"></a>

## DescribeImagesPaginator

Type annotations for
`session.create_client("ecr-public").get_paginator("describe_images")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")
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
`AsyncIterator`\[[DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef)\].

<a id="describeregistriespaginator"></a>

## DescribeRegistriesPaginator

Type annotations for
`session.create_client("ecr-public").get_paginator("describe_registries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeRegistriesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    paginator: DescribeRegistriesPaginator = client.get_paginator("describe_registries")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeRegistries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)

Arguments for `DescribeRegistriesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRegistriesPaginator.paginate` returns
`AsyncIterator`\[[DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef)\].

<a id="describerepositoriespaginator"></a>

## DescribeRepositoriesPaginator

Type annotations for
`session.create_client("ecr-public").get_paginator("describe_repositories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.paginator import DescribeRepositoriesPaginator

session = get_session()
async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    paginator: DescribeRepositoriesPaginator = client.get_paginator("describe_repositories")
```

Boto3 documentation:
[ECRPublic.Paginator.DescribeRepositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories)

Arguments for `DescribeRepositoriesPaginator.paginate` method:

- `registryId`: `str`
- `repositoryNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRepositoriesPaginator.paginate` returns
`AsyncIterator`\[[DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef)\].
