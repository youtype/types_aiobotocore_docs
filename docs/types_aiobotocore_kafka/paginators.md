<a id="paginators-for-aiobotocore-kafka-module"></a>

# Paginators for aiobotocore Kafka module

> [Index](../README.md) > [Kafka](./README.md) > Paginators

Auto-generated documentation for
[Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
type annotations stubs module
[types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

- [Paginators for aiobotocore Kafka module](#paginators-for-aiobotocore-kafka-module)
  - [ListClusterOperationsPaginator](#listclusteroperationspaginator)
  - [ListClustersPaginator](#listclusterspaginator)
  - [ListClustersV2Paginator](#listclustersv2paginator)
  - [ListConfigurationRevisionsPaginator](#listconfigurationrevisionspaginator)
  - [ListConfigurationsPaginator](#listconfigurationspaginator)
  - [ListKafkaVersionsPaginator](#listkafkaversionspaginator)
  - [ListNodesPaginator](#listnodespaginator)
  - [ListScramSecretsPaginator](#listscramsecretspaginator)

<a id="listclusteroperationspaginator"></a>

## ListClusterOperationsPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_cluster_operations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClusterOperationsPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
```

Boto3 documentation:
[Kafka.Paginator.ListClusterOperations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)

Arguments for `ListClusterOperationsPaginator.paginate` method:

- `ClusterArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClusterOperationsPaginator.paginate` returns
`AsyncIterator`\[[ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef)\].

<a id="listclusterspaginator"></a>

## ListClustersPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")
```

Boto3 documentation:
[Kafka.Paginator.ListClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)

Arguments for `ListClustersPaginator.paginate` method:

- `ClusterNameFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClustersPaginator.paginate` returns
`AsyncIterator`\[[ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)\].

<a id="listclustersv2paginator"></a>

## ListClustersV2Paginator

Type annotations for
`session.create_client("kafka").get_paginator("list_clusters_v2")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClustersV2Paginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
```

Boto3 documentation:
[Kafka.Paginator.ListClustersV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2)

Arguments for `ListClustersV2Paginator.paginate` method:

- `ClusterNameFilter`: `str`
- `ClusterTypeFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClustersV2Paginator.paginate` returns
`AsyncIterator`\[[ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef)\].

<a id="listconfigurationrevisionspaginator"></a>

## ListConfigurationRevisionsPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_configuration_revisions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListConfigurationRevisionsPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
```

Boto3 documentation:
[Kafka.Paginator.ListConfigurationRevisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions)

Arguments for `ListConfigurationRevisionsPaginator.paginate` method:

- `Arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConfigurationRevisionsPaginator.paginate` returns
`AsyncIterator`\[[ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef)\].

<a id="listconfigurationspaginator"></a>

## ListConfigurationsPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListConfigurationsPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
```

Boto3 documentation:
[Kafka.Paginator.ListConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations)

Arguments for `ListConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)\].

<a id="listkafkaversionspaginator"></a>

## ListKafkaVersionsPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_kafka_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListKafkaVersionsPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
```

Boto3 documentation:
[Kafka.Paginator.ListKafkaVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions)

Arguments for `ListKafkaVersionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKafkaVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef)\].

<a id="listnodespaginator"></a>

## ListNodesPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_nodes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListNodesPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListNodesPaginator = client.get_paginator("list_nodes")
```

Boto3 documentation:
[Kafka.Paginator.ListNodes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes)

Arguments for `ListNodesPaginator.paginate` method:

- `ClusterArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListNodesPaginator.paginate` returns
`AsyncIterator`\[[ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef)\].

<a id="listscramsecretspaginator"></a>

## ListScramSecretsPaginator

Type annotations for
`session.create_client("kafka").get_paginator("list_scram_secrets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListScramSecretsPaginator

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
```

Boto3 documentation:
[Kafka.Paginator.ListScramSecrets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets)

Arguments for `ListScramSecretsPaginator.paginate` method:

- `ClusterArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListScramSecretsPaginator.paginate` returns
`AsyncIterator`\[[ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef)\].
