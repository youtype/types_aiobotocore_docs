# Paginators

> [Index](../README.md) > [CodeDeploy](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## ListApplicationRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_application_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListApplicationRevisions.html#CodeDeploy.Paginator.ListApplicationRevisions)

```python
# ListApplicationRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListApplicationRevisionsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListApplicationRevisionsPaginator = client.get_paginator("list_application_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationRevisionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListApplicationRevisionsPaginator](./paginators.md#listapplicationrevisionspaginator)
3. item: [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationName: str,
    sortBy: ApplicationRevisionSortByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    s3Bucket: str = ...,
    s3KeyPrefix: str = ...,
    deployed: ListStateFilterActionType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListApplicationRevisionsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ApplicationRevisionSortByType](./literals.md#applicationrevisionsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ListStateFilterActionType](./literals.md#liststatefilteractiontype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationRevisionsInputPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationRevisionsInputPaginateTypeDef](./type_defs.md#listapplicationrevisionsinputpaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListApplications.html#CodeDeploy.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListApplicationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsInputPaginateTypeDef](./type_defs.md#listapplicationsinputpaginatetypedef) 
## ListDeploymentConfigsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListDeploymentConfigs.html#CodeDeploy.Paginator.ListDeploymentConfigs)

```python
# ListDeploymentConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentConfigsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListDeploymentConfigsPaginator = client.get_paginator("list_deployment_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentConfigsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListDeploymentConfigsPaginator](./paginators.md#listdeploymentconfigspaginator)
3. item: [:material-code-braces: ListDeploymentConfigsOutputTypeDef](./type_defs.md#listdeploymentconfigsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeploymentConfigsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentConfigsOutputTypeDef](./type_defs.md#listdeploymentconfigsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentConfigsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentConfigsInputPaginateTypeDef](./type_defs.md#listdeploymentconfigsinputpaginatetypedef) 
## ListDeploymentGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListDeploymentGroups.html#CodeDeploy.Paginator.ListDeploymentGroups)

```python
# ListDeploymentGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentGroupsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListDeploymentGroupsPaginator = client.get_paginator("list_deployment_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListDeploymentGroupsPaginator](./paginators.md#listdeploymentgroupspaginator)
3. item: [:material-code-braces: ListDeploymentGroupsOutputTypeDef](./type_defs.md#listdeploymentgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeploymentGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentGroupsOutputTypeDef](./type_defs.md#listdeploymentgroupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentGroupsInputPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentGroupsInputPaginateTypeDef](./type_defs.md#listdeploymentgroupsinputpaginatetypedef) 
## ListDeploymentInstancesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListDeploymentInstances.html#CodeDeploy.Paginator.ListDeploymentInstances)

```python
# ListDeploymentInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentInstancesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListDeploymentInstancesPaginator = client.get_paginator("list_deployment_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListDeploymentInstancesPaginator](./paginators.md#listdeploymentinstancespaginator)
3. item: [:material-code-braces: ListDeploymentInstancesOutputTypeDef](./type_defs.md#listdeploymentinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    deploymentId: str,
    instanceStatusFilter: Sequence[InstanceStatusType] = ...,  # (1)
    instanceTypeFilter: Sequence[InstanceTypeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListDeploymentInstancesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListDeploymentInstancesOutputTypeDef](./type_defs.md#listdeploymentinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentInstancesInputPaginateTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentInstancesInputPaginateTypeDef](./type_defs.md#listdeploymentinstancesinputpaginatetypedef) 
## ListDeploymentTargetsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListDeploymentTargets.html#CodeDeploy.Paginator.ListDeploymentTargets)

```python
# ListDeploymentTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentTargetsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListDeploymentTargetsPaginator = client.get_paginator("list_deployment_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentTargetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListDeploymentTargetsPaginator](./paginators.md#listdeploymenttargetspaginator)
3. item: [:material-code-braces: ListDeploymentTargetsOutputTypeDef](./type_defs.md#listdeploymenttargetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    deploymentId: str,
    targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDeploymentTargetsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TargetFilterNameType](./literals.md#targetfilternametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentTargetsOutputTypeDef](./type_defs.md#listdeploymenttargetsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentTargetsInputPaginateTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentTargetsInputPaginateTypeDef](./type_defs.md#listdeploymenttargetsinputpaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListDeployments.html#CodeDeploy.Paginator.ListDeployments)

```python
# ListDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationName: str = ...,
    deploymentGroupName: str = ...,
    externalId: str = ...,
    includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,  # (1)
    createTimeRange: TimeRangeTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListDeploymentsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentsInputPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputPaginateTypeDef](./type_defs.md#listdeploymentsinputpaginatetypedef) 
## ListGitHubAccountTokenNamesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_git_hub_account_token_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListGitHubAccountTokenNames.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)

```python
# ListGitHubAccountTokenNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListGitHubAccountTokenNamesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListGitHubAccountTokenNamesPaginator = client.get_paginator("list_git_hub_account_token_names")  # (2)
    async for item in paginator.paginate(...):
        item: ListGitHubAccountTokenNamesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListGitHubAccountTokenNamesPaginator](./paginators.md#listgithubaccounttokennamespaginator)
3. item: [:material-code-braces: ListGitHubAccountTokenNamesOutputTypeDef](./type_defs.md#listgithubaccounttokennamesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGitHubAccountTokenNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGitHubAccountTokenNamesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGitHubAccountTokenNamesOutputTypeDef](./type_defs.md#listgithubaccounttokennamesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGitHubAccountTokenNamesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGitHubAccountTokenNamesInputPaginateTypeDef](./type_defs.md#listgithubaccounttokennamesinputpaginatetypedef) 
## ListOnPremisesInstancesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_on_premises_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/paginator/ListOnPremisesInstances.html#CodeDeploy.Paginator.ListOnPremisesInstances)

```python
# ListOnPremisesInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListOnPremisesInstancesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    paginator: ListOnPremisesInstancesPaginator = client.get_paginator("list_on_premises_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListOnPremisesInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListOnPremisesInstancesPaginator](./paginators.md#listonpremisesinstancespaginator)
3. item: [:material-code-braces: ListOnPremisesInstancesOutputTypeDef](./type_defs.md#listonpremisesinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListOnPremisesInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    registrationStatus: RegistrationStatusType = ...,  # (1)
    tagFilters: Sequence[TagFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListOnPremisesInstancesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListOnPremisesInstancesOutputTypeDef](./type_defs.md#listonpremisesinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOnPremisesInstancesInputPaginateTypeDef = {  # (1)
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOnPremisesInstancesInputPaginateTypeDef](./type_defs.md#listonpremisesinstancesinputpaginatetypedef) 
