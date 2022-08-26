# Paginators

> [Index](../README.md) > [CodeDeploy](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## ListApplicationRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_application_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)

```python title="Usage example"
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

```python title="Method definition"
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
) -> AsyncIterator[ListApplicationRevisionsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ApplicationRevisionSortByType](./literals.md#applicationrevisionsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ListStateFilterActionType](./literals.md#liststatefilteractiontype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef](./type_defs.md#listapplicationrevisionsinputlistapplicationrevisionspaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsInputListApplicationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsInputListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsinputlistapplicationspaginatetypedef) 
## ListDeploymentConfigsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeploymentConfigsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentConfigsOutputTypeDef](./type_defs.md#listdeploymentconfigsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef](./type_defs.md#listdeploymentconfigsinputlistdeploymentconfigspaginatetypedef) 
## ListDeploymentGroupsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    applicationName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeploymentGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeploymentGroupsOutputTypeDef](./type_defs.md#listdeploymentgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef](./type_defs.md#listdeploymentgroupsinputlistdeploymentgroupspaginatetypedef) 
## ListDeploymentInstancesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    deploymentId: str,
    instanceStatusFilter: Sequence[InstanceStatusType] = ...,  # (1)
    instanceTypeFilter: Sequence[InstanceTypeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListDeploymentInstancesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListDeploymentInstancesOutputTypeDef](./type_defs.md#listdeploymentinstancesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef](./type_defs.md#listdeploymentinstancesinputlistdeploymentinstancespaginatetypedef) 
## ListDeploymentTargetsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployment_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    deploymentId: str = ...,
    targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDeploymentTargetsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TargetFilterNameType](./literals.md#targetfilternametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentTargetsOutputTypeDef](./type_defs.md#listdeploymenttargetsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef](./type_defs.md#listdeploymenttargetsinputlistdeploymenttargetspaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    applicationName: str = ...,
    deploymentGroupName: str = ...,
    externalId: str = ...,
    includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,  # (1)
    createTimeRange: TimeRangeTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListDeploymentsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentsInputListDeploymentsPaginateTypeDef = {  # (1)
    "applicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsinputlistdeploymentspaginatetypedef) 
## ListGitHubAccountTokenNamesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_git_hub_account_token_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGitHubAccountTokenNamesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGitHubAccountTokenNamesOutputTypeDef](./type_defs.md#listgithubaccounttokennamesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef](./type_defs.md#listgithubaccounttokennamesinputlistgithubaccounttokennamespaginatetypedef) 
## ListOnPremisesInstancesPaginator

Type annotations and code completion for `#!python session.create_client("codedeploy").get_paginator("list_on_premises_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    registrationStatus: RegistrationStatusType = ...,  # (1)
    tagFilters: Sequence[TagFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListOnPremisesInstancesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListOnPremisesInstancesOutputTypeDef](./type_defs.md#listonpremisesinstancesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = {  # (1)
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef](./type_defs.md#listonpremisesinstancesinputlistonpremisesinstancespaginatetypedef) 
