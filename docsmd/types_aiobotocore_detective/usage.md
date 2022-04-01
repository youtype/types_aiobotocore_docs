# Examples

> [Index](../README.md) > [Detective](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[detective]` package installed.

Write your `Detective` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("detective") as client:  # (1)
        result = await client.create_graph()  # (2)
    ```

    1. client: [DetectiveClient](./client.md)
    2. result: [:material-code-braces: CreateGraphResponseTypeDef](./type_defs.md#creategraphresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[detective]`
or a standalone `types_aiobotocore_detective` package, you have to explicitly specify
`client: DetectiveClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_detective.client import DetectiveClient
    from types_aiobotocore_detective.type_defs import CreateGraphResponseTypeDef
    from types_aiobotocore_detective.type_defs import CreateGraphRequestRequestTypeDef


    session = get_session()

    async with session.create_client("detective") as client:
        client: DetectiveClient
        kwargs: CreateGraphRequestRequestTypeDef = {...}
        result: CreateGraphResponseTypeDef = await client.create_graph(**kwargs)
    ```




