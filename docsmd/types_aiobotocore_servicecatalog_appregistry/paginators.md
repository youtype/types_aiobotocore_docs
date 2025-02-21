# Paginators

> [Index](../README.md) > [AppRegistry](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#appregistry)
    type annotations stubs module [types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("servicecatalog-appregistry").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry/paginator/ListApplications.html#AppRegistry.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef) 
## ListAssociatedAttributeGroupsPaginator

Type annotations and code completion for `#!python session.create_client("servicecatalog-appregistry").get_paginator("list_associated_attribute_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry/paginator/ListAssociatedAttributeGroups.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)

```python
# ListAssociatedAttributeGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedAttributeGroupsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAssociatedAttributeGroupsPaginator = client.get_paginator("list_associated_attribute_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedAttributeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAssociatedAttributeGroupsPaginator](./paginators.md#listassociatedattributegroupspaginator)
3. item: [:material-code-braces: ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedAttributeGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    application: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociatedAttributeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedAttributeGroupsRequestPaginateTypeDef = {  # (1)
    "application": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedAttributeGroupsRequestPaginateTypeDef](./type_defs.md#listassociatedattributegroupsrequestpaginatetypedef) 
## ListAssociatedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("servicecatalog-appregistry").get_paginator("list_associated_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry/paginator/ListAssociatedResources.html#AppRegistry.Paginator.ListAssociatedResources)

```python
# ListAssociatedResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedResourcesPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAssociatedResourcesPaginator = client.get_paginator("list_associated_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAssociatedResourcesPaginator](./paginators.md#listassociatedresourcespaginator)
3. item: [:material-code-braces: ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    application: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociatedResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedResourcesRequestPaginateTypeDef = {  # (1)
    "application": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedResourcesRequestPaginateTypeDef](./type_defs.md#listassociatedresourcesrequestpaginatetypedef) 
## ListAttributeGroupsForApplicationPaginator

Type annotations and code completion for `#!python session.create_client("servicecatalog-appregistry").get_paginator("list_attribute_groups_for_application")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry/paginator/ListAttributeGroupsForApplication.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)

```python
# ListAttributeGroupsForApplicationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAttributeGroupsForApplicationPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAttributeGroupsForApplicationPaginator = client.get_paginator("list_attribute_groups_for_application")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttributeGroupsForApplicationResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAttributeGroupsForApplicationPaginator](./paginators.md#listattributegroupsforapplicationpaginator)
3. item: [:material-code-braces: ListAttributeGroupsForApplicationResponseTypeDef](./type_defs.md#listattributegroupsforapplicationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttributeGroupsForApplicationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    application: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAttributeGroupsForApplicationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttributeGroupsForApplicationResponseTypeDef](./type_defs.md#listattributegroupsforapplicationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttributeGroupsForApplicationRequestPaginateTypeDef = {  # (1)
    "application": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttributeGroupsForApplicationRequestPaginateTypeDef](./type_defs.md#listattributegroupsforapplicationrequestpaginatetypedef) 
## ListAttributeGroupsPaginator

Type annotations and code completion for `#!python session.create_client("servicecatalog-appregistry").get_paginator("list_attribute_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry/paginator/ListAttributeGroups.html#AppRegistry.Paginator.ListAttributeGroups)

```python
# ListAttributeGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAttributeGroupsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator: ListAttributeGroupsPaginator = client.get_paginator("list_attribute_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttributeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListAttributeGroupsPaginator](./paginators.md#listattributegroupspaginator)
3. item: [:material-code-braces: ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttributeGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAttributeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttributeGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttributeGroupsRequestPaginateTypeDef](./type_defs.md#listattributegroupsrequestpaginatetypedef) 
