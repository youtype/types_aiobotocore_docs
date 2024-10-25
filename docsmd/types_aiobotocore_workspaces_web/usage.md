# Examples

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces-web]` package installed.

Write your `WorkSpacesWeb` code as usual,
type checking and code completion should work out of the box.



```python
# WorkSpacesWebClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-web") as client:  # (1)
    result = await client.associate_browser_settings()  # (2)
```

1. client: [WorkSpacesWebClient](./client.md)
2. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 



```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-web") as client:  # (1)
    paginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[workspaces-web]`
or a standalone `types_aiobotocore_workspaces_web` package, you have to explicitly specify
`client: WorkSpacesWebClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkSpacesWebClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsResponseTypeDef
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef


session = get_session()

async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
    kwargs: AssociateBrowserSettingsRequestRequestTypeDef = {...}
    result: AssociateBrowserSettingsResponseTypeDef = await client.associate_browser_settings(**kwargs)
```



```python
# ListSessionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.paginator import ListSessionsPaginator
from types_aiobotocore_workspaces_web.type_defs import ListSessionsResponseTypeDef


session = get_session()

async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)
```


