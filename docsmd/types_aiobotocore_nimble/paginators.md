# Paginators

> [Index](../README.md) > [NimbleStudio](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
    type annotations stubs module [types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

## ListEulaAcceptancesPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_eula_acceptances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListEulaAcceptancesPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListEulaAcceptancesPaginator = client.get_paginator("list_eula_acceptances")  # (2)
    async for item in paginator.paginate(...):
        item: ListEulaAcceptancesResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListEulaAcceptancesPaginator](./paginators.md#listeulaacceptancespaginator)
3. item: [:material-code-braces: ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEulaAcceptancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    eulaIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEulaAcceptancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef](./type_defs.md#listeulaacceptancesrequestlisteulaacceptancespaginatetypedef) 
## ListEulasPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_eulas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulas)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListEulasPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListEulasPaginator = client.get_paginator("list_eulas")  # (2)
    async for item in paginator.paginate(...):
        item: ListEulasResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListEulasPaginator](./paginators.md#listeulaspaginator)
3. item: [:material-code-braces: ListEulasResponseTypeDef](./type_defs.md#listeulasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEulasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    eulaIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEulasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEulasResponseTypeDef](./type_defs.md#listeulasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEulasRequestListEulasPaginateTypeDef = {  # (1)
    "eulaIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEulasRequestListEulasPaginateTypeDef](./type_defs.md#listeulasrequestlisteulaspaginatetypedef) 
## ListLaunchProfileMembersPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_launch_profile_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfileMembers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListLaunchProfileMembersPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListLaunchProfileMembersPaginator = client.get_paginator("list_launch_profile_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchProfileMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListLaunchProfileMembersPaginator](./paginators.md#listlaunchprofilememberspaginator)
3. item: [:material-code-braces: ListLaunchProfileMembersResponseTypeDef](./type_defs.md#listlaunchprofilemembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchProfileMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    launchProfileId: str,
    studioId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLaunchProfileMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLaunchProfileMembersResponseTypeDef](./type_defs.md#listlaunchprofilemembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef = {  # (1)
    "launchProfileId": ...,
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef](./type_defs.md#listlaunchprofilemembersrequestlistlaunchprofilememberspaginatetypedef) 
## ListLaunchProfilesPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_launch_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListLaunchProfilesPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListLaunchProfilesPaginator = client.get_paginator("list_launch_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListLaunchProfilesPaginator](./paginators.md#listlaunchprofilespaginator)
3. item: [:material-code-braces: ListLaunchProfilesResponseTypeDef](./type_defs.md#listlaunchprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    principalId: str = ...,
    states: Sequence[LaunchProfileStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListLaunchProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LaunchProfileStateType](./literals.md#launchprofilestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLaunchProfilesResponseTypeDef](./type_defs.md#listlaunchprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef](./type_defs.md#listlaunchprofilesrequestlistlaunchprofilespaginatetypedef) 
## ListStreamingImagesPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_streaming_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingImages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStreamingImagesPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListStreamingImagesPaginator = client.get_paginator("list_streaming_images")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamingImagesResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListStreamingImagesPaginator](./paginators.md#liststreamingimagespaginator)
3. item: [:material-code-braces: ListStreamingImagesResponseTypeDef](./type_defs.md#liststreamingimagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamingImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    owner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamingImagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamingImagesResponseTypeDef](./type_defs.md#liststreamingimagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamingImagesRequestListStreamingImagesPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamingImagesRequestListStreamingImagesPaginateTypeDef](./type_defs.md#liststreamingimagesrequestliststreamingimagespaginatetypedef) 
## ListStreamingSessionsPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_streaming_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStreamingSessionsPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListStreamingSessionsPaginator = client.get_paginator("list_streaming_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamingSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListStreamingSessionsPaginator](./paginators.md#liststreamingsessionspaginator)
3. item: [:material-code-braces: ListStreamingSessionsResponseTypeDef](./type_defs.md#liststreamingsessionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamingSessionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    createdBy: str = ...,
    ownedBy: str = ...,
    sessionIds: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamingSessionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamingSessionsResponseTypeDef](./type_defs.md#liststreamingsessionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef](./type_defs.md#liststreamingsessionsrequestliststreamingsessionspaginatetypedef) 
## ListStudioComponentsPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_studio_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudioComponentsPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListStudioComponentsPaginator = client.get_paginator("list_studio_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudioComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListStudioComponentsPaginator](./paginators.md#liststudiocomponentspaginator)
3. item: [:material-code-braces: ListStudioComponentsResponseTypeDef](./type_defs.md#liststudiocomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStudioComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    states: Sequence[StudioComponentStateType] = ...,  # (1)
    types: Sequence[StudioComponentTypeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListStudioComponentsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: StudioComponentStateType](./literals.md#studiocomponentstatetype) 
2. See [:material-code-brackets: StudioComponentTypeType](./literals.md#studiocomponenttypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListStudioComponentsResponseTypeDef](./type_defs.md#liststudiocomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStudioComponentsRequestListStudioComponentsPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudioComponentsRequestListStudioComponentsPaginateTypeDef](./type_defs.md#liststudiocomponentsrequestliststudiocomponentspaginatetypedef) 
## ListStudioMembersPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_studio_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioMembers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudioMembersPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListStudioMembersPaginator = client.get_paginator("list_studio_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudioMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListStudioMembersPaginator](./paginators.md#liststudiomemberspaginator)
3. item: [:material-code-braces: ListStudioMembersResponseTypeDef](./type_defs.md#liststudiomembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStudioMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    studioId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStudioMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStudioMembersResponseTypeDef](./type_defs.md#liststudiomembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStudioMembersRequestListStudioMembersPaginateTypeDef = {  # (1)
    "studioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudioMembersRequestListStudioMembersPaginateTypeDef](./type_defs.md#liststudiomembersrequestliststudiomemberspaginatetypedef) 
## ListStudiosPaginator

Type annotations and code completion for `#!python session.create_client("nimble").get_paginator("list_studios")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudios)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_nimble.paginator import ListStudiosPaginator

session = get_session()
async with session.create_client("nimble") as client:  # (1)
    paginator: ListStudiosPaginator = client.get_paginator("list_studios")  # (2)
    async for item in paginator.paginate(...):
        item: ListStudiosResponseTypeDef
        print(item)  # (3)
```

1. client: [NimbleStudioClient](./client.md)
2. paginator: [ListStudiosPaginator](./paginators.md#liststudiospaginator)
3. item: [:material-code-braces: ListStudiosResponseTypeDef](./type_defs.md#liststudiosresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStudiosPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStudiosResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStudiosResponseTypeDef](./type_defs.md#liststudiosresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStudiosRequestListStudiosPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStudiosRequestListStudiosPaginateTypeDef](./type_defs.md#liststudiosrequestliststudiospaginatetypedef) 
