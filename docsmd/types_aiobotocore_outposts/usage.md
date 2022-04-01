# Examples

> [Index](../README.md) > [Outposts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[outposts]` package installed.

Write your `Outposts` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("outposts") as client:  # (1)
        result = await client.create_order()  # (2)
    ```

    1. client: [OutpostsClient](./client.md)
    2. result: [:material-code-braces: CreateOrderOutputTypeDef](./type_defs.md#createorderoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[outposts]`
or a standalone `types_aiobotocore_outposts` package, you have to explicitly specify
`client: OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_outposts.client import OutpostsClient
    from types_aiobotocore_outposts.type_defs import CreateOrderOutputTypeDef
    from types_aiobotocore_outposts.type_defs import CreateOrderInputRequestTypeDef


    session = get_session()

    async with session.create_client("outposts") as client:
        client: OutpostsClient
        kwargs: CreateOrderInputRequestTypeDef = {...}
        result: CreateOrderOutputTypeDef = await client.create_order(**kwargs)
    ```




