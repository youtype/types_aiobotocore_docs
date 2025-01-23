# Paginators

> [Index](../README.md) > [LaunchWizard](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## ListDeploymentEventsPaginator

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_paginator("list_deployment_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/paginator/ListDeploymentEvents.html#LaunchWizard.Paginator.ListDeploymentEvents)

```python
# ListDeploymentEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.paginator import ListDeploymentEventsPaginator

session = get_session()
async with session.create_client("launch-wizard") as client:  # (1)
    paginator: ListDeploymentEventsPaginator = client.get_paginator("list_deployment_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
3. item: [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    deploymentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeploymentEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentEventsInputPaginateTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentEventsInputPaginateTypeDef](./type_defs.md#listdeploymenteventsinputpaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/paginator/ListDeployments.html#LaunchWizard.Paginator.ListDeployments)

```python
# ListDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("launch-wizard") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsOutputTypeDef
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[DeploymentFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDeploymentsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentsInputPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputPaginateTypeDef](./type_defs.md#listdeploymentsinputpaginatetypedef) 
## ListWorkloadDeploymentPatternsPaginator

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_paginator("list_workload_deployment_patterns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/paginator/ListWorkloadDeploymentPatterns.html#LaunchWizard.Paginator.ListWorkloadDeploymentPatterns)

```python
# ListWorkloadDeploymentPatternsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.paginator import ListWorkloadDeploymentPatternsPaginator

session = get_session()
async with session.create_client("launch-wizard") as client:  # (1)
    paginator: ListWorkloadDeploymentPatternsPaginator = client.get_paginator("list_workload_deployment_patterns")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkloadDeploymentPatternsOutputTypeDef
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListWorkloadDeploymentPatternsPaginator](./paginators.md#listworkloaddeploymentpatternspaginator)
3. item: [:material-code-braces: ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkloadDeploymentPatternsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workloadName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkloadDeploymentPatternsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkloadDeploymentPatternsInputPaginateTypeDef = {  # (1)
    "workloadName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkloadDeploymentPatternsInputPaginateTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputpaginatetypedef) 
## ListWorkloadsPaginator

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_paginator("list_workloads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/paginator/ListWorkloads.html#LaunchWizard.Paginator.ListWorkloads)

```python
# ListWorkloadsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.paginator import ListWorkloadsPaginator

session = get_session()
async with session.create_client("launch-wizard") as client:  # (1)
    paginator: ListWorkloadsPaginator = client.get_paginator("list_workloads")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkloadsOutputTypeDef
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListWorkloadsPaginator](./paginators.md#listworkloadspaginator)
3. item: [:material-code-braces: ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkloadsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkloadsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkloadsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkloadsInputPaginateTypeDef](./type_defs.md#listworkloadsinputpaginatetypedef) 
