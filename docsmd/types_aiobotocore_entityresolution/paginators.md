# Paginators

> [Index](../README.md) > [EntityResolution](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## ListIdMappingJobsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_mapping_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdMappingJobs)

```python
# ListIdMappingJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListIdMappingJobsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdMappingJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
3. item: [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIdMappingJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdMappingJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef = {  # (1)
    "workflowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef](./type_defs.md#listidmappingjobsinputlistidmappingjobspaginatetypedef) 
## ListIdMappingWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_mapping_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdMappingWorkflows)

```python
# ListIdMappingWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListIdMappingWorkflowsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListIdMappingWorkflowsPaginator = client.get_paginator("list_id_mapping_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdMappingWorkflowsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdMappingWorkflowsPaginator](./paginators.md#listidmappingworkflowspaginator)
3. item: [:material-code-braces: ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIdMappingWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdMappingWorkflowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef](./type_defs.md#listidmappingworkflowsinputlistidmappingworkflowspaginatetypedef) 
## ListIdNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListIdNamespaces)

```python
# ListIdNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListIdNamespacesPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListIdNamespacesPaginator = client.get_paginator("list_id_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdNamespacesOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdNamespacesPaginator](./paginators.md#listidnamespacespaginator)
3. item: [:material-code-braces: ListIdNamespacesOutputTypeDef](./type_defs.md#listidnamespacesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListIdNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdNamespacesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdNamespacesOutputTypeDef](./type_defs.md#listidnamespacesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdNamespacesInputListIdNamespacesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdNamespacesInputListIdNamespacesPaginateTypeDef](./type_defs.md#listidnamespacesinputlistidnamespacespaginatetypedef) 
## ListMatchingJobsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingJobs)

```python
# ListMatchingJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListMatchingJobsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListMatchingJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
3. item: [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMatchingJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMatchingJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingJobsInputListMatchingJobsPaginateTypeDef = {  # (1)
    "workflowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingJobsInputListMatchingJobsPaginateTypeDef](./type_defs.md#listmatchingjobsinputlistmatchingjobspaginatetypedef) 
## ListMatchingWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingWorkflows)

```python
# ListMatchingWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListMatchingWorkflowsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListMatchingWorkflowsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
3. item: [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMatchingWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMatchingWorkflowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputlistmatchingworkflowspaginatetypedef) 
## ListProviderServicesPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_provider_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListProviderServices)

```python
# ListProviderServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListProviderServicesPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListProviderServicesPaginator = client.get_paginator("list_provider_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListProviderServicesOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListProviderServicesPaginator](./paginators.md#listproviderservicespaginator)
3. item: [:material-code-braces: ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProviderServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    providerName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProviderServicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProviderServicesInputListProviderServicesPaginateTypeDef = {  # (1)
    "providerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProviderServicesInputListProviderServicesPaginateTypeDef](./type_defs.md#listproviderservicesinputlistproviderservicespaginatetypedef) 
## ListSchemaMappingsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_schema_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListSchemaMappings)

```python
# ListSchemaMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListSchemaMappingsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaMappingsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)
3. item: [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemaMappingsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef](./type_defs.md#listschemamappingsinputlistschemamappingspaginatetypedef) 
