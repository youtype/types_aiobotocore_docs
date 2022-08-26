# Paginators

> [Index](../README.md) > [CodeStar](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
    type annotations stubs module [types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).

## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codestar").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("codestar") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("codestar").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("codestar") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: [:material-code-braces: ListResourcesResultTypeDef](./type_defs.md#listresourcesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    projectId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourcesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourcesResultTypeDef](./type_defs.md#listresourcesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourcesRequestListResourcesPaginateTypeDef = {  # (1)
    "projectId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestListResourcesPaginateTypeDef](./type_defs.md#listresourcesrequestlistresourcespaginatetypedef) 
## ListTeamMembersPaginator

Type annotations and code completion for `#!python session.create_client("codestar").get_paginator("list_team_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListTeamMembersPaginator

session = get_session()
async with session.create_client("codestar") as client:  # (1)
    paginator: ListTeamMembersPaginator = client.get_paginator("list_team_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListTeamMembersResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarClient](./client.md)
2. paginator: [ListTeamMembersPaginator](./paginators.md#listteammemberspaginator)
3. item: [:material-code-braces: ListTeamMembersResultTypeDef](./type_defs.md#listteammembersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTeamMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    projectId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTeamMembersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTeamMembersResultTypeDef](./type_defs.md#listteammembersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTeamMembersRequestListTeamMembersPaginateTypeDef = {  # (1)
    "projectId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTeamMembersRequestListTeamMembersPaginateTypeDef](./type_defs.md#listteammembersrequestlistteammemberspaginatetypedef) 
## ListUserProfilesPaginator

Type annotations and code completion for `#!python session.create_client("codestar").get_paginator("list_user_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListUserProfilesPaginator

session = get_session()
async with session.create_client("codestar") as client:  # (1)
    paginator: ListUserProfilesPaginator = client.get_paginator("list_user_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserProfilesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarClient](./client.md)
2. paginator: [ListUserProfilesPaginator](./paginators.md#listuserprofilespaginator)
3. item: [:material-code-braces: ListUserProfilesResultTypeDef](./type_defs.md#listuserprofilesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListUserProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserProfilesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserProfilesResultTypeDef](./type_defs.md#listuserprofilesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserProfilesRequestListUserProfilesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserProfilesRequestListUserProfilesPaginateTypeDef](./type_defs.md#listuserprofilesrequestlistuserprofilespaginatetypedef) 
