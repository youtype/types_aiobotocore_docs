# Paginators

> [Index](../README.md) > [AppFabric](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#appfabric)
    type annotations stubs module [types-aiobotocore-appfabric](https://pypi.org/project/types-aiobotocore-appfabric/).

## ListAppAuthorizationsPaginator

Type annotations and code completion for `#!python session.create_client("appfabric").get_paginator("list_app_authorizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric/paginator/ListAppAuthorizations.html#AppFabric.Paginator.ListAppAuthorizations)

```python
# ListAppAuthorizationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.paginator import ListAppAuthorizationsPaginator

session = get_session()
async with session.create_client("appfabric") as client:  # (1)
    paginator: ListAppAuthorizationsPaginator = client.get_paginator("list_app_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListAppAuthorizationsPaginator](./paginators.md#listappauthorizationspaginator)
3. item: [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppAuthorizationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appBundleIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppAuthorizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppAuthorizationsRequestPaginateTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppAuthorizationsRequestPaginateTypeDef](./type_defs.md#listappauthorizationsrequestpaginatetypedef) 
## ListAppBundlesPaginator

Type annotations and code completion for `#!python session.create_client("appfabric").get_paginator("list_app_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric/paginator/ListAppBundles.html#AppFabric.Paginator.ListAppBundles)

```python
# ListAppBundlesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.paginator import ListAppBundlesPaginator

session = get_session()
async with session.create_client("appfabric") as client:  # (1)
    paginator: ListAppBundlesPaginator = client.get_paginator("list_app_bundles")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppBundlesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListAppBundlesPaginator](./paginators.md#listappbundlespaginator)
3. item: [:material-code-braces: ListAppBundlesResponseTypeDef](./type_defs.md#listappbundlesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppBundlesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppBundlesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppBundlesResponseTypeDef](./type_defs.md#listappbundlesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppBundlesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppBundlesRequestPaginateTypeDef](./type_defs.md#listappbundlesrequestpaginatetypedef) 
## ListIngestionDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("appfabric").get_paginator("list_ingestion_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric/paginator/ListIngestionDestinations.html#AppFabric.Paginator.ListIngestionDestinations)

```python
# ListIngestionDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.paginator import ListIngestionDestinationsPaginator

session = get_session()
async with session.create_client("appfabric") as client:  # (1)
    paginator: ListIngestionDestinationsPaginator = client.get_paginator("list_ingestion_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngestionDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListIngestionDestinationsPaginator](./paginators.md#listingestiondestinationspaginator)
3. item: [:material-code-braces: ListIngestionDestinationsResponseTypeDef](./type_defs.md#listingestiondestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIngestionDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIngestionDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIngestionDestinationsResponseTypeDef](./type_defs.md#listingestiondestinationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIngestionDestinationsRequestPaginateTypeDef = {  # (1)
    "appBundleIdentifier": ...,
    "ingestionIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngestionDestinationsRequestPaginateTypeDef](./type_defs.md#listingestiondestinationsrequestpaginatetypedef) 
## ListIngestionsPaginator

Type annotations and code completion for `#!python session.create_client("appfabric").get_paginator("list_ingestions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric/paginator/ListIngestions.html#AppFabric.Paginator.ListIngestions)

```python
# ListIngestionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appfabric.paginator import ListIngestionsPaginator

session = get_session()
async with session.create_client("appfabric") as client:  # (1)
    paginator: ListIngestionsPaginator = client.get_paginator("list_ingestions")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngestionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListIngestionsPaginator](./paginators.md#listingestionspaginator)
3. item: [:material-code-braces: ListIngestionsResponseTypeDef](./type_defs.md#listingestionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIngestionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appBundleIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIngestionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIngestionsResponseTypeDef](./type_defs.md#listingestionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIngestionsRequestPaginateTypeDef = {  # (1)
    "appBundleIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngestionsRequestPaginateTypeDef](./type_defs.md#listingestionsrequestpaginatetypedef) 
