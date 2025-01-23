# Paginators

> [Index](../README.md) > [MigrationHubRefactorSpaces](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#migrationhubrefactorspaces)
    type annotations stubs module [types-aiobotocore-migration-hub-refactor-spaces](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("migration-hub-refactor-spaces").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces/paginator/ListApplications.html#MigrationHubRefactorSpaces.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestPaginateTypeDef = {  # (1)
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef) 
## ListEnvironmentVpcsPaginator

Type annotations and code completion for `#!python session.create_client("migration-hub-refactor-spaces").get_paginator("list_environment_vpcs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces/paginator/ListEnvironmentVpcs.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)

```python
# ListEnvironmentVpcsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentVpcsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListEnvironmentVpcsPaginator = client.get_paginator("list_environment_vpcs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentVpcsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListEnvironmentVpcsPaginator](./paginators.md#listenvironmentvpcspaginator)
3. item: [:material-code-braces: ListEnvironmentVpcsResponseTypeDef](./type_defs.md#listenvironmentvpcsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentVpcsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEnvironmentVpcsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentVpcsResponseTypeDef](./type_defs.md#listenvironmentvpcsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentVpcsRequestPaginateTypeDef = {  # (1)
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentVpcsRequestPaginateTypeDef](./type_defs.md#listenvironmentvpcsrequestpaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("migration-hub-refactor-spaces").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces/paginator/ListEnvironments.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef) 
## ListRoutesPaginator

Type annotations and code completion for `#!python session.create_client("migration-hub-refactor-spaces").get_paginator("list_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces/paginator/ListRoutes.html#MigrationHubRefactorSpaces.Paginator.ListRoutes)

```python
# ListRoutesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListRoutesPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListRoutesPaginator = client.get_paginator("list_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutesResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListRoutesPaginator](./paginators.md#listroutespaginator)
3. item: [:material-code-braces: ListRoutesResponseTypeDef](./type_defs.md#listroutesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRoutesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutesResponseTypeDef](./type_defs.md#listroutesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutesRequestPaginateTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutesRequestPaginateTypeDef](./type_defs.md#listroutesrequestpaginatetypedef) 
## ListServicesPaginator

Type annotations and code completion for `#!python session.create_client("migration-hub-refactor-spaces").get_paginator("list_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces/paginator/ListServices.html#MigrationHubRefactorSpaces.Paginator.ListServices)

```python
# ListServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator: ListServicesPaginator = client.get_paginator("list_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicesResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListServicesPaginator](./paginators.md#listservicespaginator)
3. item: [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListServicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListServicesRequestPaginateTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestPaginateTypeDef](./type_defs.md#listservicesrequestpaginatetypedef) 
