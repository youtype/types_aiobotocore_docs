# Paginators

> [Index](../README.md) > [WorkDocs](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
    type annotations stubs module [types-aiobotocore-workdocs](https://pypi.org/project/types-aiobotocore-workdocs/).

## DescribeActivitiesPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_activities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities)

```python
# DescribeActivitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeActivitiesPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeActivitiesPaginator = client.get_paginator("describe_activities")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActivitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeActivitiesPaginator](./paginators.md#describeactivitiespaginator)
3. item: [:material-code-braces: DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeActivitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AuthenticationToken: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    OrganizationId: str = ...,
    ActivityTypes: str = ...,
    ResourceId: str = ...,
    UserId: str = ...,
    IncludeIndirectActivities: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeActivitiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = {  # (1)
    "AuthenticationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef](./type_defs.md#describeactivitiesrequestdescribeactivitiespaginatetypedef) 
## DescribeCommentsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_comments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments)

```python
# DescribeCommentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeCommentsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeCommentsPaginator = client.get_paginator("describe_comments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCommentsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeCommentsPaginator](./paginators.md#describecommentspaginator)
3. item: [:material-code-braces: DescribeCommentsResponseTypeDef](./type_defs.md#describecommentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCommentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeCommentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeCommentsResponseTypeDef](./type_defs.md#describecommentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCommentsRequestDescribeCommentsPaginateTypeDef = {  # (1)
    "DocumentId": ...,
    "VersionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCommentsRequestDescribeCommentsPaginateTypeDef](./type_defs.md#describecommentsrequestdescribecommentspaginatetypedef) 
## DescribeDocumentVersionsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_document_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions)

```python
# DescribeDocumentVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeDocumentVersionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeDocumentVersionsPaginator = client.get_paginator("describe_document_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDocumentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeDocumentVersionsPaginator](./paginators.md#describedocumentversionspaginator)
3. item: [:material-code-braces: DescribeDocumentVersionsResponseTypeDef](./type_defs.md#describedocumentversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDocumentVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DocumentId: str,
    AuthenticationToken: str = ...,
    Include: str = ...,
    Fields: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDocumentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDocumentVersionsResponseTypeDef](./type_defs.md#describedocumentversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = {  # (1)
    "DocumentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef](./type_defs.md#describedocumentversionsrequestdescribedocumentversionspaginatetypedef) 
## DescribeFolderContentsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_folder_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents)

```python
# DescribeFolderContentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeFolderContentsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeFolderContentsPaginator = client.get_paginator("describe_folder_contents")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFolderContentsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeFolderContentsPaginator](./paginators.md#describefoldercontentspaginator)
3. item: [:material-code-braces: DescribeFolderContentsResponseTypeDef](./type_defs.md#describefoldercontentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFolderContentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FolderId: str,
    AuthenticationToken: str = ...,
    Sort: ResourceSortTypeType = ...,  # (1)
    Order: OrderTypeType = ...,  # (2)
    Type: FolderContentTypeType = ...,  # (3)
    Include: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[DescribeFolderContentsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceSortTypeType](./literals.md#resourcesorttypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: FolderContentTypeType](./literals.md#foldercontenttypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: DescribeFolderContentsResponseTypeDef](./type_defs.md#describefoldercontentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = {  # (1)
    "FolderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef](./type_defs.md#describefoldercontentsrequestdescribefoldercontentspaginatetypedef) 
## DescribeGroupsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups)

```python
# DescribeGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeGroupsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeGroupsPaginator = client.get_paginator("describe_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeGroupsPaginator](./paginators.md#describegroupspaginator)
3. item: [:material-code-braces: DescribeGroupsResponseTypeDef](./type_defs.md#describegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SearchQuery: str,
    AuthenticationToken: str = ...,
    OrganizationId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGroupsResponseTypeDef](./type_defs.md#describegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGroupsRequestDescribeGroupsPaginateTypeDef = {  # (1)
    "SearchQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGroupsRequestDescribeGroupsPaginateTypeDef](./type_defs.md#describegroupsrequestdescribegroupspaginatetypedef) 
## DescribeNotificationSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_notification_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)

```python
# DescribeNotificationSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeNotificationSubscriptionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeNotificationSubscriptionsPaginator = client.get_paginator("describe_notification_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNotificationSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeNotificationSubscriptionsPaginator](./paginators.md#describenotificationsubscriptionspaginator)
3. item: [:material-code-braces: DescribeNotificationSubscriptionsResponseTypeDef](./type_defs.md#describenotificationsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNotificationSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeNotificationSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeNotificationSubscriptionsResponseTypeDef](./type_defs.md#describenotificationsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = {  # (1)
    "OrganizationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef](./type_defs.md#describenotificationsubscriptionsrequestdescribenotificationsubscriptionspaginatetypedef) 
## DescribeResourcePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_resource_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions)

```python
# DescribeResourcePermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeResourcePermissionsPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeResourcePermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeResourcePermissionsPaginator](./paginators.md#describeresourcepermissionspaginator)
3. item: [:material-code-braces: DescribeResourcePermissionsResponseTypeDef](./type_defs.md#describeresourcepermissionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeResourcePermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceId: str,
    AuthenticationToken: str = ...,
    PrincipalId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeResourcePermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeResourcePermissionsResponseTypeDef](./type_defs.md#describeresourcepermissionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef](./type_defs.md#describeresourcepermissionsrequestdescriberesourcepermissionspaginatetypedef) 
## DescribeRootFoldersPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_root_folders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)

```python
# DescribeRootFoldersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeRootFoldersPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRootFoldersResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeRootFoldersPaginator](./paginators.md#describerootfolderspaginator)
3. item: [:material-code-braces: DescribeRootFoldersResponseTypeDef](./type_defs.md#describerootfoldersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRootFoldersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AuthenticationToken: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRootFoldersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRootFoldersResponseTypeDef](./type_defs.md#describerootfoldersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = {  # (1)
    "AuthenticationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef](./type_defs.md#describerootfoldersrequestdescriberootfolderspaginatetypedef) 
## DescribeUsersPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("describe_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers)

```python
# DescribeUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import DescribeUsersPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
3. item: [:material-code-braces: DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AuthenticationToken: str = ...,
    OrganizationId: str = ...,
    UserIds: str = ...,
    Query: str = ...,
    Include: UserFilterTypeType = ...,  # (1)
    Order: OrderTypeType = ...,  # (2)
    Sort: UserSortTypeType = ...,  # (3)
    Fields: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[DescribeUsersResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: UserFilterTypeType](./literals.md#userfiltertypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: UserSortTypeType](./literals.md#usersorttypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUsersRequestDescribeUsersPaginateTypeDef = {  # (1)
    "AuthenticationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsersRequestDescribeUsersPaginateTypeDef](./type_defs.md#describeusersrequestdescribeuserspaginatetypedef) 
## SearchResourcesPaginator

Type annotations and code completion for `#!python session.create_client("workdocs").get_paginator("search_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources)

```python
# SearchResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.paginator import SearchResourcesPaginator

session = get_session()
async with session.create_client("workdocs") as client:  # (1)
    paginator: SearchResourcesPaginator = client.get_paginator("search_resources")  # (2)
    async for item in paginator.paginate(...):
        item: SearchResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)
3. item: [:material-code-braces: SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AuthenticationToken: str = ...,
    QueryText: str = ...,
    QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,  # (1)
    OrganizationId: str = ...,
    AdditionalResponseFields: Sequence[AdditionalResponseFieldTypeType] = ...,  # (2)
    Filters: FiltersTypeDef = ...,  # (3)
    OrderBy: Sequence[SearchSortResultTypeDef] = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[SearchResourcesResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: SearchQueryScopeTypeType](./literals.md#searchqueryscopetypetype) 
2. See [:material-code-brackets: AdditionalResponseFieldTypeType](./literals.md#additionalresponsefieldtypetype) 
3. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
4. See [:material-code-braces: SearchSortResultTypeDef](./type_defs.md#searchsortresulttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchResourcesRequestSearchResourcesPaginateTypeDef = {  # (1)
    "AuthenticationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchResourcesRequestSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesrequestsearchresourcespaginatetypedef) 
