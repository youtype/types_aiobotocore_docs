# Examples

> [Index](../README.md) > [WorkLink](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkLink](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
    type annotations stubs module [types-aiobotocore-worklink](https://pypi.org/project/types-aiobotocore-worklink/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[worklink]` package installed.

Write your `WorkLink` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("worklink") as client:  # (1)
        result = await client.associate_website_authorization_provider()  # (2)
    ```

    1. client: [WorkLinkClient](./client.md)
    2. result: [:material-code-braces: AssociateWebsiteAuthorizationProviderResponseTypeDef](./type_defs.md#associatewebsiteauthorizationproviderresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[worklink]`
or a standalone `types_aiobotocore_worklink` package, you have to explicitly specify
`client: WorkLinkClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_worklink.client import WorkLinkClient
    from types_aiobotocore_worklink.type_defs import AssociateWebsiteAuthorizationProviderResponseTypeDef
    from types_aiobotocore_worklink.type_defs import AssociateWebsiteAuthorizationProviderRequestRequestTypeDef


    session = get_session()

    async with session.create_client("worklink") as client:
        client: WorkLinkClient
        kwargs: AssociateWebsiteAuthorizationProviderRequestRequestTypeDef = {...}
        result: AssociateWebsiteAuthorizationProviderResponseTypeDef = await client.associate_website_authorization_provider(**kwargs)
    ```




