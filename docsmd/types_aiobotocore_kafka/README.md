# Kafka module

> [Index](../README.md) > Kafka


!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Kafka` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Kafka` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kafka]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kafka]'

# standalone installation
python -m pip install types-aiobotocore-kafka
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kafka
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KafkaClient

Type annotations and code completion for  `#!python session.create_client("kafka")` as [KafkaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client)

```python
# KafkaClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_kafka.client import KafkaClient


session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("kafka").get_paginator("...")`.

```python
# DescribeTopicPartitionsPaginator usage example

from types_aiobotocore_kafka.paginator import DescribeTopicPartitionsPaginator

def get_describe_topic_partitions_paginator() -> DescribeTopicPartitionsPaginator:
    return client.get_paginator("describe_topic_partitions"))
```

- [DescribeTopicPartitionsPaginator](./paginators.md#describetopicpartitionspaginator)
- [ListClientVpcConnectionsPaginator](./paginators.md#listclientvpcconnectionspaginator)
- [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
- [ListClusterOperationsV2Paginator](./paginators.md#listclusteroperationsv2paginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListClustersV2Paginator](./paginators.md#listclustersv2paginator)
- [ListConfigurationRevisionsPaginator](./paginators.md#listconfigurationrevisionspaginator)
- [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
- [ListKafkaVersionsPaginator](./paginators.md#listkafkaversionspaginator)
- [ListNodesPaginator](./paginators.md#listnodespaginator)
- [ListReplicatorsPaginator](./paginators.md#listreplicatorspaginator)
- [ListScramSecretsPaginator](./paginators.md#listscramsecretspaginator)
- [ListTopicsPaginator](./paginators.md#listtopicspaginator)
- [ListVpcConnectionsPaginator](./paginators.md#listvpcconnectionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BrokerAZDistributionType usage example

from types_aiobotocore_kafka.literals import BrokerAZDistributionType

def get_value() -> BrokerAZDistributionType:
    return "DEFAULT"
```

- [BrokerAZDistributionType](./literals.md#brokerazdistributiontype)
- [ClientBrokerType](./literals.md#clientbrokertype)
- [ClusterStateType](./literals.md#clusterstatetype)
- [ClusterTypeType](./literals.md#clustertypetype)
- [ConfigurationStateType](./literals.md#configurationstatetype)
- [CustomerActionStatusType](./literals.md#customeractionstatustype)
- [DescribeTopicPartitionsPaginatorName](./literals.md#describetopicpartitionspaginatorname)
- [EnhancedMonitoringType](./literals.md#enhancedmonitoringtype)
- [KafkaVersionStatusType](./literals.md#kafkaversionstatustype)
- [ListClientVpcConnectionsPaginatorName](./literals.md#listclientvpcconnectionspaginatorname)
- [ListClusterOperationsPaginatorName](./literals.md#listclusteroperationspaginatorname)
- [ListClusterOperationsV2PaginatorName](./literals.md#listclusteroperationsv2paginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListClustersV2PaginatorName](./literals.md#listclustersv2paginatorname)
- [ListConfigurationRevisionsPaginatorName](./literals.md#listconfigurationrevisionspaginatorname)
- [ListConfigurationsPaginatorName](./literals.md#listconfigurationspaginatorname)
- [ListKafkaVersionsPaginatorName](./literals.md#listkafkaversionspaginatorname)
- [ListNodesPaginatorName](./literals.md#listnodespaginatorname)
- [ListReplicatorsPaginatorName](./literals.md#listreplicatorspaginatorname)
- [ListScramSecretsPaginatorName](./literals.md#listscramsecretspaginatorname)
- [ListTopicsPaginatorName](./literals.md#listtopicspaginatorname)
- [ListVpcConnectionsPaginatorName](./literals.md#listvpcconnectionspaginatorname)
- [NodeTypeType](./literals.md#nodetypetype)
- [RebalancingStatusType](./literals.md#rebalancingstatustype)
- [ReplicationStartingPositionTypeType](./literals.md#replicationstartingpositiontypetype)
- [ReplicationTopicNameConfigurationTypeType](./literals.md#replicationtopicnameconfigurationtypetype)
- [ReplicatorStateType](./literals.md#replicatorstatetype)
- [StorageModeType](./literals.md#storagemodetype)
- [TargetCompressionTypeType](./literals.md#targetcompressiontypetype)
- [TopicStateType](./literals.md#topicstatetype)
- [UserIdentityTypeType](./literals.md#useridentitytypetype)
- [VpcConnectionStateType](./literals.md#vpcconnectionstatetype)
- [KafkaServiceName](./literals.md#kafkaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef)
- [BatchAssociateScramSecretRequestTypeDef](./type_defs.md#batchassociatescramsecretrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UnprocessedScramSecretTypeDef](./type_defs.md#unprocessedscramsecrettypedef)
- [BatchDisassociateScramSecretRequestTypeDef](./type_defs.md#batchdisassociatescramsecretrequesttypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BrokerCountUpdateInfoTypeDef](./type_defs.md#brokercountupdateinfotypedef)
- [ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef)
- [CloudWatchLogsTypeDef](./type_defs.md#cloudwatchlogstypedef)
- [FirehoseTypeDef](./type_defs.md#firehosetypedef)
- [S3TypeDef](./type_defs.md#s3typedef)
- [BrokerSoftwareInfoTypeDef](./type_defs.md#brokersoftwareinfotypedef)
- [TlsOutputTypeDef](./type_defs.md#tlsoutputtypedef)
- [UnauthenticatedTypeDef](./type_defs.md#unauthenticatedtypedef)
- [ClientVpcConnectionTypeDef](./type_defs.md#clientvpcconnectiontypedef)
- [RebalancingTypeDef](./type_defs.md#rebalancingtypedef)
- [StateInfoTypeDef](./type_defs.md#stateinfotypedef)
- [ErrorInfoTypeDef](./type_defs.md#errorinfotypedef)
- [ClusterOperationStepInfoTypeDef](./type_defs.md#clusteroperationstepinfotypedef)
- [ClusterOperationV2SummaryTypeDef](./type_defs.md#clusteroperationv2summarytypedef)
- [CompatibleKafkaVersionTypeDef](./type_defs.md#compatiblekafkaversiontypedef)
- [ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef)
- [ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef)
- [PublicAccessTypeDef](./type_defs.md#publicaccesstypedef)
- [ConsumerGroupReplicationOutputTypeDef](./type_defs.md#consumergroupreplicationoutputtypedef)
- [ConsumerGroupReplicationTypeDef](./type_defs.md#consumergroupreplicationtypedef)
- [ConsumerGroupReplicationUpdateTypeDef](./type_defs.md#consumergroupreplicationupdatetypedef)
- [ControllerNodeInfoTypeDef](./type_defs.md#controllernodeinfotypedef)
- [CreateVpcConnectionRequestTypeDef](./type_defs.md#createvpcconnectionrequesttypedef)
- [DeleteClusterPolicyRequestTypeDef](./type_defs.md#deleteclusterpolicyrequesttypedef)
- [DeleteClusterRequestTypeDef](./type_defs.md#deleteclusterrequesttypedef)
- [DeleteConfigurationRequestTypeDef](./type_defs.md#deleteconfigurationrequesttypedef)
- [DeleteReplicatorRequestTypeDef](./type_defs.md#deletereplicatorrequesttypedef)
- [DeleteVpcConnectionRequestTypeDef](./type_defs.md#deletevpcconnectionrequesttypedef)
- [DescribeClusterOperationRequestTypeDef](./type_defs.md#describeclusteroperationrequesttypedef)
- [DescribeClusterOperationV2RequestTypeDef](./type_defs.md#describeclusteroperationv2requesttypedef)
- [DescribeClusterRequestTypeDef](./type_defs.md#describeclusterrequesttypedef)
- [DescribeClusterV2RequestTypeDef](./type_defs.md#describeclusterv2requesttypedef)
- [DescribeConfigurationRequestTypeDef](./type_defs.md#describeconfigurationrequesttypedef)
- [DescribeConfigurationRevisionRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequesttypedef)
- [DescribeReplicatorRequestTypeDef](./type_defs.md#describereplicatorrequesttypedef)
- [ReplicationStateInfoTypeDef](./type_defs.md#replicationstateinfotypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeTopicPartitionsRequestTypeDef](./type_defs.md#describetopicpartitionsrequesttypedef)
- [TopicPartitionInfoTypeDef](./type_defs.md#topicpartitioninfotypedef)
- [DescribeTopicRequestTypeDef](./type_defs.md#describetopicrequesttypedef)
- [DescribeVpcConnectionRequestTypeDef](./type_defs.md#describevpcconnectionrequesttypedef)
- [EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef)
- [EncryptionInTransitTypeDef](./type_defs.md#encryptionintransittypedef)
- [GetBootstrapBrokersRequestTypeDef](./type_defs.md#getbootstrapbrokersrequesttypedef)
- [GetClusterPolicyRequestTypeDef](./type_defs.md#getclusterpolicyrequesttypedef)
- [GetCompatibleKafkaVersionsRequestTypeDef](./type_defs.md#getcompatiblekafkaversionsrequesttypedef)
- [IamTypeDef](./type_defs.md#iamtypedef)
- [JmxExporterInfoTypeDef](./type_defs.md#jmxexporterinfotypedef)
- [JmxExporterTypeDef](./type_defs.md#jmxexportertypedef)
- [KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef)
- [KafkaClusterClientVpcConfigTypeDef](./type_defs.md#kafkaclusterclientvpcconfigtypedef)
- [KafkaVersionTypeDef](./type_defs.md#kafkaversiontypedef)
- [ListClientVpcConnectionsRequestTypeDef](./type_defs.md#listclientvpcconnectionsrequesttypedef)
- [ListClusterOperationsRequestTypeDef](./type_defs.md#listclusteroperationsrequesttypedef)
- [ListClusterOperationsV2RequestTypeDef](./type_defs.md#listclusteroperationsv2requesttypedef)
- [ListClustersRequestTypeDef](./type_defs.md#listclustersrequesttypedef)
- [ListClustersV2RequestTypeDef](./type_defs.md#listclustersv2requesttypedef)
- [ListConfigurationRevisionsRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequesttypedef)
- [ListConfigurationsRequestTypeDef](./type_defs.md#listconfigurationsrequesttypedef)
- [ListKafkaVersionsRequestTypeDef](./type_defs.md#listkafkaversionsrequesttypedef)
- [ListNodesRequestTypeDef](./type_defs.md#listnodesrequesttypedef)
- [ListReplicatorsRequestTypeDef](./type_defs.md#listreplicatorsrequesttypedef)
- [ListScramSecretsRequestTypeDef](./type_defs.md#listscramsecretsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListTopicsRequestTypeDef](./type_defs.md#listtopicsrequesttypedef)
- [TopicInfoTypeDef](./type_defs.md#topicinfotypedef)
- [ListVpcConnectionsRequestTypeDef](./type_defs.md#listvpcconnectionsrequesttypedef)
- [VpcConnectionTypeDef](./type_defs.md#vpcconnectiontypedef)
- [NodeExporterInfoTypeDef](./type_defs.md#nodeexporterinfotypedef)
- [NodeExporterTypeDef](./type_defs.md#nodeexportertypedef)
- [ZookeeperNodeInfoTypeDef](./type_defs.md#zookeepernodeinfotypedef)
- [PutClusterPolicyRequestTypeDef](./type_defs.md#putclusterpolicyrequesttypedef)
- [RebootBrokerRequestTypeDef](./type_defs.md#rebootbrokerrequesttypedef)
- [RejectClientVpcConnectionRequestTypeDef](./type_defs.md#rejectclientvpcconnectionrequesttypedef)
- [ReplicationInfoSummaryTypeDef](./type_defs.md#replicationinfosummarytypedef)
- [ReplicationStartingPositionTypeDef](./type_defs.md#replicationstartingpositiontypedef)
- [ReplicationTopicNameConfigurationTypeDef](./type_defs.md#replicationtopicnameconfigurationtypedef)
- [ScramTypeDef](./type_defs.md#scramtypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TlsTypeDef](./type_defs.md#tlstypedef)
- [TopicReplicationUpdateTypeDef](./type_defs.md#topicreplicationupdatetypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateBrokerCountRequestTypeDef](./type_defs.md#updatebrokercountrequesttypedef)
- [UpdateBrokerTypeRequestTypeDef](./type_defs.md#updatebrokertyperequesttypedef)
- [UserIdentityTypeDef](./type_defs.md#useridentitytypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [VpcConnectivityTlsTypeDef](./type_defs.md#vpcconnectivitytlstypedef)
- [VpcConnectivityIamTypeDef](./type_defs.md#vpcconnectivityiamtypedef)
- [VpcConnectivityScramTypeDef](./type_defs.md#vpcconnectivityscramtypedef)
- [KafkaClusterSummaryTypeDef](./type_defs.md#kafkaclustersummarytypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [CreateClusterV2ResponseTypeDef](./type_defs.md#createclusterv2responsetypedef)
- [CreateReplicatorResponseTypeDef](./type_defs.md#createreplicatorresponsetypedef)
- [CreateVpcConnectionResponseTypeDef](./type_defs.md#createvpcconnectionresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DeleteConfigurationResponseTypeDef](./type_defs.md#deleteconfigurationresponsetypedef)
- [DeleteReplicatorResponseTypeDef](./type_defs.md#deletereplicatorresponsetypedef)
- [DeleteVpcConnectionResponseTypeDef](./type_defs.md#deletevpcconnectionresponsetypedef)
- [DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef)
- [DescribeTopicResponseTypeDef](./type_defs.md#describetopicresponsetypedef)
- [DescribeVpcConnectionResponseTypeDef](./type_defs.md#describevpcconnectionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetBootstrapBrokersResponseTypeDef](./type_defs.md#getbootstrapbrokersresponsetypedef)
- [GetClusterPolicyResponseTypeDef](./type_defs.md#getclusterpolicyresponsetypedef)
- [ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutClusterPolicyResponseTypeDef](./type_defs.md#putclusterpolicyresponsetypedef)
- [RebootBrokerResponseTypeDef](./type_defs.md#rebootbrokerresponsetypedef)
- [UpdateBrokerCountResponseTypeDef](./type_defs.md#updatebrokercountresponsetypedef)
- [UpdateBrokerStorageResponseTypeDef](./type_defs.md#updatebrokerstorageresponsetypedef)
- [UpdateBrokerTypeResponseTypeDef](./type_defs.md#updatebrokertyperesponsetypedef)
- [UpdateClusterConfigurationResponseTypeDef](./type_defs.md#updateclusterconfigurationresponsetypedef)
- [UpdateClusterKafkaVersionResponseTypeDef](./type_defs.md#updateclusterkafkaversionresponsetypedef)
- [UpdateConnectivityResponseTypeDef](./type_defs.md#updateconnectivityresponsetypedef)
- [UpdateMonitoringResponseTypeDef](./type_defs.md#updatemonitoringresponsetypedef)
- [UpdateRebalancingResponseTypeDef](./type_defs.md#updaterebalancingresponsetypedef)
- [UpdateReplicationInfoResponseTypeDef](./type_defs.md#updatereplicationinforesponsetypedef)
- [UpdateSecurityResponseTypeDef](./type_defs.md#updatesecurityresponsetypedef)
- [UpdateStorageResponseTypeDef](./type_defs.md#updatestorageresponsetypedef)
- [BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef)
- [BatchDisassociateScramSecretResponseTypeDef](./type_defs.md#batchdisassociatescramsecretresponsetypedef)
- [CreateConfigurationRequestTypeDef](./type_defs.md#createconfigurationrequesttypedef)
- [UpdateConfigurationRequestTypeDef](./type_defs.md#updateconfigurationrequesttypedef)
- [BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef)
- [EBSStorageInfoTypeDef](./type_defs.md#ebsstorageinfotypedef)
- [UpdateStorageRequestTypeDef](./type_defs.md#updatestoragerequesttypedef)
- [BrokerLogsTypeDef](./type_defs.md#brokerlogstypedef)
- [BrokerNodeInfoTypeDef](./type_defs.md#brokernodeinfotypedef)
- [ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef)
- [UpdateRebalancingRequestTypeDef](./type_defs.md#updaterebalancingrequesttypedef)
- [ClusterOperationStepTypeDef](./type_defs.md#clusteroperationsteptypedef)
- [ListClusterOperationsV2ResponseTypeDef](./type_defs.md#listclusteroperationsv2responsetypedef)
- [GetCompatibleKafkaVersionsResponseTypeDef](./type_defs.md#getcompatiblekafkaversionsresponsetypedef)
- [UpdateClusterConfigurationRequestTypeDef](./type_defs.md#updateclusterconfigurationrequesttypedef)
- [UpdateClusterKafkaVersionRequestTypeDef](./type_defs.md#updateclusterkafkaversionrequesttypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef)
- [DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef)
- [ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef)
- [UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef)
- [ConsumerGroupReplicationUnionTypeDef](./type_defs.md#consumergroupreplicationuniontypedef)
- [DescribeTopicPartitionsRequestPaginateTypeDef](./type_defs.md#describetopicpartitionsrequestpaginatetypedef)
- [ListClientVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listclientvpcconnectionsrequestpaginatetypedef)
- [ListClusterOperationsRequestPaginateTypeDef](./type_defs.md#listclusteroperationsrequestpaginatetypedef)
- [ListClusterOperationsV2RequestPaginateTypeDef](./type_defs.md#listclusteroperationsv2requestpaginatetypedef)
- [ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
- [ListClustersV2RequestPaginateTypeDef](./type_defs.md#listclustersv2requestpaginatetypedef)
- [ListConfigurationRevisionsRequestPaginateTypeDef](./type_defs.md#listconfigurationrevisionsrequestpaginatetypedef)
- [ListConfigurationsRequestPaginateTypeDef](./type_defs.md#listconfigurationsrequestpaginatetypedef)
- [ListKafkaVersionsRequestPaginateTypeDef](./type_defs.md#listkafkaversionsrequestpaginatetypedef)
- [ListNodesRequestPaginateTypeDef](./type_defs.md#listnodesrequestpaginatetypedef)
- [ListReplicatorsRequestPaginateTypeDef](./type_defs.md#listreplicatorsrequestpaginatetypedef)
- [ListScramSecretsRequestPaginateTypeDef](./type_defs.md#listscramsecretsrequestpaginatetypedef)
- [ListTopicsRequestPaginateTypeDef](./type_defs.md#listtopicsrequestpaginatetypedef)
- [ListVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listvpcconnectionsrequestpaginatetypedef)
- [DescribeTopicPartitionsResponseTypeDef](./type_defs.md#describetopicpartitionsresponsetypedef)
- [EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef)
- [ServerlessSaslTypeDef](./type_defs.md#serverlesssasltypedef)
- [KafkaClusterDescriptionTypeDef](./type_defs.md#kafkaclusterdescriptiontypedef)
- [KafkaClusterClientVpcConfigUnionTypeDef](./type_defs.md#kafkaclusterclientvpcconfiguniontypedef)
- [ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef)
- [ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef)
- [ListVpcConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef)
- [PrometheusInfoTypeDef](./type_defs.md#prometheusinfotypedef)
- [PrometheusTypeDef](./type_defs.md#prometheustypedef)
- [TopicReplicationOutputTypeDef](./type_defs.md#topicreplicationoutputtypedef)
- [TopicReplicationTypeDef](./type_defs.md#topicreplicationtypedef)
- [SaslTypeDef](./type_defs.md#sasltypedef)
- [TlsUnionTypeDef](./type_defs.md#tlsuniontypedef)
- [UpdateReplicationInfoRequestTypeDef](./type_defs.md#updatereplicationinforequesttypedef)
- [VpcConnectionInfoServerlessTypeDef](./type_defs.md#vpcconnectioninfoserverlesstypedef)
- [VpcConnectionInfoTypeDef](./type_defs.md#vpcconnectioninfotypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [VpcConnectivitySaslTypeDef](./type_defs.md#vpcconnectivitysasltypedef)
- [ReplicatorSummaryTypeDef](./type_defs.md#replicatorsummarytypedef)
- [UpdateBrokerStorageRequestTypeDef](./type_defs.md#updatebrokerstoragerequesttypedef)
- [StorageInfoTypeDef](./type_defs.md#storageinfotypedef)
- [LoggingInfoTypeDef](./type_defs.md#logginginfotypedef)
- [NodeInfoTypeDef](./type_defs.md#nodeinfotypedef)
- [ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)
- [ServerlessClientAuthenticationTypeDef](./type_defs.md#serverlessclientauthenticationtypedef)
- [KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef)
- [OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef)
- [OpenMonitoringTypeDef](./type_defs.md#openmonitoringtypedef)
- [ReplicationInfoDescriptionTypeDef](./type_defs.md#replicationinfodescriptiontypedef)
- [TopicReplicationUnionTypeDef](./type_defs.md#topicreplicationuniontypedef)
- [ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef)
- [ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef)
- [ClusterOperationV2ServerlessTypeDef](./type_defs.md#clusteroperationv2serverlesstypedef)
- [VpcConnectivityClientAuthenticationTypeDef](./type_defs.md#vpcconnectivityclientauthenticationtypedef)
- [ListReplicatorsResponseTypeDef](./type_defs.md#listreplicatorsresponsetypedef)
- [ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef)
- [ServerlessRequestTypeDef](./type_defs.md#serverlessrequesttypedef)
- [ServerlessTypeDef](./type_defs.md#serverlesstypedef)
- [UpdateMonitoringRequestTypeDef](./type_defs.md#updatemonitoringrequesttypedef)
- [DescribeReplicatorResponseTypeDef](./type_defs.md#describereplicatorresponsetypedef)
- [ReplicationInfoTypeDef](./type_defs.md#replicationinfotypedef)
- [ClientAuthenticationUnionTypeDef](./type_defs.md#clientauthenticationuniontypedef)
- [VpcConnectivityTypeDef](./type_defs.md#vpcconnectivitytypedef)
- [CreateReplicatorRequestTypeDef](./type_defs.md#createreplicatorrequesttypedef)
- [UpdateSecurityRequestTypeDef](./type_defs.md#updatesecurityrequesttypedef)
- [ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef)
- [BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef)
- [BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef)
- [MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef)
- [UpdateConnectivityRequestTypeDef](./type_defs.md#updateconnectivityrequesttypedef)
- [ClusterInfoTypeDef](./type_defs.md#clusterinfotypedef)
- [ProvisionedTypeDef](./type_defs.md#provisionedtypedef)
- [BrokerNodeGroupInfoUnionTypeDef](./type_defs.md#brokernodegroupinfouniontypedef)
- [ClusterOperationInfoTypeDef](./type_defs.md#clusteroperationinfotypedef)
- [ClusterOperationV2ProvisionedTypeDef](./type_defs.md#clusteroperationv2provisionedtypedef)
- [DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
- [ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef)
- [DescribeClusterOperationResponseTypeDef](./type_defs.md#describeclusteroperationresponsetypedef)
- [ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef)
- [ClusterOperationV2TypeDef](./type_defs.md#clusteroperationv2typedef)
- [DescribeClusterV2ResponseTypeDef](./type_defs.md#describeclusterv2responsetypedef)
- [ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef)
- [CreateClusterV2RequestTypeDef](./type_defs.md#createclusterv2requesttypedef)
- [DescribeClusterOperationV2ResponseTypeDef](./type_defs.md#describeclusteroperationv2responsetypedef)

