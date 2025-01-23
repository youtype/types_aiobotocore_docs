# Paginators

> [Index](../README.md) > [DataExchange](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#dataexchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## ListDataGrantsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_data_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListDataGrants.html#DataExchange.Paginator.ListDataGrants)

```python
# ListDataGrantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataGrantsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListDataGrantsPaginator = client.get_paginator("list_data_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataGrantsPaginator](./paginators.md#listdatagrantspaginator)
3. item: [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataGrantsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataGrantsRequestPaginateTypeDef](./type_defs.md#listdatagrantsrequestpaginatetypedef) 
## ListDataSetRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_data_set_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListDataSetRevisions.html#DataExchange.Paginator.ListDataSetRevisions)

```python
# ListDataSetRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListDataSetRevisionsPaginator = client.get_paginator("list_data_set_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataSetRevisionsPaginator](./paginators.md#listdatasetrevisionspaginator)
3. item: [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSetRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataSetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataSetRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetRevisionsRequestPaginateTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetRevisionsRequestPaginateTypeDef](./type_defs.md#listdatasetrevisionsrequestpaginatetypedef) 
## ListDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListDataSets.html#DataExchange.Paginator.ListDataSets)

```python
# ListDataSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListDataSetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Origin: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetsRequestPaginateTypeDef = {  # (1)
    "Origin": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef) 
## ListEventActionsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_event_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListEventActions.html#DataExchange.Paginator.ListEventActions)

```python
# ListEventActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListEventActionsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListEventActionsPaginator = client.get_paginator("list_event_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListEventActionsPaginator](./paginators.md#listeventactionspaginator)
3. item: [:material-code-braces: ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EventSourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventActionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventActionsRequestPaginateTypeDef = {  # (1)
    "EventSourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventActionsRequestPaginateTypeDef](./type_defs.md#listeventactionsrequestpaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListJobs.html#DataExchange.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataSetId: str = ...,
    RevisionId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef) 
## ListReceivedDataGrantsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_received_data_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListReceivedDataGrants.html#DataExchange.Paginator.ListReceivedDataGrants)

```python
# ListReceivedDataGrantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListReceivedDataGrantsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListReceivedDataGrantsPaginator = client.get_paginator("list_received_data_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListReceivedDataGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListReceivedDataGrantsPaginator](./paginators.md#listreceiveddatagrantspaginator)
3. item: [:material-code-braces: ListReceivedDataGrantsResponseTypeDef](./type_defs.md#listreceiveddatagrantsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReceivedDataGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AcceptanceState: Sequence[AcceptanceStateFilterValueType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListReceivedDataGrantsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AcceptanceStateFilterValueType](./literals.md#acceptancestatefiltervaluetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListReceivedDataGrantsResponseTypeDef](./type_defs.md#listreceiveddatagrantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReceivedDataGrantsRequestPaginateTypeDef = {  # (1)
    "AcceptanceState": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReceivedDataGrantsRequestPaginateTypeDef](./type_defs.md#listreceiveddatagrantsrequestpaginatetypedef) 
## ListRevisionAssetsPaginator

Type annotations and code completion for `#!python session.create_client("dataexchange").get_paginator("list_revision_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange/paginator/ListRevisionAssets.html#DataExchange.Paginator.ListRevisionAssets)

```python
# ListRevisionAssetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.paginator import ListRevisionAssetsPaginator

session = get_session()
async with session.create_client("dataexchange") as client:  # (1)
    paginator: ListRevisionAssetsPaginator = client.get_paginator("list_revision_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRevisionAssetsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListRevisionAssetsPaginator](./paginators.md#listrevisionassetspaginator)
3. item: [:material-code-braces: ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRevisionAssetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRevisionAssetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRevisionAssetsRequestPaginateTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRevisionAssetsRequestPaginateTypeDef](./type_defs.md#listrevisionassetsrequestpaginatetypedef) 
