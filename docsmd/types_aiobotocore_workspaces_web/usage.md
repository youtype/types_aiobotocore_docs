# Examples

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#workspacesweb)
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
# ListDataProtectionSettingsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-web") as client:  # (1)
    paginator = client.get_paginator("list_data_protection_settings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListDataProtectionSettingsPaginator](./paginators.md#listdataprotectionsettingspaginator)
3. item: [:material-code-braces: ListDataProtectionSettingsResponseTypeDef](./type_defs.md#listdataprotectionsettingsresponsetypedef) 




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
from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestTypeDef


session = get_session()

async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
    kwargs: AssociateBrowserSettingsRequestTypeDef = {...}
    result: AssociateBrowserSettingsResponseTypeDef = await client.associate_browser_settings(**kwargs)
```



```python
# ListDataProtectionSettingsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
from types_aiobotocore_workspaces_web.paginator import ListDataProtectionSettingsPaginator
from types_aiobotocore_workspaces_web.type_defs import ListDataProtectionSettingsResponseTypeDef


session = get_session()

async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
    paginator: ListDataProtectionSettingsPaginator = client.get_paginator("list_data_protection_settings")
    async for item in paginator.paginate(...):
        item: ListDataProtectionSettingsResponseTypeDef
        print(item)
```


