# Examples

> [Index](../README.md) > [imagebuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[imagebuilder]` package installed.

Write your `imagebuilder` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("imagebuilder") as client:  # (1)
        result = await client.cancel_image_creation()  # (2)
    ```

    1. client: [imagebuilderClient](./client.md)
    2. result: [:material-code-braces: CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[imagebuilder]`
or a standalone `types_aiobotocore_imagebuilder` package, you have to explicitly specify
`client: imagebuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_imagebuilder.client import imagebuilderClient
    from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationResponseTypeDef
    from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationRequestRequestTypeDef


    session = get_session()

    async with session.create_client("imagebuilder") as client:
        client: imagebuilderClient
        kwargs: CancelImageCreationRequestRequestTypeDef = {...}
        result: CancelImageCreationResponseTypeDef = await client.cancel_image_creation(**kwargs)
    ```




