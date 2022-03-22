<a id="paginators-for-aiobotocore-dataexchange-module"></a>

# Paginators for aiobotocore DataExchange module

> [Index](../README.md) > [DataExchange](./README.md) > Paginators

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
`session.create_client("dataexchange").get_paginator("list_data_set_revisions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataSetRevisionsPaginator = client.get_paginator("list_data_set_revisions")
```

Boto3 documentation:
[DataExchange.Paginator.ListDataSetRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)

Arguments for `ListDataSetRevisionsPaginator.paginate` method:

- `DataSetId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataSetRevisionsPaginator.paginate` returns
`AsyncIterator`\[[ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDataSetsPaginator

Type annotations for
`session.create_client("dataexchange").get_paginator("list_data_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
```

Boto3 documentation:
[DataExchange.Paginator.ListDataSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)

Arguments for `ListDataSetsPaginator.paginate` method:

- `Origin`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataSetsPaginator.paginate` returns
`AsyncIterator`\[[ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listeventactionspaginator"></a>

## ListEventActionsPaginator

Type annotations for
`session.create_client("dataexchange").get_paginator("list_event_actions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListEventActionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListEventActionsPaginator = client.get_paginator("list_event_actions")
```

Boto3 documentation:
[DataExchange.Paginator.ListEventActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)

Arguments for `ListEventActionsPaginator.paginate` method:

- `EventSourceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEventActionsPaginator.paginate` returns
`AsyncIterator`\[[ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("dataexchange").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[DataExchange.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `DataSetId`: `str`
- `RevisionId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listrevisionassetspaginator"></a>

## ListRevisionAssetsPaginator

Type annotations for
`session.create_client("dataexchange").get_paginator("list_revision_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListRevisionAssetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListRevisionAssetsPaginator = client.get_paginator("list_revision_assets")
```

Boto3 documentation:
[DataExchange.Paginator.ListRevisionAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)

Arguments for `ListRevisionAssetsPaginator.paginate` method:

- `DataSetId`: `str` *(required)*
- `RevisionId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRevisionAssetsPaginator.paginate` returns
`AsyncIterator`\[[ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef)\].
