# Paginators

> [Index](../README.md) > [PrivateCAConnectorforSCEP](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep)
    type annotations stubs module [types-aiobotocore-pca-connector-scep](https://pypi.org/project/types-aiobotocore-pca-connector-scep/).

## ListChallengeMetadataPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-scep").get_paginator("list_challenge_metadata")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep/paginator/ListChallengeMetadata.html#PrivateCAConnectorforSCEP.Paginator.ListChallengeMetadata)

```python
# ListChallengeMetadataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_scep.paginator import ListChallengeMetadataPaginator

session = get_session()
async with session.create_client("pca-connector-scep") as client:  # (1)
    paginator: ListChallengeMetadataPaginator = client.get_paginator("list_challenge_metadata")  # (2)
    async for item in paginator.paginate(...):
        item: ListChallengeMetadataResponseTypeDef
        print(item)  # (3)
```

1. client: [PrivateCAConnectorforSCEPClient](./client.md)
2. paginator: [ListChallengeMetadataPaginator](./paginators.md#listchallengemetadatapaginator)
3. item: [:material-code-braces: ListChallengeMetadataResponseTypeDef](./type_defs.md#listchallengemetadataresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChallengeMetadataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChallengeMetadataResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChallengeMetadataResponseTypeDef](./type_defs.md#listchallengemetadataresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChallengeMetadataRequestPaginateTypeDef = {  # (1)
    "ConnectorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChallengeMetadataRequestPaginateTypeDef](./type_defs.md#listchallengemetadatarequestpaginatetypedef) 
## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("pca-connector-scep").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep/paginator/ListConnectors.html#PrivateCAConnectorforSCEP.Paginator.ListConnectors)

```python
# ListConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_scep.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("pca-connector-scep") as client:  # (1)
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [PrivateCAConnectorforSCEPClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef) 
