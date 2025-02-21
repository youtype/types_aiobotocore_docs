# Examples

> [Index](../README.md) > [OpenSearchServiceServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#opensearchserviceserverless)
    type annotations stubs module [types-aiobotocore-opensearchserverless](https://pypi.org/project/types-aiobotocore-opensearchserverless/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[opensearchserverless]` package installed.

Write your `OpenSearchServiceServerless` code as usual,
type checking and code completion should work out of the box.



```python
# OpenSearchServiceServerlessClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opensearchserverless") as client:  # (1)
    result = await client.batch_get_collection()  # (2)
```

1. client: [OpenSearchServiceServerlessClient](./client.md)
2. result: [:material-code-braces: BatchGetCollectionResponseTypeDef](./type_defs.md#batchgetcollectionresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[opensearchserverless]`
or a standalone `types_aiobotocore_opensearchserverless` package, you have to explicitly specify
`client: OpenSearchServiceServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OpenSearchServiceServerlessClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opensearchserverless.client import OpenSearchServiceServerlessClient
from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionResponseTypeDef
from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionRequestTypeDef


session = get_session()

async with session.create_client("opensearchserverless") as client:
    client: OpenSearchServiceServerlessClient
    kwargs: BatchGetCollectionRequestTypeDef = {...}
    result: BatchGetCollectionResponseTypeDef = await client.batch_get_collection(**kwargs)
```




