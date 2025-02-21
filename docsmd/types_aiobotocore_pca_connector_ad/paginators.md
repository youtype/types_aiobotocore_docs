# Paginators

> [Index](../README.md) > [PcaConnectorAd](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad)
    type annotations stubs module [types-aiobotocore-pca-connector-ad](https://pypi.org/project/types-aiobotocore-pca-connector-ad/).

## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/paginator/ListConnectors.html#PcaConnectorAd.Paginator.ListConnectors)

```python
# ListConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef) 
## ListDirectoryRegistrationsPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator("list_directory_registrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/paginator/ListDirectoryRegistrations.html#PcaConnectorAd.Paginator.ListDirectoryRegistrations)

```python
# ListDirectoryRegistrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.paginator import ListDirectoryRegistrationsPaginator

session = get_session()
async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator: ListDirectoryRegistrationsPaginator = client.get_paginator("list_directory_registrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDirectoryRegistrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListDirectoryRegistrationsPaginator](./paginators.md#listdirectoryregistrationspaginator)
3. item: [:material-code-braces: ListDirectoryRegistrationsResponseTypeDef](./type_defs.md#listdirectoryregistrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDirectoryRegistrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDirectoryRegistrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDirectoryRegistrationsResponseTypeDef](./type_defs.md#listdirectoryregistrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDirectoryRegistrationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDirectoryRegistrationsRequestPaginateTypeDef](./type_defs.md#listdirectoryregistrationsrequestpaginatetypedef) 
## ListServicePrincipalNamesPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator("list_service_principal_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/paginator/ListServicePrincipalNames.html#PcaConnectorAd.Paginator.ListServicePrincipalNames)

```python
# ListServicePrincipalNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.paginator import ListServicePrincipalNamesPaginator

session = get_session()
async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator: ListServicePrincipalNamesPaginator = client.get_paginator("list_service_principal_names")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicePrincipalNamesResponseTypeDef
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListServicePrincipalNamesPaginator](./paginators.md#listserviceprincipalnamespaginator)
3. item: [:material-code-braces: ListServicePrincipalNamesResponseTypeDef](./type_defs.md#listserviceprincipalnamesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServicePrincipalNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryRegistrationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListServicePrincipalNamesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServicePrincipalNamesResponseTypeDef](./type_defs.md#listserviceprincipalnamesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListServicePrincipalNamesRequestPaginateTypeDef = {  # (1)
    "DirectoryRegistrationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicePrincipalNamesRequestPaginateTypeDef](./type_defs.md#listserviceprincipalnamesrequestpaginatetypedef) 
## ListTemplateGroupAccessControlEntriesPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator("list_template_group_access_control_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/paginator/ListTemplateGroupAccessControlEntries.html#PcaConnectorAd.Paginator.ListTemplateGroupAccessControlEntries)

```python
# ListTemplateGroupAccessControlEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.paginator import ListTemplateGroupAccessControlEntriesPaginator

session = get_session()
async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator: ListTemplateGroupAccessControlEntriesPaginator = client.get_paginator("list_template_group_access_control_entries")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateGroupAccessControlEntriesResponseTypeDef
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListTemplateGroupAccessControlEntriesPaginator](./paginators.md#listtemplategroupaccesscontrolentriespaginator)
3. item: [:material-code-braces: ListTemplateGroupAccessControlEntriesResponseTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplateGroupAccessControlEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TemplateArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTemplateGroupAccessControlEntriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTemplateGroupAccessControlEntriesResponseTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateGroupAccessControlEntriesRequestPaginateTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesrequestpaginatetypedef) 
## ListTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator("list_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/paginator/ListTemplates.html#PcaConnectorAd.Paginator.ListTemplates)

```python
# ListTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.paginator import ListTemplatesPaginator

session = get_session()
async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator: ListTemplatesPaginator = client.get_paginator("list_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
3. item: [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplatesRequestPaginateTypeDef = {  # (1)
    "ConnectorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestPaginateTypeDef](./type_defs.md#listtemplatesrequestpaginatetypedef) 
