# Type definitions

> [Index](../README.md) > [Kafka](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ConsumerGroupReplicationUnionTypeDef

```python
# ConsumerGroupReplicationUnionTypeDef definition

ConsumerGroupReplicationUnionTypeDef = Union[
    ConsumerGroupReplicationTypeDef,  # (1)
    ConsumerGroupReplicationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConsumerGroupReplicationTypeDef](./type_defs.md#consumergroupreplicationtypedef) 
2. See [:material-code-braces: ConsumerGroupReplicationOutputTypeDef](./type_defs.md#consumergroupreplicationoutputtypedef) 

## KafkaClusterClientVpcConfigUnionTypeDef

```python
# KafkaClusterClientVpcConfigUnionTypeDef definition

KafkaClusterClientVpcConfigUnionTypeDef = Union[
    KafkaClusterClientVpcConfigTypeDef,  # (1)
    KafkaClusterClientVpcConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KafkaClusterClientVpcConfigTypeDef](./type_defs.md#kafkaclusterclientvpcconfigtypedef) 
2. See [:material-code-braces: KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef) 

## TlsUnionTypeDef

```python
# TlsUnionTypeDef definition

TlsUnionTypeDef = Union[
    TlsTypeDef,  # (1)
    TlsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TlsTypeDef](./type_defs.md#tlstypedef) 
2. See [:material-code-braces: TlsOutputTypeDef](./type_defs.md#tlsoutputtypedef) 

## VpcConfigUnionTypeDef

```python
# VpcConfigUnionTypeDef definition

VpcConfigUnionTypeDef = Union[
    VpcConfigTypeDef,  # (1)
    VpcConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 

## TopicReplicationUnionTypeDef

```python
# TopicReplicationUnionTypeDef definition

TopicReplicationUnionTypeDef = Union[
    TopicReplicationTypeDef,  # (1)
    TopicReplicationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TopicReplicationTypeDef](./type_defs.md#topicreplicationtypedef) 
2. See [:material-code-braces: TopicReplicationOutputTypeDef](./type_defs.md#topicreplicationoutputtypedef) 

## ClientAuthenticationUnionTypeDef

```python
# ClientAuthenticationUnionTypeDef definition

ClientAuthenticationUnionTypeDef = Union[
    ClientAuthenticationTypeDef,  # (1)
    ClientAuthenticationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) 
2. See [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 

## BrokerNodeGroupInfoUnionTypeDef

```python
# BrokerNodeGroupInfoUnionTypeDef definition

BrokerNodeGroupInfoUnionTypeDef = Union[
    BrokerNodeGroupInfoTypeDef,  # (1)
    BrokerNodeGroupInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef) 
2. See [:material-code-braces: BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef) 



## AmazonMskClusterTypeDef

```python
# AmazonMskClusterTypeDef definition

class AmazonMskClusterTypeDef(TypedDict):
    MskClusterArn: str,
```

## BatchAssociateScramSecretRequestRequestTypeDef

```python
# BatchAssociateScramSecretRequestRequestTypeDef definition

class BatchAssociateScramSecretRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    SecretArnList: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## UnprocessedScramSecretTypeDef

```python
# UnprocessedScramSecretTypeDef definition

class UnprocessedScramSecretTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    SecretArn: NotRequired[str],
```

## BatchDisassociateScramSecretRequestRequestTypeDef

```python
# BatchDisassociateScramSecretRequestRequestTypeDef definition

class BatchDisassociateScramSecretRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    SecretArnList: Sequence[str],
```

## BrokerCountUpdateInfoTypeDef

```python
# BrokerCountUpdateInfoTypeDef definition

class BrokerCountUpdateInfoTypeDef(TypedDict):
    CreatedBrokerIds: NotRequired[List[float]],
    DeletedBrokerIds: NotRequired[List[float]],
```

## ProvisionedThroughputTypeDef

```python
# ProvisionedThroughputTypeDef definition

class ProvisionedThroughputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    VolumeThroughput: NotRequired[int],
```

## CloudWatchLogsTypeDef

```python
# CloudWatchLogsTypeDef definition

class CloudWatchLogsTypeDef(TypedDict):
    Enabled: bool,
    LogGroup: NotRequired[str],
```

## FirehoseTypeDef

```python
# FirehoseTypeDef definition

class FirehoseTypeDef(TypedDict):
    Enabled: bool,
    DeliveryStream: NotRequired[str],
```

## S3TypeDef

```python
# S3TypeDef definition

class S3TypeDef(TypedDict):
    Enabled: bool,
    Bucket: NotRequired[str],
    Prefix: NotRequired[str],
```

## BrokerSoftwareInfoTypeDef

```python
# BrokerSoftwareInfoTypeDef definition

class BrokerSoftwareInfoTypeDef(TypedDict):
    ConfigurationArn: NotRequired[str],
    ConfigurationRevision: NotRequired[int],
    KafkaVersion: NotRequired[str],
```

## TlsOutputTypeDef

```python
# TlsOutputTypeDef definition

class TlsOutputTypeDef(TypedDict):
    CertificateAuthorityArnList: NotRequired[List[str]],
    Enabled: NotRequired[bool],
```

## UnauthenticatedTypeDef

```python
# UnauthenticatedTypeDef definition

class UnauthenticatedTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## ClientVpcConnectionTypeDef

```python
# ClientVpcConnectionTypeDef definition

class ClientVpcConnectionTypeDef(TypedDict):
    VpcConnectionArn: str,
    Authentication: NotRequired[str],
    CreationTime: NotRequired[datetime],
    State: NotRequired[VpcConnectionStateType],  # (1)
    Owner: NotRequired[str],
```

1. See [:material-code-brackets: VpcConnectionStateType](./literals.md#vpcconnectionstatetype) 
## StateInfoTypeDef

```python
# StateInfoTypeDef definition

class StateInfoTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorString: NotRequired[str],
```

## ClusterOperationStepInfoTypeDef

```python
# ClusterOperationStepInfoTypeDef definition

class ClusterOperationStepInfoTypeDef(TypedDict):
    StepStatus: NotRequired[str],
```

## ClusterOperationV2SummaryTypeDef

```python
# ClusterOperationV2SummaryTypeDef definition

class ClusterOperationV2SummaryTypeDef(TypedDict):
    ClusterArn: NotRequired[str],
    ClusterType: NotRequired[ClusterTypeType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    OperationArn: NotRequired[str],
    OperationState: NotRequired[str],
    OperationType: NotRequired[str],
```

1. See [:material-code-brackets: ClusterTypeType](./literals.md#clustertypetype) 
## CompatibleKafkaVersionTypeDef

```python
# CompatibleKafkaVersionTypeDef definition

class CompatibleKafkaVersionTypeDef(TypedDict):
    SourceVersion: NotRequired[str],
    TargetVersions: NotRequired[List[str]],
```

## ConfigurationInfoTypeDef

```python
# ConfigurationInfoTypeDef definition

class ConfigurationInfoTypeDef(TypedDict):
    Arn: str,
    Revision: int,
```

## ConfigurationRevisionTypeDef

```python
# ConfigurationRevisionTypeDef definition

class ConfigurationRevisionTypeDef(TypedDict):
    CreationTime: datetime,
    Revision: int,
    Description: NotRequired[str],
```

## PublicAccessTypeDef

```python
# PublicAccessTypeDef definition

class PublicAccessTypeDef(TypedDict):
    Type: NotRequired[str],
```

## ConsumerGroupReplicationOutputTypeDef

```python
# ConsumerGroupReplicationOutputTypeDef definition

class ConsumerGroupReplicationOutputTypeDef(TypedDict):
    ConsumerGroupsToReplicate: List[str],
    ConsumerGroupsToExclude: NotRequired[List[str]],
    DetectAndCopyNewConsumerGroups: NotRequired[bool],
    SynchroniseConsumerGroupOffsets: NotRequired[bool],
```

## ConsumerGroupReplicationTypeDef

```python
# ConsumerGroupReplicationTypeDef definition

class ConsumerGroupReplicationTypeDef(TypedDict):
    ConsumerGroupsToReplicate: Sequence[str],
    ConsumerGroupsToExclude: NotRequired[Sequence[str]],
    DetectAndCopyNewConsumerGroups: NotRequired[bool],
    SynchroniseConsumerGroupOffsets: NotRequired[bool],
```

## ConsumerGroupReplicationUpdateTypeDef

```python
# ConsumerGroupReplicationUpdateTypeDef definition

class ConsumerGroupReplicationUpdateTypeDef(TypedDict):
    ConsumerGroupsToExclude: Sequence[str],
    ConsumerGroupsToReplicate: Sequence[str],
    DetectAndCopyNewConsumerGroups: bool,
    SynchroniseConsumerGroupOffsets: bool,
```

## ControllerNodeInfoTypeDef

```python
# ControllerNodeInfoTypeDef definition

class ControllerNodeInfoTypeDef(TypedDict):
    Endpoints: NotRequired[List[str]],
```

## CreateVpcConnectionRequestRequestTypeDef

```python
# CreateVpcConnectionRequestRequestTypeDef definition

class CreateVpcConnectionRequestRequestTypeDef(TypedDict):
    TargetClusterArn: str,
    Authentication: str,
    VpcId: str,
    ClientSubnets: Sequence[str],
    SecurityGroups: Sequence[str],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteClusterPolicyRequestRequestTypeDef

```python
# DeleteClusterPolicyRequestRequestTypeDef definition

class DeleteClusterPolicyRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: NotRequired[str],
```

## DeleteConfigurationRequestRequestTypeDef

```python
# DeleteConfigurationRequestRequestTypeDef definition

class DeleteConfigurationRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteReplicatorRequestRequestTypeDef

```python
# DeleteReplicatorRequestRequestTypeDef definition

class DeleteReplicatorRequestRequestTypeDef(TypedDict):
    ReplicatorArn: str,
    CurrentVersion: NotRequired[str],
```

## DeleteVpcConnectionRequestRequestTypeDef

```python
# DeleteVpcConnectionRequestRequestTypeDef definition

class DeleteVpcConnectionRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DescribeClusterOperationRequestRequestTypeDef

```python
# DescribeClusterOperationRequestRequestTypeDef definition

class DescribeClusterOperationRequestRequestTypeDef(TypedDict):
    ClusterOperationArn: str,
```

## DescribeClusterOperationV2RequestRequestTypeDef

```python
# DescribeClusterOperationV2RequestRequestTypeDef definition

class DescribeClusterOperationV2RequestRequestTypeDef(TypedDict):
    ClusterOperationArn: str,
```

## DescribeClusterRequestRequestTypeDef

```python
# DescribeClusterRequestRequestTypeDef definition

class DescribeClusterRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DescribeClusterV2RequestRequestTypeDef

```python
# DescribeClusterV2RequestRequestTypeDef definition

class DescribeClusterV2RequestRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DescribeConfigurationRequestRequestTypeDef

```python
# DescribeConfigurationRequestRequestTypeDef definition

class DescribeConfigurationRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DescribeConfigurationRevisionRequestRequestTypeDef

```python
# DescribeConfigurationRevisionRequestRequestTypeDef definition

class DescribeConfigurationRevisionRequestRequestTypeDef(TypedDict):
    Arn: str,
    Revision: int,
```

## DescribeReplicatorRequestRequestTypeDef

```python
# DescribeReplicatorRequestRequestTypeDef definition

class DescribeReplicatorRequestRequestTypeDef(TypedDict):
    ReplicatorArn: str,
```

## ReplicationStateInfoTypeDef

```python
# ReplicationStateInfoTypeDef definition

class ReplicationStateInfoTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## DescribeVpcConnectionRequestRequestTypeDef

```python
# DescribeVpcConnectionRequestRequestTypeDef definition

class DescribeVpcConnectionRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## EncryptionAtRestTypeDef

```python
# EncryptionAtRestTypeDef definition

class EncryptionAtRestTypeDef(TypedDict):
    DataVolumeKMSKeyId: str,
```

## EncryptionInTransitTypeDef

```python
# EncryptionInTransitTypeDef definition

class EncryptionInTransitTypeDef(TypedDict):
    ClientBroker: NotRequired[ClientBrokerType],  # (1)
    InCluster: NotRequired[bool],
```

1. See [:material-code-brackets: ClientBrokerType](./literals.md#clientbrokertype) 
## GetBootstrapBrokersRequestRequestTypeDef

```python
# GetBootstrapBrokersRequestRequestTypeDef definition

class GetBootstrapBrokersRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## GetClusterPolicyRequestRequestTypeDef

```python
# GetClusterPolicyRequestRequestTypeDef definition

class GetClusterPolicyRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## GetCompatibleKafkaVersionsRequestRequestTypeDef

```python
# GetCompatibleKafkaVersionsRequestRequestTypeDef definition

class GetCompatibleKafkaVersionsRequestRequestTypeDef(TypedDict):
    ClusterArn: NotRequired[str],
```

## IamTypeDef

```python
# IamTypeDef definition

class IamTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## JmxExporterInfoTypeDef

```python
# JmxExporterInfoTypeDef definition

class JmxExporterInfoTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## JmxExporterTypeDef

```python
# JmxExporterTypeDef definition

class JmxExporterTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## KafkaClusterClientVpcConfigOutputTypeDef

```python
# KafkaClusterClientVpcConfigOutputTypeDef definition

class KafkaClusterClientVpcConfigOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: NotRequired[List[str]],
```

## KafkaClusterClientVpcConfigTypeDef

```python
# KafkaClusterClientVpcConfigTypeDef definition

class KafkaClusterClientVpcConfigTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## KafkaVersionTypeDef

```python
# KafkaVersionTypeDef definition

class KafkaVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    Status: NotRequired[KafkaVersionStatusType],  # (1)
```

1. See [:material-code-brackets: KafkaVersionStatusType](./literals.md#kafkaversionstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListClientVpcConnectionsRequestRequestTypeDef

```python
# ListClientVpcConnectionsRequestRequestTypeDef definition

class ListClientVpcConnectionsRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClusterOperationsRequestRequestTypeDef

```python
# ListClusterOperationsRequestRequestTypeDef definition

class ListClusterOperationsRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClusterOperationsV2RequestRequestTypeDef

```python
# ListClusterOperationsV2RequestRequestTypeDef definition

class ListClusterOperationsV2RequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClustersRequestRequestTypeDef

```python
# ListClustersRequestRequestTypeDef definition

class ListClustersRequestRequestTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClustersV2RequestRequestTypeDef

```python
# ListClustersV2RequestRequestTypeDef definition

class ListClustersV2RequestRequestTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    ClusterTypeFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationRevisionsRequestRequestTypeDef

```python
# ListConfigurationRevisionsRequestRequestTypeDef definition

class ListConfigurationRevisionsRequestRequestTypeDef(TypedDict):
    Arn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationsRequestRequestTypeDef

```python
# ListConfigurationsRequestRequestTypeDef definition

class ListConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListKafkaVersionsRequestRequestTypeDef

```python
# ListKafkaVersionsRequestRequestTypeDef definition

class ListKafkaVersionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListNodesRequestRequestTypeDef

```python
# ListNodesRequestRequestTypeDef definition

class ListNodesRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListReplicatorsRequestRequestTypeDef

```python
# ListReplicatorsRequestRequestTypeDef definition

class ListReplicatorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ReplicatorNameFilter: NotRequired[str],
```

## ListScramSecretsRequestRequestTypeDef

```python
# ListScramSecretsRequestRequestTypeDef definition

class ListScramSecretsRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVpcConnectionsRequestRequestTypeDef

```python
# ListVpcConnectionsRequestRequestTypeDef definition

class ListVpcConnectionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## VpcConnectionTypeDef

```python
# VpcConnectionTypeDef definition

class VpcConnectionTypeDef(TypedDict):
    VpcConnectionArn: str,
    TargetClusterArn: str,
    CreationTime: NotRequired[datetime],
    Authentication: NotRequired[str],
    VpcId: NotRequired[str],
    State: NotRequired[VpcConnectionStateType],  # (1)
```

1. See [:material-code-brackets: VpcConnectionStateType](./literals.md#vpcconnectionstatetype) 
## NodeExporterInfoTypeDef

```python
# NodeExporterInfoTypeDef definition

class NodeExporterInfoTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## NodeExporterTypeDef

```python
# NodeExporterTypeDef definition

class NodeExporterTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## ZookeeperNodeInfoTypeDef

```python
# ZookeeperNodeInfoTypeDef definition

class ZookeeperNodeInfoTypeDef(TypedDict):
    AttachedENIId: NotRequired[str],
    ClientVpcIpAddress: NotRequired[str],
    Endpoints: NotRequired[List[str]],
    ZookeeperId: NotRequired[float],
    ZookeeperVersion: NotRequired[str],
```

## PutClusterPolicyRequestRequestTypeDef

```python
# PutClusterPolicyRequestRequestTypeDef definition

class PutClusterPolicyRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    Policy: str,
    CurrentVersion: NotRequired[str],
```

## RebootBrokerRequestRequestTypeDef

```python
# RebootBrokerRequestRequestTypeDef definition

class RebootBrokerRequestRequestTypeDef(TypedDict):
    BrokerIds: Sequence[str],
    ClusterArn: str,
```

## RejectClientVpcConnectionRequestRequestTypeDef

```python
# RejectClientVpcConnectionRequestRequestTypeDef definition

class RejectClientVpcConnectionRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    VpcConnectionArn: str,
```

## ReplicationInfoSummaryTypeDef

```python
# ReplicationInfoSummaryTypeDef definition

class ReplicationInfoSummaryTypeDef(TypedDict):
    SourceKafkaClusterAlias: NotRequired[str],
    TargetKafkaClusterAlias: NotRequired[str],
```

## ReplicationStartingPositionTypeDef

```python
# ReplicationStartingPositionTypeDef definition

class ReplicationStartingPositionTypeDef(TypedDict):
    Type: NotRequired[ReplicationStartingPositionTypeType],  # (1)
```

1. See [:material-code-brackets: ReplicationStartingPositionTypeType](./literals.md#replicationstartingpositiontypetype) 
## ReplicationTopicNameConfigurationTypeDef

```python
# ReplicationTopicNameConfigurationTypeDef definition

class ReplicationTopicNameConfigurationTypeDef(TypedDict):
    Type: NotRequired[ReplicationTopicNameConfigurationTypeType],  # (1)
```

1. See [:material-code-brackets: ReplicationTopicNameConfigurationTypeType](./literals.md#replicationtopicnameconfigurationtypetype) 
## ScramTypeDef

```python
# ScramTypeDef definition

class ScramTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: NotRequired[List[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## TlsTypeDef

```python
# TlsTypeDef definition

class TlsTypeDef(TypedDict):
    CertificateAuthorityArnList: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

## TopicReplicationUpdateTypeDef

```python
# TopicReplicationUpdateTypeDef definition

class TopicReplicationUpdateTypeDef(TypedDict):
    CopyAccessControlListsForTopics: bool,
    CopyTopicConfigurations: bool,
    DetectAndCopyNewTopics: bool,
    TopicsToExclude: Sequence[str],
    TopicsToReplicate: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateBrokerCountRequestRequestTypeDef

```python
# UpdateBrokerCountRequestRequestTypeDef definition

class UpdateBrokerCountRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetNumberOfBrokerNodes: int,
```

## UpdateBrokerTypeRequestRequestTypeDef

```python
# UpdateBrokerTypeRequestRequestTypeDef definition

class UpdateBrokerTypeRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetInstanceType: str,
```

## UserIdentityTypeDef

```python
# UserIdentityTypeDef definition

class UserIdentityTypeDef(TypedDict):
    Type: NotRequired[UserIdentityTypeType],  # (1)
    PrincipalId: NotRequired[str],
```

1. See [:material-code-brackets: UserIdentityTypeType](./literals.md#useridentitytypetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## VpcConnectivityTlsTypeDef

```python
# VpcConnectivityTlsTypeDef definition

class VpcConnectivityTlsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConnectivityIamTypeDef

```python
# VpcConnectivityIamTypeDef definition

class VpcConnectivityIamTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConnectivityScramTypeDef

```python
# VpcConnectivityScramTypeDef definition

class VpcConnectivityScramTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## KafkaClusterSummaryTypeDef

```python
# KafkaClusterSummaryTypeDef definition

class KafkaClusterSummaryTypeDef(TypedDict):
    AmazonMskCluster: NotRequired[AmazonMskClusterTypeDef],  # (1)
    KafkaClusterAlias: NotRequired[str],
```

1. See [:material-code-braces: AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterName: str,
    State: ClusterStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterV2ResponseTypeDef

```python
# CreateClusterV2ResponseTypeDef definition

class CreateClusterV2ResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterName: str,
    State: ClusterStateType,  # (1)
    ClusterType: ClusterTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-brackets: ClusterTypeType](./literals.md#clustertypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicatorResponseTypeDef

```python
# CreateReplicatorResponseTypeDef definition

class CreateReplicatorResponseTypeDef(TypedDict):
    ReplicatorArn: str,
    ReplicatorName: str,
    ReplicatorState: ReplicatorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplicatorStateType](./literals.md#replicatorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcConnectionResponseTypeDef

```python
# CreateVpcConnectionResponseTypeDef definition

class CreateVpcConnectionResponseTypeDef(TypedDict):
    VpcConnectionArn: str,
    State: VpcConnectionStateType,  # (1)
    Authentication: str,
    VpcId: str,
    ClientSubnets: List[str],
    SecurityGroups: List[str],
    CreationTime: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VpcConnectionStateType](./literals.md#vpcconnectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    ClusterArn: str,
    State: ClusterStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteConfigurationResponseTypeDef

```python
# DeleteConfigurationResponseTypeDef definition

class DeleteConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    State: ConfigurationStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicatorResponseTypeDef

```python
# DeleteReplicatorResponseTypeDef definition

class DeleteReplicatorResponseTypeDef(TypedDict):
    ReplicatorArn: str,
    ReplicatorState: ReplicatorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplicatorStateType](./literals.md#replicatorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVpcConnectionResponseTypeDef

```python
# DeleteVpcConnectionResponseTypeDef definition

class DeleteVpcConnectionResponseTypeDef(TypedDict):
    VpcConnectionArn: str,
    State: VpcConnectionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VpcConnectionStateType](./literals.md#vpcconnectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationRevisionResponseTypeDef

```python
# DescribeConfigurationRevisionResponseTypeDef definition

class DescribeConfigurationRevisionResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    Description: str,
    Revision: int,
    ServerProperties: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVpcConnectionResponseTypeDef

```python
# DescribeVpcConnectionResponseTypeDef definition

class DescribeVpcConnectionResponseTypeDef(TypedDict):
    VpcConnectionArn: str,
    TargetClusterArn: str,
    State: VpcConnectionStateType,  # (1)
    Authentication: str,
    VpcId: str,
    Subnets: List[str],
    SecurityGroups: List[str],
    CreationTime: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VpcConnectionStateType](./literals.md#vpcconnectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBootstrapBrokersResponseTypeDef

```python
# GetBootstrapBrokersResponseTypeDef definition

class GetBootstrapBrokersResponseTypeDef(TypedDict):
    BootstrapBrokerString: str,
    BootstrapBrokerStringTls: str,
    BootstrapBrokerStringSaslScram: str,
    BootstrapBrokerStringSaslIam: str,
    BootstrapBrokerStringPublicTls: str,
    BootstrapBrokerStringPublicSaslScram: str,
    BootstrapBrokerStringPublicSaslIam: str,
    BootstrapBrokerStringVpcConnectivityTls: str,
    BootstrapBrokerStringVpcConnectivitySaslScram: str,
    BootstrapBrokerStringVpcConnectivitySaslIam: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterPolicyResponseTypeDef

```python
# GetClusterPolicyResponseTypeDef definition

class GetClusterPolicyResponseTypeDef(TypedDict):
    CurrentVersion: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScramSecretsResponseTypeDef

```python
# ListScramSecretsResponseTypeDef definition

class ListScramSecretsResponseTypeDef(TypedDict):
    SecretArnList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutClusterPolicyResponseTypeDef

```python
# PutClusterPolicyResponseTypeDef definition

class PutClusterPolicyResponseTypeDef(TypedDict):
    CurrentVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootBrokerResponseTypeDef

```python
# RebootBrokerResponseTypeDef definition

class RebootBrokerResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerCountResponseTypeDef

```python
# UpdateBrokerCountResponseTypeDef definition

class UpdateBrokerCountResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerStorageResponseTypeDef

```python
# UpdateBrokerStorageResponseTypeDef definition

class UpdateBrokerStorageResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerTypeResponseTypeDef

```python
# UpdateBrokerTypeResponseTypeDef definition

class UpdateBrokerTypeResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigurationResponseTypeDef

```python
# UpdateClusterConfigurationResponseTypeDef definition

class UpdateClusterConfigurationResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterKafkaVersionResponseTypeDef

```python
# UpdateClusterKafkaVersionResponseTypeDef definition

class UpdateClusterKafkaVersionResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectivityResponseTypeDef

```python
# UpdateConnectivityResponseTypeDef definition

class UpdateConnectivityResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitoringResponseTypeDef

```python
# UpdateMonitoringResponseTypeDef definition

class UpdateMonitoringResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationInfoResponseTypeDef

```python
# UpdateReplicationInfoResponseTypeDef definition

class UpdateReplicationInfoResponseTypeDef(TypedDict):
    ReplicatorArn: str,
    ReplicatorState: ReplicatorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplicatorStateType](./literals.md#replicatorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityResponseTypeDef

```python
# UpdateSecurityResponseTypeDef definition

class UpdateSecurityResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStorageResponseTypeDef

```python
# UpdateStorageResponseTypeDef definition

class UpdateStorageResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAssociateScramSecretResponseTypeDef

```python
# BatchAssociateScramSecretResponseTypeDef definition

class BatchAssociateScramSecretResponseTypeDef(TypedDict):
    ClusterArn: str,
    UnprocessedScramSecrets: List[UnprocessedScramSecretTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedScramSecretTypeDef](./type_defs.md#unprocessedscramsecrettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateScramSecretResponseTypeDef

```python
# BatchDisassociateScramSecretResponseTypeDef definition

class BatchDisassociateScramSecretResponseTypeDef(TypedDict):
    ClusterArn: str,
    UnprocessedScramSecrets: List[UnprocessedScramSecretTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedScramSecretTypeDef](./type_defs.md#unprocessedscramsecrettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationRequestRequestTypeDef

```python
# CreateConfigurationRequestRequestTypeDef definition

class CreateConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
    ServerProperties: BlobTypeDef,
    Description: NotRequired[str],
    KafkaVersions: NotRequired[Sequence[str]],
```

## UpdateConfigurationRequestRequestTypeDef

```python
# UpdateConfigurationRequestRequestTypeDef definition

class UpdateConfigurationRequestRequestTypeDef(TypedDict):
    Arn: str,
    ServerProperties: BlobTypeDef,
    Description: NotRequired[str],
```

## BrokerEBSVolumeInfoTypeDef

```python
# BrokerEBSVolumeInfoTypeDef definition

class BrokerEBSVolumeInfoTypeDef(TypedDict):
    KafkaBrokerNodeId: str,
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    VolumeSizeGB: NotRequired[int],
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## EBSStorageInfoTypeDef

```python
# EBSStorageInfoTypeDef definition

class EBSStorageInfoTypeDef(TypedDict):
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    VolumeSize: NotRequired[int],
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## UpdateStorageRequestRequestTypeDef

```python
# UpdateStorageRequestRequestTypeDef definition

class UpdateStorageRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    StorageMode: NotRequired[StorageModeType],  # (2)
    VolumeSizeGB: NotRequired[int],
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
2. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
## BrokerLogsTypeDef

```python
# BrokerLogsTypeDef definition

class BrokerLogsTypeDef(TypedDict):
    CloudWatchLogs: NotRequired[CloudWatchLogsTypeDef],  # (1)
    Firehose: NotRequired[FirehoseTypeDef],  # (2)
    S3: NotRequired[S3TypeDef],  # (3)
```

1. See [:material-code-braces: CloudWatchLogsTypeDef](./type_defs.md#cloudwatchlogstypedef) 
2. See [:material-code-braces: FirehoseTypeDef](./type_defs.md#firehosetypedef) 
3. See [:material-code-braces: S3TypeDef](./type_defs.md#s3typedef) 
## BrokerNodeInfoTypeDef

```python
# BrokerNodeInfoTypeDef definition

class BrokerNodeInfoTypeDef(TypedDict):
    AttachedENIId: NotRequired[str],
    BrokerId: NotRequired[float],
    ClientSubnet: NotRequired[str],
    ClientVpcIpAddress: NotRequired[str],
    CurrentBrokerSoftwareInfo: NotRequired[BrokerSoftwareInfoTypeDef],  # (1)
    Endpoints: NotRequired[List[str]],
```

1. See [:material-code-braces: BrokerSoftwareInfoTypeDef](./type_defs.md#brokersoftwareinfotypedef) 
## ListClientVpcConnectionsResponseTypeDef

```python
# ListClientVpcConnectionsResponseTypeDef definition

class ListClientVpcConnectionsResponseTypeDef(TypedDict):
    ClientVpcConnections: List[ClientVpcConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClientVpcConnectionTypeDef](./type_defs.md#clientvpcconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterOperationStepTypeDef

```python
# ClusterOperationStepTypeDef definition

class ClusterOperationStepTypeDef(TypedDict):
    StepInfo: NotRequired[ClusterOperationStepInfoTypeDef],  # (1)
    StepName: NotRequired[str],
```

1. See [:material-code-braces: ClusterOperationStepInfoTypeDef](./type_defs.md#clusteroperationstepinfotypedef) 
## ListClusterOperationsV2ResponseTypeDef

```python
# ListClusterOperationsV2ResponseTypeDef definition

class ListClusterOperationsV2ResponseTypeDef(TypedDict):
    ClusterOperationInfoList: List[ClusterOperationV2SummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterOperationV2SummaryTypeDef](./type_defs.md#clusteroperationv2summarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCompatibleKafkaVersionsResponseTypeDef

```python
# GetCompatibleKafkaVersionsResponseTypeDef definition

class GetCompatibleKafkaVersionsResponseTypeDef(TypedDict):
    CompatibleKafkaVersions: List[CompatibleKafkaVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompatibleKafkaVersionTypeDef](./type_defs.md#compatiblekafkaversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigurationRequestRequestTypeDef

```python
# UpdateClusterConfigurationRequestRequestTypeDef definition

class UpdateClusterConfigurationRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    ConfigurationInfo: ConfigurationInfoTypeDef,  # (1)
    CurrentVersion: str,
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
## UpdateClusterKafkaVersionRequestRequestTypeDef

```python
# UpdateClusterKafkaVersionRequestRequestTypeDef definition

class UpdateClusterKafkaVersionRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetKafkaVersion: str,
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    Description: str,
    KafkaVersions: List[str],
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    Name: str,
    State: ConfigurationStateType,  # (2)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
## CreateConfigurationResponseTypeDef

```python
# CreateConfigurationResponseTypeDef definition

class CreateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    Name: str,
    State: ConfigurationStateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationResponseTypeDef

```python
# DescribeConfigurationResponseTypeDef definition

class DescribeConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    Description: str,
    KafkaVersions: List[str],
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    Name: str,
    State: ConfigurationStateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationRevisionsResponseTypeDef

```python
# ListConfigurationRevisionsResponseTypeDef definition

class ListConfigurationRevisionsResponseTypeDef(TypedDict):
    Revisions: List[ConfigurationRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfigurationResponseTypeDef

```python
# UpdateConfigurationResponseTypeDef definition

class UpdateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptionInfoTypeDef

```python
# EncryptionInfoTypeDef definition

class EncryptionInfoTypeDef(TypedDict):
    EncryptionAtRest: NotRequired[EncryptionAtRestTypeDef],  # (1)
    EncryptionInTransit: NotRequired[EncryptionInTransitTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef) 
2. See [:material-code-braces: EncryptionInTransitTypeDef](./type_defs.md#encryptionintransittypedef) 
## ServerlessSaslTypeDef

```python
# ServerlessSaslTypeDef definition

class ServerlessSaslTypeDef(TypedDict):
    Iam: NotRequired[IamTypeDef],  # (1)
```

1. See [:material-code-braces: IamTypeDef](./type_defs.md#iamtypedef) 
## KafkaClusterDescriptionTypeDef

```python
# KafkaClusterDescriptionTypeDef definition

class KafkaClusterDescriptionTypeDef(TypedDict):
    AmazonMskCluster: NotRequired[AmazonMskClusterTypeDef],  # (1)
    KafkaClusterAlias: NotRequired[str],
    VpcConfig: NotRequired[KafkaClusterClientVpcConfigOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef) 
2. See [:material-code-braces: KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef) 
## ListKafkaVersionsResponseTypeDef

```python
# ListKafkaVersionsResponseTypeDef definition

class ListKafkaVersionsResponseTypeDef(TypedDict):
    KafkaVersions: List[KafkaVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: KafkaVersionTypeDef](./type_defs.md#kafkaversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClientVpcConnectionsRequestPaginateTypeDef

```python
# ListClientVpcConnectionsRequestPaginateTypeDef definition

class ListClientVpcConnectionsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClusterOperationsRequestPaginateTypeDef

```python
# ListClusterOperationsRequestPaginateTypeDef definition

class ListClusterOperationsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClusterOperationsV2RequestPaginateTypeDef

```python
# ListClusterOperationsV2RequestPaginateTypeDef definition

class ListClusterOperationsV2RequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersV2RequestPaginateTypeDef

```python
# ListClustersV2RequestPaginateTypeDef definition

class ListClustersV2RequestPaginateTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    ClusterTypeFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationRevisionsRequestPaginateTypeDef

```python
# ListConfigurationRevisionsRequestPaginateTypeDef definition

class ListConfigurationRevisionsRequestPaginateTypeDef(TypedDict):
    Arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationsRequestPaginateTypeDef

```python
# ListConfigurationsRequestPaginateTypeDef definition

class ListConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKafkaVersionsRequestPaginateTypeDef

```python
# ListKafkaVersionsRequestPaginateTypeDef definition

class ListKafkaVersionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodesRequestPaginateTypeDef

```python
# ListNodesRequestPaginateTypeDef definition

class ListNodesRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReplicatorsRequestPaginateTypeDef

```python
# ListReplicatorsRequestPaginateTypeDef definition

class ListReplicatorsRequestPaginateTypeDef(TypedDict):
    ReplicatorNameFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScramSecretsRequestPaginateTypeDef

```python
# ListScramSecretsRequestPaginateTypeDef definition

class ListScramSecretsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVpcConnectionsRequestPaginateTypeDef

```python
# ListVpcConnectionsRequestPaginateTypeDef definition

class ListVpcConnectionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVpcConnectionsResponseTypeDef

```python
# ListVpcConnectionsResponseTypeDef definition

class ListVpcConnectionsResponseTypeDef(TypedDict):
    VpcConnections: List[VpcConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VpcConnectionTypeDef](./type_defs.md#vpcconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrometheusInfoTypeDef

```python
# PrometheusInfoTypeDef definition

class PrometheusInfoTypeDef(TypedDict):
    JmxExporter: NotRequired[JmxExporterInfoTypeDef],  # (1)
    NodeExporter: NotRequired[NodeExporterInfoTypeDef],  # (2)
```

1. See [:material-code-braces: JmxExporterInfoTypeDef](./type_defs.md#jmxexporterinfotypedef) 
2. See [:material-code-braces: NodeExporterInfoTypeDef](./type_defs.md#nodeexporterinfotypedef) 
## PrometheusTypeDef

```python
# PrometheusTypeDef definition

class PrometheusTypeDef(TypedDict):
    JmxExporter: NotRequired[JmxExporterTypeDef],  # (1)
    NodeExporter: NotRequired[NodeExporterTypeDef],  # (2)
```

1. See [:material-code-braces: JmxExporterTypeDef](./type_defs.md#jmxexportertypedef) 
2. See [:material-code-braces: NodeExporterTypeDef](./type_defs.md#nodeexportertypedef) 
## TopicReplicationOutputTypeDef

```python
# TopicReplicationOutputTypeDef definition

class TopicReplicationOutputTypeDef(TypedDict):
    TopicsToReplicate: List[str],
    CopyAccessControlListsForTopics: NotRequired[bool],
    CopyTopicConfigurations: NotRequired[bool],
    DetectAndCopyNewTopics: NotRequired[bool],
    StartingPosition: NotRequired[ReplicationStartingPositionTypeDef],  # (1)
    TopicNameConfiguration: NotRequired[ReplicationTopicNameConfigurationTypeDef],  # (2)
    TopicsToExclude: NotRequired[List[str]],
```

1. See [:material-code-braces: ReplicationStartingPositionTypeDef](./type_defs.md#replicationstartingpositiontypedef) 
2. See [:material-code-braces: ReplicationTopicNameConfigurationTypeDef](./type_defs.md#replicationtopicnameconfigurationtypedef) 
## TopicReplicationTypeDef

```python
# TopicReplicationTypeDef definition

class TopicReplicationTypeDef(TypedDict):
    TopicsToReplicate: Sequence[str],
    CopyAccessControlListsForTopics: NotRequired[bool],
    CopyTopicConfigurations: NotRequired[bool],
    DetectAndCopyNewTopics: NotRequired[bool],
    StartingPosition: NotRequired[ReplicationStartingPositionTypeDef],  # (1)
    TopicNameConfiguration: NotRequired[ReplicationTopicNameConfigurationTypeDef],  # (2)
    TopicsToExclude: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ReplicationStartingPositionTypeDef](./type_defs.md#replicationstartingpositiontypedef) 
2. See [:material-code-braces: ReplicationTopicNameConfigurationTypeDef](./type_defs.md#replicationtopicnameconfigurationtypedef) 
## SaslTypeDef

```python
# SaslTypeDef definition

class SaslTypeDef(TypedDict):
    Scram: NotRequired[ScramTypeDef],  # (1)
    Iam: NotRequired[IamTypeDef],  # (2)
```

1. See [:material-code-braces: ScramTypeDef](./type_defs.md#scramtypedef) 
2. See [:material-code-braces: IamTypeDef](./type_defs.md#iamtypedef) 
## UpdateReplicationInfoRequestRequestTypeDef

```python
# UpdateReplicationInfoRequestRequestTypeDef definition

class UpdateReplicationInfoRequestRequestTypeDef(TypedDict):
    CurrentVersion: str,
    ReplicatorArn: str,
    SourceKafkaClusterArn: str,
    TargetKafkaClusterArn: str,
    ConsumerGroupReplication: NotRequired[ConsumerGroupReplicationUpdateTypeDef],  # (1)
    TopicReplication: NotRequired[TopicReplicationUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ConsumerGroupReplicationUpdateTypeDef](./type_defs.md#consumergroupreplicationupdatetypedef) 
2. See [:material-code-braces: TopicReplicationUpdateTypeDef](./type_defs.md#topicreplicationupdatetypedef) 
## VpcConnectionInfoServerlessTypeDef

```python
# VpcConnectionInfoServerlessTypeDef definition

class VpcConnectionInfoServerlessTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    Owner: NotRequired[str],
    UserIdentity: NotRequired[UserIdentityTypeDef],  # (1)
    VpcConnectionArn: NotRequired[str],
```

1. See [:material-code-braces: UserIdentityTypeDef](./type_defs.md#useridentitytypedef) 
## VpcConnectionInfoTypeDef

```python
# VpcConnectionInfoTypeDef definition

class VpcConnectionInfoTypeDef(TypedDict):
    VpcConnectionArn: NotRequired[str],
    Owner: NotRequired[str],
    UserIdentity: NotRequired[UserIdentityTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-braces: UserIdentityTypeDef](./type_defs.md#useridentitytypedef) 
## VpcConnectivitySaslTypeDef

```python
# VpcConnectivitySaslTypeDef definition

class VpcConnectivitySaslTypeDef(TypedDict):
    Scram: NotRequired[VpcConnectivityScramTypeDef],  # (1)
    Iam: NotRequired[VpcConnectivityIamTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConnectivityScramTypeDef](./type_defs.md#vpcconnectivityscramtypedef) 
2. See [:material-code-braces: VpcConnectivityIamTypeDef](./type_defs.md#vpcconnectivityiamtypedef) 
## ReplicatorSummaryTypeDef

```python
# ReplicatorSummaryTypeDef definition

class ReplicatorSummaryTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    CurrentVersion: NotRequired[str],
    IsReplicatorReference: NotRequired[bool],
    KafkaClustersSummary: NotRequired[List[KafkaClusterSummaryTypeDef]],  # (1)
    ReplicationInfoSummaryList: NotRequired[List[ReplicationInfoSummaryTypeDef]],  # (2)
    ReplicatorArn: NotRequired[str],
    ReplicatorName: NotRequired[str],
    ReplicatorResourceArn: NotRequired[str],
    ReplicatorState: NotRequired[ReplicatorStateType],  # (3)
```

1. See [:material-code-braces: KafkaClusterSummaryTypeDef](./type_defs.md#kafkaclustersummarytypedef) 
2. See [:material-code-braces: ReplicationInfoSummaryTypeDef](./type_defs.md#replicationinfosummarytypedef) 
3. See [:material-code-brackets: ReplicatorStateType](./literals.md#replicatorstatetype) 
## UpdateBrokerStorageRequestRequestTypeDef

```python
# UpdateBrokerStorageRequestRequestTypeDef definition

class UpdateBrokerStorageRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef],  # (1)
```

1. See [:material-code-braces: BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef) 
## StorageInfoTypeDef

```python
# StorageInfoTypeDef definition

class StorageInfoTypeDef(TypedDict):
    EbsStorageInfo: NotRequired[EBSStorageInfoTypeDef],  # (1)
```

1. See [:material-code-braces: EBSStorageInfoTypeDef](./type_defs.md#ebsstorageinfotypedef) 
## LoggingInfoTypeDef

```python
# LoggingInfoTypeDef definition

class LoggingInfoTypeDef(TypedDict):
    BrokerLogs: BrokerLogsTypeDef,  # (1)
```

1. See [:material-code-braces: BrokerLogsTypeDef](./type_defs.md#brokerlogstypedef) 
## NodeInfoTypeDef

```python
# NodeInfoTypeDef definition

class NodeInfoTypeDef(TypedDict):
    AddedToClusterTime: NotRequired[str],
    BrokerNodeInfo: NotRequired[BrokerNodeInfoTypeDef],  # (1)
    ControllerNodeInfo: NotRequired[ControllerNodeInfoTypeDef],  # (2)
    InstanceType: NotRequired[str],
    NodeARN: NotRequired[str],
    NodeType: NotRequired[NodeTypeType],  # (3)
    ZookeeperNodeInfo: NotRequired[ZookeeperNodeInfoTypeDef],  # (4)
```

1. See [:material-code-braces: BrokerNodeInfoTypeDef](./type_defs.md#brokernodeinfotypedef) 
2. See [:material-code-braces: ControllerNodeInfoTypeDef](./type_defs.md#controllernodeinfotypedef) 
3. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
4. See [:material-code-braces: ZookeeperNodeInfoTypeDef](./type_defs.md#zookeepernodeinfotypedef) 
## ListConfigurationsResponseTypeDef

```python
# ListConfigurationsResponseTypeDef definition

class ListConfigurationsResponseTypeDef(TypedDict):
    Configurations: List[ConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerlessClientAuthenticationTypeDef

```python
# ServerlessClientAuthenticationTypeDef definition

class ServerlessClientAuthenticationTypeDef(TypedDict):
    Sasl: NotRequired[ServerlessSaslTypeDef],  # (1)
```

1. See [:material-code-braces: ServerlessSaslTypeDef](./type_defs.md#serverlesssasltypedef) 
## KafkaClusterTypeDef

```python
# KafkaClusterTypeDef definition

class KafkaClusterTypeDef(TypedDict):
    AmazonMskCluster: AmazonMskClusterTypeDef,  # (1)
    VpcConfig: KafkaClusterClientVpcConfigUnionTypeDef,  # (2)
```

1. See [:material-code-braces: AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef) 
2. See [:material-code-braces: KafkaClusterClientVpcConfigTypeDef](./type_defs.md#kafkaclusterclientvpcconfigtypedef) [:material-code-braces: KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef) 
## OpenMonitoringInfoTypeDef

```python
# OpenMonitoringInfoTypeDef definition

class OpenMonitoringInfoTypeDef(TypedDict):
    Prometheus: PrometheusInfoTypeDef,  # (1)
```

1. See [:material-code-braces: PrometheusInfoTypeDef](./type_defs.md#prometheusinfotypedef) 
## OpenMonitoringTypeDef

```python
# OpenMonitoringTypeDef definition

class OpenMonitoringTypeDef(TypedDict):
    Prometheus: PrometheusTypeDef,  # (1)
```

1. See [:material-code-braces: PrometheusTypeDef](./type_defs.md#prometheustypedef) 
## ReplicationInfoDescriptionTypeDef

```python
# ReplicationInfoDescriptionTypeDef definition

class ReplicationInfoDescriptionTypeDef(TypedDict):
    ConsumerGroupReplication: NotRequired[ConsumerGroupReplicationOutputTypeDef],  # (1)
    SourceKafkaClusterAlias: NotRequired[str],
    TargetCompressionType: NotRequired[TargetCompressionTypeType],  # (2)
    TargetKafkaClusterAlias: NotRequired[str],
    TopicReplication: NotRequired[TopicReplicationOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ConsumerGroupReplicationOutputTypeDef](./type_defs.md#consumergroupreplicationoutputtypedef) 
2. See [:material-code-brackets: TargetCompressionTypeType](./literals.md#targetcompressiontypetype) 
3. See [:material-code-braces: TopicReplicationOutputTypeDef](./type_defs.md#topicreplicationoutputtypedef) 
## ClientAuthenticationOutputTypeDef

```python
# ClientAuthenticationOutputTypeDef definition

class ClientAuthenticationOutputTypeDef(TypedDict):
    Sasl: NotRequired[SaslTypeDef],  # (1)
    Tls: NotRequired[TlsOutputTypeDef],  # (2)
    Unauthenticated: NotRequired[UnauthenticatedTypeDef],  # (3)
```

1. See [:material-code-braces: SaslTypeDef](./type_defs.md#sasltypedef) 
2. See [:material-code-braces: TlsOutputTypeDef](./type_defs.md#tlsoutputtypedef) 
3. See [:material-code-braces: UnauthenticatedTypeDef](./type_defs.md#unauthenticatedtypedef) 
## ClientAuthenticationTypeDef

```python
# ClientAuthenticationTypeDef definition

class ClientAuthenticationTypeDef(TypedDict):
    Sasl: NotRequired[SaslTypeDef],  # (1)
    Tls: NotRequired[TlsUnionTypeDef],  # (2)
    Unauthenticated: NotRequired[UnauthenticatedTypeDef],  # (3)
```

1. See [:material-code-braces: SaslTypeDef](./type_defs.md#sasltypedef) 
2. See [:material-code-braces: TlsTypeDef](./type_defs.md#tlstypedef) [:material-code-braces: TlsOutputTypeDef](./type_defs.md#tlsoutputtypedef) 
3. See [:material-code-braces: UnauthenticatedTypeDef](./type_defs.md#unauthenticatedtypedef) 
## ClusterOperationV2ServerlessTypeDef

```python
# ClusterOperationV2ServerlessTypeDef definition

class ClusterOperationV2ServerlessTypeDef(TypedDict):
    VpcConnectionInfo: NotRequired[VpcConnectionInfoServerlessTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConnectionInfoServerlessTypeDef](./type_defs.md#vpcconnectioninfoserverlesstypedef) 
## VpcConnectivityClientAuthenticationTypeDef

```python
# VpcConnectivityClientAuthenticationTypeDef definition

class VpcConnectivityClientAuthenticationTypeDef(TypedDict):
    Sasl: NotRequired[VpcConnectivitySaslTypeDef],  # (1)
    Tls: NotRequired[VpcConnectivityTlsTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConnectivitySaslTypeDef](./type_defs.md#vpcconnectivitysasltypedef) 
2. See [:material-code-braces: VpcConnectivityTlsTypeDef](./type_defs.md#vpcconnectivitytlstypedef) 
## ListReplicatorsResponseTypeDef

```python
# ListReplicatorsResponseTypeDef definition

class ListReplicatorsResponseTypeDef(TypedDict):
    Replicators: List[ReplicatorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReplicatorSummaryTypeDef](./type_defs.md#replicatorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodesResponseTypeDef

```python
# ListNodesResponseTypeDef definition

class ListNodesResponseTypeDef(TypedDict):
    NodeInfoList: List[NodeInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeInfoTypeDef](./type_defs.md#nodeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerlessRequestTypeDef

```python
# ServerlessRequestTypeDef definition

class ServerlessRequestTypeDef(TypedDict):
    VpcConfigs: Sequence[VpcConfigUnionTypeDef],  # (1)
    ClientAuthentication: NotRequired[ServerlessClientAuthenticationTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
2. See [:material-code-braces: ServerlessClientAuthenticationTypeDef](./type_defs.md#serverlessclientauthenticationtypedef) 
## ServerlessTypeDef

```python
# ServerlessTypeDef definition

class ServerlessTypeDef(TypedDict):
    VpcConfigs: List[VpcConfigOutputTypeDef],  # (1)
    ClientAuthentication: NotRequired[ServerlessClientAuthenticationTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
2. See [:material-code-braces: ServerlessClientAuthenticationTypeDef](./type_defs.md#serverlessclientauthenticationtypedef) 
## UpdateMonitoringRequestRequestTypeDef

```python
# UpdateMonitoringRequestRequestTypeDef definition

class UpdateMonitoringRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (1)
    OpenMonitoring: NotRequired[OpenMonitoringInfoTypeDef],  # (2)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (3)
```

1. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
2. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
3. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
## DescribeReplicatorResponseTypeDef

```python
# DescribeReplicatorResponseTypeDef definition

class DescribeReplicatorResponseTypeDef(TypedDict):
    CreationTime: datetime,
    CurrentVersion: str,
    IsReplicatorReference: bool,
    KafkaClusters: List[KafkaClusterDescriptionTypeDef],  # (1)
    ReplicationInfoList: List[ReplicationInfoDescriptionTypeDef],  # (2)
    ReplicatorArn: str,
    ReplicatorDescription: str,
    ReplicatorName: str,
    ReplicatorResourceArn: str,
    ReplicatorState: ReplicatorStateType,  # (3)
    ServiceExecutionRoleArn: str,
    StateInfo: ReplicationStateInfoTypeDef,  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: KafkaClusterDescriptionTypeDef](./type_defs.md#kafkaclusterdescriptiontypedef) 
2. See [:material-code-braces: ReplicationInfoDescriptionTypeDef](./type_defs.md#replicationinfodescriptiontypedef) 
3. See [:material-code-brackets: ReplicatorStateType](./literals.md#replicatorstatetype) 
4. See [:material-code-braces: ReplicationStateInfoTypeDef](./type_defs.md#replicationstateinfotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationInfoTypeDef

```python
# ReplicationInfoTypeDef definition

class ReplicationInfoTypeDef(TypedDict):
    ConsumerGroupReplication: ConsumerGroupReplicationUnionTypeDef,  # (1)
    SourceKafkaClusterArn: str,
    TargetCompressionType: TargetCompressionTypeType,  # (2)
    TargetKafkaClusterArn: str,
    TopicReplication: TopicReplicationUnionTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumerGroupReplicationTypeDef](./type_defs.md#consumergroupreplicationtypedef) [:material-code-braces: ConsumerGroupReplicationOutputTypeDef](./type_defs.md#consumergroupreplicationoutputtypedef) 
2. See [:material-code-brackets: TargetCompressionTypeType](./literals.md#targetcompressiontypetype) 
3. See [:material-code-braces: TopicReplicationTypeDef](./type_defs.md#topicreplicationtypedef) [:material-code-braces: TopicReplicationOutputTypeDef](./type_defs.md#topicreplicationoutputtypedef) 
## UpdateSecurityRequestRequestTypeDef

```python
# UpdateSecurityRequestRequestTypeDef definition

class UpdateSecurityRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    ClientAuthentication: NotRequired[ClientAuthenticationTypeDef],  # (1)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (2)
```

1. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) 
2. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
## VpcConnectivityTypeDef

```python
# VpcConnectivityTypeDef definition

class VpcConnectivityTypeDef(TypedDict):
    ClientAuthentication: NotRequired[VpcConnectivityClientAuthenticationTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConnectivityClientAuthenticationTypeDef](./type_defs.md#vpcconnectivityclientauthenticationtypedef) 
## CreateReplicatorRequestRequestTypeDef

```python
# CreateReplicatorRequestRequestTypeDef definition

class CreateReplicatorRequestRequestTypeDef(TypedDict):
    KafkaClusters: Sequence[KafkaClusterTypeDef],  # (1)
    ReplicationInfoList: Sequence[ReplicationInfoTypeDef],  # (2)
    ReplicatorName: str,
    ServiceExecutionRoleArn: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef) 
2. See [:material-code-braces: ReplicationInfoTypeDef](./type_defs.md#replicationinfotypedef) 
## ConnectivityInfoTypeDef

```python
# ConnectivityInfoTypeDef definition

class ConnectivityInfoTypeDef(TypedDict):
    PublicAccess: NotRequired[PublicAccessTypeDef],  # (1)
    VpcConnectivity: NotRequired[VpcConnectivityTypeDef],  # (2)
```

1. See [:material-code-braces: PublicAccessTypeDef](./type_defs.md#publicaccesstypedef) 
2. See [:material-code-braces: VpcConnectivityTypeDef](./type_defs.md#vpcconnectivitytypedef) 
## BrokerNodeGroupInfoOutputTypeDef

```python
# BrokerNodeGroupInfoOutputTypeDef definition

class BrokerNodeGroupInfoOutputTypeDef(TypedDict):
    ClientSubnets: List[str],
    InstanceType: str,
    BrokerAZDistribution: NotRequired[BrokerAZDistributionType],  # (1)
    SecurityGroups: NotRequired[List[str]],
    StorageInfo: NotRequired[StorageInfoTypeDef],  # (2)
    ConnectivityInfo: NotRequired[ConnectivityInfoTypeDef],  # (3)
    ZoneIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: BrokerAZDistributionType](./literals.md#brokerazdistributiontype) 
2. See [:material-code-braces: StorageInfoTypeDef](./type_defs.md#storageinfotypedef) 
3. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
## BrokerNodeGroupInfoTypeDef

```python
# BrokerNodeGroupInfoTypeDef definition

class BrokerNodeGroupInfoTypeDef(TypedDict):
    ClientSubnets: Sequence[str],
    InstanceType: str,
    BrokerAZDistribution: NotRequired[BrokerAZDistributionType],  # (1)
    SecurityGroups: NotRequired[Sequence[str]],
    StorageInfo: NotRequired[StorageInfoTypeDef],  # (2)
    ConnectivityInfo: NotRequired[ConnectivityInfoTypeDef],  # (3)
    ZoneIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: BrokerAZDistributionType](./literals.md#brokerazdistributiontype) 
2. See [:material-code-braces: StorageInfoTypeDef](./type_defs.md#storageinfotypedef) 
3. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
## MutableClusterInfoTypeDef

```python
# MutableClusterInfoTypeDef definition

class MutableClusterInfoTypeDef(TypedDict):
    BrokerEBSVolumeInfo: NotRequired[List[BrokerEBSVolumeInfoTypeDef]],  # (1)
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (2)
    NumberOfBrokerNodes: NotRequired[int],
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (3)
    OpenMonitoring: NotRequired[OpenMonitoringTypeDef],  # (4)
    KafkaVersion: NotRequired[str],
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (5)
    InstanceType: NotRequired[str],
    ClientAuthentication: NotRequired[ClientAuthenticationOutputTypeDef],  # (6)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (7)
    ConnectivityInfo: NotRequired[ConnectivityInfoTypeDef],  # (8)
    StorageMode: NotRequired[StorageModeType],  # (9)
    BrokerCountUpdateInfo: NotRequired[BrokerCountUpdateInfoTypeDef],  # (10)
```

1. See [:material-code-braces: BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef) 
2. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
3. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
4. See [:material-code-braces: OpenMonitoringTypeDef](./type_defs.md#openmonitoringtypedef) 
5. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
6. See [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 
7. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
8. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
9. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
10. See [:material-code-braces: BrokerCountUpdateInfoTypeDef](./type_defs.md#brokercountupdateinfotypedef) 
## UpdateConnectivityRequestRequestTypeDef

```python
# UpdateConnectivityRequestRequestTypeDef definition

class UpdateConnectivityRequestRequestTypeDef(TypedDict):
    ClusterArn: str,
    ConnectivityInfo: ConnectivityInfoTypeDef,  # (1)
    CurrentVersion: str,
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
## ClusterInfoTypeDef

```python
# ClusterInfoTypeDef definition

class ClusterInfoTypeDef(TypedDict):
    ActiveOperationArn: NotRequired[str],
    BrokerNodeGroupInfo: NotRequired[BrokerNodeGroupInfoOutputTypeDef],  # (1)
    ClientAuthentication: NotRequired[ClientAuthenticationOutputTypeDef],  # (2)
    ClusterArn: NotRequired[str],
    ClusterName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CurrentBrokerSoftwareInfo: NotRequired[BrokerSoftwareInfoTypeDef],  # (3)
    CurrentVersion: NotRequired[str],
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (4)
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (5)
    OpenMonitoring: NotRequired[OpenMonitoringTypeDef],  # (6)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (7)
    NumberOfBrokerNodes: NotRequired[int],
    State: NotRequired[ClusterStateType],  # (8)
    StateInfo: NotRequired[StateInfoTypeDef],  # (9)
    Tags: NotRequired[Dict[str, str]],
    ZookeeperConnectString: NotRequired[str],
    ZookeeperConnectStringTls: NotRequired[str],
    StorageMode: NotRequired[StorageModeType],  # (10)
    CustomerActionStatus: NotRequired[CustomerActionStatusType],  # (11)
```

1. See [:material-code-braces: BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef) 
2. See [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 
3. See [:material-code-braces: BrokerSoftwareInfoTypeDef](./type_defs.md#brokersoftwareinfotypedef) 
4. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
5. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
6. See [:material-code-braces: OpenMonitoringTypeDef](./type_defs.md#openmonitoringtypedef) 
7. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
8. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
9. See [:material-code-braces: StateInfoTypeDef](./type_defs.md#stateinfotypedef) 
10. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
11. See [:material-code-brackets: CustomerActionStatusType](./literals.md#customeractionstatustype) 
## ProvisionedTypeDef

```python
# ProvisionedTypeDef definition

class ProvisionedTypeDef(TypedDict):
    BrokerNodeGroupInfo: BrokerNodeGroupInfoOutputTypeDef,  # (1)
    NumberOfBrokerNodes: int,
    CurrentBrokerSoftwareInfo: NotRequired[BrokerSoftwareInfoTypeDef],  # (2)
    ClientAuthentication: NotRequired[ClientAuthenticationOutputTypeDef],  # (3)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (4)
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (5)
    OpenMonitoring: NotRequired[OpenMonitoringInfoTypeDef],  # (6)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (7)
    ZookeeperConnectString: NotRequired[str],
    ZookeeperConnectStringTls: NotRequired[str],
    StorageMode: NotRequired[StorageModeType],  # (8)
    CustomerActionStatus: NotRequired[CustomerActionStatusType],  # (9)
```

1. See [:material-code-braces: BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef) 
2. See [:material-code-braces: BrokerSoftwareInfoTypeDef](./type_defs.md#brokersoftwareinfotypedef) 
3. See [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 
4. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
5. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
6. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
7. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
8. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
9. See [:material-code-brackets: CustomerActionStatusType](./literals.md#customeractionstatustype) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,  # (1)
    ClusterName: str,
    KafkaVersion: str,
    NumberOfBrokerNodes: int,
    ClientAuthentication: NotRequired[ClientAuthenticationTypeDef],  # (2)
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (3)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (4)
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (5)
    OpenMonitoring: NotRequired[OpenMonitoringInfoTypeDef],  # (6)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (7)
    Tags: NotRequired[Mapping[str, str]],
    StorageMode: NotRequired[StorageModeType],  # (8)
```

1. See [:material-code-braces: BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef) 
2. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) 
3. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
4. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
5. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
6. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
7. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
8. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
## ClusterOperationInfoTypeDef

```python
# ClusterOperationInfoTypeDef definition

class ClusterOperationInfoTypeDef(TypedDict):
    ClientRequestId: NotRequired[str],
    ClusterArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ErrorInfo: NotRequired[ErrorInfoTypeDef],  # (1)
    OperationArn: NotRequired[str],
    OperationState: NotRequired[str],
    OperationSteps: NotRequired[List[ClusterOperationStepTypeDef]],  # (2)
    OperationType: NotRequired[str],
    SourceClusterInfo: NotRequired[MutableClusterInfoTypeDef],  # (3)
    TargetClusterInfo: NotRequired[MutableClusterInfoTypeDef],  # (3)
    VpcConnectionInfo: NotRequired[VpcConnectionInfoTypeDef],  # (5)
```

1. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
2. See [:material-code-braces: ClusterOperationStepTypeDef](./type_defs.md#clusteroperationsteptypedef) 
3. See [:material-code-braces: MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef) 
4. See [:material-code-braces: MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef) 
5. See [:material-code-braces: VpcConnectionInfoTypeDef](./type_defs.md#vpcconnectioninfotypedef) 
## ClusterOperationV2ProvisionedTypeDef

```python
# ClusterOperationV2ProvisionedTypeDef definition

class ClusterOperationV2ProvisionedTypeDef(TypedDict):
    OperationSteps: NotRequired[List[ClusterOperationStepTypeDef]],  # (1)
    SourceClusterInfo: NotRequired[MutableClusterInfoTypeDef],  # (2)
    TargetClusterInfo: NotRequired[MutableClusterInfoTypeDef],  # (2)
    VpcConnectionInfo: NotRequired[VpcConnectionInfoTypeDef],  # (4)
```

1. See [:material-code-braces: ClusterOperationStepTypeDef](./type_defs.md#clusteroperationsteptypedef) 
2. See [:material-code-braces: MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef) 
3. See [:material-code-braces: MutableClusterInfoTypeDef](./type_defs.md#mutableclusterinfotypedef) 
4. See [:material-code-braces: VpcConnectionInfoTypeDef](./type_defs.md#vpcconnectioninfotypedef) 
## DescribeClusterResponseTypeDef

```python
# DescribeClusterResponseTypeDef definition

class DescribeClusterResponseTypeDef(TypedDict):
    ClusterInfo: ClusterInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterInfoTypeDef](./type_defs.md#clusterinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    ClusterInfoList: List[ClusterInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterInfoTypeDef](./type_defs.md#clusterinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    ActiveOperationArn: NotRequired[str],
    ClusterType: NotRequired[ClusterTypeType],  # (1)
    ClusterArn: NotRequired[str],
    ClusterName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CurrentVersion: NotRequired[str],
    State: NotRequired[ClusterStateType],  # (2)
    StateInfo: NotRequired[StateInfoTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
    Provisioned: NotRequired[ProvisionedTypeDef],  # (4)
    Serverless: NotRequired[ServerlessTypeDef],  # (5)
```

1. See [:material-code-brackets: ClusterTypeType](./literals.md#clustertypetype) 
2. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
3. See [:material-code-braces: StateInfoTypeDef](./type_defs.md#stateinfotypedef) 
4. See [:material-code-braces: ProvisionedTypeDef](./type_defs.md#provisionedtypedef) 
5. See [:material-code-braces: ServerlessTypeDef](./type_defs.md#serverlesstypedef) 
## ProvisionedRequestTypeDef

```python
# ProvisionedRequestTypeDef definition

class ProvisionedRequestTypeDef(TypedDict):
    BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,  # (1)
    KafkaVersion: str,
    NumberOfBrokerNodes: int,
    ClientAuthentication: NotRequired[ClientAuthenticationUnionTypeDef],  # (2)
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (3)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (4)
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (5)
    OpenMonitoring: NotRequired[OpenMonitoringInfoTypeDef],  # (6)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (7)
    StorageMode: NotRequired[StorageModeType],  # (8)
```

1. See [:material-code-braces: BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef) [:material-code-braces: BrokerNodeGroupInfoOutputTypeDef](./type_defs.md#brokernodegroupinfooutputtypedef) 
2. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 
3. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
4. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
5. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
6. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
7. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
8. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
## DescribeClusterOperationResponseTypeDef

```python
# DescribeClusterOperationResponseTypeDef definition

class DescribeClusterOperationResponseTypeDef(TypedDict):
    ClusterOperationInfo: ClusterOperationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterOperationInfoTypeDef](./type_defs.md#clusteroperationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClusterOperationsResponseTypeDef

```python
# ListClusterOperationsResponseTypeDef definition

class ListClusterOperationsResponseTypeDef(TypedDict):
    ClusterOperationInfoList: List[ClusterOperationInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterOperationInfoTypeDef](./type_defs.md#clusteroperationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterOperationV2TypeDef

```python
# ClusterOperationV2TypeDef definition

class ClusterOperationV2TypeDef(TypedDict):
    ClusterArn: NotRequired[str],
    ClusterType: NotRequired[ClusterTypeType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ErrorInfo: NotRequired[ErrorInfoTypeDef],  # (2)
    OperationArn: NotRequired[str],
    OperationState: NotRequired[str],
    OperationType: NotRequired[str],
    Provisioned: NotRequired[ClusterOperationV2ProvisionedTypeDef],  # (3)
    Serverless: NotRequired[ClusterOperationV2ServerlessTypeDef],  # (4)
```

1. See [:material-code-brackets: ClusterTypeType](./literals.md#clustertypetype) 
2. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
3. See [:material-code-braces: ClusterOperationV2ProvisionedTypeDef](./type_defs.md#clusteroperationv2provisionedtypedef) 
4. See [:material-code-braces: ClusterOperationV2ServerlessTypeDef](./type_defs.md#clusteroperationv2serverlesstypedef) 
## DescribeClusterV2ResponseTypeDef

```python
# DescribeClusterV2ResponseTypeDef definition

class DescribeClusterV2ResponseTypeDef(TypedDict):
    ClusterInfo: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersV2ResponseTypeDef

```python
# ListClustersV2ResponseTypeDef definition

class ListClustersV2ResponseTypeDef(TypedDict):
    ClusterInfoList: List[ClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterV2RequestRequestTypeDef

```python
# CreateClusterV2RequestRequestTypeDef definition

class CreateClusterV2RequestRequestTypeDef(TypedDict):
    ClusterName: str,
    Tags: NotRequired[Mapping[str, str]],
    Provisioned: NotRequired[ProvisionedRequestTypeDef],  # (1)
    Serverless: NotRequired[ServerlessRequestTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef) 
2. See [:material-code-braces: ServerlessRequestTypeDef](./type_defs.md#serverlessrequesttypedef) 
## DescribeClusterOperationV2ResponseTypeDef

```python
# DescribeClusterOperationV2ResponseTypeDef definition

class DescribeClusterOperationV2ResponseTypeDef(TypedDict):
    ClusterOperationInfo: ClusterOperationV2TypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterOperationV2TypeDef](./type_defs.md#clusteroperationv2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
