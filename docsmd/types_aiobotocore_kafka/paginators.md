# Paginators

> [Index](../README.md) > [Kafka](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## DescribeTopicPartitionsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("describe_topic_partitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/DescribeTopicPartitions.html#Kafka.Paginator.DescribeTopicPartitions)

```python
# DescribeTopicPartitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import DescribeTopicPartitionsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: DescribeTopicPartitionsPaginator = client.get_paginator("describe_topic_partitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTopicPartitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [DescribeTopicPartitionsPaginator](./paginators.md#describetopicpartitionspaginator)
3. item: `AioPageIterator[DescribeTopicPartitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTopicPartitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    TopicName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeTopicPartitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeTopicPartitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTopicPartitionsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
    "TopicName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTopicPartitionsRequestPaginateTypeDef](./type_defs.md#describetopicpartitionsrequestpaginatetypedef)
## ListClientVpcConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_client_vpc_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListClientVpcConnections.html#Kafka.Paginator.ListClientVpcConnections)

```python
# ListClientVpcConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClientVpcConnectionsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListClientVpcConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClientVpcConnectionsPaginator](./paginators.md#listclientvpcconnectionspaginator)
3. item: `AioPageIterator[ListClientVpcConnectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClientVpcConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClientVpcConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClientVpcConnectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClientVpcConnectionsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClientVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listclientvpcconnectionsrequestpaginatetypedef)
## ListClusterOperationsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_cluster_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListClusterOperations.html#Kafka.Paginator.ListClusterOperations)

```python
# ListClusterOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClusterOperationsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListClusterOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
3. item: `AioPageIterator[ListClusterOperationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClusterOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClusterOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClusterOperationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClusterOperationsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClusterOperationsRequestPaginateTypeDef](./type_defs.md#listclusteroperationsrequestpaginatetypedef)
## ListClusterOperationsV2Paginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_cluster_operations_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListClusterOperationsV2.html#Kafka.Paginator.ListClusterOperationsV2)

```python
# ListClusterOperationsV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClusterOperationsV2Paginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListClusterOperationsV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClusterOperationsV2Paginator](./paginators.md#listclusteroperationsv2paginator)
3. item: `AioPageIterator[ListClusterOperationsV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClusterOperationsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClusterOperationsV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClusterOperationsV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClusterOperationsV2RequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClusterOperationsV2RequestPaginateTypeDef](./type_defs.md#listclusteroperationsv2requestpaginatetypedef)
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListClusters.html#Kafka.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: `AioPageIterator[ListClustersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterNameFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClustersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "ClusterNameFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
## ListClustersV2Paginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_clusters_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListClustersV2.html#Kafka.Paginator.ListClustersV2)

```python
# ListClustersV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListClustersV2Paginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClustersV2Paginator](./paginators.md#listclustersv2paginator)
3. item: `AioPageIterator[ListClustersV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListClustersV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterNameFilter: str = ...,
    ClusterTypeFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListClustersV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListClustersV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersV2RequestPaginateTypeDef = {  # (1)
    "ClusterNameFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersV2RequestPaginateTypeDef](./type_defs.md#listclustersv2requestpaginatetypedef)
## ListConfigurationRevisionsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_configuration_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListConfigurationRevisions.html#Kafka.Paginator.ListConfigurationRevisions)

```python
# ListConfigurationRevisionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListConfigurationRevisionsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationRevisionsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListConfigurationRevisionsPaginator](./paginators.md#listconfigurationrevisionspaginator)
3. item: `AioPageIterator[ListConfigurationRevisionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfigurationRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfigurationRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfigurationRevisionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationRevisionsRequestPaginateTypeDef = {  # (1)
    "Arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationRevisionsRequestPaginateTypeDef](./type_defs.md#listconfigurationrevisionsrequestpaginatetypedef)
## ListConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListConfigurations.html#Kafka.Paginator.ListConfigurations)

```python
# ListConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListConfigurationsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
3. item: `AioPageIterator[ListConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsRequestPaginateTypeDef](./type_defs.md#listconfigurationsrequestpaginatetypedef)
## ListKafkaVersionsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_kafka_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListKafkaVersions.html#Kafka.Paginator.ListKafkaVersions)

```python
# ListKafkaVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListKafkaVersionsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListKafkaVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListKafkaVersionsPaginator](./paginators.md#listkafkaversionspaginator)
3. item: `AioPageIterator[ListKafkaVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListKafkaVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListKafkaVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListKafkaVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListKafkaVersionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKafkaVersionsRequestPaginateTypeDef](./type_defs.md#listkafkaversionsrequestpaginatetypedef)
## ListNodesPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListNodes.html#Kafka.Paginator.ListNodes)

```python
# ListNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListNodesPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListNodesPaginator = client.get_paginator("list_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListNodesResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListNodesPaginator](./paginators.md#listnodespaginator)
3. item: `AioPageIterator[ListNodesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListNodesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNodesRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestPaginateTypeDef](./type_defs.md#listnodesrequestpaginatetypedef)
## ListReplicatorsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_replicators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListReplicators.html#Kafka.Paginator.ListReplicators)

```python
# ListReplicatorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListReplicatorsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListReplicatorsPaginator = client.get_paginator("list_replicators")  # (2)
    async for item in paginator.paginate(...):
        item: ListReplicatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListReplicatorsPaginator](./paginators.md#listreplicatorspaginator)
3. item: `AioPageIterator[ListReplicatorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReplicatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicatorNameFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListReplicatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListReplicatorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReplicatorsRequestPaginateTypeDef = {  # (1)
    "ReplicatorNameFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReplicatorsRequestPaginateTypeDef](./type_defs.md#listreplicatorsrequestpaginatetypedef)
## ListScramSecretsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_scram_secrets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListScramSecrets.html#Kafka.Paginator.ListScramSecrets)

```python
# ListScramSecretsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListScramSecretsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")  # (2)
    async for item in paginator.paginate(...):
        item: ListScramSecretsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListScramSecretsPaginator](./paginators.md#listscramsecretspaginator)
3. item: `AioPageIterator[ListScramSecretsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListScramSecretsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListScramSecretsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListScramSecretsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListScramSecretsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScramSecretsRequestPaginateTypeDef](./type_defs.md#listscramsecretsrequestpaginatetypedef)
## ListTopicsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_topics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListTopics.html#Kafka.Paginator.ListTopics)

```python
# ListTopicsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListTopicsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListTopicsPaginator = client.get_paginator("list_topics")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListTopicsPaginator](./paginators.md#listtopicspaginator)
3. item: `AioPageIterator[ListTopicsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTopicsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    TopicNameFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTopicsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTopicsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsRequestPaginateTypeDef](./type_defs.md#listtopicsrequestpaginatetypedef)
## ListVpcConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator("list_vpc_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/paginator/ListVpcConnections.html#Kafka.Paginator.ListVpcConnections)

```python
# ListVpcConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.paginator import ListVpcConnectionsPaginator

session = get_session()
async with session.create_client("kafka") as client:  # (1)
    paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListVpcConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListVpcConnectionsPaginator](./paginators.md#listvpcconnectionspaginator)
3. item: `AioPageIterator[ListVpcConnectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVpcConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVpcConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVpcConnectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVpcConnectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listvpcconnectionsrequestpaginatetypedef)
