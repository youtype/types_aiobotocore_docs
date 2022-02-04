<a id="kafkaclient-for-aiobotocore-kafka-module"></a>

# KafkaClient for aiobotocore Kafka module

> [Index](..) > [Kafka](.) > KafkaClient

Auto-generated documentation for
[Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
type annotations stubs module
[types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

- [KafkaClient for aiobotocore Kafka module](#kafkaclient-for-aiobotocore-kafka-module)
  - [KafkaClient](#kafkaclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_associate_scram_secret](#batch_associate_scram_secret)
    - [batch_disassociate_scram_secret](#batch_disassociate_scram_secret)
    - [can_paginate](#can_paginate)
    - [create_cluster](#create_cluster)
    - [create_cluster_v2](#create_cluster_v2)
    - [create_configuration](#create_configuration)
    - [delete_cluster](#delete_cluster)
    - [delete_configuration](#delete_configuration)
    - [describe_cluster](#describe_cluster)
    - [describe_cluster_operation](#describe_cluster_operation)
    - [describe_cluster_v2](#describe_cluster_v2)
    - [describe_configuration](#describe_configuration)
    - [describe_configuration_revision](#describe_configuration_revision)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_bootstrap_brokers](#get_bootstrap_brokers)
    - [get_compatible_kafka_versions](#get_compatible_kafka_versions)
    - [list_cluster_operations](#list_cluster_operations)
    - [list_clusters](#list_clusters)
    - [list_clusters_v2](#list_clusters_v2)
    - [list_configuration_revisions](#list_configuration_revisions)
    - [list_configurations](#list_configurations)
    - [list_kafka_versions](#list_kafka_versions)
    - [list_nodes](#list_nodes)
    - [list_scram_secrets](#list_scram_secrets)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [reboot_broker](#reboot_broker)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_broker_count](#update_broker_count)
    - [update_broker_storage](#update_broker_storage)
    - [update_broker_type](#update_broker_type)
    - [update_cluster_configuration](#update_cluster_configuration)
    - [update_cluster_kafka_version](#update_cluster_kafka_version)
    - [update_configuration](#update_configuration)
    - [update_connectivity](#update_connectivity)
    - [update_monitoring](#update_monitoring)
    - [update_security](#update_security)
    - [get_paginator](#get_paginator)

<a id="kafkaclient"></a>

## KafkaClient

Type annotations for `aiobotocore.create_client("kafka")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_kafka.client import KafkaClient

def get_kafka_client() -> KafkaClient:
    return Session().client("kafka")
```

Boto3 documentation:
[Kafka.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_kafka.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

KafkaClient exceptions.

Type annotations for `aiobotocore.create_client("kafka").exceptions` method.

Boto3 documentation:
[Kafka.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_associate_scram_secret"></a>

### batch_associate_scram_secret

Associates one or more Scram Secrets with an Amazon MSK cluster.

Type annotations for
`aiobotocore.create_client("kafka").batch_associate_scram_secret` method.

Boto3 documentation:
[Kafka.Client.batch_associate_scram_secret](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.batch_associate_scram_secret)

Asynchronous method. Use `await batch_associate_scram_secret(...)` for a
synchronous call.

Arguments mapping described in
[BatchAssociateScramSecretRequestRequestTypeDef](./type_defs.md#batchassociatescramsecretrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `SecretArnList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef).

<a id="batch_disassociate_scram_secret"></a>

### batch_disassociate_scram_secret

Disassociates one or more Scram Secrets from an Amazon MSK cluster.

Type annotations for
`aiobotocore.create_client("kafka").batch_disassociate_scram_secret` method.

Boto3 documentation:
[Kafka.Client.batch_disassociate_scram_secret](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.batch_disassociate_scram_secret)

Asynchronous method. Use `await batch_disassociate_scram_secret(...)` for a
synchronous call.

Arguments mapping described in
[BatchDisassociateScramSecretRequestRequestTypeDef](./type_defs.md#batchdisassociatescramsecretrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `SecretArnList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[BatchDisassociateScramSecretResponseTypeDef](./type_defs.md#batchdisassociatescramsecretresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("kafka").can_paginate` method.

Boto3 documentation:
[Kafka.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_cluster"></a>

### create_cluster

Creates a new MSK cluster.

Type annotations for `aiobotocore.create_client("kafka").create_cluster`
method.

Boto3 documentation:
[Kafka.Client.create_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster)

Asynchronous method. Use `await create_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef).

Keyword-only arguments:

- `BrokerNodeGroupInfo`:
  [BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef)
  *(required)*
- `ClusterName`: `str` *(required)*
- `KafkaVersion`: `str` *(required)*
- `NumberOfBrokerNodes`: `int` *(required)*
- `ClientAuthentication`:
  [ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef)
- `ConfigurationInfo`:
  [ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef)
- `EncryptionInfo`:
  [EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef)
- `EnhancedMonitoring`:
  [EnhancedMonitoringType](./literals.md#enhancedmonitoringtype)
- `OpenMonitoring`:
  [OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef)
- `LoggingInfo`: [LoggingInfoTypeDef](./type_defs.md#logginginfotypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef).

<a id="create_cluster_v2"></a>

### create_cluster_v2

Creates a new MSK cluster.

Type annotations for `aiobotocore.create_client("kafka").create_cluster_v2`
method.

Boto3 documentation:
[Kafka.Client.create_cluster_v2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster_v2)

Asynchronous method. Use `await create_cluster_v2(...)` for a synchronous call.

Arguments mapping described in
[CreateClusterV2RequestRequestTypeDef](./type_defs.md#createclusterv2requestrequesttypedef).

Keyword-only arguments:

- `ClusterName`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]
- `Provisioned`:
  [ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef)
- `Serverless`:
  [ServerlessRequestTypeDef](./type_defs.md#serverlessrequesttypedef)

Returns a `Coroutine` for
[CreateClusterV2ResponseTypeDef](./type_defs.md#createclusterv2responsetypedef).

<a id="create_configuration"></a>

### create_configuration

Creates a new MSK configuration.

Type annotations for `aiobotocore.create_client("kafka").create_configuration`
method.

Boto3 documentation:
[Kafka.Client.create_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)

Asynchronous method. Use `await create_configuration(...)` for a synchronous
call.

Arguments mapping described in
[CreateConfigurationRequestRequestTypeDef](./type_defs.md#createconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ServerProperties`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `Description`: `str`
- `KafkaVersions`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef).

<a id="delete_cluster"></a>

### delete_cluster

Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
request.

Type annotations for `aiobotocore.create_client("kafka").delete_cluster`
method.

Boto3 documentation:
[Kafka.Client.delete_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster)

Asynchronous method. Use `await delete_cluster(...)` for a synchronous call.

Arguments mapping described in
[DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str`

Returns a `Coroutine` for
[DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef).

<a id="delete_configuration"></a>

### delete_configuration

Deletes an MSK Configuration.

Type annotations for `aiobotocore.create_client("kafka").delete_configuration`
method.

Boto3 documentation:
[Kafka.Client.delete_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_configuration)

Asynchronous method. Use `await delete_configuration(...)` for a synchronous
call.

Arguments mapping described in
[DeleteConfigurationRequestRequestTypeDef](./type_defs.md#deleteconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteConfigurationResponseTypeDef](./type_defs.md#deleteconfigurationresponsetypedef).

<a id="describe_cluster"></a>

### describe_cluster

Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
specified in the request.

Type annotations for `aiobotocore.create_client("kafka").describe_cluster`
method.

Boto3 documentation:
[Kafka.Client.describe_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster)

Asynchronous method. Use `await describe_cluster(...)` for a synchronous call.

Arguments mapping described in
[DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef).

<a id="describe_cluster_operation"></a>

### describe_cluster_operation

Returns a description of the cluster operation specified by the ARN.

Type annotations for
`aiobotocore.create_client("kafka").describe_cluster_operation` method.

Boto3 documentation:
[Kafka.Client.describe_cluster_operation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation)

Asynchronous method. Use `await describe_cluster_operation(...)` for a
synchronous call.

Arguments mapping described in
[DescribeClusterOperationRequestRequestTypeDef](./type_defs.md#describeclusteroperationrequestrequesttypedef).

Keyword-only arguments:

- `ClusterOperationArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterOperationResponseTypeDef](./type_defs.md#describeclusteroperationresponsetypedef).

<a id="describe_cluster_v2"></a>

### describe_cluster_v2

Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
specified in the request.

Type annotations for `aiobotocore.create_client("kafka").describe_cluster_v2`
method.

Boto3 documentation:
[Kafka.Client.describe_cluster_v2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_v2)

Asynchronous method. Use `await describe_cluster_v2(...)` for a synchronous
call.

Arguments mapping described in
[DescribeClusterV2RequestRequestTypeDef](./type_defs.md#describeclusterv2requestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterV2ResponseTypeDef](./type_defs.md#describeclusterv2responsetypedef).

<a id="describe_configuration"></a>

### describe_configuration

Returns a description of this MSK configuration.

Type annotations for
`aiobotocore.create_client("kafka").describe_configuration` method.

Boto3 documentation:
[Kafka.Client.describe_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration)

Asynchronous method. Use `await describe_configuration(...)` for a synchronous
call.

Arguments mapping described in
[DescribeConfigurationRequestRequestTypeDef](./type_defs.md#describeconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef).

<a id="describe_configuration_revision"></a>

### describe_configuration_revision

Returns a description of this revision of the configuration.

Type annotations for
`aiobotocore.create_client("kafka").describe_configuration_revision` method.

Boto3 documentation:
[Kafka.Client.describe_configuration_revision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration_revision)

Asynchronous method. Use `await describe_configuration_revision(...)` for a
synchronous call.

Arguments mapping described in
[DescribeConfigurationRevisionRequestRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `Revision`: `int` *(required)*

Returns a `Coroutine` for
[DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("kafka").generate_presigned_url` method.

Boto3 documentation:
[Kafka.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_bootstrap_brokers"></a>

### get_bootstrap_brokers

A list of brokers that a client application can use to bootstrap.

Type annotations for `aiobotocore.create_client("kafka").get_bootstrap_brokers`
method.

Boto3 documentation:
[Kafka.Client.get_bootstrap_brokers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_bootstrap_brokers)

Asynchronous method. Use `await get_bootstrap_brokers(...)` for a synchronous
call.

Arguments mapping described in
[GetBootstrapBrokersRequestRequestTypeDef](./type_defs.md#getbootstrapbrokersrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for
[GetBootstrapBrokersResponseTypeDef](./type_defs.md#getbootstrapbrokersresponsetypedef).

<a id="get_compatible_kafka_versions"></a>

### get_compatible_kafka_versions

Gets the Apache Kafka versions to which you can update the MSK cluster.

Type annotations for
`aiobotocore.create_client("kafka").get_compatible_kafka_versions` method.

Boto3 documentation:
[Kafka.Client.get_compatible_kafka_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_compatible_kafka_versions)

Asynchronous method. Use `await get_compatible_kafka_versions(...)` for a
synchronous call.

Arguments mapping described in
[GetCompatibleKafkaVersionsRequestRequestTypeDef](./type_defs.md#getcompatiblekafkaversionsrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str`

Returns a `Coroutine` for
[GetCompatibleKafkaVersionsResponseTypeDef](./type_defs.md#getcompatiblekafkaversionsresponsetypedef).

<a id="list_cluster_operations"></a>

### list_cluster_operations

Returns a list of all the operations that have been performed on the specified
MSK cluster.

Type annotations for
`aiobotocore.create_client("kafka").list_cluster_operations` method.

Boto3 documentation:
[Kafka.Client.list_cluster_operations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations)

Asynchronous method. Use `await list_cluster_operations(...)` for a synchronous
call.

Arguments mapping described in
[ListClusterOperationsRequestRequestTypeDef](./type_defs.md#listclusteroperationsrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef).

<a id="list_clusters"></a>

### list_clusters

Returns a list of all the MSK clusters in the current Region.

Type annotations for `aiobotocore.create_client("kafka").list_clusters` method.

Boto3 documentation:
[Kafka.Client.list_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters)

Asynchronous method. Use `await list_clusters(...)` for a synchronous call.

Arguments mapping described in
[ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef).

Keyword-only arguments:

- `ClusterNameFilter`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef).

<a id="list_clusters_v2"></a>

### list_clusters_v2

Returns a list of all the MSK clusters in the current Region.

Type annotations for `aiobotocore.create_client("kafka").list_clusters_v2`
method.

Boto3 documentation:
[Kafka.Client.list_clusters_v2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters_v2)

Asynchronous method. Use `await list_clusters_v2(...)` for a synchronous call.

Arguments mapping described in
[ListClustersV2RequestRequestTypeDef](./type_defs.md#listclustersv2requestrequesttypedef).

Keyword-only arguments:

- `ClusterNameFilter`: `str`
- `ClusterTypeFilter`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef).

<a id="list_configuration_revisions"></a>

### list_configuration_revisions

Returns a list of all the MSK configurations in this Region.

Type annotations for
`aiobotocore.create_client("kafka").list_configuration_revisions` method.

Boto3 documentation:
[Kafka.Client.list_configuration_revisions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_configuration_revisions)

Asynchronous method. Use `await list_configuration_revisions(...)` for a
synchronous call.

Arguments mapping described in
[ListConfigurationRevisionsRequestRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef).

<a id="list_configurations"></a>

### list_configurations

Returns a list of all the MSK configurations in this Region.

Type annotations for `aiobotocore.create_client("kafka").list_configurations`
method.

Boto3 documentation:
[Kafka.Client.list_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_configurations)

Asynchronous method. Use `await list_configurations(...)` for a synchronous
call.

Arguments mapping described in
[ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef).

<a id="list_kafka_versions"></a>

### list_kafka_versions

Returns a list of Apache Kafka versions.

Type annotations for `aiobotocore.create_client("kafka").list_kafka_versions`
method.

Boto3 documentation:
[Kafka.Client.list_kafka_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_kafka_versions)

Asynchronous method. Use `await list_kafka_versions(...)` for a synchronous
call.

Arguments mapping described in
[ListKafkaVersionsRequestRequestTypeDef](./type_defs.md#listkafkaversionsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef).

<a id="list_nodes"></a>

### list_nodes

Returns a list of the broker nodes in the cluster.

Type annotations for `aiobotocore.create_client("kafka").list_nodes` method.

Boto3 documentation:
[Kafka.Client.list_nodes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_nodes)

Asynchronous method. Use `await list_nodes(...)` for a synchronous call.

Arguments mapping described in
[ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef).

<a id="list_scram_secrets"></a>

### list_scram_secrets

Returns a list of the Scram Secrets associated with an Amazon MSK cluster.

Type annotations for `aiobotocore.create_client("kafka").list_scram_secrets`
method.

Boto3 documentation:
[Kafka.Client.list_scram_secrets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_scram_secrets)

Asynchronous method. Use `await list_scram_secrets(...)` for a synchronous
call.

Arguments mapping described in
[ListScramSecretsRequestRequestTypeDef](./type_defs.md#listscramsecretsrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of the tags associated with the specified resource.

Type annotations for
`aiobotocore.create_client("kafka").list_tags_for_resource` method.

Boto3 documentation:
[Kafka.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="reboot_broker"></a>

### reboot_broker

Reboots brokers.

Type annotations for `aiobotocore.create_client("kafka").reboot_broker` method.

Boto3 documentation:
[Kafka.Client.reboot_broker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reboot_broker)

Asynchronous method. Use `await reboot_broker(...)` for a synchronous call.

Arguments mapping described in
[RebootBrokerRequestRequestTypeDef](./type_defs.md#rebootbrokerrequestrequesttypedef).

Keyword-only arguments:

- `BrokerIds`: `Sequence`\[`str`\] *(required)*
- `ClusterArn`: `str` *(required)*

Returns a `Coroutine` for
[RebootBrokerResponseTypeDef](./type_defs.md#rebootbrokerresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds tags to the specified MSK resource.

Type annotations for `aiobotocore.create_client("kafka").tag_resource` method.

Boto3 documentation:
[Kafka.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

<a id="untag_resource"></a>

### untag_resource

Removes the tags associated with the keys that are provided in the query.

Type annotations for `aiobotocore.create_client("kafka").untag_resource`
method.

Boto3 documentation:
[Kafka.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_broker_count"></a>

### update_broker_count

Updates the number of broker nodes in the cluster.

Type annotations for `aiobotocore.create_client("kafka").update_broker_count`
method.

Boto3 documentation:
[Kafka.Client.update_broker_count](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_broker_count)

Asynchronous method. Use `await update_broker_count(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBrokerCountRequestRequestTypeDef](./type_defs.md#updatebrokercountrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `TargetNumberOfBrokerNodes`: `int` *(required)*

Returns a `Coroutine` for
[UpdateBrokerCountResponseTypeDef](./type_defs.md#updatebrokercountresponsetypedef).

<a id="update_broker_storage"></a>

### update_broker_storage

Updates the EBS storage associated with MSK brokers.

Type annotations for `aiobotocore.create_client("kafka").update_broker_storage`
method.

Boto3 documentation:
[Kafka.Client.update_broker_storage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_broker_storage)

Asynchronous method. Use `await update_broker_storage(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBrokerStorageRequestRequestTypeDef](./type_defs.md#updatebrokerstoragerequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `TargetBrokerEBSVolumeInfo`:
  `Sequence`\[[BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateBrokerStorageResponseTypeDef](./type_defs.md#updatebrokerstorageresponsetypedef).

<a id="update_broker_type"></a>

### update_broker_type

Updates EC2 instance type.

Type annotations for `aiobotocore.create_client("kafka").update_broker_type`
method.

Boto3 documentation:
[Kafka.Client.update_broker_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_broker_type)

Asynchronous method. Use `await update_broker_type(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBrokerTypeRequestRequestTypeDef](./type_defs.md#updatebrokertyperequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `TargetInstanceType`: `str` *(required)*

Returns a `Coroutine` for
[UpdateBrokerTypeResponseTypeDef](./type_defs.md#updatebrokertyperesponsetypedef).

<a id="update_cluster_configuration"></a>

### update_cluster_configuration

Updates the cluster with the configuration that is specified in the request
body.

Type annotations for
`aiobotocore.create_client("kafka").update_cluster_configuration` method.

Boto3 documentation:
[Kafka.Client.update_cluster_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_configuration)

Asynchronous method. Use `await update_cluster_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateClusterConfigurationRequestRequestTypeDef](./type_defs.md#updateclusterconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `ConfigurationInfo`:
  [ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef)
  *(required)*
- `CurrentVersion`: `str` *(required)*

Returns a `Coroutine` for
[UpdateClusterConfigurationResponseTypeDef](./type_defs.md#updateclusterconfigurationresponsetypedef).

<a id="update_cluster_kafka_version"></a>

### update_cluster_kafka_version

Updates the Apache Kafka version for the cluster.

Type annotations for
`aiobotocore.create_client("kafka").update_cluster_kafka_version` method.

Boto3 documentation:
[Kafka.Client.update_cluster_kafka_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_kafka_version)

Asynchronous method. Use `await update_cluster_kafka_version(...)` for a
synchronous call.

Arguments mapping described in
[UpdateClusterKafkaVersionRequestRequestTypeDef](./type_defs.md#updateclusterkafkaversionrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `TargetKafkaVersion`: `str` *(required)*
- `ConfigurationInfo`:
  [ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef)

Returns a `Coroutine` for
[UpdateClusterKafkaVersionResponseTypeDef](./type_defs.md#updateclusterkafkaversionresponsetypedef).

<a id="update_configuration"></a>

### update_configuration

Updates an MSK configuration.

Type annotations for `aiobotocore.create_client("kafka").update_configuration`
method.

Boto3 documentation:
[Kafka.Client.update_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_configuration)

Asynchronous method. Use `await update_configuration(...)` for a synchronous
call.

Arguments mapping described in
[UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `ServerProperties`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef).

<a id="update_connectivity"></a>

### update_connectivity

Updates the cluster's connectivity configuration.

Type annotations for `aiobotocore.create_client("kafka").update_connectivity`
method.

Boto3 documentation:
[Kafka.Client.update_connectivity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_connectivity)

Asynchronous method. Use `await update_connectivity(...)` for a synchronous
call.

Arguments mapping described in
[UpdateConnectivityRequestRequestTypeDef](./type_defs.md#updateconnectivityrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `ConnectivityInfo`:
  [ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef)
  *(required)*
- `CurrentVersion`: `str` *(required)*

Returns a `Coroutine` for
[UpdateConnectivityResponseTypeDef](./type_defs.md#updateconnectivityresponsetypedef).

<a id="update_monitoring"></a>

### update_monitoring

Updates the monitoring settings for the cluster.

Type annotations for `aiobotocore.create_client("kafka").update_monitoring`
method.

Boto3 documentation:
[Kafka.Client.update_monitoring](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_monitoring)

Asynchronous method. Use `await update_monitoring(...)` for a synchronous call.

Arguments mapping described in
[UpdateMonitoringRequestRequestTypeDef](./type_defs.md#updatemonitoringrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `EnhancedMonitoring`:
  [EnhancedMonitoringType](./literals.md#enhancedmonitoringtype)
- `OpenMonitoring`:
  [OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef)
- `LoggingInfo`: [LoggingInfoTypeDef](./type_defs.md#logginginfotypedef)

Returns a `Coroutine` for
[UpdateMonitoringResponseTypeDef](./type_defs.md#updatemonitoringresponsetypedef).

<a id="update_security"></a>

### update_security

Updates the security settings for the cluster.

Type annotations for `aiobotocore.create_client("kafka").update_security`
method.

Boto3 documentation:
[Kafka.Client.update_security](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)

Asynchronous method. Use `await update_security(...)` for a synchronous call.

Arguments mapping described in
[UpdateSecurityRequestRequestTypeDef](./type_defs.md#updatesecurityrequestrequesttypedef).

Keyword-only arguments:

- `ClusterArn`: `str` *(required)*
- `CurrentVersion`: `str` *(required)*
- `ClientAuthentication`:
  [ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef)
- `EncryptionInfo`:
  [EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef)

Returns a `Coroutine` for
[UpdateSecurityResponseTypeDef](./type_defs.md#updatesecurityresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("kafka").get_paginator` method
with overloads.

- `client.get_paginator("list_cluster_operations")` ->
  [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
- `client.get_paginator("list_clusters")` ->
  [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_clusters_v2")` ->
  [ListClustersV2Paginator](./paginators.md#listclustersv2paginator)
- `client.get_paginator("list_configuration_revisions")` ->
  [ListConfigurationRevisionsPaginator](./paginators.md#listconfigurationrevisionspaginator)
- `client.get_paginator("list_configurations")` ->
  [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
- `client.get_paginator("list_kafka_versions")` ->
  [ListKafkaVersionsPaginator](./paginators.md#listkafkaversionspaginator)
- `client.get_paginator("list_nodes")` ->
  [ListNodesPaginator](./paginators.md#listnodespaginator)
- `client.get_paginator("list_scram_secrets")` ->
  [ListScramSecretsPaginator](./paginators.md#listscramsecretspaginator)
