# Examples

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appintegrations]` package installed.

Write your `AppIntegrationsService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("appintegrations") as client:  # (1)
        result = await client.create_data_integration()  # (2)
    ```

    1. client: [AppIntegrationsServiceClient](./client.md)
    2. result: [:material-code-braces: CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[appintegrations]`
or a standalone `types_aiobotocore_appintegrations` package, you have to explicitly specify
`client: AppIntegrationsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
    from types_aiobotocore_appintegrations.type_defs import CreateDataIntegrationResponseTypeDef
    from types_aiobotocore_appintegrations.type_defs import CreateDataIntegrationRequestRequestTypeDef


    session = get_session()

    async with session.create_client("appintegrations") as client:
        client: AppIntegrationsServiceClient
        kwargs: CreateDataIntegrationRequestRequestTypeDef = {...}
        result: CreateDataIntegrationResponseTypeDef = await client.create_data_integration(**kwargs)
    ```




