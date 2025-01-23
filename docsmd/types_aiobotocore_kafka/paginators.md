# Paginators

> [Index](../README.md) > [Kafka](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

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
3. item: [:material-code-braces: ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClientVpcConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClientVpcConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef) 


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
3. item: [:material-code-braces: ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClusterOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClusterOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef) 


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
3. item: [:material-code-braces: ListClusterOperationsV2ResponseTypeDef](./type_defs.md#listclusteroperationsv2responsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClusterOperationsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClusterOperationsV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClusterOperationsV2ResponseTypeDef](./type_defs.md#listclusteroperationsv2responsetypedef) 


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
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterNameFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


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
3. item: [:material-code-braces: ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef) 


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
) -> AioPageIterator[ListClustersV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef) 


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
3. item: [:material-code-braces: ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConfigurationRevisionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef) 


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
3. item: [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


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
3. item: [:material-code-braces: ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKafkaVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKafkaVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef) 


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
3. item: [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


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
3. item: [:material-code-braces: ListReplicatorsResponseTypeDef](./type_defs.md#listreplicatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReplicatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicatorNameFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListReplicatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReplicatorsResponseTypeDef](./type_defs.md#listreplicatorsresponsetypedef) 


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
3. item: [:material-code-braces: ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListScramSecretsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListScramSecretsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListScramSecretsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScramSecretsRequestPaginateTypeDef](./type_defs.md#listscramsecretsrequestpaginatetypedef) 
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
3. item: [:material-code-braces: ListVpcConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVpcConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListVpcConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVpcConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVpcConnectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listvpcconnectionsrequestpaginatetypedef) 
