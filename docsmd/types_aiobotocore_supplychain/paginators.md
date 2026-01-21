# Paginators

> [Index](../README.md) > [SupplyChain](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## ListDataIntegrationEventsPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_data_integration_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListDataIntegrationEvents.html#SupplyChain.Paginator.ListDataIntegrationEvents)

```python
# ListDataIntegrationEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListDataIntegrationEventsPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListDataIntegrationEventsPaginator = client.get_paginator("list_data_integration_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataIntegrationEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataIntegrationEventsPaginator](./paginators.md#listdataintegrationeventspaginator)
3. item: `AioPageIterator[ListDataIntegrationEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataIntegrationEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    eventType: DataIntegrationEventTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataIntegrationEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataIntegrationEventTypeType](./literals.md#dataintegrationeventtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataIntegrationEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataIntegrationEventsRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationEventsRequestPaginateTypeDef](./type_defs.md#listdataintegrationeventsrequestpaginatetypedef)
## ListDataIntegrationFlowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_data_integration_flow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListDataIntegrationFlowExecutions.html#SupplyChain.Paginator.ListDataIntegrationFlowExecutions)

```python
# ListDataIntegrationFlowExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListDataIntegrationFlowExecutionsPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListDataIntegrationFlowExecutionsPaginator = client.get_paginator("list_data_integration_flow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataIntegrationFlowExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataIntegrationFlowExecutionsPaginator](./paginators.md#listdataintegrationflowexecutionspaginator)
3. item: `AioPageIterator[ListDataIntegrationFlowExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataIntegrationFlowExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    flowName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataIntegrationFlowExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataIntegrationFlowExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataIntegrationFlowExecutionsRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
    "flowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationFlowExecutionsRequestPaginateTypeDef](./type_defs.md#listdataintegrationflowexecutionsrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListDataIntegrationFlowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataIntegrationFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataIntegrationFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataIntegrationFlowsResponseTypeDef]`


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
3. item: `AioPageIterator[ListDataLakeDatasetsResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListDataLakeDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataLakeDatasetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataLakeDatasetsRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataLakeDatasetsRequestPaginateTypeDef](./type_defs.md#listdatalakedatasetsrequestpaginatetypedef)
## ListDataLakeNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("supplychain").get_paginator("list_data_lake_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain/paginator/ListDataLakeNamespaces.html#SupplyChain.Paginator.ListDataLakeNamespaces)

```python
# ListDataLakeNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.paginator import ListDataLakeNamespacesPaginator

session = get_session()
async with session.create_client("supplychain") as client:  # (1)
    paginator: ListDataLakeNamespacesPaginator = client.get_paginator("list_data_lake_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataLakeNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. paginator: [ListDataLakeNamespacesPaginator](./paginators.md#listdatalakenamespacespaginator)
3. item: `AioPageIterator[ListDataLakeNamespacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataLakeNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    instanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataLakeNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataLakeNamespacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataLakeNamespacesRequestPaginateTypeDef = {  # (1)
    "instanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataLakeNamespacesRequestPaginateTypeDef](./type_defs.md#listdatalakenamespacesrequestpaginatetypedef)
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
3. item: `AioPageIterator[ListInstancesResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListInstancesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[InstanceStateType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesRequestPaginateTypeDef = {  # (1)
    "instanceNameFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestPaginateTypeDef](./type_defs.md#listinstancesrequestpaginatetypedef)
