<a id="paginators-for-aiobotocore-codestar-module"></a>

# Paginators for aiobotocore CodeStar module

> [Index](..) > [CodeStar](.) > Paginators

Auto-generated documentation for
[CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
type annotations stubs module
[types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).

- [Paginators for aiobotocore CodeStar module](#paginators-for-aiobotocore-codestar-module)
  - [ListProjectsPaginator](#listprojectspaginator)
  - [ListResourcesPaginator](#listresourcespaginator)
  - [ListTeamMembersPaginator](#listteammemberspaginator)
  - [ListUserProfilesPaginator](#listuserprofilespaginator)

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("codestar").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[CodeStar.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`AsyncIterable`\[[ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef)\].

<a id="listresourcespaginator"></a>

## ListResourcesPaginator

Type annotations for
`session.create_client("codestar").get_paginator("list_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")
```

Boto3 documentation:
[CodeStar.Paginator.ListResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)

Arguments for `ListResourcesPaginator.paginate` method:

- `projectId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourcesPaginator.paginate` returns
`AsyncIterable`\[[ListResourcesResultTypeDef](./type_defs.md#listresourcesresulttypedef)\].

<a id="listteammemberspaginator"></a>

## ListTeamMembersPaginator

Type annotations for
`session.create_client("codestar").get_paginator("list_team_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListTeamMembersPaginator

session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
    paginator: ListTeamMembersPaginator = client.get_paginator("list_team_members")
```

Boto3 documentation:
[CodeStar.Paginator.ListTeamMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)

Arguments for `ListTeamMembersPaginator.paginate` method:

- `projectId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTeamMembersPaginator.paginate` returns
`AsyncIterable`\[[ListTeamMembersResultTypeDef](./type_defs.md#listteammembersresulttypedef)\].

<a id="listuserprofilespaginator"></a>

## ListUserProfilesPaginator

Type annotations for
`session.create_client("codestar").get_paginator("list_user_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar.paginator import ListUserProfilesPaginator

session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
    paginator: ListUserProfilesPaginator = client.get_paginator("list_user_profiles")
```

Boto3 documentation:
[CodeStar.Paginator.ListUserProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)

Arguments for `ListUserProfilesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUserProfilesPaginator.paginate` returns
`AsyncIterable`\[[ListUserProfilesResultTypeDef](./type_defs.md#listuserprofilesresulttypedef)\].
