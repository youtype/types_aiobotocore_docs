# Examples

> [Index](../README.md) > [SES](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
    type annotations stubs module [types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ses]` package installed.

Write your `SES` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ses") as client:  # (1)
        result = await client.create_custom_verification_email_template()  # (2)
    ```

    1. client: [SESClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ses") as client:  # (1)
        paginator = client.get_paginator("list_configuration_sets")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SESClient](./client.md)
    2. paginator: [ListConfigurationSetsPaginator](./paginators.md#listconfigurationsetspaginator)
    3. item: [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ses") as client:  # (1)
        waiter = client.get_waiter("identity_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [SESClient](./client.md)
    2. waiter: [IdentityExistsWaiter](./waiters.md#identityexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ses]`
or a standalone `types_aiobotocore_ses` package, you have to explicitly specify
`client: SESClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ses.client import SESClient
    from types_aiobotocore_ses.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_ses.type_defs import CreateCustomVerificationEmailTemplateRequestRequestTypeDef


    session = get_session()

    async with session.create_client("ses") as client:
        client: SESClient
        kwargs: CreateCustomVerificationEmailTemplateRequestRequestTypeDef = {...}
        result: EmptyResponseMetadataTypeDef = await client.create_custom_verification_email_template(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ses.client import SESClient
    from types_aiobotocore_ses.paginator import ListConfigurationSetsPaginator
    from types_aiobotocore_ses.type_defs import ListConfigurationSetsResponseTypeDef


    session = get_session()

    async with session.create_client("ses") as client:
        client: SESClient
        paginator: ListConfigurationSetsPaginator = client.get_paginator("list_configuration_sets")
        async for item in paginator.paginate(...):
            item: ListConfigurationSetsResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ses.client import SESClient
    from types_aiobotocore_ses.waiter import IdentityExistsWaiter


    session = get_session()

    async with session.create_client("ses") as client:
        client: SESClient
        waiter: IdentityExistsWaiter = client.get_waiter("identity_exists")
        await waiter.wait()
    ```
