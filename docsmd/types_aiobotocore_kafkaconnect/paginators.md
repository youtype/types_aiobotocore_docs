# Paginators

> [Index](../README.md) > [KafkaConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#kafkaconnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

## ListConnectorOperationsPaginator

Type annotations and code completion for `#!python session.create_client("kafkaconnect").get_paginator("list_connector_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/paginator/ListConnectorOperations.html#KafkaConnect.Paginator.ListConnectorOperations)

```python
# ListConnectorOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListConnectorOperationsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:  # (1)
    paginator: ListConnectorOperationsPaginator = client.get_paginator("list_connector_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListConnectorOperationsPaginator](./paginators.md#listconnectoroperationspaginator)
3. item: [:material-code-braces: ListConnectorOperationsResponseTypeDef](./type_defs.md#listconnectoroperationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    connectorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorOperationsResponseTypeDef](./type_defs.md#listconnectoroperationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorOperationsRequestPaginateTypeDef = {  # (1)
    "connectorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorOperationsRequestPaginateTypeDef](./type_defs.md#listconnectoroperationsrequestpaginatetypedef) 
## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("kafkaconnect").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/paginator/ListConnectors.html#KafkaConnect.Paginator.ListConnectors)

```python
# ListConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:  # (1)
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    connectorNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorsRequestPaginateTypeDef = {  # (1)
    "connectorNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef) 
## ListCustomPluginsPaginator

Type annotations and code completion for `#!python session.create_client("kafkaconnect").get_paginator("list_custom_plugins")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/paginator/ListCustomPlugins.html#KafkaConnect.Paginator.ListCustomPlugins)

```python
# ListCustomPluginsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListCustomPluginsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:  # (1)
    paginator: ListCustomPluginsPaginator = client.get_paginator("list_custom_plugins")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomPluginsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListCustomPluginsPaginator](./paginators.md#listcustompluginspaginator)
3. item: [:material-code-braces: ListCustomPluginsResponseTypeDef](./type_defs.md#listcustompluginsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomPluginsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomPluginsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomPluginsResponseTypeDef](./type_defs.md#listcustompluginsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomPluginsRequestPaginateTypeDef = {  # (1)
    "namePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomPluginsRequestPaginateTypeDef](./type_defs.md#listcustompluginsrequestpaginatetypedef) 
## ListWorkerConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("kafkaconnect").get_paginator("list_worker_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect/paginator/ListWorkerConfigurations.html#KafkaConnect.Paginator.ListWorkerConfigurations)

```python
# ListWorkerConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListWorkerConfigurationsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:  # (1)
    paginator: ListWorkerConfigurationsPaginator = client.get_paginator("list_worker_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkerConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListWorkerConfigurationsPaginator](./paginators.md#listworkerconfigurationspaginator)
3. item: [:material-code-braces: ListWorkerConfigurationsResponseTypeDef](./type_defs.md#listworkerconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkerConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkerConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkerConfigurationsResponseTypeDef](./type_defs.md#listworkerconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkerConfigurationsRequestPaginateTypeDef = {  # (1)
    "namePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkerConfigurationsRequestPaginateTypeDef](./type_defs.md#listworkerconfigurationsrequestpaginatetypedef) 
