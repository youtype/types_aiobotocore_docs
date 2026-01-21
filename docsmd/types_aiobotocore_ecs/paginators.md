# Paginators

> [Index](../README.md) > [ECS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## ListAccountSettingsPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_account_settings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListAccountSettings.html#ECS.Paginator.ListAccountSettings)

```python
# ListAccountSettingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountSettingsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
3. item: `AioPageIterator[ListAccountSettingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountSettingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: SettingNameType = ...,  # (1)
    value: str = ...,
    principalArn: str = ...,
    effectiveSettings: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAccountSettingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAccountSettingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountSettingsRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountSettingsRequestPaginateTypeDef](./type_defs.md#listaccountsettingsrequestpaginatetypedef)
## ListAttributesPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListAttributes.html#ECS.Paginator.ListAttributes)

```python
# ListAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListAttributesPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListAttributesPaginator = client.get_paginator("list_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListAttributesPaginator](./paginators.md#listattributespaginator)
3. item: `AioPageIterator[ListAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetType: TargetTypeType,  # (1)
    cluster: str = ...,
    attributeName: str = ...,
    attributeValue: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAttributesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAttributesRequestPaginateTypeDef = {  # (1)
    "targetType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttributesRequestPaginateTypeDef](./type_defs.md#listattributesrequestpaginatetypedef)
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListClusters.html#ECS.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: `AioPageIterator[ListClustersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClustersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
## ListContainerInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_container_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListContainerInstances.html#ECS.Paginator.ListContainerInstances)

```python
# ListContainerInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListContainerInstancesPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListContainerInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListContainerInstancesPaginator](./paginators.md#listcontainerinstancespaginator)
3. item: `AioPageIterator[ListContainerInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContainerInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cluster: str = ...,
    filter: str = ...,
    status: ContainerInstanceStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListContainerInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListContainerInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContainerInstancesRequestPaginateTypeDef = {  # (1)
    "cluster": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContainerInstancesRequestPaginateTypeDef](./type_defs.md#listcontainerinstancesrequestpaginatetypedef)
## ListServicesByNamespacePaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_services_by_namespace")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListServicesByNamespace.html#ECS.Paginator.ListServicesByNamespace)

```python
# ListServicesByNamespacePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListServicesByNamespacePaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListServicesByNamespacePaginator = client.get_paginator("list_services_by_namespace")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicesByNamespaceResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListServicesByNamespacePaginator](./paginators.md#listservicesbynamespacepaginator)
3. item: `AioPageIterator[ListServicesByNamespaceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServicesByNamespacePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListServicesByNamespaceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListServicesByNamespaceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServicesByNamespaceRequestPaginateTypeDef = {  # (1)
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicesByNamespaceRequestPaginateTypeDef](./type_defs.md#listservicesbynamespacerequestpaginatetypedef)
## ListServicesPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListServices.html#ECS.Paginator.ListServices)

```python
# ListServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListServicesPaginator = client.get_paginator("list_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListServicesPaginator](./paginators.md#listservicespaginator)
3. item: `AioPageIterator[ListServicesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cluster: str = ...,
    launchType: LaunchTypeType = ...,  # (1)
    schedulingStrategy: SchedulingStrategyType = ...,  # (2)
    resourceManagementType: ResourceManagementTypeType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListServicesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype)
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype)
3. See [:material-code-brackets: ResourceManagementTypeType](./literals.md#resourcemanagementtypetype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListServicesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServicesRequestPaginateTypeDef = {  # (1)
    "cluster": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestPaginateTypeDef](./type_defs.md#listservicesrequestpaginatetypedef)
## ListTaskDefinitionFamiliesPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_task_definition_families")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListTaskDefinitionFamilies.html#ECS.Paginator.ListTaskDefinitionFamilies)

```python
# ListTaskDefinitionFamiliesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTaskDefinitionFamiliesPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaskDefinitionFamiliesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListTaskDefinitionFamiliesPaginator](./paginators.md#listtaskdefinitionfamiliespaginator)
3. item: `AioPageIterator[ListTaskDefinitionFamiliesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTaskDefinitionFamiliesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    familyPrefix: str = ...,
    status: TaskDefinitionFamilyStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListTaskDefinitionFamiliesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTaskDefinitionFamiliesRequestPaginateTypeDef = {  # (1)
    "familyPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaskDefinitionFamiliesRequestPaginateTypeDef](./type_defs.md#listtaskdefinitionfamiliesrequestpaginatetypedef)
## ListTaskDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_task_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListTaskDefinitions.html#ECS.Paginator.ListTaskDefinitions)

```python
# ListTaskDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTaskDefinitionsPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaskDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListTaskDefinitionsPaginator](./paginators.md#listtaskdefinitionspaginator)
3. item: `AioPageIterator[ListTaskDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTaskDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    familyPrefix: str = ...,
    status: TaskDefinitionStatusType = ...,  # (1)
    sort: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListTaskDefinitionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype)
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListTaskDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTaskDefinitionsRequestPaginateTypeDef = {  # (1)
    "familyPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaskDefinitionsRequestPaginateTypeDef](./type_defs.md#listtaskdefinitionsrequestpaginatetypedef)
## ListTasksPaginator

Type annotations and code completion for `#!python session.create_client("ecs").get_paginator("list_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/paginator/ListTasks.html#ECS.Paginator.ListTasks)

```python
# ListTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTasksPaginator

session = get_session()
async with session.create_client("ecs") as client:  # (1)
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [ECSClient](./client.md)
2. paginator: [ListTasksPaginator](./paginators.md#listtaskspaginator)
3. item: `AioPageIterator[ListTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cluster: str = ...,
    containerInstance: str = ...,
    family: str = ...,
    startedBy: str = ...,
    serviceName: str = ...,
    desiredStatus: DesiredStatusType = ...,  # (1)
    launchType: LaunchTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListTasksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DesiredStatusType](./literals.md#desiredstatustype)
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTasksRequestPaginateTypeDef = {  # (1)
    "cluster": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestPaginateTypeDef](./type_defs.md#listtasksrequestpaginatetypedef)
