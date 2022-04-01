# Examples

> [Index](../README.md) > [OpenSearchService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[opensearch]` package installed.

Write your `OpenSearchService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("opensearch") as client:  # (1)
        result = await client.accept_inbound_connection()  # (2)
    ```

    1. client: [OpenSearchServiceClient](./client.md)
    2. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[opensearch]`
or a standalone `types_aiobotocore_opensearch` package, you have to explicitly specify
`client: OpenSearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_opensearch.client import OpenSearchServiceClient
    from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionResponseTypeDef
    from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionRequestRequestTypeDef


    session = get_session()

    async with session.create_client("opensearch") as client:
        client: OpenSearchServiceClient
        kwargs: AcceptInboundConnectionRequestRequestTypeDef = {...}
        result: AcceptInboundConnectionResponseTypeDef = await client.accept_inbound_connection(**kwargs)
    ```




