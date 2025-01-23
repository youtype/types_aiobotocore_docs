# Paginators

> [Index](../README.md) > [EntityResolution](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## ListIdMappingJobsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_mapping_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListIdMappingJobs.html#EntityResolution.Paginator.ListIdMappingJobs)

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
) -> AioPageIterator[ListIdMappingJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdMappingJobsInputPaginateTypeDef = {  # (1)
    "workflowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdMappingJobsInputPaginateTypeDef](./type_defs.md#listidmappingjobsinputpaginatetypedef) 
## ListIdMappingWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_mapping_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListIdMappingWorkflows.html#EntityResolution.Paginator.ListIdMappingWorkflows)

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
) -> AioPageIterator[ListIdMappingWorkflowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdMappingWorkflowsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdMappingWorkflowsInputPaginateTypeDef](./type_defs.md#listidmappingworkflowsinputpaginatetypedef) 
## ListIdNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_id_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListIdNamespaces.html#EntityResolution.Paginator.ListIdNamespaces)

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
) -> AioPageIterator[ListIdNamespacesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdNamespacesOutputTypeDef](./type_defs.md#listidnamespacesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdNamespacesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdNamespacesInputPaginateTypeDef](./type_defs.md#listidnamespacesinputpaginatetypedef) 
## ListMatchingJobsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListMatchingJobs.html#EntityResolution.Paginator.ListMatchingJobs)

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
) -> AioPageIterator[ListMatchingJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingJobsInputPaginateTypeDef = {  # (1)
    "workflowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingJobsInputPaginateTypeDef](./type_defs.md#listmatchingjobsinputpaginatetypedef) 
## ListMatchingWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListMatchingWorkflows.html#EntityResolution.Paginator.ListMatchingWorkflows)

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
) -> AioPageIterator[ListMatchingWorkflowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingWorkflowsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingWorkflowsInputPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputpaginatetypedef) 
## ListProviderServicesPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_provider_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListProviderServices.html#EntityResolution.Paginator.ListProviderServices)

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
) -> AioPageIterator[ListProviderServicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProviderServicesInputPaginateTypeDef = {  # (1)
    "providerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProviderServicesInputPaginateTypeDef](./type_defs.md#listproviderservicesinputpaginatetypedef) 
## ListSchemaMappingsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_schema_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution/paginator/ListSchemaMappings.html#EntityResolution.Paginator.ListSchemaMappings)

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
) -> AioPageIterator[ListSchemaMappingsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaMappingsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaMappingsInputPaginateTypeDef](./type_defs.md#listschemamappingsinputpaginatetypedef) 
