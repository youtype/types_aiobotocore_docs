<a id="examples-for-aiobotocore-workspacesweb-module"></a>

# Examples for aiobotocore WorkSpacesWeb module

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Examples

- [Examples for aiobotocore WorkSpacesWeb module](#examples-for-aiobotocore-workspacesweb-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces-web]` package installed.

Write your `WorkSpacesWeb` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WorkSpacesWebClient
# and provides type checking and code completion
async with session.create_client("workspaces-web") as client:
    
    # result has type AssociateBrowserSettingsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_browser_settings()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[workspaces-web]` or a standalone
`types_aiobotocore_workspaces_web` package, you have to explicitly specify
`client: WorkSpacesWebClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsResponseTypeDef






session = get_session()

async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient

    
    result: AssociateBrowserSettingsResponseTypeDef = client.associate_browser_settings()
    

    

    
```
