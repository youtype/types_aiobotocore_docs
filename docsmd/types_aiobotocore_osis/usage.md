# Examples

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[osis]` package installed.

Write your `OpenSearchIngestion` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OpenSearchIngestionClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("osis") as client:  # (1)
    result = await client.create_pipeline()  # (2)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. result: [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)



#### Paginator usage example

```python
# ListPipelineEndpointConnectionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("osis") as client:  # (1)
    paginator = client.get_paginator("list_pipeline_endpoint_connections")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. paginator: [ListPipelineEndpointConnectionsPaginator](./paginators.md#listpipelineendpointconnectionspaginator)
3. item: [:material-code-braces: ListPipelineEndpointConnectionsResponseTypeDef](./type_defs.md#listpipelineendpointconnectionsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[osis]`
or a standalone `types_aiobotocore_osis` package, you have to explicitly specify
`client: OpenSearchIngestionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OpenSearchIngestionClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_osis.client import OpenSearchIngestionClient
from types_aiobotocore_osis.type_defs import CreatePipelineResponseTypeDef
from types_aiobotocore_osis.type_defs import CreatePipelineRequestTypeDef


session = get_session()

async with session.create_client("osis") as client:
    client: OpenSearchIngestionClient
    kwargs: CreatePipelineRequestTypeDef = {...}
    result: CreatePipelineResponseTypeDef = await client.create_pipeline(**kwargs)
```



#### Paginator usage example

```python
# ListPipelineEndpointConnectionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_osis.client import OpenSearchIngestionClient
from types_aiobotocore_osis.paginator import ListPipelineEndpointConnectionsPaginator
from types_aiobotocore_osis.type_defs import ListPipelineEndpointConnectionsResponseTypeDef


session = get_session()

async with session.create_client("osis") as client:
    client: OpenSearchIngestionClient
    paginator: ListPipelineEndpointConnectionsPaginator = client.get_paginator("list_pipeline_endpoint_connections")
    async for item in paginator.paginate(...):
        item: ListPipelineEndpointConnectionsResponseTypeDef
        print(item)
```


