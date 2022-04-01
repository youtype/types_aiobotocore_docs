# Examples

> [Index](../README.md) > [PI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pi]` package installed.

Write your `PI` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("pi") as client:  # (1)
        result = await client.describe_dimension_keys()  # (2)
    ```

    1. client: [PIClient](./client.md)
    2. result: [:material-code-braces: DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[pi]`
or a standalone `types_aiobotocore_pi` package, you have to explicitly specify
`client: PIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_pi.client import PIClient
    from types_aiobotocore_pi.type_defs import DescribeDimensionKeysResponseTypeDef
    from types_aiobotocore_pi.type_defs import DescribeDimensionKeysRequestRequestTypeDef


    session = get_session()

    async with session.create_client("pi") as client:
        client: PIClient
        kwargs: DescribeDimensionKeysRequestRequestTypeDef = {...}
        result: DescribeDimensionKeysResponseTypeDef = await client.describe_dimension_keys(**kwargs)
    ```




