<a id="paginators-for-aiobotocore-workdocs-module"></a>

# Paginators for aiobotocore WorkDocs module

> [Index](..) > [WorkDocs](.) > Paginators

Auto-generated documentation for
[WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
type annotations stubs module
[types-aiobotocore-workdocs](https://pypi.org/project/types-aiobotocore-workdocs/).

- [Paginators for aiobotocore WorkDocs module](#paginators-for-aiobotocore-workdocs-module)
  - [DescribeActivitiesPaginator](#describeactivitiespaginator)
  - [DescribeCommentsPaginator](#describecommentspaginator)
  - [DescribeDocumentVersionsPaginator](#describedocumentversionspaginator)
  - [DescribeFolderContentsPaginator](#describefoldercontentspaginator)
  - [DescribeGroupsPaginator](#describegroupspaginator)
  - [DescribeNotificationSubscriptionsPaginator](#describenotificationsubscriptionspaginator)
  - [DescribeResourcePermissionsPaginator](#describeresourcepermissionspaginator)
  - [DescribeRootFoldersPaginator](#describerootfolderspaginator)
  - [DescribeUsersPaginator](#describeuserspaginator)

<a id="describeactivitiespaginator"></a>

## DescribeActivitiesPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_activities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeActivitiesPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeActivitiesPaginator = client.get_paginator("describe_activities")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeActivities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities)

Arguments for `DescribeActivitiesPaginator.paginate` method:

- `AuthenticationToken`: `str`
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `OrganizationId`: `str`
- `ActivityTypes`: `str`
- `ResourceId`: `str`
- `UserId`: `str`
- `IncludeIndirectActivities`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeActivitiesPaginator.paginate` returns
`_PageIterator`\[[DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef)\].

<a id="describecommentspaginator"></a>

## DescribeCommentsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_comments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeCommentsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeCommentsPaginator = client.get_paginator("describe_comments")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeComments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments)

Arguments for `DescribeCommentsPaginator.paginate` method:

- `DocumentId`: `str` *(required)*
- `VersionId`: `str` *(required)*
- `AuthenticationToken`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeCommentsPaginator.paginate` returns
`_PageIterator`\[[DescribeCommentsResponseTypeDef](./type_defs.md#describecommentsresponsetypedef)\].

<a id="describedocumentversionspaginator"></a>

## DescribeDocumentVersionsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_document_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeDocumentVersionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeDocumentVersionsPaginator = client.get_paginator("describe_document_versions")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeDocumentVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions)

Arguments for `DescribeDocumentVersionsPaginator.paginate` method:

- `DocumentId`: `str` *(required)*
- `AuthenticationToken`: `str`
- `Include`: `str`
- `Fields`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDocumentVersionsPaginator.paginate` returns
`_PageIterator`\[[DescribeDocumentVersionsResponseTypeDef](./type_defs.md#describedocumentversionsresponsetypedef)\].

<a id="describefoldercontentspaginator"></a>

## DescribeFolderContentsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_folder_contents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeFolderContentsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeFolderContentsPaginator = client.get_paginator("describe_folder_contents")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeFolderContents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents)

Arguments for `DescribeFolderContentsPaginator.paginate` method:

- `FolderId`: `str` *(required)*
- `AuthenticationToken`: `str`
- `Sort`: [ResourceSortTypeType](./literals.md#resourcesorttypetype)
- `Order`: [OrderTypeType](./literals.md#ordertypetype)
- `Type`: [FolderContentTypeType](./literals.md#foldercontenttypetype)
- `Include`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFolderContentsPaginator.paginate` returns
`_PageIterator`\[[DescribeFolderContentsResponseTypeDef](./type_defs.md#describefoldercontentsresponsetypedef)\].

<a id="describegroupspaginator"></a>

## DescribeGroupsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeGroupsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeGroupsPaginator = client.get_paginator("describe_groups")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups)

Arguments for `DescribeGroupsPaginator.paginate` method:

- `SearchQuery`: `str` *(required)*
- `AuthenticationToken`: `str`
- `OrganizationId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGroupsPaginator.paginate` returns
`_PageIterator`\[[DescribeGroupsResponseTypeDef](./type_defs.md#describegroupsresponsetypedef)\].

<a id="describenotificationsubscriptionspaginator"></a>

## DescribeNotificationSubscriptionsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_notification_subscriptions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeNotificationSubscriptionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeNotificationSubscriptionsPaginator = client.get_paginator("describe_notification_subscriptions")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeNotificationSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)

Arguments for `DescribeNotificationSubscriptionsPaginator.paginate` method:

- `OrganizationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeNotificationSubscriptionsPaginator.paginate` returns
`_PageIterator`\[[DescribeNotificationSubscriptionsResponseTypeDef](./type_defs.md#describenotificationsubscriptionsresponsetypedef)\].

<a id="describeresourcepermissionspaginator"></a>

## DescribeResourcePermissionsPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_resource_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeResourcePermissionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeResourcePermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions)

Arguments for `DescribeResourcePermissionsPaginator.paginate` method:

- `ResourceId`: `str` *(required)*
- `AuthenticationToken`: `str`
- `PrincipalId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeResourcePermissionsPaginator.paginate` returns
`_PageIterator`\[[DescribeResourcePermissionsResponseTypeDef](./type_defs.md#describeresourcepermissionsresponsetypedef)\].

<a id="describerootfolderspaginator"></a>

## DescribeRootFoldersPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_root_folders")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeRootFoldersPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeRootFolders](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)

Arguments for `DescribeRootFoldersPaginator.paginate` method:

- `AuthenticationToken`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRootFoldersPaginator.paginate` returns
`_PageIterator`\[[DescribeRootFoldersResponseTypeDef](./type_defs.md#describerootfoldersresponsetypedef)\].

<a id="describeuserspaginator"></a>

## DescribeUsersPaginator

Type annotations for
`session.create_client("workdocs").get_paginator("describe_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeUsersPaginator

session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
```

Boto3 documentation:
[WorkDocs.Paginator.DescribeUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers)

Arguments for `DescribeUsersPaginator.paginate` method:

- `AuthenticationToken`: `str`
- `OrganizationId`: `str`
- `UserIds`: `str`
- `Query`: `str`
- `Include`: [UserFilterTypeType](./literals.md#userfiltertypetype)
- `Order`: [OrderTypeType](./literals.md#ordertypetype)
- `Sort`: [UserSortTypeType](./literals.md#usersorttypetype)
- `Fields`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeUsersPaginator.paginate` returns
`_PageIterator`\[[DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef)\].
