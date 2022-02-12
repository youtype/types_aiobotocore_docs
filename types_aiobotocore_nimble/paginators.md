<a id="paginators-for-aiobotocore-nimblestudio-module"></a>

# Paginators for aiobotocore NimbleStudio module

> [Index](..) > [NimbleStudio](.) > Paginators

Auto-generated documentation for
[NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
type annotations stubs module
[types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

- [Paginators for aiobotocore NimbleStudio module](#paginators-for-aiobotocore-nimblestudio-module)
  - [ListEulaAcceptancesPaginator](#listeulaacceptancespaginator)
  - [ListEulasPaginator](#listeulaspaginator)
  - [ListLaunchProfileMembersPaginator](#listlaunchprofilememberspaginator)
  - [ListLaunchProfilesPaginator](#listlaunchprofilespaginator)
  - [ListStreamingImagesPaginator](#liststreamingimagespaginator)
  - [ListStreamingSessionsPaginator](#liststreamingsessionspaginator)
  - [ListStudioComponentsPaginator](#liststudiocomponentspaginator)
  - [ListStudioMembersPaginator](#liststudiomemberspaginator)
  - [ListStudiosPaginator](#liststudiospaginator)

<a id="listeulaacceptancespaginator"></a>

## ListEulaAcceptancesPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_eula_acceptances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListEulaAcceptancesPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListEulaAcceptancesPaginator = client.get_paginator("list_eula_acceptances")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListEulaAcceptances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances)

Arguments for `ListEulaAcceptancesPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `eulaIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEulaAcceptancesPaginator.paginate` returns
`AsyncIterable`\[[ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef)\].

<a id="listeulaspaginator"></a>

## ListEulasPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_eulas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListEulasPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListEulasPaginator = client.get_paginator("list_eulas")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListEulas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)

Arguments for `ListEulasPaginator.paginate` method:

- `eulaIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEulasPaginator.paginate` returns
`AsyncIterable`\[[ListEulasResponseTypeDef](./type_defs.md#listeulasresponsetypedef)\].

<a id="listlaunchprofilememberspaginator"></a>

## ListLaunchProfileMembersPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_launch_profile_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListLaunchProfileMembersPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListLaunchProfileMembersPaginator = client.get_paginator("list_launch_profile_members")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListLaunchProfileMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)

Arguments for `ListLaunchProfileMembersPaginator.paginate` method:

- `launchProfileId`: `str` *(required)*
- `studioId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLaunchProfileMembersPaginator.paginate` returns
`AsyncIterable`\[[ListLaunchProfileMembersResponseTypeDef](./type_defs.md#listlaunchprofilemembersresponsetypedef)\].

<a id="listlaunchprofilespaginator"></a>

## ListLaunchProfilesPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_launch_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListLaunchProfilesPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListLaunchProfilesPaginator = client.get_paginator("list_launch_profiles")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListLaunchProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles)

Arguments for `ListLaunchProfilesPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `principalId`: `str`
- `states`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLaunchProfilesPaginator.paginate` returns
`AsyncIterable`\[[ListLaunchProfilesResponseTypeDef](./type_defs.md#listlaunchprofilesresponsetypedef)\].

<a id="liststreamingimagespaginator"></a>

## ListStreamingImagesPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_streaming_images")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStreamingImagesPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListStreamingImagesPaginator = client.get_paginator("list_streaming_images")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListStreamingImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)

Arguments for `ListStreamingImagesPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `owner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamingImagesPaginator.paginate` returns
`AsyncIterable`\[[ListStreamingImagesResponseTypeDef](./type_defs.md#liststreamingimagesresponsetypedef)\].

<a id="liststreamingsessionspaginator"></a>

## ListStreamingSessionsPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_streaming_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStreamingSessionsPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListStreamingSessionsPaginator = client.get_paginator("list_streaming_sessions")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListStreamingSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions)

Arguments for `ListStreamingSessionsPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `createdBy`: `str`
- `ownedBy`: `str`
- `sessionIds`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamingSessionsPaginator.paginate` returns
`AsyncIterable`\[[ListStreamingSessionsResponseTypeDef](./type_defs.md#liststreamingsessionsresponsetypedef)\].

<a id="liststudiocomponentspaginator"></a>

## ListStudioComponentsPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_studio_components")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudioComponentsPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListStudioComponentsPaginator = client.get_paginator("list_studio_components")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListStudioComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents)

Arguments for `ListStudioComponentsPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `states`: `Sequence`\[`str`\]
- `types`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStudioComponentsPaginator.paginate` returns
`AsyncIterable`\[[ListStudioComponentsResponseTypeDef](./type_defs.md#liststudiocomponentsresponsetypedef)\].

<a id="liststudiomemberspaginator"></a>

## ListStudioMembersPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_studio_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudioMembersPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListStudioMembersPaginator = client.get_paginator("list_studio_members")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListStudioMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)

Arguments for `ListStudioMembersPaginator.paginate` method:

- `studioId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStudioMembersPaginator.paginate` returns
`AsyncIterable`\[[ListStudioMembersResponseTypeDef](./type_defs.md#liststudiomembersresponsetypedef)\].

<a id="liststudiospaginator"></a>

## ListStudiosPaginator

Type annotations for
`session.create_client("nimble").get_paginator("list_studios")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudiosPaginator

session = get_session()
async with session.create_client("nimble") as client:
    client: NimbleStudioClient
    paginator: ListStudiosPaginator = client.get_paginator("list_studios")
```

Boto3 documentation:
[NimbleStudio.Paginator.ListStudios](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)

Arguments for `ListStudiosPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStudiosPaginator.paginate` returns
`AsyncIterable`\[[ListStudiosResponseTypeDef](./type_defs.md#liststudiosresponsetypedef)\].
