# Paginators

> [Index](../README.md) > [WorkSpaces](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## DescribeAccountModificationsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_account_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeAccountModificationsPaginator = client.get_paginator("describe_account_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountModificationsResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
3. item: [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccountModificationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountModificationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef](./type_defs.md#describeaccountmodificationsrequestdescribeaccountmodificationspaginatetypedef) 
## DescribeIpGroupsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_ip_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeIpGroupsPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeIpGroupsPaginator = client.get_paginator("describe_ip_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeIpGroupsPaginator](./paginators.md#describeipgroupspaginator)
3. item: [:material-code-braces: DescribeIpGroupsResultTypeDef](./type_defs.md#describeipgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIpGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeIpGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeIpGroupsResultTypeDef](./type_defs.md#describeipgroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = {  # (1)
    "GroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef](./type_defs.md#describeipgroupsrequestdescribeipgroupspaginatetypedef) 
## DescribeWorkspaceBundlesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceBundlesPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeWorkspaceBundlesPaginator = client.get_paginator("describe_workspace_bundles")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWorkspaceBundlesResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeWorkspaceBundlesPaginator](./paginators.md#describeworkspacebundlespaginator)
3. item: [:material-code-braces: DescribeWorkspaceBundlesResultTypeDef](./type_defs.md#describeworkspacebundlesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceBundlesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    BundleIds: Sequence[str] = ...,
    Owner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeWorkspaceBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeWorkspaceBundlesResultTypeDef](./type_defs.md#describeworkspacebundlesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = {  # (1)
    "BundleIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef](./type_defs.md#describeworkspacebundlesrequestdescribeworkspacebundlespaginatetypedef) 
## DescribeWorkspaceDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceDirectoriesPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeWorkspaceDirectoriesPaginator = client.get_paginator("describe_workspace_directories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWorkspaceDirectoriesResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeWorkspaceDirectoriesPaginator](./paginators.md#describeworkspacedirectoriespaginator)
3. item: [:material-code-braces: DescribeWorkspaceDirectoriesResultTypeDef](./type_defs.md#describeworkspacedirectoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceDirectoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryIds: Sequence[str] = ...,
    Limit: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeWorkspaceDirectoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeWorkspaceDirectoriesResultTypeDef](./type_defs.md#describeworkspacedirectoriesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = {  # (1)
    "DirectoryIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef](./type_defs.md#describeworkspacedirectoriesrequestdescribeworkspacedirectoriespaginatetypedef) 
## DescribeWorkspaceImagesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeWorkspaceImagesPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeWorkspaceImagesPaginator = client.get_paginator("describe_workspace_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWorkspaceImagesResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeWorkspaceImagesPaginator](./paginators.md#describeworkspaceimagespaginator)
3. item: [:material-code-braces: DescribeWorkspaceImagesResultTypeDef](./type_defs.md#describeworkspaceimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    ImageType: ImageTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeWorkspaceImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeWorkspaceImagesResultTypeDef](./type_defs.md#describeworkspaceimagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef](./type_defs.md#describeworkspaceimagesrequestdescribeworkspaceimagespaginatetypedef) 
## DescribeWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeWorkspacesPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeWorkspacesPaginator = client.get_paginator("describe_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWorkspacesResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeWorkspacesPaginator](./paginators.md#describeworkspacespaginator)
3. item: [:material-code-braces: DescribeWorkspacesResultTypeDef](./type_defs.md#describeworkspacesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWorkspacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    DirectoryId: str = ...,
    UserName: str = ...,
    BundleId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeWorkspacesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeWorkspacesResultTypeDef](./type_defs.md#describeworkspacesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef](./type_defs.md#describeworkspacesrequestdescribeworkspacespaginatetypedef) 
## DescribeWorkspacesConnectionStatusPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspaces_connection_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import DescribeWorkspacesConnectionStatusPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: DescribeWorkspacesConnectionStatusPaginator = client.get_paginator("describe_workspaces_connection_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWorkspacesConnectionStatusResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeWorkspacesConnectionStatusPaginator](./paginators.md#describeworkspacesconnectionstatuspaginator)
3. item: [:material-code-braces: DescribeWorkspacesConnectionStatusResultTypeDef](./type_defs.md#describeworkspacesconnectionstatusresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWorkspacesConnectionStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeWorkspacesConnectionStatusResultTypeDef](./type_defs.md#describeworkspacesconnectionstatusresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef](./type_defs.md#describeworkspacesconnectionstatusrequestdescribeworkspacesconnectionstatuspaginatetypedef) 
## ListAvailableManagementCidrRangesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("list_available_management_cidr_ranges")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import ListAvailableManagementCidrRangesPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: ListAvailableManagementCidrRangesPaginator = client.get_paginator("list_available_management_cidr_ranges")  # (2)
    async for item in paginator.paginate(...):
        item: ListAvailableManagementCidrRangesResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [ListAvailableManagementCidrRangesPaginator](./paginators.md#listavailablemanagementcidrrangespaginator)
3. item: [:material-code-braces: ListAvailableManagementCidrRangesResultTypeDef](./type_defs.md#listavailablemanagementcidrrangesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAvailableManagementCidrRangesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ManagementCidrRangeConstraint: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAvailableManagementCidrRangesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAvailableManagementCidrRangesResultTypeDef](./type_defs.md#listavailablemanagementcidrrangesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = {  # (1)
    "ManagementCidrRangeConstraint": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef](./type_defs.md#listavailablemanagementcidrrangesrequestlistavailablemanagementcidrrangespaginatetypedef) 
