# Examples

> [Index](../README.md) > [Account](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[account]` package installed.

Write your `Account` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("account") as client:  # (1)
        result = await client.get_alternate_contact()  # (2)
    ```

    1. client: [AccountClient](./client.md)
    2. result: [:material-code-braces: GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[account]`
or a standalone `types_aiobotocore_account` package, you have to explicitly specify
`client: AccountClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_account.client import AccountClient
    from types_aiobotocore_account.type_defs import GetAlternateContactResponseTypeDef
    from types_aiobotocore_account.type_defs import GetAlternateContactRequestRequestTypeDef


    session = get_session()

    async with session.create_client("account") as client:
        client: AccountClient
        kwargs: GetAlternateContactRequestRequestTypeDef = {...}
        result: GetAlternateContactResponseTypeDef = await client.get_alternate_contact(**kwargs)
    ```




