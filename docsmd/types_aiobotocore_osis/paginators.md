# Paginators

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## ListPipelineEndpointConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("osis").get_paginator("list_pipeline_endpoint_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis/paginator/ListPipelineEndpointConnections.html#OpenSearchIngestion.Paginator.ListPipelineEndpointConnections)

```python
# ListPipelineEndpointConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_osis.paginator import ListPipelineEndpointConnectionsPaginator

session = get_session()
async with session.create_client("osis") as client:  # (1)
    paginator: ListPipelineEndpointConnectionsPaginator = client.get_paginator("list_pipeline_endpoint_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelineEndpointConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. paginator: [ListPipelineEndpointConnectionsPaginator](./paginators.md#listpipelineendpointconnectionspaginator)
3. item: `AioPageIterator[ListPipelineEndpointConnectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelineEndpointConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPipelineEndpointConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPipelineEndpointConnectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelineEndpointConnectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelineEndpointConnectionsRequestPaginateTypeDef](./type_defs.md#listpipelineendpointconnectionsrequestpaginatetypedef)
## ListPipelineEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("osis").get_paginator("list_pipeline_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis/paginator/ListPipelineEndpoints.html#OpenSearchIngestion.Paginator.ListPipelineEndpoints)

```python
# ListPipelineEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_osis.paginator import ListPipelineEndpointsPaginator

session = get_session()
async with session.create_client("osis") as client:  # (1)
    paginator: ListPipelineEndpointsPaginator = client.get_paginator("list_pipeline_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelineEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. paginator: [ListPipelineEndpointsPaginator](./paginators.md#listpipelineendpointspaginator)
3. item: `AioPageIterator[ListPipelineEndpointsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelineEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPipelineEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPipelineEndpointsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelineEndpointsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelineEndpointsRequestPaginateTypeDef](./type_defs.md#listpipelineendpointsrequestpaginatetypedef)
