# Examples

> [Index](../README.md) > [AppConfig](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appconfig]` package installed.

Write your `AppConfig` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("appconfig") as client:  # (1)
        result = await client.create_application()  # (2)
    ```

    1. client: [AppConfigClient](./client.md)
    2. result: [:material-code-braces: ApplicationResponseMetadataTypeDef](./type_defs.md#applicationresponsemetadatatypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[appconfig]`
or a standalone `types_aiobotocore_appconfig` package, you have to explicitly specify
`client: AppConfigClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_appconfig.client import AppConfigClient
    from types_aiobotocore_appconfig.type_defs import ApplicationResponseMetadataTypeDef
    from types_aiobotocore_appconfig.type_defs import CreateApplicationRequestRequestTypeDef


    session = get_session()

    async with session.create_client("appconfig") as client:
        client: AppConfigClient
        kwargs: CreateApplicationRequestRequestTypeDef = {...}
        result: ApplicationResponseMetadataTypeDef = await client.create_application(**kwargs)
    ```




