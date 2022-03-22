<a id="paginators-for-aiobotocore-kafkaconnect-module"></a>

# Paginators for aiobotocore KafkaConnect module

> [Index](../README.md) > [KafkaConnect](./README.md) > Paginators

Auto-generated documentation for
[KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
type annotations stubs module
[types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

- [Paginators for aiobotocore KafkaConnect module](#paginators-for-aiobotocore-kafkaconnect-module)
  - [ListConnectorsPaginator](#listconnectorspaginator)
  - [ListCustomPluginsPaginator](#listcustompluginspaginator)
  - [ListWorkerConfigurationsPaginator](#listworkerconfigurationspaginator)

<a id="listconnectorspaginator"></a>

## ListConnectorsPaginator

Type annotations for
`session.create_client("kafkaconnect").get_paginator("list_connectors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")
```

Boto3 documentation:
[KafkaConnect.Paginator.ListConnectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors)

Arguments for `ListConnectorsPaginator.paginate` method:

- `connectorNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConnectorsPaginator.paginate` returns
`AsyncIterator`\[[ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)\].

<a id="listcustompluginspaginator"></a>

## ListCustomPluginsPaginator

Type annotations for
`session.create_client("kafkaconnect").get_paginator("list_custom_plugins")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListCustomPluginsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
    paginator: ListCustomPluginsPaginator = client.get_paginator("list_custom_plugins")
```

Boto3 documentation:
[KafkaConnect.Paginator.ListCustomPlugins](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins)

Arguments for `ListCustomPluginsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomPluginsPaginator.paginate` returns
`AsyncIterator`\[[ListCustomPluginsResponseTypeDef](./type_defs.md#listcustompluginsresponsetypedef)\].

<a id="listworkerconfigurationspaginator"></a>

## ListWorkerConfigurationsPaginator

Type annotations for
`session.create_client("kafkaconnect").get_paginator("list_worker_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.paginator import ListWorkerConfigurationsPaginator

session = get_session()
async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
    paginator: ListWorkerConfigurationsPaginator = client.get_paginator("list_worker_configurations")
```

Boto3 documentation:
[KafkaConnect.Paginator.ListWorkerConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations)

Arguments for `ListWorkerConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkerConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[ListWorkerConfigurationsResponseTypeDef](./type_defs.md#listworkerconfigurationsresponsetypedef)\].
