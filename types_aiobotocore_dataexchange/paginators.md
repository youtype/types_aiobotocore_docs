<a id="paginators-for-aiobotocore-dataexchange-module"></a>

# Paginators for aiobotocore DataExchange module

> [Index](..) > [DataExchange](.) > Paginators

Auto-generated documentation for
[DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
type annotations stubs module
[types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

- [Paginators for aiobotocore DataExchange module](#paginators-for-aiobotocore-dataexchange-module)
  - [ListDataSetRevisionsPaginator](#listdatasetrevisionspaginator)
  - [ListDataSetsPaginator](#listdatasetspaginator)
  - [ListEventActionsPaginator](#listeventactionspaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListRevisionAssetsPaginator](#listrevisionassetspaginator)

<a id="listdatasetrevisionspaginator"></a>

## ListDataSetRevisionsPaginator

Type annotations for
`aiobotocore.create_client("dataexchange").get_paginator("list_data_set_revisions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator

def get_list_data_set_revisions_paginator() -> ListDataSetRevisionsPaginator:
    return Session().create_client("dataexchange").get_paginator("list_data_set_revisions")
```

Boto3 documentation:
[DataExchange.Paginator.ListDataSetRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)

Arguments for `ListDataSetRevisionsPaginator.paginate` method:

- `DataSetId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataSetRevisionsPaginator.paginate` returns
`_PageIterator`\[[ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDataSetsPaginator

Type annotations for
`aiobotocore.create_client("dataexchange").get_paginator("list_data_sets")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dataexchange.paginator import ListDataSetsPaginator

def get_list_data_sets_paginator() -> ListDataSetsPaginator:
    return Session().create_client("dataexchange").get_paginator("list_data_sets")
```

Boto3 documentation:
[DataExchange.Paginator.ListDataSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)

Arguments for `ListDataSetsPaginator.paginate` method:

- `Origin`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataSetsPaginator.paginate` returns
`_PageIterator`\[[ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listeventactionspaginator"></a>

## ListEventActionsPaginator

Type annotations for
`aiobotocore.create_client("dataexchange").get_paginator("list_event_actions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dataexchange.paginator import ListEventActionsPaginator

def get_list_event_actions_paginator() -> ListEventActionsPaginator:
    return Session().create_client("dataexchange").get_paginator("list_event_actions")
```

Boto3 documentation:
[DataExchange.Paginator.ListEventActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)

Arguments for `ListEventActionsPaginator.paginate` method:

- `EventSourceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEventActionsPaginator.paginate` returns
`_PageIterator`\[[ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`aiobotocore.create_client("dataexchange").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dataexchange.paginator import ListJobsPaginator

def get_list_jobs_paginator() -> ListJobsPaginator:
    return Session().create_client("dataexchange").get_paginator("list_jobs")
```

Boto3 documentation:
[DataExchange.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `DataSetId`: `str`
- `RevisionId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`_PageIterator`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listrevisionassetspaginator"></a>

## ListRevisionAssetsPaginator

Type annotations for
`aiobotocore.create_client("dataexchange").get_paginator("list_revision_assets")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dataexchange.paginator import ListRevisionAssetsPaginator

def get_list_revision_assets_paginator() -> ListRevisionAssetsPaginator:
    return Session().create_client("dataexchange").get_paginator("list_revision_assets")
```

Boto3 documentation:
[DataExchange.Paginator.ListRevisionAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)

Arguments for `ListRevisionAssetsPaginator.paginate` method:

- `DataSetId`: `str` *(required)*
- `RevisionId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRevisionAssetsPaginator.paginate` returns
`_PageIterator`\[[ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef)\].
