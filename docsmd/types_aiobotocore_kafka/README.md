# Kafka module

> [Index](../README.md) > Kafka


!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
# ListClientVpcConnectionsPaginator usage example

from types_aiobotocore_kafka.paginator import ListClientVpcConnectionsPaginator

def get_list_client_vpc_connections_paginator() -> ListClientVpcConnectionsPaginator:
    return client.get_paginator("list_client_vpc_connections"))
```

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
- [ListVpcConnectionsPaginatorName](./literals.md#listvpcconnectionspaginatorname)
- [NodeTypeType](./literals.md#nodetypetype)
- [ReplicationStartingPositionTypeType](./literals.md#replicationstartingpositiontypetype)
- [ReplicationTopicNameConfigurationTypeType](./literals.md#replicationtopicnameconfigurationtypetype)
- [ReplicatorStateType](./literals.md#replicatorstatetype)
- [StorageModeType](./literals.md#storagemodetype)
- [TargetCompressionTypeType](./literals.md#targetcompressiontypetype)
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
- [BatchAssociateScramSecretRequestRequestTypeDef](./type_defs.md#batchassociatescramsecretrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UnprocessedScramSecretTypeDef](./type_defs.md#unprocessedscramsecrettypedef)
- [BatchDisassociateScramSecretRequestRequestTypeDef](./type_defs.md#batchdisassociatescramsecretrequestrequesttypedef)
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
- [CreateVpcConnectionRequestRequestTypeDef](./type_defs.md#createvpcconnectionrequestrequesttypedef)
- [DeleteClusterPolicyRequestRequestTypeDef](./type_defs.md#deleteclusterpolicyrequestrequesttypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteConfigurationRequestRequestTypeDef](./type_defs.md#deleteconfigurationrequestrequesttypedef)
- [DeleteReplicatorRequestRequestTypeDef](./type_defs.md#deletereplicatorrequestrequesttypedef)
- [DeleteVpcConnectionRequestRequestTypeDef](./type_defs.md#deletevpcconnectionrequestrequesttypedef)
- [DescribeClusterOperationRequestRequestTypeDef](./type_defs.md#describeclusteroperationrequestrequesttypedef)
- [DescribeClusterOperationV2RequestRequestTypeDef](./type_defs.md#describeclusteroperationv2requestrequesttypedef)
- [DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef)
- [DescribeClusterV2RequestRequestTypeDef](./type_defs.md#describeclusterv2requestrequesttypedef)
- [DescribeConfigurationRequestRequestTypeDef](./type_defs.md#describeconfigurationrequestrequesttypedef)
- [DescribeConfigurationRevisionRequestRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequestrequesttypedef)
- [DescribeReplicatorRequestRequestTypeDef](./type_defs.md#describereplicatorrequestrequesttypedef)
- [ReplicationStateInfoTypeDef](./type_defs.md#replicationstateinfotypedef)
- [DescribeVpcConnectionRequestRequestTypeDef](./type_defs.md#describevpcconnectionrequestrequesttypedef)
- [EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef)
- [EncryptionInTransitTypeDef](./type_defs.md#encryptionintransittypedef)
- [GetBootstrapBrokersRequestRequestTypeDef](./type_defs.md#getbootstrapbrokersrequestrequesttypedef)
- [GetClusterPolicyRequestRequestTypeDef](./type_defs.md#getclusterpolicyrequestrequesttypedef)
- [GetCompatibleKafkaVersionsRequestRequestTypeDef](./type_defs.md#getcompatiblekafkaversionsrequestrequesttypedef)
- [IamTypeDef](./type_defs.md#iamtypedef)
- [JmxExporterInfoTypeDef](./type_defs.md#jmxexporterinfotypedef)
- [JmxExporterTypeDef](./type_defs.md#jmxexportertypedef)
- [KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef)
- [KafkaClusterClientVpcConfigTypeDef](./type_defs.md#kafkaclusterclientvpcconfigtypedef)
- [KafkaVersionTypeDef](./type_defs.md#kafkaversiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListClientVpcConnectionsRequestRequestTypeDef](./type_defs.md#listclientvpcconnectionsrequestrequesttypedef)
- [ListClusterOperationsRequestRequestTypeDef](./type_defs.md#listclusteroperationsrequestrequesttypedef)
- [ListClusterOperationsV2RequestRequestTypeDef](./type_defs.md#listclusteroperationsv2requestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListClustersV2RequestRequestTypeDef](./type_defs.md#listclustersv2requestrequesttypedef)
- [ListConfigurationRevisionsRequestRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequestrequesttypedef)
- [ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef)
- [ListKafkaVersionsRequestRequestTypeDef](./type_defs.md#listkafkaversionsrequestrequesttypedef)
- [ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef)
- [ListReplicatorsRequestRequestTypeDef](./type_defs.md#listreplicatorsrequestrequesttypedef)
- [ListScramSecretsRequestRequestTypeDef](./type_defs.md#listscramsecretsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVpcConnectionsRequestRequestTypeDef](./type_defs.md#listvpcconnectionsrequestrequesttypedef)
- [VpcConnectionTypeDef](./type_defs.md#vpcconnectiontypedef)
- [NodeExporterInfoTypeDef](./type_defs.md#nodeexporterinfotypedef)
- [NodeExporterTypeDef](./type_defs.md#nodeexportertypedef)
- [ZookeeperNodeInfoTypeDef](./type_defs.md#zookeepernodeinfotypedef)
- [PutClusterPolicyRequestRequestTypeDef](./type_defs.md#putclusterpolicyrequestrequesttypedef)
- [RebootBrokerRequestRequestTypeDef](./type_defs.md#rebootbrokerrequestrequesttypedef)
- [RejectClientVpcConnectionRequestRequestTypeDef](./type_defs.md#rejectclientvpcconnectionrequestrequesttypedef)
- [ReplicationInfoSummaryTypeDef](./type_defs.md#replicationinfosummarytypedef)
- [ReplicationStartingPositionTypeDef](./type_defs.md#replicationstartingpositiontypedef)
- [ReplicationTopicNameConfigurationTypeDef](./type_defs.md#replicationtopicnameconfigurationtypedef)
- [ScramTypeDef](./type_defs.md#scramtypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TlsTypeDef](./type_defs.md#tlstypedef)
- [TopicReplicationUpdateTypeDef](./type_defs.md#topicreplicationupdatetypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateBrokerCountRequestRequestTypeDef](./type_defs.md#updatebrokercountrequestrequesttypedef)
- [UpdateBrokerTypeRequestRequestTypeDef](./type_defs.md#updatebrokertyperequestrequesttypedef)
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
- [UpdateReplicationInfoResponseTypeDef](./type_defs.md#updatereplicationinforesponsetypedef)
- [UpdateSecurityResponseTypeDef](./type_defs.md#updatesecurityresponsetypedef)
- [UpdateStorageResponseTypeDef](./type_defs.md#updatestorageresponsetypedef)
- [BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef)
- [BatchDisassociateScramSecretResponseTypeDef](./type_defs.md#batchdisassociatescramsecretresponsetypedef)
- [CreateConfigurationRequestRequestTypeDef](./type_defs.md#createconfigurationrequestrequesttypedef)
- [UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef)
- [BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef)
- [EBSStorageInfoTypeDef](./type_defs.md#ebsstorageinfotypedef)
- [UpdateStorageRequestRequestTypeDef](./type_defs.md#updatestoragerequestrequesttypedef)
- [BrokerLogsTypeDef](./type_defs.md#brokerlogstypedef)
- [BrokerNodeInfoTypeDef](./type_defs.md#brokernodeinfotypedef)
- [ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef)
- [ClusterOperationStepTypeDef](./type_defs.md#clusteroperationsteptypedef)
- [ListClusterOperationsV2ResponseTypeDef](./type_defs.md#listclusteroperationsv2responsetypedef)
- [GetCompatibleKafkaVersionsResponseTypeDef](./type_defs.md#getcompatiblekafkaversionsresponsetypedef)
- [UpdateClusterConfigurationRequestRequestTypeDef](./type_defs.md#updateclusterconfigurationrequestrequesttypedef)
- [UpdateClusterKafkaVersionRequestRequestTypeDef](./type_defs.md#updateclusterkafkaversionrequestrequesttypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef)
- [DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef)
- [ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef)
- [UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef)
- [ConsumerGroupReplicationUnionTypeDef](./type_defs.md#consumergroupreplicationuniontypedef)
- [EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef)
- [ServerlessSaslTypeDef](./type_defs.md#serverlesssasltypedef)
- [KafkaClusterDescriptionTypeDef](./type_defs.md#kafkaclusterdescriptiontypedef)
- [KafkaClusterClientVpcConfigUnionTypeDef](./type_defs.md#kafkaclusterclientvpcconfiguniontypedef)
- [ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef)
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
- [ListVpcConnectionsRequestPaginateTypeDef](./type_defs.md#listvpcconnectionsrequestpaginatetypedef)
- [ListVpcConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef)
- [PrometheusInfoTypeDef](./type_defs.md#prometheusinfotypedef)
- [PrometheusTypeDef](./type_defs.md#prometheustypedef)
- [TopicReplicationOutputTypeDef](./type_defs.md#topicreplicationoutputtypedef)
- [TopicReplicationTypeDef](./type_defs.md#topicreplicationtypedef)
- [SaslTypeDef](./type_defs.md#sasltypedef)
- [TlsUnionTypeDef](./type_defs.md#tlsuniontypedef)
- [UpdateReplicationInfoRequestRequestTypeDef](./type_defs.md#updatereplicationinforequestrequesttypedef)
- [VpcConnectionInfoServerlessTypeDef](./type_defs.md#vpcconnectioninfoserverlesstypedef)
- [VpcConnectionInfoTypeDef](./type_defs.md#vpcconnectioninfotypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [VpcConnectivitySaslTypeDef](./type_defs.md#vpcconnectivitysasltypedef)
- [ReplicatorSummaryTypeDef](./type_defs.md#replicatorsummarytypedef)
- [UpdateBrokerStorageRequestRequestTypeDef](./type_defs.md#updatebrokerstoragerequestrequesttypedef)
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
- [UpdateMonitoringRequestRequestTypeDef](./type_defs.md#updatemonitoringrequestrequesttypedef)
- [DescribeReplicatorResponseTypeDef](./type_defs.md#describereplicatorresponsetypedef)
- [ReplicationInfoTypeDef](./type_defs.md#replicationinfotypedef)
- [ClientAuthenticationUnionTypeDef](./type_defs.md#clientauthenticationuniontypedef)
- [UpdateSecurityRequestRequestTypeDef](./type_defs.md#updatesecurityrequestrequesttypedef)
- [VpcConnectivityTypeDef](./type_defs.md#vpcconnectivitytypedef)
- [CreateReplicatorRequestRequestTypeDef](./type_defs.md#createreplicatorrequestrequesttypedef)
- [ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef)
- [BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef)
- [BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef)
- [MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef)
- [UpdateConnectivityRequestRequestTypeDef](./type_defs.md#updateconnectivityrequestrequesttypedef)
- [ClusterInfoTypeDef](./type_defs.md#clusterinfotypedef)
- [ProvisionedTypeDef](./type_defs.md#provisionedtypedef)
- [BrokerNodeGroupInfoUnionTypeDef](./type_defs.md#brokernodegroupinfouniontypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [ClusterOperationInfoTypeDef](./type_defs.md#clusteroperationinfotypedef)
- [ClusterOperationV2ProvisionedTypeDef](./type_defs.md#clusteroperationv2provisionedtypedef)
- [DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef)
- [DescribeClusterOperationResponseTypeDef](./type_defs.md#describeclusteroperationresponsetypedef)
- [ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef)
- [ClusterOperationV2TypeDef](./type_defs.md#clusteroperationv2typedef)
- [DescribeClusterV2ResponseTypeDef](./type_defs.md#describeclusterv2responsetypedef)
- [ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef)
- [CreateClusterV2RequestRequestTypeDef](./type_defs.md#createclusterv2requestrequesttypedef)
- [DescribeClusterOperationV2ResponseTypeDef](./type_defs.md#describeclusteroperationv2responsetypedef)

