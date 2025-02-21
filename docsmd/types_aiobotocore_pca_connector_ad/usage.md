# Examples

> [Index](../README.md) > [PcaConnectorAd](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad)
    type annotations stubs module [types-aiobotocore-pca-connector-ad](https://pypi.org/project/types-aiobotocore-pca-connector-ad/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pca-connector-ad]` package installed.

Write your `PcaConnectorAd` code as usual,
type checking and code completion should work out of the box.



```python
# PcaConnectorAdClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pca-connector-ad") as client:  # (1)
    result = await client.create_connector()  # (2)
```

1. client: [PcaConnectorAdClient](./client.md)
2. result: [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 



```python
# ListConnectorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pca-connector-ad") as client:  # (1)
    paginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PcaConnectorAdClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pca-connector-ad]`
or a standalone `types_aiobotocore_pca_connector_ad` package, you have to explicitly specify
`client: PcaConnectorAdClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PcaConnectorAdClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.client import PcaConnectorAdClient
from types_aiobotocore_pca_connector_ad.type_defs import CreateConnectorResponseTypeDef
from types_aiobotocore_pca_connector_ad.type_defs import CreateConnectorRequestTypeDef


session = get_session()

async with session.create_client("pca-connector-ad") as client:
    client: PcaConnectorAdClient
    kwargs: CreateConnectorRequestTypeDef = {...}
    result: CreateConnectorResponseTypeDef = await client.create_connector(**kwargs)
```



```python
# ListConnectorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_ad.client import PcaConnectorAdClient
from types_aiobotocore_pca_connector_ad.paginator import ListConnectorsPaginator
from types_aiobotocore_pca_connector_ad.type_defs import ListConnectorsResponseTypeDef


session = get_session()

async with session.create_client("pca-connector-ad") as client:
    client: PcaConnectorAdClient
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)
```


