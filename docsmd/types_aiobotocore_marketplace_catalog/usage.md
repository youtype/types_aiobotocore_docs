# Examples

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-catalog]` package installed.

Write your `MarketplaceCatalog` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("marketplace-catalog") as client:  # (1)
        result = await client.cancel_change_set()  # (2)
    ```

    1. client: [MarketplaceCatalogClient](./client.md)
    2. result: [:material-code-braces: CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[marketplace-catalog]`
or a standalone `types_aiobotocore_marketplace_catalog` package, you have to explicitly specify
`client: MarketplaceCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient
    from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetResponseTypeDef
    from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef


    session = get_session()

    async with session.create_client("marketplace-catalog") as client:
        client: MarketplaceCatalogClient
        kwargs: CancelChangeSetRequestRequestTypeDef = {...}
        result: CancelChangeSetResponseTypeDef = await client.cancel_change_set(**kwargs)
    ```




