<a id="paginators-for-aiobotocore-workspaces-module"></a>

# Paginators for aiobotocore WorkSpaces module

> [Index](..) > [WorkSpaces](.) > Paginators

Auto-generated documentation for
[WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
type annotations stubs module
[types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

- [Paginators for aiobotocore WorkSpaces module](#paginators-for-aiobotocore-workspaces-module)
  - [DescribeAccountModificationsPaginator](#describeaccountmodificationspaginator)
  - [DescribeIpGroupsPaginator](#describeipgroupspaginator)
  - [DescribeWorkspaceBundlesPaginator](#describeworkspacebundlespaginator)
  - [DescribeWorkspaceDirectoriesPaginator](#describeworkspacedirectoriespaginator)
  - [DescribeWorkspaceImagesPaginator](#describeworkspaceimagespaginator)
  - [DescribeWorkspacesPaginator](#describeworkspacespaginator)
  - [DescribeWorkspacesConnectionStatusPaginator](#describeworkspacesconnectionstatuspaginator)
  - [ListAvailableManagementCidrRangesPaginator](#listavailablemanagementcidrrangespaginator)

<a id="describeaccountmodificationspaginator"></a>

## DescribeAccountModificationsPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_account_modifications")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator

def get_describe_account_modifications_paginator() -> DescribeAccountModificationsPaginator:
    return Session().create_client("workspaces").get_paginator("describe_account_modifications")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeAccountModifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)

Arguments for `DescribeAccountModificationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAccountModificationsPaginator.paginate` returns
`_PageIterator`\[[DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef)\].

<a id="describeipgroupspaginator"></a>

## DescribeIpGroupsPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_ip_groups")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeIpGroupsPaginator

def get_describe_ip_groups_paginator() -> DescribeIpGroupsPaginator:
    return Session().create_client("workspaces").get_paginator("describe_ip_groups")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeIpGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)

Arguments for `DescribeIpGroupsPaginator.paginate` method:

- `GroupIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeIpGroupsPaginator.paginate` returns
`_PageIterator`\[[DescribeIpGroupsResultTypeDef](./type_defs.md#describeipgroupsresulttypedef)\].

<a id="describeworkspacebundlespaginator"></a>

## DescribeWorkspaceBundlesPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_workspace_bundles")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceBundlesPaginator

def get_describe_workspace_bundles_paginator() -> DescribeWorkspaceBundlesPaginator:
    return Session().create_client("workspaces").get_paginator("describe_workspace_bundles")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeWorkspaceBundles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles)

Arguments for `DescribeWorkspaceBundlesPaginator.paginate` method:

- `BundleIds`: `Sequence`\[`str`\]
- `Owner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeWorkspaceBundlesPaginator.paginate` returns
`_PageIterator`\[[DescribeWorkspaceBundlesResultTypeDef](./type_defs.md#describeworkspacebundlesresulttypedef)\].

<a id="describeworkspacedirectoriespaginator"></a>

## DescribeWorkspaceDirectoriesPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_workspace_directories")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceDirectoriesPaginator

def get_describe_workspace_directories_paginator() -> DescribeWorkspaceDirectoriesPaginator:
    return Session().create_client("workspaces").get_paginator("describe_workspace_directories")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeWorkspaceDirectories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories)

Arguments for `DescribeWorkspaceDirectoriesPaginator.paginate` method:

- `DirectoryIds`: `Sequence`\[`str`\]
- `Limit`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeWorkspaceDirectoriesPaginator.paginate` returns
`_PageIterator`\[[DescribeWorkspaceDirectoriesResultTypeDef](./type_defs.md#describeworkspacedirectoriesresulttypedef)\].

<a id="describeworkspaceimagespaginator"></a>

## DescribeWorkspaceImagesPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_workspace_images")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceImagesPaginator

def get_describe_workspace_images_paginator() -> DescribeWorkspaceImagesPaginator:
    return Session().create_client("workspaces").get_paginator("describe_workspace_images")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeWorkspaceImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages)

Arguments for `DescribeWorkspaceImagesPaginator.paginate` method:

- `ImageIds`: `Sequence`\[`str`\]
- `ImageType`: [ImageTypeType](./literals.md#imagetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeWorkspaceImagesPaginator.paginate` returns
`_PageIterator`\[[DescribeWorkspaceImagesResultTypeDef](./type_defs.md#describeworkspaceimagesresulttypedef)\].

<a id="describeworkspacespaginator"></a>

## DescribeWorkspacesPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_workspaces")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeWorkspacesPaginator

def get_describe_workspaces_paginator() -> DescribeWorkspacesPaginator:
    return Session().create_client("workspaces").get_paginator("describe_workspaces")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeWorkspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces)

Arguments for `DescribeWorkspacesPaginator.paginate` method:

- `WorkspaceIds`: `Sequence`\[`str`\]
- `DirectoryId`: `str`
- `UserName`: `str`
- `BundleId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeWorkspacesPaginator.paginate` returns
`_PageIterator`\[[DescribeWorkspacesResultTypeDef](./type_defs.md#describeworkspacesresulttypedef)\].

<a id="describeworkspacesconnectionstatuspaginator"></a>

## DescribeWorkspacesConnectionStatusPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("describe_workspaces_connection_status")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import DescribeWorkspacesConnectionStatusPaginator

def get_describe_workspaces_connection_status_paginator() -> DescribeWorkspacesConnectionStatusPaginator:
    return Session().create_client("workspaces").get_paginator("describe_workspaces_connection_status")
```

Boto3 documentation:
[WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)

Arguments for `DescribeWorkspacesConnectionStatusPaginator.paginate` method:

- `WorkspaceIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeWorkspacesConnectionStatusPaginator.paginate` returns
`_PageIterator`\[[DescribeWorkspacesConnectionStatusResultTypeDef](./type_defs.md#describeworkspacesconnectionstatusresulttypedef)\].

<a id="listavailablemanagementcidrrangespaginator"></a>

## ListAvailableManagementCidrRangesPaginator

Type annotations for
`aiobotocore.create_client("workspaces").get_paginator("list_available_management_cidr_ranges")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_workspaces.paginator import ListAvailableManagementCidrRangesPaginator

def get_list_available_management_cidr_ranges_paginator() -> ListAvailableManagementCidrRangesPaginator:
    return Session().create_client("workspaces").get_paginator("list_available_management_cidr_ranges")
```

Boto3 documentation:
[WorkSpaces.Paginator.ListAvailableManagementCidrRanges](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)

Arguments for `ListAvailableManagementCidrRangesPaginator.paginate` method:

- `ManagementCidrRangeConstraint`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAvailableManagementCidrRangesPaginator.paginate` returns
`_PageIterator`\[[ListAvailableManagementCidrRangesResultTypeDef](./type_defs.md#listavailablemanagementcidrrangesresulttypedef)\].
