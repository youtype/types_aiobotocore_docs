<a id="paginators-for-aiobotocore-ecs-module"></a>

# Paginators for aiobotocore ECS module

> [Index](../README.md) > [ECS](./README.md) > Paginators

Auto-generated documentation for
[ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
type annotations stubs module
[types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

- [Paginators for aiobotocore ECS module](#paginators-for-aiobotocore-ecs-module)
  - [ListAccountSettingsPaginator](#listaccountsettingspaginator)
  - [ListAttributesPaginator](#listattributespaginator)
  - [ListClustersPaginator](#listclusterspaginator)
  - [ListContainerInstancesPaginator](#listcontainerinstancespaginator)
  - [ListServicesPaginator](#listservicespaginator)
  - [ListTaskDefinitionFamiliesPaginator](#listtaskdefinitionfamiliespaginator)
  - [ListTaskDefinitionsPaginator](#listtaskdefinitionspaginator)
  - [ListTasksPaginator](#listtaskspaginator)

<a id="listaccountsettingspaginator"></a>

## ListAccountSettingsPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_account_settings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
```

Boto3 documentation:
[ECS.Paginator.ListAccountSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)

Arguments for `ListAccountSettingsPaginator.paginate` method:

- `name`: [SettingNameType](./literals.md#settingnametype)
- `value`: `str`
- `principalArn`: `str`
- `effectiveSettings`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountSettingsPaginator.paginate` returns
`AsyncIterator`\[[ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef)\].

<a id="listattributespaginator"></a>

## ListAttributesPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListAttributesPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
```

Boto3 documentation:
[ECS.Paginator.ListAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)

Arguments for `ListAttributesPaginator.paginate` method:

- `targetType`: `Literal['container-instance']` (see
  [TargetTypeType](./literals.md#targettypetype)) *(required)*
- `cluster`: `str`
- `attributeName`: `str`
- `attributeValue`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttributesPaginator.paginate` returns
`AsyncIterator`\[[ListAttributesResponseTypeDef](./type_defs.md#listattributesresponsetypedef)\].

<a id="listclusterspaginator"></a>

## ListClustersPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")
```

Boto3 documentation:
[ECS.Paginator.ListClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)

Arguments for `ListClustersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClustersPaginator.paginate` returns
`AsyncIterator`\[[ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)\].

<a id="listcontainerinstancespaginator"></a>

## ListContainerInstancesPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_container_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListContainerInstancesPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")
```

Boto3 documentation:
[ECS.Paginator.ListContainerInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)

Arguments for `ListContainerInstancesPaginator.paginate` method:

- `cluster`: `str`
- `filter`: `str`
- `status`:
  [ContainerInstanceStatusType](./literals.md#containerinstancestatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContainerInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListContainerInstancesResponseTypeDef](./type_defs.md#listcontainerinstancesresponsetypedef)\].

<a id="listservicespaginator"></a>

## ListServicesPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_services")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListServicesPaginator = client.get_paginator("list_services")
```

Boto3 documentation:
[ECS.Paginator.ListServices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)

Arguments for `ListServicesPaginator.paginate` method:

- `cluster`: `str`
- `launchType`: [LaunchTypeType](./literals.md#launchtypetype)
- `schedulingStrategy`:
  [SchedulingStrategyType](./literals.md#schedulingstrategytype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServicesPaginator.paginate` returns
`AsyncIterator`\[[ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)\].

<a id="listtaskdefinitionfamiliespaginator"></a>

## ListTaskDefinitionFamiliesPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_task_definition_families")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTaskDefinitionFamiliesPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")
```

Boto3 documentation:
[ECS.Paginator.ListTaskDefinitionFamilies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)

Arguments for `ListTaskDefinitionFamiliesPaginator.paginate` method:

- `familyPrefix`: `str`
- `status`:
  [TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTaskDefinitionFamiliesPaginator.paginate` returns
`AsyncIterator`\[[ListTaskDefinitionFamiliesResponseTypeDef](./type_defs.md#listtaskdefinitionfamiliesresponsetypedef)\].

<a id="listtaskdefinitionspaginator"></a>

## ListTaskDefinitionsPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_task_definitions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTaskDefinitionsPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")
```

Boto3 documentation:
[ECS.Paginator.ListTaskDefinitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)

Arguments for `ListTaskDefinitionsPaginator.paginate` method:

- `familyPrefix`: `str`
- `status`: [TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype)
- `sort`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTaskDefinitionsPaginator.paginate` returns
`AsyncIterator`\[[ListTaskDefinitionsResponseTypeDef](./type_defs.md#listtaskdefinitionsresponsetypedef)\].

<a id="listtaskspaginator"></a>

## ListTasksPaginator

Type annotations for
`session.create_client("ecs").get_paginator("list_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.paginator import ListTasksPaginator

session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")
```

Boto3 documentation:
[ECS.Paginator.ListTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)

Arguments for `ListTasksPaginator.paginate` method:

- `cluster`: `str`
- `containerInstance`: `str`
- `family`: `str`
- `startedBy`: `str`
- `serviceName`: `str`
- `desiredStatus`: [DesiredStatusType](./literals.md#desiredstatustype)
- `launchType`: [LaunchTypeType](./literals.md#launchtypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTasksPaginator.paginate` returns
`AsyncIterator`\[[ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef)\].
