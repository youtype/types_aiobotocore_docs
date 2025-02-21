# Examples

> [Index](../README.md) > [PrivateCAConnectorforSCEP](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep)
    type annotations stubs module [types-aiobotocore-pca-connector-scep](https://pypi.org/project/types-aiobotocore-pca-connector-scep/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pca-connector-scep]` package installed.

Write your `PrivateCAConnectorforSCEP` code as usual,
type checking and code completion should work out of the box.



```python
# PrivateCAConnectorforSCEPClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pca-connector-scep") as client:  # (1)
    result = await client.create_challenge()  # (2)
```

1. client: [PrivateCAConnectorforSCEPClient](./client.md)
2. result: [:material-code-braces: CreateChallengeResponseTypeDef](./type_defs.md#createchallengeresponsetypedef) 



```python
# ListChallengeMetadataPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pca-connector-scep") as client:  # (1)
    paginator = client.get_paginator("list_challenge_metadata")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PrivateCAConnectorforSCEPClient](./client.md)
2. paginator: [ListChallengeMetadataPaginator](./paginators.md#listchallengemetadatapaginator)
3. item: [:material-code-braces: ListChallengeMetadataResponseTypeDef](./type_defs.md#listchallengemetadataresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pca-connector-scep]`
or a standalone `types_aiobotocore_pca_connector_scep` package, you have to explicitly specify
`client: PrivateCAConnectorforSCEPClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PrivateCAConnectorforSCEPClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_scep.client import PrivateCAConnectorforSCEPClient
from types_aiobotocore_pca_connector_scep.type_defs import CreateChallengeResponseTypeDef
from types_aiobotocore_pca_connector_scep.type_defs import CreateChallengeRequestTypeDef


session = get_session()

async with session.create_client("pca-connector-scep") as client:
    client: PrivateCAConnectorforSCEPClient
    kwargs: CreateChallengeRequestTypeDef = {...}
    result: CreateChallengeResponseTypeDef = await client.create_challenge(**kwargs)
```



```python
# ListChallengeMetadataPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_scep.client import PrivateCAConnectorforSCEPClient
from types_aiobotocore_pca_connector_scep.paginator import ListChallengeMetadataPaginator
from types_aiobotocore_pca_connector_scep.type_defs import ListChallengeMetadataResponseTypeDef


session = get_session()

async with session.create_client("pca-connector-scep") as client:
    client: PrivateCAConnectorforSCEPClient
    paginator: ListChallengeMetadataPaginator = client.get_paginator("list_challenge_metadata")
    async for item in paginator.paginate(...):
        item: ListChallengeMetadataResponseTypeDef
        print(item)
```


