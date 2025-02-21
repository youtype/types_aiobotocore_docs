# Paginators

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## ListApplicationAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_application_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListApplicationAssociations.html#AppIntegrationsService.Paginator.ListApplicationAssociations)

```python
# ListApplicationAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListApplicationAssociationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListApplicationAssociationsPaginator = client.get_paginator("list_application_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
3. item: [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApplicationAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationAssociationsRequestPaginateTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationAssociationsRequestPaginateTypeDef](./type_defs.md#listapplicationassociationsrequestpaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListApplications.html#AppIntegrationsService.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
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
## ListDataIntegrationAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_data_integration_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListDataIntegrationAssociations.html#AppIntegrationsService.Paginator.ListDataIntegrationAssociations)

```python
# ListDataIntegrationAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListDataIntegrationAssociationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListDataIntegrationAssociationsPaginator = client.get_paginator("list_data_integration_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataIntegrationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListDataIntegrationAssociationsPaginator](./paginators.md#listdataintegrationassociationspaginator)
3. item: [:material-code-braces: ListDataIntegrationAssociationsResponseTypeDef](./type_defs.md#listdataintegrationassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataIntegrationAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataIntegrationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataIntegrationAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataIntegrationAssociationsResponseTypeDef](./type_defs.md#listdataintegrationassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataIntegrationAssociationsRequestPaginateTypeDef = {  # (1)
    "DataIntegrationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationAssociationsRequestPaginateTypeDef](./type_defs.md#listdataintegrationassociationsrequestpaginatetypedef) 
## ListDataIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_data_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListDataIntegrations.html#AppIntegrationsService.Paginator.ListDataIntegrations)

```python
# ListDataIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListDataIntegrationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListDataIntegrationsPaginator = client.get_paginator("list_data_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataIntegrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListDataIntegrationsPaginator](./paginators.md#listdataintegrationspaginator)
3. item: [:material-code-braces: ListDataIntegrationsResponseTypeDef](./type_defs.md#listdataintegrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataIntegrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataIntegrationsResponseTypeDef](./type_defs.md#listdataintegrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataIntegrationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationsRequestPaginateTypeDef](./type_defs.md#listdataintegrationsrequestpaginatetypedef) 
## ListEventIntegrationAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_event_integration_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListEventIntegrationAssociations.html#AppIntegrationsService.Paginator.ListEventIntegrationAssociations)

```python
# ListEventIntegrationAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListEventIntegrationAssociationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListEventIntegrationAssociationsPaginator = client.get_paginator("list_event_integration_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventIntegrationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListEventIntegrationAssociationsPaginator](./paginators.md#listeventintegrationassociationspaginator)
3. item: [:material-code-braces: ListEventIntegrationAssociationsResponseTypeDef](./type_defs.md#listeventintegrationassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventIntegrationAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EventIntegrationName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventIntegrationAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventIntegrationAssociationsResponseTypeDef](./type_defs.md#listeventintegrationassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventIntegrationAssociationsRequestPaginateTypeDef = {  # (1)
    "EventIntegrationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventIntegrationAssociationsRequestPaginateTypeDef](./type_defs.md#listeventintegrationassociationsrequestpaginatetypedef) 
## ListEventIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("appintegrations").get_paginator("list_event_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations/paginator/ListEventIntegrations.html#AppIntegrationsService.Paginator.ListEventIntegrations)

```python
# ListEventIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.paginator import ListEventIntegrationsPaginator

session = get_session()
async with session.create_client("appintegrations") as client:  # (1)
    paginator: ListEventIntegrationsPaginator = client.get_paginator("list_event_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventIntegrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListEventIntegrationsPaginator](./paginators.md#listeventintegrationspaginator)
3. item: [:material-code-braces: ListEventIntegrationsResponseTypeDef](./type_defs.md#listeventintegrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventIntegrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventIntegrationsResponseTypeDef](./type_defs.md#listeventintegrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventIntegrationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventIntegrationsRequestPaginateTypeDef](./type_defs.md#listeventintegrationsrequestpaginatetypedef) 
