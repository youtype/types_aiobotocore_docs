# Paginators

> [Index](../README.md) > [GameSparks](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GameSparks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
    type annotations stubs module [types-aiobotocore-gamesparks](https://pypi.org/project/types-aiobotocore-gamesparks/).

## ListExtensionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_extension_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListExtensionVersionsPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListExtensionVersionsPaginator = client.get_paginator("list_extension_versions")
```


### paginate

Type annotations and code completion for `#!python ListExtensionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListExtensionVersionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExtensionVersionsResultTypeDef](./type_defs.md#listextensionversionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = {  # (1)
    "Name": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef](./type_defs.md#listextensionversionsrequestlistextensionversionspaginatetypedef) 
## ListExtensionsPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_extensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListExtensionsPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListExtensionsPaginator = client.get_paginator("list_extensions")
```


### paginate

Type annotations and code completion for `#!python ListExtensionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListExtensionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExtensionsResultTypeDef](./type_defs.md#listextensionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListExtensionsRequestListExtensionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExtensionsRequestListExtensionsPaginateTypeDef](./type_defs.md#listextensionsrequestlistextensionspaginatetypedef) 
## ListGamesPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_games")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListGamesPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListGamesPaginator = client.get_paginator("list_games")
```


### paginate

Type annotations and code completion for `#!python ListGamesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGamesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGamesResultTypeDef](./type_defs.md#listgamesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListGamesRequestListGamesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGamesRequestListGamesPaginateTypeDef](./type_defs.md#listgamesrequestlistgamespaginatetypedef) 
## ListGeneratedCodeJobsPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_generated_code_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListGeneratedCodeJobsPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListGeneratedCodeJobsPaginator = client.get_paginator("list_generated_code_jobs")
```


### paginate

Type annotations and code completion for `#!python ListGeneratedCodeJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GameName: str,
    SnapshotId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGeneratedCodeJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeneratedCodeJobsResultTypeDef](./type_defs.md#listgeneratedcodejobsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = {  # (1)
    "GameName": ...,
    "SnapshotId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef](./type_defs.md#listgeneratedcodejobsrequestlistgeneratedcodejobspaginatetypedef) 
## ListSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListSnapshotsPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")
```


### paginate

Type annotations and code completion for `#!python ListSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GameName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSnapshotsResultTypeDef](./type_defs.md#listsnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSnapshotsRequestListSnapshotsPaginateTypeDef = {  # (1)
    "GameName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotsRequestListSnapshotsPaginateTypeDef](./type_defs.md#listsnapshotsrequestlistsnapshotspaginatetypedef) 
## ListStageDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_stage_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListStageDeploymentsPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListStageDeploymentsPaginator = client.get_paginator("list_stage_deployments")
```


### paginate

Type annotations and code completion for `#!python ListStageDeploymentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GameName: str,
    StageName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStageDeploymentsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStageDeploymentsResultTypeDef](./type_defs.md#liststagedeploymentsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = {  # (1)
    "GameName": ...,
    "StageName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef](./type_defs.md#liststagedeploymentsrequestliststagedeploymentspaginatetypedef) 
## ListStagesPaginator

Type annotations and code completion for `#!python session.create_client("gamesparks").get_paginator("list_stages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_gamesparks.paginator import ListStagesPaginator

session = get_session()
async with session.create_client("gamesparks") as client:
    client: GameSparksClient
    paginator: ListStagesPaginator = client.get_paginator("list_stages")
```


### paginate

Type annotations and code completion for `#!python ListStagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GameName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStagesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStagesResultTypeDef](./type_defs.md#liststagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListStagesRequestListStagesPaginateTypeDef = {  # (1)
    "GameName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStagesRequestListStagesPaginateTypeDef](./type_defs.md#liststagesrequestliststagespaginatetypedef) 
