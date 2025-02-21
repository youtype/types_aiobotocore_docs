# Paginators

> [Index](../README.md) > [AppSync](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#appsync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## ListApiKeysPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_api_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListApiKeys.html#AppSync.Paginator.ListApiKeys)

```python
# ListApiKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListApiKeysPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListApiKeysPaginator = client.get_paginator("list_api_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListApiKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
3. item: [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApiKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApiKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApiKeysRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApiKeysRequestPaginateTypeDef](./type_defs.md#listapikeysrequestpaginatetypedef) 
## ListApisPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListApis.html#AppSync.Paginator.ListApis)

```python
# ListApisPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListApisPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListApisPaginator = client.get_paginator("list_apis")  # (2)
    async for item in paginator.paginate(...):
        item: ListApisResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListApisPaginator](./paginators.md#listapispaginator)
3. item: [:material-code-braces: ListApisResponseTypeDef](./type_defs.md#listapisresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApisPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApisResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApisResponseTypeDef](./type_defs.md#listapisresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApisRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApisRequestPaginateTypeDef](./type_defs.md#listapisrequestpaginatetypedef) 
## ListChannelNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_channel_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListChannelNamespaces.html#AppSync.Paginator.ListChannelNamespaces)

```python
# ListChannelNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListChannelNamespacesPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListChannelNamespacesPaginator = client.get_paginator("list_channel_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListChannelNamespacesPaginator](./paginators.md#listchannelnamespacespaginator)
3. item: [:material-code-braces: ListChannelNamespacesResponseTypeDef](./type_defs.md#listchannelnamespacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChannelNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelNamespacesResponseTypeDef](./type_defs.md#listchannelnamespacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelNamespacesRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelNamespacesRequestPaginateTypeDef](./type_defs.md#listchannelnamespacesrequestpaginatetypedef) 
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListDataSources.html#AppSync.Paginator.ListDataSources)

```python
# ListDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListDataSourcesPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
3. item: [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourcesRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef) 
## ListDomainNamesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_domain_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListDomainNames.html#AppSync.Paginator.ListDomainNames)

```python
# ListDomainNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListDomainNamesPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListDomainNamesPaginator = client.get_paginator("list_domain_names")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainNamesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListDomainNamesPaginator](./paginators.md#listdomainnamespaginator)
3. item: [:material-code-braces: ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDomainNamesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainNamesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainNamesRequestPaginateTypeDef](./type_defs.md#listdomainnamesrequestpaginatetypedef) 
## ListFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListFunctions.html#AppSync.Paginator.ListFunctions)

```python
# ListFunctionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListFunctionsPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListFunctionsPaginator = client.get_paginator("list_functions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFunctionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
3. item: [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFunctionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFunctionsRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestPaginateTypeDef](./type_defs.md#listfunctionsrequestpaginatetypedef) 
## ListGraphqlApisPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_graphql_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListGraphqlApis.html#AppSync.Paginator.ListGraphqlApis)

```python
# ListGraphqlApisPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListGraphqlApisPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListGraphqlApisPaginator = client.get_paginator("list_graphql_apis")  # (2)
    async for item in paginator.paginate(...):
        item: ListGraphqlApisResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListGraphqlApisPaginator](./paginators.md#listgraphqlapispaginator)
3. item: [:material-code-braces: ListGraphqlApisResponseTypeDef](./type_defs.md#listgraphqlapisresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGraphqlApisPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiType: GraphQLApiTypeType = ...,  # (1)
    owner: OwnershipType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListGraphqlApisResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: GraphQLApiTypeType](./literals.md#graphqlapitypetype) 
2. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListGraphqlApisResponseTypeDef](./type_defs.md#listgraphqlapisresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGraphqlApisRequestPaginateTypeDef = {  # (1)
    "apiType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGraphqlApisRequestPaginateTypeDef](./type_defs.md#listgraphqlapisrequestpaginatetypedef) 
## ListResolversByFunctionPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_resolvers_by_function")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListResolversByFunction.html#AppSync.Paginator.ListResolversByFunction)

```python
# ListResolversByFunctionPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListResolversByFunctionPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListResolversByFunctionPaginator = client.get_paginator("list_resolvers_by_function")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolversByFunctionResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListResolversByFunctionPaginator](./paginators.md#listresolversbyfunctionpaginator)
3. item: [:material-code-braces: ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolversByFunctionPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    functionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResolversByFunctionResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolversByFunctionRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
    "functionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolversByFunctionRequestPaginateTypeDef](./type_defs.md#listresolversbyfunctionrequestpaginatetypedef) 
## ListResolversPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_resolvers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListResolvers.html#AppSync.Paginator.ListResolvers)

```python
# ListResolversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListResolversPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListResolversPaginator = client.get_paginator("list_resolvers")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolversResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListResolversPaginator](./paginators.md#listresolverspaginator)
3. item: [:material-code-braces: ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    typeName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResolversResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolversRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolversRequestPaginateTypeDef](./type_defs.md#listresolversrequestpaginatetypedef) 
## ListSourceApiAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_source_api_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListSourceApiAssociations.html#AppSync.Paginator.ListSourceApiAssociations)

```python
# ListSourceApiAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListSourceApiAssociationsPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListSourceApiAssociationsPaginator = client.get_paginator("list_source_api_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceApiAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListSourceApiAssociationsPaginator](./paginators.md#listsourceapiassociationspaginator)
3. item: [:material-code-braces: ListSourceApiAssociationsResponseTypeDef](./type_defs.md#listsourceapiassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSourceApiAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSourceApiAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSourceApiAssociationsResponseTypeDef](./type_defs.md#listsourceapiassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceApiAssociationsRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceApiAssociationsRequestPaginateTypeDef](./type_defs.md#listsourceapiassociationsrequestpaginatetypedef) 
## ListTypesByAssociationPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_types_by_association")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListTypesByAssociation.html#AppSync.Paginator.ListTypesByAssociation)

```python
# ListTypesByAssociationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListTypesByAssociationPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListTypesByAssociationPaginator = client.get_paginator("list_types_by_association")  # (2)
    async for item in paginator.paginate(...):
        item: ListTypesByAssociationResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListTypesByAssociationPaginator](./paginators.md#listtypesbyassociationpaginator)
3. item: [:material-code-braces: ListTypesByAssociationResponseTypeDef](./type_defs.md#listtypesbyassociationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTypesByAssociationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    mergedApiIdentifier: str,
    associationId: str,
    format: TypeDefinitionFormatType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTypesByAssociationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTypesByAssociationResponseTypeDef](./type_defs.md#listtypesbyassociationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTypesByAssociationRequestPaginateTypeDef = {  # (1)
    "mergedApiIdentifier": ...,
    "associationId": ...,
    "format": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypesByAssociationRequestPaginateTypeDef](./type_defs.md#listtypesbyassociationrequestpaginatetypedef) 
## ListTypesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync/paginator/ListTypes.html#AppSync.Paginator.ListTypes)

```python
# ListTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListTypesPaginator

session = get_session()
async with session.create_client("appsync") as client:  # (1)
    paginator: ListTypesPaginator = client.get_paginator("list_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListTypesPaginator](./paginators.md#listtypespaginator)
3. item: [:material-code-braces: ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    apiId: str,
    format: TypeDefinitionFormatType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTypesRequestPaginateTypeDef = {  # (1)
    "apiId": ...,
    "format": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypesRequestPaginateTypeDef](./type_defs.md#listtypesrequestpaginatetypedef) 
