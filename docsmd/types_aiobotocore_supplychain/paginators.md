# Paginators

> [Index](../README.md) > [SupplyChain](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## ListDataIntegrationFlowsPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_data_integration_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListDataIntegrationFlows.html#SupplyChain.Paginator.ListDataIntegrationFlows)

```python
# ListDataIntegrationFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListDataIntegrationFlowsPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListDataIntegrationFlowsPaginator = client.get_paginator("list_data_integration_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataIntegrationFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataIntegrationFlowsPaginator](./paginators.md#listdataintegrationflowspaginator)
3. item: [:material-code-braces: ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataIntegrationFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataIntegrationFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataIntegrationFlowsRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationFlowsRequestPaginateTypeDef](./type_defs.md#listdataintegrationflowsrequestpaginatetypedef) 
## ListDataLakeDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_data_lake_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListDataLakeDatasets.html#SupplyChain.Paginator.ListDataLakeDatasets)

```python
# ListDataLakeDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListDataLakeDatasetsPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListDataLakeDatasetsPaginator = client.get_paginator("list_data_lake_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataLakeDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataLakeDatasetsPaginator](./paginators.md#listdatalakedatasetspaginator)
3. item: [:material-code-braces: ListDataLakeDatasetsResponseTypeDef](./type_defs.md#listdatalakedatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataLakeDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataLakeDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataLakeDatasetsResponseTypeDef](./type_defs.md#listdatalakedatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataLakeDatasetsRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataLakeDatasetsRequestPaginateTypeDef](./type_defs.md#listdatalakedatasetsrequestpaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListInstances.html#SupplyChain.Paginator.ListInstances)

```python
# ListInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceNameFilter: Sequence[str] = ...,
    instanceStateFilter: Sequence[InstanceStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesRequestPaginateTypeDef = {  # (1)
    "instanceNameFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestPaginateTypeDef](./type_defs.md#listinstancesrequestpaginatetypedef) 
