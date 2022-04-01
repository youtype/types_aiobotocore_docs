# Paginators

> [Index](../README.md) > [DataExchange](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## ListDataSetRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_data_set_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataSetRevisionsPaginator = client.get_paginator("list_data_set_revisions")
```


### paginate

Type annotations and code completion for `#!python ListDataSetRevisionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DataSetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataSetRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef](./type_defs.md#listdatasetrevisionsrequestlistdatasetrevisionspaginatetypedef) 
## ListDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
```


### paginate

Type annotations and code completion for `#!python ListDataSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Origin: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataSetsRequestListDataSetsPaginateTypeDef = {  # (1)
    "Origin": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestListDataSetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListEventActionsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_event_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListEventActionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListEventActionsPaginator = client.get_paginator("list_event_actions")
```


### paginate

Type annotations and code completion for `#!python ListEventActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EventSourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEventActionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEventActionsRequestListEventActionsPaginateTypeDef = {  # (1)
    "EventSourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventActionsRequestListEventActionsPaginateTypeDef](./type_defs.md#listeventactionsrequestlisteventactionspaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DataSetId: str = ...,
    RevisionId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListRevisionAssetsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_revision_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListRevisionAssetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListRevisionAssetsPaginator = client.get_paginator("list_revision_assets")
```


### paginate

Type annotations and code completion for `#!python ListRevisionAssetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRevisionAssetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef](./type_defs.md#listrevisionassetsrequestlistrevisionassetspaginatetypedef) 
