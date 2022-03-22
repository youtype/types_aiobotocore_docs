<a id="examples-for-aiobotocore-opensearchservice-module"></a>

# Examples for aiobotocore OpenSearchService module

> [Index](../README.md) > [OpenSearchService](./README.md) > Examples

- [Examples for aiobotocore OpenSearchService module](#examples-for-aiobotocore-opensearchservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[opensearch]` package installed.

Write your `OpenSearchService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type OpenSearchServiceClient
# and provides type checking and code completion
async with session.create_client("opensearch") as client:
    
    # result has type AcceptInboundConnectionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_inbound_connection()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[opensearch]` or a standalone
`types_aiobotocore_opensearch` package, you have to explicitly specify
`client: OpenSearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient
from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionResponseTypeDef






session = get_session()

async with session.create_client("opensearch") as client:
    client: OpenSearchServiceClient

    
    result: AcceptInboundConnectionResponseTypeDef = client.accept_inbound_connection()
    

    

    
```
