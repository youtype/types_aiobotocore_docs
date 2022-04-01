# Examples

> [Index](../README.md) > [ManagedBlockchain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
    type annotations stubs module [types-aiobotocore-managedblockchain](https://pypi.org/project/types-aiobotocore-managedblockchain/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[managedblockchain]` package installed.

Write your `ManagedBlockchain` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("managedblockchain") as client:  # (1)
        result = await client.create_member()  # (2)
    ```

    1. client: [ManagedBlockchainClient](./client.md)
    2. result: [:material-code-braces: CreateMemberOutputTypeDef](./type_defs.md#creatememberoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[managedblockchain]`
or a standalone `types_aiobotocore_managedblockchain` package, you have to explicitly specify
`client: ManagedBlockchainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient
    from types_aiobotocore_managedblockchain.type_defs import CreateMemberOutputTypeDef
    from types_aiobotocore_managedblockchain.type_defs import CreateMemberInputRequestTypeDef


    session = get_session()

    async with session.create_client("managedblockchain") as client:
        client: ManagedBlockchainClient
        kwargs: CreateMemberInputRequestTypeDef = {...}
        result: CreateMemberOutputTypeDef = await client.create_member(**kwargs)
    ```




