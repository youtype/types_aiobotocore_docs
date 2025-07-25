# Examples

> [Index](../README.md) > [MultipartyApproval](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MultipartyApproval](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa.html#multipartyapproval)
    type annotations stubs module [types-aiobotocore-mpa](https://pypi.org/project/types-aiobotocore-mpa/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mpa]` package installed.

Write your `MultipartyApproval` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MultipartyApprovalClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mpa") as client:  # (1)
    result = await client.create_approval_team()  # (2)
```

1. client: [MultipartyApprovalClient](./client.md)
2. result: [:material-code-braces: CreateApprovalTeamResponseTypeDef](./type_defs.md#createapprovalteamresponsetypedef)



#### Paginator usage example

```python
# ListApprovalTeamsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mpa") as client:  # (1)
    paginator = client.get_paginator("list_approval_teams")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListApprovalTeamsPaginator](./paginators.md#listapprovalteamspaginator)
3. item: [:material-code-braces: ListApprovalTeamsResponseTypeDef](./type_defs.md#listapprovalteamsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[mpa]`
or a standalone `types_aiobotocore_mpa` package, you have to explicitly specify
`client: MultipartyApprovalClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MultipartyApprovalClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mpa.client import MultipartyApprovalClient
from types_aiobotocore_mpa.type_defs import CreateApprovalTeamResponseTypeDef
from types_aiobotocore_mpa.type_defs import CreateApprovalTeamRequestTypeDef


session = get_session()

async with session.create_client("mpa") as client:
    client: MultipartyApprovalClient
    kwargs: CreateApprovalTeamRequestTypeDef = {...}
    result: CreateApprovalTeamResponseTypeDef = await client.create_approval_team(**kwargs)
```



#### Paginator usage example

```python
# ListApprovalTeamsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mpa.client import MultipartyApprovalClient
from types_aiobotocore_mpa.paginator import ListApprovalTeamsPaginator
from types_aiobotocore_mpa.type_defs import ListApprovalTeamsResponseTypeDef


session = get_session()

async with session.create_client("mpa") as client:
    client: MultipartyApprovalClient
    paginator: ListApprovalTeamsPaginator = client.get_paginator("list_approval_teams")
    async for item in paginator.paginate(...):
        item: ListApprovalTeamsResponseTypeDef
        print(item)
```


