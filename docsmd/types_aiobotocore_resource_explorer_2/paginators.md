# Paginators

> [Index](../README.md) > [ResourceExplorer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## GetResourceExplorerSetupPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("get_resource_explorer_setup")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/GetResourceExplorerSetup.html#ResourceExplorer.Paginator.GetResourceExplorerSetup)

```python
# GetResourceExplorerSetupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import GetResourceExplorerSetupPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: GetResourceExplorerSetupPaginator = client.get_paginator("get_resource_explorer_setup")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceExplorerSetupOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [GetResourceExplorerSetupPaginator](./paginators.md#getresourceexplorersetuppaginator)
3. item: `AioPageIterator[GetResourceExplorerSetupOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetResourceExplorerSetupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TaskId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetResourceExplorerSetupOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetResourceExplorerSetupOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetResourceExplorerSetupInputPaginateTypeDef = {  # (1)
    "TaskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceExplorerSetupInputPaginateTypeDef](./type_defs.md#getresourceexplorersetupinputpaginatetypedef)
## ListIndexesForMembersPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_indexes_for_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListIndexesForMembers.html#ResourceExplorer.Paginator.ListIndexesForMembers)

```python
# ListIndexesForMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesForMembersPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesForMembersPaginator = client.get_paginator("list_indexes_for_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesForMembersOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
3. item: `AioPageIterator[ListIndexesForMembersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIndexesForMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountIdList: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIndexesForMembersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIndexesForMembersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesForMembersInputPaginateTypeDef = {  # (1)
    "AccountIdList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesForMembersInputPaginateTypeDef](./type_defs.md#listindexesformembersinputpaginatetypedef)
## ListIndexesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListIndexes.html#ResourceExplorer.Paginator.ListIndexes)

```python
# ListIndexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesPaginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: `AioPageIterator[ListIndexesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIndexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Type: IndexTypeType = ...,  # (1)
    Regions: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListIndexesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListIndexesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesInputPaginateTypeDef = {  # (1)
    "Type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesInputPaginateTypeDef](./type_defs.md#listindexesinputpaginatetypedef)
## ListManagedViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_managed_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListManagedViews.html#ResourceExplorer.Paginator.ListManagedViews)

```python
# ListManagedViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListManagedViewsPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListManagedViewsPaginator = client.get_paginator("list_managed_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListManagedViewsPaginator](./paginators.md#listmanagedviewspaginator)
3. item: `AioPageIterator[ListManagedViewsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServicePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedViewsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedViewsInputPaginateTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedViewsInputPaginateTypeDef](./type_defs.md#listmanagedviewsinputpaginatetypedef)
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListResources.html#ResourceExplorer.Paginator.ListResources)

```python
# ListResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: `AioPageIterator[ListResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: SearchFilterTypeDef = ...,  # (1)
    ViewArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcesInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesInputPaginateTypeDef](./type_defs.md#listresourcesinputpaginatetypedef)
## ListServiceIndexesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_service_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListServiceIndexes.html#ResourceExplorer.Paginator.ListServiceIndexes)

```python
# ListServiceIndexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListServiceIndexesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListServiceIndexesPaginator = client.get_paginator("list_service_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListServiceIndexesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListServiceIndexesPaginator](./paginators.md#listserviceindexespaginator)
3. item: `AioPageIterator[ListServiceIndexesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServiceIndexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Regions: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListServiceIndexesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListServiceIndexesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServiceIndexesInputPaginateTypeDef = {  # (1)
    "Regions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServiceIndexesInputPaginateTypeDef](./type_defs.md#listserviceindexesinputpaginatetypedef)
## ListServiceViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_service_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListServiceViews.html#ResourceExplorer.Paginator.ListServiceViews)

```python
# ListServiceViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListServiceViewsPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListServiceViewsPaginator = client.get_paginator("list_service_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListServiceViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListServiceViewsPaginator](./paginators.md#listserviceviewspaginator)
3. item: `AioPageIterator[ListServiceViewsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServiceViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListServiceViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListServiceViewsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServiceViewsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServiceViewsInputPaginateTypeDef](./type_defs.md#listserviceviewsinputpaginatetypedef)
## ListStreamingAccessForServicesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_streaming_access_for_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListStreamingAccessForServices.html#ResourceExplorer.Paginator.ListStreamingAccessForServices)

```python
# ListStreamingAccessForServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListStreamingAccessForServicesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListStreamingAccessForServicesPaginator = client.get_paginator("list_streaming_access_for_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamingAccessForServicesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListStreamingAccessForServicesPaginator](./paginators.md#liststreamingaccessforservicespaginator)
3. item: `AioPageIterator[ListStreamingAccessForServicesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamingAccessForServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamingAccessForServicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamingAccessForServicesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamingAccessForServicesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamingAccessForServicesInputPaginateTypeDef](./type_defs.md#liststreamingaccessforservicesinputpaginatetypedef)
## ListSupportedResourceTypesPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_supported_resource_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListSupportedResourceTypes.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)

```python
# ListSupportedResourceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListSupportedResourceTypesPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListSupportedResourceTypesPaginator = client.get_paginator("list_supported_resource_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListSupportedResourceTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListSupportedResourceTypesPaginator](./paginators.md#listsupportedresourcetypespaginator)
3. item: `AioPageIterator[ListSupportedResourceTypesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSupportedResourceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSupportedResourceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSupportedResourceTypesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSupportedResourceTypesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSupportedResourceTypesInputPaginateTypeDef](./type_defs.md#listsupportedresourcetypesinputpaginatetypedef)
## ListViewsPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("list_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/ListViews.html#ResourceExplorer.Paginator.ListViews)

```python
# ListViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import ListViewsPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: ListViewsPaginator = client.get_paginator("list_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListViewsPaginator](./paginators.md#listviewspaginator)
3. item: `AioPageIterator[ListViewsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListViewsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListViewsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViewsInputPaginateTypeDef](./type_defs.md#listviewsinputpaginatetypedef)
## SearchPaginator

Type annotations and code completion for `#!python session.create_client("resource-explorer-2").get_paginator("search")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2/paginator/Search.html#ResourceExplorer.Paginator.Search)

```python
# SearchPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.paginator import SearchPaginator

session = get_session()
async with session.create_client("resource-explorer-2") as client:  # (1)
    paginator: SearchPaginator = client.get_paginator("search")  # (2)
    async for item in paginator.paginate(...):
        item: SearchOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [SearchPaginator](./paginators.md#searchpaginator)
3. item: `AioPageIterator[SearchOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QueryString: str,
    ViewArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[SearchOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[SearchOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchInputPaginateTypeDef = {  # (1)
    "QueryString": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchInputPaginateTypeDef](./type_defs.md#searchinputpaginatetypedef)
