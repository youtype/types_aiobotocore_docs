# Examples

> [Index](../README.md) > [OpenSearchService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#opensearchservice)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[opensearch]` package installed.

Write your `OpenSearchService` code as usual,
type checking and code completion should work out of the box.



```python
# OpenSearchServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opensearch") as client:  # (1)
    result = await client.accept_inbound_connection()  # (2)
```

1. client: [OpenSearchServiceClient](./client.md)
2. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opensearch") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpenSearchServiceClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[opensearch]`
or a standalone `types_aiobotocore_opensearch` package, you have to explicitly specify
`client: OpenSearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OpenSearchServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient
from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionResponseTypeDef
from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionRequestTypeDef


session = get_session()

async with session.create_client("opensearch") as client:
    client: OpenSearchServiceClient
    kwargs: AcceptInboundConnectionRequestTypeDef = {...}
    result: AcceptInboundConnectionResponseTypeDef = await client.accept_inbound_connection(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opensearch.client import OpenSearchServiceClient
from types_aiobotocore_opensearch.paginator import ListApplicationsPaginator
from types_aiobotocore_opensearch.type_defs import ListApplicationsResponseTypeDef


session = get_session()

async with session.create_client("opensearch") as client:
    client: OpenSearchServiceClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
```


