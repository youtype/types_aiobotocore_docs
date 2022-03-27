# Examples

> [Index](../README.md) > [IdentityStore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[identitystore]` package installed.

Write your `IdentityStore` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("identitystore") as client:  # (1)
        result = await client.describe_group()  # (2)
    ```

    1. client: [IdentityStoreClient](./client.md)
    2. result: [:material-code-braces: DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[identitystore]`
or a standalone `types_aiobotocore_identitystore` package, you have to explicitly specify
`client: IdentityStoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_identitystore.client import IdentityStoreClient
    from types_aiobotocore_identitystore.type_defs import DescribeGroupResponseTypeDef
    from types_aiobotocore_identitystore.type_defs import DescribeGroupRequestRequestTypeDef


    session = get_session()

    async with session.create_client("identitystore") as client:
        client: IdentityStoreClient
        kwargs: DescribeGroupRequestRequestTypeDef = {...}
        result: DescribeGroupResponseTypeDef = await client.describe_group(**kwargs)
    ```




