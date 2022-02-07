<a id="paginators-for-aiobotocore-cloudwatchevidently-module"></a>

# Paginators for aiobotocore CloudWatchEvidently module

> [Index](..) > [CloudWatchEvidently](.) > Paginators

Auto-generated documentation for
[CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
type annotations stubs module
[types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

- [Paginators for aiobotocore CloudWatchEvidently module](#paginators-for-aiobotocore-cloudwatchevidently-module)
  - [ListExperimentsPaginator](#listexperimentspaginator)
  - [ListFeaturesPaginator](#listfeaturespaginator)
  - [ListLaunchesPaginator](#listlaunchespaginator)
  - [ListProjectsPaginator](#listprojectspaginator)

<a id="listexperimentspaginator"></a>

## ListExperimentsPaginator

Type annotations for
`session.create_client("evidently").get_paginator("list_experiments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListExperimentsPaginator

session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    paginator: ListExperimentsPaginator = client.get_paginator("list_experiments")
```

Boto3 documentation:
[CloudWatchEvidently.Paginator.ListExperiments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments)

Arguments for `ListExperimentsPaginator.paginate` method:

- `project`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListExperimentsPaginator.paginate` returns
`_PageIterator`\[[ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef)\].

<a id="listfeaturespaginator"></a>

## ListFeaturesPaginator

Type annotations for
`session.create_client("evidently").get_paginator("list_features")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListFeaturesPaginator

session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    paginator: ListFeaturesPaginator = client.get_paginator("list_features")
```

Boto3 documentation:
[CloudWatchEvidently.Paginator.ListFeatures](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)

Arguments for `ListFeaturesPaginator.paginate` method:

- `project`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFeaturesPaginator.paginate` returns
`_PageIterator`\[[ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef)\].

<a id="listlaunchespaginator"></a>

## ListLaunchesPaginator

Type annotations for
`session.create_client("evidently").get_paginator("list_launches")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListLaunchesPaginator

session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    paginator: ListLaunchesPaginator = client.get_paginator("list_launches")
```

Boto3 documentation:
[CloudWatchEvidently.Paginator.ListLaunches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches)

Arguments for `ListLaunchesPaginator.paginate` method:

- `project`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLaunchesPaginator.paginate` returns
`_PageIterator`\[[ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("evidently").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("evidently") as client:
    client: CloudWatchEvidentlyClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[CloudWatchEvidently.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`_PageIterator`\[[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)\].
