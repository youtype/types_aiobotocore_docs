# Paginators

> [Index](../README.md) > [EMR](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## ListBootstrapActionsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_bootstrap_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListBootstrapActions.html#EMR.Paginator.ListBootstrapActions)

```python
# ListBootstrapActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListBootstrapActionsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListBootstrapActionsPaginator = client.get_paginator("list_bootstrap_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListBootstrapActionsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListBootstrapActionsPaginator](./paginators.md#listbootstrapactionspaginator)
3. item: [:material-code-braces: ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBootstrapActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBootstrapActionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBootstrapActionsInputPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBootstrapActionsInputPaginateTypeDef](./type_defs.md#listbootstrapactionsinputpaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListClusters.html#EMR.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    ClusterStates: Sequence[ClusterStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListClustersOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersInputPaginateTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersInputPaginateTypeDef](./type_defs.md#listclustersinputpaginatetypedef) 
## ListInstanceFleetsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_instance_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListInstanceFleets.html#EMR.Paginator.ListInstanceFleets)

```python
# ListInstanceFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListInstanceFleetsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListInstanceFleetsPaginator = client.get_paginator("list_instance_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceFleetsOutputPaginatorTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstanceFleetsPaginator](./paginators.md#listinstancefleetspaginator)
3. item: [:material-code-braces: ListInstanceFleetsOutputPaginatorTypeDef](./type_defs.md#listinstancefleetsoutputpaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInstanceFleetsOutputPaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceFleetsOutputPaginatorTypeDef](./type_defs.md#listinstancefleetsoutputpaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceFleetsInputPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceFleetsInputPaginateTypeDef](./type_defs.md#listinstancefleetsinputpaginatetypedef) 
## ListInstanceGroupsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_instance_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListInstanceGroups.html#EMR.Paginator.ListInstanceGroups)

```python
# ListInstanceGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListInstanceGroupsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListInstanceGroupsPaginator = client.get_paginator("list_instance_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceGroupsOutputPaginatorTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstanceGroupsPaginator](./paginators.md#listinstancegroupspaginator)
3. item: [:material-code-braces: ListInstanceGroupsOutputPaginatorTypeDef](./type_defs.md#listinstancegroupsoutputpaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInstanceGroupsOutputPaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceGroupsOutputPaginatorTypeDef](./type_defs.md#listinstancegroupsoutputpaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceGroupsInputPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceGroupsInputPaginateTypeDef](./type_defs.md#listinstancegroupsinputpaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListInstances.html#EMR.Paginator.ListInstances)

```python
# ListInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    InstanceGroupId: str = ...,
    InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,  # (1)
    InstanceFleetId: str = ...,
    InstanceFleetType: InstanceFleetTypeType = ...,  # (2)
    InstanceStates: Sequence[InstanceStateType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListInstancesOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesInputPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesInputPaginateTypeDef](./type_defs.md#listinstancesinputpaginatetypedef) 
## ListNotebookExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_notebook_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListNotebookExecutions.html#EMR.Paginator.ListNotebookExecutions)

```python
# ListNotebookExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListNotebookExecutionsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListNotebookExecutionsPaginator = client.get_paginator("list_notebook_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotebookExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListNotebookExecutionsPaginator](./paginators.md#listnotebookexecutionspaginator)
3. item: [:material-code-braces: ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListNotebookExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EditorId: str = ...,
    Status: NotebookExecutionStatusType = ...,  # (1)
    From: TimestampTypeDef = ...,
    To: TimestampTypeDef = ...,
    ExecutionEngineId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListNotebookExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNotebookExecutionsInputPaginateTypeDef = {  # (1)
    "EditorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotebookExecutionsInputPaginateTypeDef](./type_defs.md#listnotebookexecutionsinputpaginatetypedef) 
## ListSecurityConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_security_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListSecurityConfigurations.html#EMR.Paginator.ListSecurityConfigurations)

```python
# ListSecurityConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListSecurityConfigurationsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
3. item: [:material-code-braces: ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSecurityConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityConfigurationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityConfigurationsInputPaginateTypeDef](./type_defs.md#listsecurityconfigurationsinputpaginatetypedef) 
## ListStepsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListSteps.html#EMR.Paginator.ListSteps)

```python
# ListStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListStepsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListStepsPaginator = client.get_paginator("list_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListStepsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStepsPaginator](./paginators.md#liststepspaginator)
3. item: [:material-code-braces: ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    StepStates: Sequence[StepStateType] = ...,  # (1)
    StepIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListStepsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStepsInputPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStepsInputPaginateTypeDef](./type_defs.md#liststepsinputpaginatetypedef) 
## ListStudioSessionMappingsPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_studio_session_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListStudioSessionMappings.html#EMR.Paginator.ListStudioSessionMappings)

```python
# ListStudioSessionMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListStudioSessionMappingsPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListStudioSessionMappingsPaginator = client.get_paginator("list_studio_session_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudioSessionMappingsOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStudioSessionMappingsPaginator](./paginators.md#liststudiosessionmappingspaginator)
3. item: [:material-code-braces: ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStudioSessionMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StudioId: str = ...,
    IdentityType: IdentityTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListStudioSessionMappingsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStudioSessionMappingsInputPaginateTypeDef = {  # (1)
    "StudioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudioSessionMappingsInputPaginateTypeDef](./type_defs.md#liststudiosessionmappingsinputpaginatetypedef) 
## ListStudiosPaginator

Type annotations and code completion for `#!python session.create_client("emr").get_paginator("list_studios")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr/paginator/ListStudios.html#EMR.Paginator.ListStudios)

```python
# ListStudiosPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.paginator import ListStudiosPaginator

session = get_session()
async with session.create_client("emr") as client:  # (1)
    paginator: ListStudiosPaginator = client.get_paginator("list_studios")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudiosOutputTypeDef
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListStudiosPaginator](./paginators.md#liststudiospaginator)
3. item: [:material-code-braces: ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStudiosPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListStudiosOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStudiosInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudiosInputPaginateTypeDef](./type_defs.md#liststudiosinputpaginatetypedef) 
