# Examples

> [Index](../README.md) > [DataExchange](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dataexchange]` package installed.

Write your `DataExchange` code as usual,
type checking and code completion should work out of the box.



```python
# DataExchangeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dataexchange") as client:  # (1)
    result = await client.cancel_job()  # (2)
```

1. client: [DataExchangeClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListDataSetRevisionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dataexchange") as client:  # (1)
    paginator = client.get_paginator("list_data_set_revisions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataSetRevisionsPaginator](./paginators.md#listdatasetrevisionspaginator)
3. item: [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[dataexchange]`
or a standalone `types_aiobotocore_dataexchange` package, you have to explicitly specify
`client: DataExchangeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DataExchangeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_dataexchange.type_defs import CancelJobRequestRequestTypeDef


session = get_session()

async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    kwargs: CancelJobRequestRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.cancel_job(**kwargs)
```



```python
# ListDataSetRevisionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator
from types_aiobotocore_dataexchange.type_defs import ListDataSetRevisionsResponseTypeDef


session = get_session()

async with session.create_client("dataexchange") as client:
    client: DataExchangeClient
    paginator: ListDataSetRevisionsPaginator = client.get_paginator("list_data_set_revisions")
    async for item in paginator.paginate(...):
        item: ListDataSetRevisionsResponseTypeDef
        print(item)
```


