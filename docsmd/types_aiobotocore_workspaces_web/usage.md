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



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("workspaces-web") as client:  # (1)
        result = await client.associate_browser_settings()  # (2)
    ```

    1. client: [WorkSpacesWebClient](./client.md)
    2. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[workspaces-web]`
or a standalone `types_aiobotocore_workspaces_web` package, you have to explicitly specify
`client: WorkSpacesWebClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
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




