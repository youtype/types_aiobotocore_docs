# Paginators

> [Index](../README.md) > [WorkSpaces](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## DescribeAccountModificationsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_account_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeAccountModifications.html#WorkSpaces.Paginator.DescribeAccountModifications)

```python
# DescribeAccountModificationsPaginator usage example

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
3. item: `AioPageIterator[DescribeAccountModificationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAccountModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAccountModificationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAccountModificationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountModificationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountModificationsRequestPaginateTypeDef](./type_defs.md#describeaccountmodificationsrequestpaginatetypedef)
## DescribeIpGroupsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_ip_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeIpGroups.html#WorkSpaces.Paginator.DescribeIpGroups)

```python
# DescribeIpGroupsPaginator usage example

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
3. item: `AioPageIterator[DescribeIpGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeIpGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpGroupsRequestPaginateTypeDef = {  # (1)
    "GroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpGroupsRequestPaginateTypeDef](./type_defs.md#describeipgroupsrequestpaginatetypedef)
## DescribeWorkspaceBundlesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeWorkspaceBundles.html#WorkSpaces.Paginator.DescribeWorkspaceBundles)

```python
# DescribeWorkspaceBundlesPaginator usage example

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
3. item: `AioPageIterator[DescribeWorkspaceBundlesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceBundlesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BundleIds: Sequence[str] = ...,
    Owner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeWorkspaceBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeWorkspaceBundlesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWorkspaceBundlesRequestPaginateTypeDef = {  # (1)
    "BundleIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceBundlesRequestPaginateTypeDef](./type_defs.md#describeworkspacebundlesrequestpaginatetypedef)
## DescribeWorkspaceDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeWorkspaceDirectories.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories)

```python
# DescribeWorkspaceDirectoriesPaginator usage example

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
3. item: `AioPageIterator[DescribeWorkspaceDirectoriesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceDirectoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryIds: Sequence[str] = ...,
    WorkspaceDirectoryNames: Sequence[str] = ...,
    Limit: int = ...,
    Filters: Sequence[DescribeWorkspaceDirectoriesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeWorkspaceDirectoriesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[DescribeWorkspaceDirectoriesFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeWorkspaceDirectoriesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWorkspaceDirectoriesRequestPaginateTypeDef = {  # (1)
    "DirectoryIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesRequestPaginateTypeDef](./type_defs.md#describeworkspacedirectoriesrequestpaginatetypedef)
## DescribeWorkspaceImagesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspace_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeWorkspaceImages.html#WorkSpaces.Paginator.DescribeWorkspaceImages)

```python
# DescribeWorkspaceImagesPaginator usage example

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
3. item: `AioPageIterator[DescribeWorkspaceImagesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeWorkspaceImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    ImageType: ImageTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeWorkspaceImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeWorkspaceImagesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWorkspaceImagesRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceImagesRequestPaginateTypeDef](./type_defs.md#describeworkspaceimagesrequestpaginatetypedef)
## DescribeWorkspacesConnectionStatusPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspaces_connection_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeWorkspacesConnectionStatus.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)

```python
# DescribeWorkspacesConnectionStatusPaginator usage example

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
3. item: `AioPageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeWorkspacesConnectionStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWorkspacesConnectionStatusRequestPaginateTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesConnectionStatusRequestPaginateTypeDef](./type_defs.md#describeworkspacesconnectionstatusrequestpaginatetypedef)
## DescribeWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("describe_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/DescribeWorkspaces.html#WorkSpaces.Paginator.DescribeWorkspaces)

```python
# DescribeWorkspacesPaginator usage example

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
3. item: `AioPageIterator[DescribeWorkspacesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    DirectoryId: str = ...,
    UserName: str = ...,
    BundleId: str = ...,
    WorkspaceName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeWorkspacesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeWorkspacesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWorkspacesRequestPaginateTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesRequestPaginateTypeDef](./type_defs.md#describeworkspacesrequestpaginatetypedef)
## ListAccountLinksPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("list_account_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/ListAccountLinks.html#WorkSpaces.Paginator.ListAccountLinks)

```python
# ListAccountLinksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces.paginator import ListAccountLinksPaginator

session = get_session()
async with session.create_client("workspaces") as client:  # (1)
    paginator: ListAccountLinksPaginator = client.get_paginator("list_account_links")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountLinksResultTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [ListAccountLinksPaginator](./paginators.md#listaccountlinkspaginator)
3. item: `AioPageIterator[ListAccountLinksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountLinksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LinkStatusFilter: Sequence[AccountLinkStatusEnumType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAccountLinksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[AccountLinkStatusEnumType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAccountLinksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountLinksRequestPaginateTypeDef = {  # (1)
    "LinkStatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountLinksRequestPaginateTypeDef](./type_defs.md#listaccountlinksrequestpaginatetypedef)
## ListAvailableManagementCidrRangesPaginator

Type annotations and code completion for `#!python session.create_client("workspaces").get_paginator("list_available_management_cidr_ranges")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces/paginator/ListAvailableManagementCidrRanges.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)

```python
# ListAvailableManagementCidrRangesPaginator usage example

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
3. item: `AioPageIterator[ListAvailableManagementCidrRangesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAvailableManagementCidrRangesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ManagementCidrRangeConstraint: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAvailableManagementCidrRangesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAvailableManagementCidrRangesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAvailableManagementCidrRangesRequestPaginateTypeDef = {  # (1)
    "ManagementCidrRangeConstraint": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagementCidrRangesRequestPaginateTypeDef](./type_defs.md#listavailablemanagementcidrrangesrequestpaginatetypedef)
