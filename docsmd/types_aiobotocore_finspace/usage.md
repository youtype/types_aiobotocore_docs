# Examples

> [Index](../README.md) > [finspace](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[finspace]` package installed.

Write your `finspace` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("finspace") as client:  # (1)
        result = await client.create_environment()  # (2)
    ```

    1. client: [finspaceClient](./client.md)
    2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[finspace]`
or a standalone `types_aiobotocore_finspace` package, you have to explicitly specify
`client: finspaceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_finspace.client import finspaceClient
    from types_aiobotocore_finspace.type_defs import CreateEnvironmentResponseTypeDef
    from types_aiobotocore_finspace.type_defs import CreateEnvironmentRequestRequestTypeDef


    session = get_session()

    async with session.create_client("finspace") as client:
        client: finspaceClient
        kwargs: CreateEnvironmentRequestRequestTypeDef = {...}
        result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)
    ```




