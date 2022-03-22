<a id="paginators-for-aiobotocore-codedeploy-module"></a>

# Paginators for aiobotocore CodeDeploy module

> [Index](../README.md) > [CodeDeploy](./README.md) > Paginators

Auto-generated documentation for
[CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
type annotations stubs module
[types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

- [Paginators for aiobotocore CodeDeploy module](#paginators-for-aiobotocore-codedeploy-module)
  - [ListApplicationRevisionsPaginator](#listapplicationrevisionspaginator)
  - [ListApplicationsPaginator](#listapplicationspaginator)
  - [ListDeploymentConfigsPaginator](#listdeploymentconfigspaginator)
  - [ListDeploymentGroupsPaginator](#listdeploymentgroupspaginator)
  - [ListDeploymentInstancesPaginator](#listdeploymentinstancespaginator)
  - [ListDeploymentTargetsPaginator](#listdeploymenttargetspaginator)
  - [ListDeploymentsPaginator](#listdeploymentspaginator)
  - [ListGitHubAccountTokenNamesPaginator](#listgithubaccounttokennamespaginator)
  - [ListOnPremisesInstancesPaginator](#listonpremisesinstancespaginator)

<a id="listapplicationrevisionspaginator"></a>

## ListApplicationRevisionsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_application_revisions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListApplicationRevisionsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListApplicationRevisionsPaginator = client.get_paginator("list_application_revisions")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListApplicationRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)

Arguments for `ListApplicationRevisionsPaginator.paginate` method:

- `applicationName`: `str` *(required)*
- `sortBy`:
  [ApplicationRevisionSortByType](./literals.md#applicationrevisionsortbytype)
- `sortOrder`: [SortOrderType](./literals.md#sortordertype)
- `s3Bucket`: `str`
- `s3KeyPrefix`: `str`
- `deployed`:
  [ListStateFilterActionType](./literals.md#liststatefilteractiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationRevisionsPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef)\].

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)\].

<a id="listdeploymentconfigspaginator"></a>

## ListDeploymentConfigsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_deployment_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentConfigsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListDeploymentConfigsPaginator = client.get_paginator("list_deployment_configs")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListDeploymentConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)

Arguments for `ListDeploymentConfigsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentConfigsOutputTypeDef](./type_defs.md#listdeploymentconfigsoutputtypedef)\].

<a id="listdeploymentgroupspaginator"></a>

## ListDeploymentGroupsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_deployment_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentGroupsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListDeploymentGroupsPaginator = client.get_paginator("list_deployment_groups")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListDeploymentGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)

Arguments for `ListDeploymentGroupsPaginator.paginate` method:

- `applicationName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentGroupsOutputTypeDef](./type_defs.md#listdeploymentgroupsoutputtypedef)\].

<a id="listdeploymentinstancespaginator"></a>

## ListDeploymentInstancesPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_deployment_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentInstancesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListDeploymentInstancesPaginator = client.get_paginator("list_deployment_instances")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListDeploymentInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)

Arguments for `ListDeploymentInstancesPaginator.paginate` method:

- `deploymentId`: `str` *(required)*
- `instanceStatusFilter`:
  `Sequence`\[[InstanceStatusType](./literals.md#instancestatustype)\]
- `instanceTypeFilter`:
  `Sequence`\[[InstanceTypeType](./literals.md#instancetypetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentInstancesOutputTypeDef](./type_defs.md#listdeploymentinstancesoutputtypedef)\].

<a id="listdeploymenttargetspaginator"></a>

## ListDeploymentTargetsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_deployment_targets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentTargetsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListDeploymentTargetsPaginator = client.get_paginator("list_deployment_targets")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListDeploymentTargets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)

Arguments for `ListDeploymentTargetsPaginator.paginate` method:

- `deploymentId`: `str`
- `targetFilters`:
  `Mapping`\[[TargetFilterNameType](./literals.md#targetfilternametype),
  `Sequence`\[`str`\]\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentTargetsPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentTargetsOutputTypeDef](./type_defs.md#listdeploymenttargetsoutputtypedef)\].

<a id="listdeploymentspaginator"></a>

## ListDeploymentsPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_deployments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListDeployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)

Arguments for `ListDeploymentsPaginator.paginate` method:

- `applicationName`: `str`
- `deploymentGroupName`: `str`
- `externalId`: `str`
- `includeOnlyStatuses`:
  `Sequence`\[[DeploymentStatusType](./literals.md#deploymentstatustype)\]
- `createTimeRange`: [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentsPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef)\].

<a id="listgithubaccounttokennamespaginator"></a>

## ListGitHubAccountTokenNamesPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_git_hub_account_token_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListGitHubAccountTokenNamesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListGitHubAccountTokenNamesPaginator = client.get_paginator("list_git_hub_account_token_names")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListGitHubAccountTokenNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)

Arguments for `ListGitHubAccountTokenNamesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGitHubAccountTokenNamesPaginator.paginate` returns
`AsyncIterator`\[[ListGitHubAccountTokenNamesOutputTypeDef](./type_defs.md#listgithubaccounttokennamesoutputtypedef)\].

<a id="listonpremisesinstancespaginator"></a>

## ListOnPremisesInstancesPaginator

Type annotations for
`session.create_client("codedeploy").get_paginator("list_on_premises_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.paginator import ListOnPremisesInstancesPaginator

session = get_session()
async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListOnPremisesInstancesPaginator = client.get_paginator("list_on_premises_instances")
```

Boto3 documentation:
[CodeDeploy.Paginator.ListOnPremisesInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)

Arguments for `ListOnPremisesInstancesPaginator.paginate` method:

- `registrationStatus`:
  [RegistrationStatusType](./literals.md#registrationstatustype)
- `tagFilters`:
  `Sequence`\[[TagFilterTypeDef](./type_defs.md#tagfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOnPremisesInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListOnPremisesInstancesOutputTypeDef](./type_defs.md#listonpremisesinstancesoutputtypedef)\].
