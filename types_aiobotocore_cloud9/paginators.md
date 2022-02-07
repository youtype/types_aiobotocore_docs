<a id="paginators-for-aiobotocore-cloud9-module"></a>

# Paginators for aiobotocore Cloud9 module

> [Index](..) > [Cloud9](.) > Paginators

Auto-generated documentation for
[Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
type annotations stubs module
[types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

- [Paginators for aiobotocore Cloud9 module](#paginators-for-aiobotocore-cloud9-module)
  - [DescribeEnvironmentMembershipsPaginator](#describeenvironmentmembershipspaginator)
  - [ListEnvironmentsPaginator](#listenvironmentspaginator)

<a id="describeenvironmentmembershipspaginator"></a>

## DescribeEnvironmentMembershipsPaginator

Type annotations for
`session.create_client("cloud9").get_paginator("describe_environment_memberships")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator

session = get_session()
async with session.create_client("cloud9") as client:
    client: Cloud9Client
    paginator: DescribeEnvironmentMembershipsPaginator = client.get_paginator("describe_environment_memberships")
```

Boto3 documentation:
[Cloud9.Paginator.DescribeEnvironmentMemberships](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships)

Arguments for `DescribeEnvironmentMembershipsPaginator.paginate` method:

- `userArn`: `str`
- `environmentId`: `str`
- `permissions`: `Sequence`\[[PermissionsType](./literals.md#permissionstype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEnvironmentMembershipsPaginator.paginate` returns
`_PageIterator`\[[DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef)\].

<a id="listenvironmentspaginator"></a>

## ListEnvironmentsPaginator

Type annotations for
`session.create_client("cloud9").get_paginator("list_environments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloud9.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("cloud9") as client:
    client: Cloud9Client
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
```

Boto3 documentation:
[Cloud9.Paginator.ListEnvironments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)

Arguments for `ListEnvironmentsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnvironmentsPaginator.paginate` returns
`_PageIterator`\[[ListEnvironmentsResultTypeDef](./type_defs.md#listenvironmentsresulttypedef)\].
