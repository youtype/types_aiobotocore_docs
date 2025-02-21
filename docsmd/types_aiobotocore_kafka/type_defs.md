# Type definitions

> [Index](../README.md) > [Kafka](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# ConsumerGroupReplicationUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import ConsumerGroupReplicationUnionTypeDef


def get_value() -> ConsumerGroupReplicationUnionTypeDef:
    return ...


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
# KafkaClusterClientVpcConfigUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterClientVpcConfigUnionTypeDef


def get_value() -> KafkaClusterClientVpcConfigUnionTypeDef:
    return ...


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
# TlsUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import TlsUnionTypeDef


def get_value() -> TlsUnionTypeDef:
    return ...


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
# VpcConfigUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import VpcConfigUnionTypeDef


def get_value() -> VpcConfigUnionTypeDef:
    return ...


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
# TopicReplicationUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import TopicReplicationUnionTypeDef


def get_value() -> TopicReplicationUnionTypeDef:
    return ...


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
# ClientAuthenticationUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import ClientAuthenticationUnionTypeDef


def get_value() -> ClientAuthenticationUnionTypeDef:
    return ...


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
# BrokerNodeGroupInfoUnionTypeDef Union usage example

from types_aiobotocore_kafka.type_defs import BrokerNodeGroupInfoUnionTypeDef


def get_value() -> BrokerNodeGroupInfoUnionTypeDef:
    return ...


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
# AmazonMskClusterTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import AmazonMskClusterTypeDef


def get_value() -> AmazonMskClusterTypeDef:
    return {
        "MskClusterArn": ...,
    }


# AmazonMskClusterTypeDef definition

class AmazonMskClusterTypeDef(TypedDict):
    MskClusterArn: str,
```

## BatchAssociateScramSecretRequestTypeDef

```python
# BatchAssociateScramSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretRequestTypeDef


def get_value() -> BatchAssociateScramSecretRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# BatchAssociateScramSecretRequestTypeDef definition

class BatchAssociateScramSecretRequestTypeDef(TypedDict):
    ClusterArn: str,
    SecretArnList: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# UnprocessedScramSecretTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UnprocessedScramSecretTypeDef


def get_value() -> UnprocessedScramSecretTypeDef:
    return {
        "ErrorCode": ...,
    }


# UnprocessedScramSecretTypeDef definition

class UnprocessedScramSecretTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    SecretArn: NotRequired[str],
```

## BatchDisassociateScramSecretRequestTypeDef

```python
# BatchDisassociateScramSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BatchDisassociateScramSecretRequestTypeDef


def get_value() -> BatchDisassociateScramSecretRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# BatchDisassociateScramSecretRequestTypeDef definition

class BatchDisassociateScramSecretRequestTypeDef(TypedDict):
    ClusterArn: str,
    SecretArnList: Sequence[str],
```

## BrokerCountUpdateInfoTypeDef

```python
# BrokerCountUpdateInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerCountUpdateInfoTypeDef


def get_value() -> BrokerCountUpdateInfoTypeDef:
    return {
        "CreatedBrokerIds": ...,
    }


# BrokerCountUpdateInfoTypeDef definition

class BrokerCountUpdateInfoTypeDef(TypedDict):
    CreatedBrokerIds: NotRequired[List[float]],
    DeletedBrokerIds: NotRequired[List[float]],
```

## ProvisionedThroughputTypeDef

```python
# ProvisionedThroughputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ProvisionedThroughputTypeDef


def get_value() -> ProvisionedThroughputTypeDef:
    return {
        "Enabled": ...,
    }


# ProvisionedThroughputTypeDef definition

class ProvisionedThroughputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    VolumeThroughput: NotRequired[int],
```

## CloudWatchLogsTypeDef

```python
# CloudWatchLogsTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CloudWatchLogsTypeDef


def get_value() -> CloudWatchLogsTypeDef:
    return {
        "Enabled": ...,
    }


# CloudWatchLogsTypeDef definition

class CloudWatchLogsTypeDef(TypedDict):
    Enabled: bool,
    LogGroup: NotRequired[str],
```

## FirehoseTypeDef

```python
# FirehoseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import FirehoseTypeDef


def get_value() -> FirehoseTypeDef:
    return {
        "DeliveryStream": ...,
    }


# FirehoseTypeDef definition

class FirehoseTypeDef(TypedDict):
    Enabled: bool,
    DeliveryStream: NotRequired[str],
```

## S3TypeDef

```python
# S3TypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import S3TypeDef


def get_value() -> S3TypeDef:
    return {
        "Bucket": ...,
    }


# S3TypeDef definition

class S3TypeDef(TypedDict):
    Enabled: bool,
    Bucket: NotRequired[str],
    Prefix: NotRequired[str],
```

## BrokerSoftwareInfoTypeDef

```python
# BrokerSoftwareInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerSoftwareInfoTypeDef


def get_value() -> BrokerSoftwareInfoTypeDef:
    return {
        "ConfigurationArn": ...,
    }


# BrokerSoftwareInfoTypeDef definition

class BrokerSoftwareInfoTypeDef(TypedDict):
    ConfigurationArn: NotRequired[str],
    ConfigurationRevision: NotRequired[int],
    KafkaVersion: NotRequired[str],
```

## TlsOutputTypeDef

```python
# TlsOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TlsOutputTypeDef


def get_value() -> TlsOutputTypeDef:
    return {
        "CertificateAuthorityArnList": ...,
    }


# TlsOutputTypeDef definition

class TlsOutputTypeDef(TypedDict):
    CertificateAuthorityArnList: NotRequired[List[str]],
    Enabled: NotRequired[bool],
```

## UnauthenticatedTypeDef

```python
# UnauthenticatedTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UnauthenticatedTypeDef


def get_value() -> UnauthenticatedTypeDef:
    return {
        "Enabled": ...,
    }


# UnauthenticatedTypeDef definition

class UnauthenticatedTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## ClientVpcConnectionTypeDef

```python
# ClientVpcConnectionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClientVpcConnectionTypeDef


def get_value() -> ClientVpcConnectionTypeDef:
    return {
        "Authentication": ...,
    }


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
# StateInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import StateInfoTypeDef


def get_value() -> StateInfoTypeDef:
    return {
        "Code": ...,
    }


# StateInfoTypeDef definition

class StateInfoTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ErrorInfoTypeDef


def get_value() -> ErrorInfoTypeDef:
    return {
        "ErrorCode": ...,
    }


# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorString: NotRequired[str],
```

## ClusterOperationStepInfoTypeDef

```python
# ClusterOperationStepInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationStepInfoTypeDef


def get_value() -> ClusterOperationStepInfoTypeDef:
    return {
        "StepStatus": ...,
    }


# ClusterOperationStepInfoTypeDef definition

class ClusterOperationStepInfoTypeDef(TypedDict):
    StepStatus: NotRequired[str],
```

## ClusterOperationV2SummaryTypeDef

```python
# ClusterOperationV2SummaryTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationV2SummaryTypeDef


def get_value() -> ClusterOperationV2SummaryTypeDef:
    return {
        "ClusterArn": ...,
    }


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
# CompatibleKafkaVersionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CompatibleKafkaVersionTypeDef


def get_value() -> CompatibleKafkaVersionTypeDef:
    return {
        "SourceVersion": ...,
    }


# CompatibleKafkaVersionTypeDef definition

class CompatibleKafkaVersionTypeDef(TypedDict):
    SourceVersion: NotRequired[str],
    TargetVersions: NotRequired[List[str]],
```

## ConfigurationInfoTypeDef

```python
# ConfigurationInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConfigurationInfoTypeDef


def get_value() -> ConfigurationInfoTypeDef:
    return {
        "Arn": ...,
    }


# ConfigurationInfoTypeDef definition

class ConfigurationInfoTypeDef(TypedDict):
    Arn: str,
    Revision: int,
```

## ConfigurationRevisionTypeDef

```python
# ConfigurationRevisionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConfigurationRevisionTypeDef


def get_value() -> ConfigurationRevisionTypeDef:
    return {
        "CreationTime": ...,
    }


# ConfigurationRevisionTypeDef definition

class ConfigurationRevisionTypeDef(TypedDict):
    CreationTime: datetime,
    Revision: int,
    Description: NotRequired[str],
```

## PublicAccessTypeDef

```python
# PublicAccessTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PublicAccessTypeDef


def get_value() -> PublicAccessTypeDef:
    return {
        "Type": ...,
    }


# PublicAccessTypeDef definition

class PublicAccessTypeDef(TypedDict):
    Type: NotRequired[str],
```

## ConsumerGroupReplicationOutputTypeDef

```python
# ConsumerGroupReplicationOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConsumerGroupReplicationOutputTypeDef


def get_value() -> ConsumerGroupReplicationOutputTypeDef:
    return {
        "ConsumerGroupsToExclude": ...,
    }


# ConsumerGroupReplicationOutputTypeDef definition

class ConsumerGroupReplicationOutputTypeDef(TypedDict):
    ConsumerGroupsToReplicate: List[str],
    ConsumerGroupsToExclude: NotRequired[List[str]],
    DetectAndCopyNewConsumerGroups: NotRequired[bool],
    SynchroniseConsumerGroupOffsets: NotRequired[bool],
```

## ConsumerGroupReplicationTypeDef

```python
# ConsumerGroupReplicationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConsumerGroupReplicationTypeDef


def get_value() -> ConsumerGroupReplicationTypeDef:
    return {
        "ConsumerGroupsToExclude": ...,
    }


# ConsumerGroupReplicationTypeDef definition

class ConsumerGroupReplicationTypeDef(TypedDict):
    ConsumerGroupsToReplicate: Sequence[str],
    ConsumerGroupsToExclude: NotRequired[Sequence[str]],
    DetectAndCopyNewConsumerGroups: NotRequired[bool],
    SynchroniseConsumerGroupOffsets: NotRequired[bool],
```

## ConsumerGroupReplicationUpdateTypeDef

```python
# ConsumerGroupReplicationUpdateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConsumerGroupReplicationUpdateTypeDef


def get_value() -> ConsumerGroupReplicationUpdateTypeDef:
    return {
        "ConsumerGroupsToExclude": ...,
    }


# ConsumerGroupReplicationUpdateTypeDef definition

class ConsumerGroupReplicationUpdateTypeDef(TypedDict):
    ConsumerGroupsToExclude: Sequence[str],
    ConsumerGroupsToReplicate: Sequence[str],
    DetectAndCopyNewConsumerGroups: bool,
    SynchroniseConsumerGroupOffsets: bool,
```

## ControllerNodeInfoTypeDef

```python
# ControllerNodeInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ControllerNodeInfoTypeDef


def get_value() -> ControllerNodeInfoTypeDef:
    return {
        "Endpoints": ...,
    }


# ControllerNodeInfoTypeDef definition

class ControllerNodeInfoTypeDef(TypedDict):
    Endpoints: NotRequired[List[str]],
```

## CreateVpcConnectionRequestTypeDef

```python
# CreateVpcConnectionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateVpcConnectionRequestTypeDef


def get_value() -> CreateVpcConnectionRequestTypeDef:
    return {
        "TargetClusterArn": ...,
    }


# CreateVpcConnectionRequestTypeDef definition

class CreateVpcConnectionRequestTypeDef(TypedDict):
    TargetClusterArn: str,
    Authentication: str,
    VpcId: str,
    ClientSubnets: Sequence[str],
    SecurityGroups: Sequence[str],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteClusterPolicyRequestTypeDef

```python
# DeleteClusterPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteClusterPolicyRequestTypeDef


def get_value() -> DeleteClusterPolicyRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# DeleteClusterPolicyRequestTypeDef definition

class DeleteClusterPolicyRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DeleteClusterRequestTypeDef

```python
# DeleteClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteClusterRequestTypeDef


def get_value() -> DeleteClusterRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# DeleteClusterRequestTypeDef definition

class DeleteClusterRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: NotRequired[str],
```

## DeleteConfigurationRequestTypeDef

```python
# DeleteConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteConfigurationRequestTypeDef


def get_value() -> DeleteConfigurationRequestTypeDef:
    return {
        "Arn": ...,
    }


# DeleteConfigurationRequestTypeDef definition

class DeleteConfigurationRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteReplicatorRequestTypeDef

```python
# DeleteReplicatorRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteReplicatorRequestTypeDef


def get_value() -> DeleteReplicatorRequestTypeDef:
    return {
        "ReplicatorArn": ...,
    }


# DeleteReplicatorRequestTypeDef definition

class DeleteReplicatorRequestTypeDef(TypedDict):
    ReplicatorArn: str,
    CurrentVersion: NotRequired[str],
```

## DeleteVpcConnectionRequestTypeDef

```python
# DeleteVpcConnectionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteVpcConnectionRequestTypeDef


def get_value() -> DeleteVpcConnectionRequestTypeDef:
    return {
        "Arn": ...,
    }


# DeleteVpcConnectionRequestTypeDef definition

class DeleteVpcConnectionRequestTypeDef(TypedDict):
    Arn: str,
```

## DescribeClusterOperationRequestTypeDef

```python
# DescribeClusterOperationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterOperationRequestTypeDef


def get_value() -> DescribeClusterOperationRequestTypeDef:
    return {
        "ClusterOperationArn": ...,
    }


# DescribeClusterOperationRequestTypeDef definition

class DescribeClusterOperationRequestTypeDef(TypedDict):
    ClusterOperationArn: str,
```

## DescribeClusterOperationV2RequestTypeDef

```python
# DescribeClusterOperationV2RequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterOperationV2RequestTypeDef


def get_value() -> DescribeClusterOperationV2RequestTypeDef:
    return {
        "ClusterOperationArn": ...,
    }


# DescribeClusterOperationV2RequestTypeDef definition

class DescribeClusterOperationV2RequestTypeDef(TypedDict):
    ClusterOperationArn: str,
```

## DescribeClusterRequestTypeDef

```python
# DescribeClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterRequestTypeDef


def get_value() -> DescribeClusterRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# DescribeClusterRequestTypeDef definition

class DescribeClusterRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DescribeClusterV2RequestTypeDef

```python
# DescribeClusterV2RequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterV2RequestTypeDef


def get_value() -> DescribeClusterV2RequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# DescribeClusterV2RequestTypeDef definition

class DescribeClusterV2RequestTypeDef(TypedDict):
    ClusterArn: str,
```

## DescribeConfigurationRequestTypeDef

```python
# DescribeConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeConfigurationRequestTypeDef


def get_value() -> DescribeConfigurationRequestTypeDef:
    return {
        "Arn": ...,
    }


# DescribeConfigurationRequestTypeDef definition

class DescribeConfigurationRequestTypeDef(TypedDict):
    Arn: str,
```

## DescribeConfigurationRevisionRequestTypeDef

```python
# DescribeConfigurationRevisionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeConfigurationRevisionRequestTypeDef


def get_value() -> DescribeConfigurationRevisionRequestTypeDef:
    return {
        "Arn": ...,
    }


# DescribeConfigurationRevisionRequestTypeDef definition

class DescribeConfigurationRevisionRequestTypeDef(TypedDict):
    Arn: str,
    Revision: int,
```

## DescribeReplicatorRequestTypeDef

```python
# DescribeReplicatorRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeReplicatorRequestTypeDef


def get_value() -> DescribeReplicatorRequestTypeDef:
    return {
        "ReplicatorArn": ...,
    }


# DescribeReplicatorRequestTypeDef definition

class DescribeReplicatorRequestTypeDef(TypedDict):
    ReplicatorArn: str,
```

## ReplicationStateInfoTypeDef

```python
# ReplicationStateInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationStateInfoTypeDef


def get_value() -> ReplicationStateInfoTypeDef:
    return {
        "Code": ...,
    }


# ReplicationStateInfoTypeDef definition

class ReplicationStateInfoTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## DescribeVpcConnectionRequestTypeDef

```python
# DescribeVpcConnectionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeVpcConnectionRequestTypeDef


def get_value() -> DescribeVpcConnectionRequestTypeDef:
    return {
        "Arn": ...,
    }


# DescribeVpcConnectionRequestTypeDef definition

class DescribeVpcConnectionRequestTypeDef(TypedDict):
    Arn: str,
```

## EncryptionAtRestTypeDef

```python
# EncryptionAtRestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import EncryptionAtRestTypeDef


def get_value() -> EncryptionAtRestTypeDef:
    return {
        "DataVolumeKMSKeyId": ...,
    }


# EncryptionAtRestTypeDef definition

class EncryptionAtRestTypeDef(TypedDict):
    DataVolumeKMSKeyId: str,
```

## EncryptionInTransitTypeDef

```python
# EncryptionInTransitTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import EncryptionInTransitTypeDef


def get_value() -> EncryptionInTransitTypeDef:
    return {
        "ClientBroker": ...,
    }


# EncryptionInTransitTypeDef definition

class EncryptionInTransitTypeDef(TypedDict):
    ClientBroker: NotRequired[ClientBrokerType],  # (1)
    InCluster: NotRequired[bool],
```

1. See [:material-code-brackets: ClientBrokerType](./literals.md#clientbrokertype) 
## GetBootstrapBrokersRequestTypeDef

```python
# GetBootstrapBrokersRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetBootstrapBrokersRequestTypeDef


def get_value() -> GetBootstrapBrokersRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# GetBootstrapBrokersRequestTypeDef definition

class GetBootstrapBrokersRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## GetClusterPolicyRequestTypeDef

```python
# GetClusterPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetClusterPolicyRequestTypeDef


def get_value() -> GetClusterPolicyRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# GetClusterPolicyRequestTypeDef definition

class GetClusterPolicyRequestTypeDef(TypedDict):
    ClusterArn: str,
```

## GetCompatibleKafkaVersionsRequestTypeDef

```python
# GetCompatibleKafkaVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetCompatibleKafkaVersionsRequestTypeDef


def get_value() -> GetCompatibleKafkaVersionsRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# GetCompatibleKafkaVersionsRequestTypeDef definition

class GetCompatibleKafkaVersionsRequestTypeDef(TypedDict):
    ClusterArn: NotRequired[str],
```

## IamTypeDef

```python
# IamTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import IamTypeDef


def get_value() -> IamTypeDef:
    return {
        "Enabled": ...,
    }


# IamTypeDef definition

class IamTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## JmxExporterInfoTypeDef

```python
# JmxExporterInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import JmxExporterInfoTypeDef


def get_value() -> JmxExporterInfoTypeDef:
    return {
        "EnabledInBroker": ...,
    }


# JmxExporterInfoTypeDef definition

class JmxExporterInfoTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## JmxExporterTypeDef

```python
# JmxExporterTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import JmxExporterTypeDef


def get_value() -> JmxExporterTypeDef:
    return {
        "EnabledInBroker": ...,
    }


# JmxExporterTypeDef definition

class JmxExporterTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## KafkaClusterClientVpcConfigOutputTypeDef

```python
# KafkaClusterClientVpcConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterClientVpcConfigOutputTypeDef


def get_value() -> KafkaClusterClientVpcConfigOutputTypeDef:
    return {
        "SecurityGroupIds": ...,
    }


# KafkaClusterClientVpcConfigOutputTypeDef definition

class KafkaClusterClientVpcConfigOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: NotRequired[List[str]],
```

## KafkaClusterClientVpcConfigTypeDef

```python
# KafkaClusterClientVpcConfigTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterClientVpcConfigTypeDef


def get_value() -> KafkaClusterClientVpcConfigTypeDef:
    return {
        "SecurityGroupIds": ...,
    }


# KafkaClusterClientVpcConfigTypeDef definition

class KafkaClusterClientVpcConfigTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## KafkaVersionTypeDef

```python
# KafkaVersionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaVersionTypeDef


def get_value() -> KafkaVersionTypeDef:
    return {
        "Version": ...,
    }


# KafkaVersionTypeDef definition

class KafkaVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    Status: NotRequired[KafkaVersionStatusType],  # (1)
```

1. See [:material-code-brackets: KafkaVersionStatusType](./literals.md#kafkaversionstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListClientVpcConnectionsRequestTypeDef

```python
# ListClientVpcConnectionsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClientVpcConnectionsRequestTypeDef


def get_value() -> ListClientVpcConnectionsRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClientVpcConnectionsRequestTypeDef definition

class ListClientVpcConnectionsRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClusterOperationsRequestTypeDef

```python
# ListClusterOperationsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsRequestTypeDef


def get_value() -> ListClusterOperationsRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClusterOperationsRequestTypeDef definition

class ListClusterOperationsRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClusterOperationsV2RequestTypeDef

```python
# ListClusterOperationsV2RequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsV2RequestTypeDef


def get_value() -> ListClusterOperationsV2RequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClusterOperationsV2RequestTypeDef definition

class ListClusterOperationsV2RequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClustersRequestTypeDef

```python
# ListClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersRequestTypeDef


def get_value() -> ListClustersRequestTypeDef:
    return {
        "ClusterNameFilter": ...,
    }


# ListClustersRequestTypeDef definition

class ListClustersRequestTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListClustersV2RequestTypeDef

```python
# ListClustersV2RequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersV2RequestTypeDef


def get_value() -> ListClustersV2RequestTypeDef:
    return {
        "ClusterNameFilter": ...,
    }


# ListClustersV2RequestTypeDef definition

class ListClustersV2RequestTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    ClusterTypeFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationRevisionsRequestTypeDef

```python
# ListConfigurationRevisionsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationRevisionsRequestTypeDef


def get_value() -> ListConfigurationRevisionsRequestTypeDef:
    return {
        "Arn": ...,
    }


# ListConfigurationRevisionsRequestTypeDef definition

class ListConfigurationRevisionsRequestTypeDef(TypedDict):
    Arn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationsRequestTypeDef

```python
# ListConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationsRequestTypeDef


def get_value() -> ListConfigurationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListConfigurationsRequestTypeDef definition

class ListConfigurationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListKafkaVersionsRequestTypeDef

```python
# ListKafkaVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListKafkaVersionsRequestTypeDef


def get_value() -> ListKafkaVersionsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListKafkaVersionsRequestTypeDef definition

class ListKafkaVersionsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListNodesRequestTypeDef

```python
# ListNodesRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListNodesRequestTypeDef


def get_value() -> ListNodesRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListNodesRequestTypeDef definition

class ListNodesRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListReplicatorsRequestTypeDef

```python
# ListReplicatorsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListReplicatorsRequestTypeDef


def get_value() -> ListReplicatorsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListReplicatorsRequestTypeDef definition

class ListReplicatorsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ReplicatorNameFilter: NotRequired[str],
```

## ListScramSecretsRequestTypeDef

```python
# ListScramSecretsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListScramSecretsRequestTypeDef


def get_value() -> ListScramSecretsRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListScramSecretsRequestTypeDef definition

class ListScramSecretsRequestTypeDef(TypedDict):
    ClusterArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVpcConnectionsRequestTypeDef

```python
# ListVpcConnectionsRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListVpcConnectionsRequestTypeDef


def get_value() -> ListVpcConnectionsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListVpcConnectionsRequestTypeDef definition

class ListVpcConnectionsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## VpcConnectionTypeDef

```python
# VpcConnectionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectionTypeDef


def get_value() -> VpcConnectionTypeDef:
    return {
        "VpcConnectionArn": ...,
    }


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
# NodeExporterInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import NodeExporterInfoTypeDef


def get_value() -> NodeExporterInfoTypeDef:
    return {
        "EnabledInBroker": ...,
    }


# NodeExporterInfoTypeDef definition

class NodeExporterInfoTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## NodeExporterTypeDef

```python
# NodeExporterTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import NodeExporterTypeDef


def get_value() -> NodeExporterTypeDef:
    return {
        "EnabledInBroker": ...,
    }


# NodeExporterTypeDef definition

class NodeExporterTypeDef(TypedDict):
    EnabledInBroker: bool,
```

## ZookeeperNodeInfoTypeDef

```python
# ZookeeperNodeInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ZookeeperNodeInfoTypeDef


def get_value() -> ZookeeperNodeInfoTypeDef:
    return {
        "AttachedENIId": ...,
    }


# ZookeeperNodeInfoTypeDef definition

class ZookeeperNodeInfoTypeDef(TypedDict):
    AttachedENIId: NotRequired[str],
    ClientVpcIpAddress: NotRequired[str],
    Endpoints: NotRequired[List[str]],
    ZookeeperId: NotRequired[float],
    ZookeeperVersion: NotRequired[str],
```

## PutClusterPolicyRequestTypeDef

```python
# PutClusterPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PutClusterPolicyRequestTypeDef


def get_value() -> PutClusterPolicyRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# PutClusterPolicyRequestTypeDef definition

class PutClusterPolicyRequestTypeDef(TypedDict):
    ClusterArn: str,
    Policy: str,
    CurrentVersion: NotRequired[str],
```

## RebootBrokerRequestTypeDef

```python
# RebootBrokerRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import RebootBrokerRequestTypeDef


def get_value() -> RebootBrokerRequestTypeDef:
    return {
        "BrokerIds": ...,
    }


# RebootBrokerRequestTypeDef definition

class RebootBrokerRequestTypeDef(TypedDict):
    BrokerIds: Sequence[str],
    ClusterArn: str,
```

## RejectClientVpcConnectionRequestTypeDef

```python
# RejectClientVpcConnectionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import RejectClientVpcConnectionRequestTypeDef


def get_value() -> RejectClientVpcConnectionRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# RejectClientVpcConnectionRequestTypeDef definition

class RejectClientVpcConnectionRequestTypeDef(TypedDict):
    ClusterArn: str,
    VpcConnectionArn: str,
```

## ReplicationInfoSummaryTypeDef

```python
# ReplicationInfoSummaryTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationInfoSummaryTypeDef


def get_value() -> ReplicationInfoSummaryTypeDef:
    return {
        "SourceKafkaClusterAlias": ...,
    }


# ReplicationInfoSummaryTypeDef definition

class ReplicationInfoSummaryTypeDef(TypedDict):
    SourceKafkaClusterAlias: NotRequired[str],
    TargetKafkaClusterAlias: NotRequired[str],
```

## ReplicationStartingPositionTypeDef

```python
# ReplicationStartingPositionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationStartingPositionTypeDef


def get_value() -> ReplicationStartingPositionTypeDef:
    return {
        "Type": ...,
    }


# ReplicationStartingPositionTypeDef definition

class ReplicationStartingPositionTypeDef(TypedDict):
    Type: NotRequired[ReplicationStartingPositionTypeType],  # (1)
```

1. See [:material-code-brackets: ReplicationStartingPositionTypeType](./literals.md#replicationstartingpositiontypetype) 
## ReplicationTopicNameConfigurationTypeDef

```python
# ReplicationTopicNameConfigurationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationTopicNameConfigurationTypeDef


def get_value() -> ReplicationTopicNameConfigurationTypeDef:
    return {
        "Type": ...,
    }


# ReplicationTopicNameConfigurationTypeDef definition

class ReplicationTopicNameConfigurationTypeDef(TypedDict):
    Type: NotRequired[ReplicationTopicNameConfigurationTypeType],  # (1)
```

1. See [:material-code-brackets: ReplicationTopicNameConfigurationTypeType](./literals.md#replicationtopicnameconfigurationtypetype) 
## ScramTypeDef

```python
# ScramTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ScramTypeDef


def get_value() -> ScramTypeDef:
    return {
        "Enabled": ...,
    }


# ScramTypeDef definition

class ScramTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConfigOutputTypeDef


def get_value() -> VpcConfigOutputTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: NotRequired[List[str]],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## TlsTypeDef

```python
# TlsTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TlsTypeDef


def get_value() -> TlsTypeDef:
    return {
        "CertificateAuthorityArnList": ...,
    }


# TlsTypeDef definition

class TlsTypeDef(TypedDict):
    CertificateAuthorityArnList: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

## TopicReplicationUpdateTypeDef

```python
# TopicReplicationUpdateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TopicReplicationUpdateTypeDef


def get_value() -> TopicReplicationUpdateTypeDef:
    return {
        "CopyAccessControlListsForTopics": ...,
    }


# TopicReplicationUpdateTypeDef definition

class TopicReplicationUpdateTypeDef(TypedDict):
    CopyAccessControlListsForTopics: bool,
    CopyTopicConfigurations: bool,
    DetectAndCopyNewTopics: bool,
    TopicsToExclude: Sequence[str],
    TopicsToReplicate: Sequence[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateBrokerCountRequestTypeDef

```python
# UpdateBrokerCountRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerCountRequestTypeDef


def get_value() -> UpdateBrokerCountRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerCountRequestTypeDef definition

class UpdateBrokerCountRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetNumberOfBrokerNodes: int,
```

## UpdateBrokerTypeRequestTypeDef

```python
# UpdateBrokerTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerTypeRequestTypeDef


def get_value() -> UpdateBrokerTypeRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerTypeRequestTypeDef definition

class UpdateBrokerTypeRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetInstanceType: str,
```

## UserIdentityTypeDef

```python
# UserIdentityTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UserIdentityTypeDef


def get_value() -> UserIdentityTypeDef:
    return {
        "Type": ...,
    }


# UserIdentityTypeDef definition

class UserIdentityTypeDef(TypedDict):
    Type: NotRequired[UserIdentityTypeType],  # (1)
    PrincipalId: NotRequired[str],
```

1. See [:material-code-brackets: UserIdentityTypeType](./literals.md#useridentitytypetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConfigTypeDef


def get_value() -> VpcConfigTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## VpcConnectivityTlsTypeDef

```python
# VpcConnectivityTlsTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivityTlsTypeDef


def get_value() -> VpcConnectivityTlsTypeDef:
    return {
        "Enabled": ...,
    }


# VpcConnectivityTlsTypeDef definition

class VpcConnectivityTlsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConnectivityIamTypeDef

```python
# VpcConnectivityIamTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivityIamTypeDef


def get_value() -> VpcConnectivityIamTypeDef:
    return {
        "Enabled": ...,
    }


# VpcConnectivityIamTypeDef definition

class VpcConnectivityIamTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VpcConnectivityScramTypeDef

```python
# VpcConnectivityScramTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivityScramTypeDef


def get_value() -> VpcConnectivityScramTypeDef:
    return {
        "Enabled": ...,
    }


# VpcConnectivityScramTypeDef definition

class VpcConnectivityScramTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## KafkaClusterSummaryTypeDef

```python
# KafkaClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterSummaryTypeDef


def get_value() -> KafkaClusterSummaryTypeDef:
    return {
        "AmazonMskCluster": ...,
    }


# KafkaClusterSummaryTypeDef definition

class KafkaClusterSummaryTypeDef(TypedDict):
    AmazonMskCluster: NotRequired[AmazonMskClusterTypeDef],  # (1)
    KafkaClusterAlias: NotRequired[str],
```

1. See [:material-code-braces: AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateClusterResponseTypeDef


def get_value() -> CreateClusterResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


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
# CreateClusterV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateClusterV2ResponseTypeDef


def get_value() -> CreateClusterV2ResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


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
# CreateReplicatorResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateReplicatorResponseTypeDef


def get_value() -> CreateReplicatorResponseTypeDef:
    return {
        "ReplicatorArn": ...,
    }


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
# CreateVpcConnectionResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateVpcConnectionResponseTypeDef


def get_value() -> CreateVpcConnectionResponseTypeDef:
    return {
        "VpcConnectionArn": ...,
    }


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
# DeleteClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteClusterResponseTypeDef


def get_value() -> DeleteClusterResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


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
# DeleteConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteConfigurationResponseTypeDef


def get_value() -> DeleteConfigurationResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# DeleteReplicatorResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteReplicatorResponseTypeDef


def get_value() -> DeleteReplicatorResponseTypeDef:
    return {
        "ReplicatorArn": ...,
    }


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
# DeleteVpcConnectionResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DeleteVpcConnectionResponseTypeDef


def get_value() -> DeleteVpcConnectionResponseTypeDef:
    return {
        "VpcConnectionArn": ...,
    }


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
# DescribeConfigurationRevisionResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeConfigurationRevisionResponseTypeDef


def get_value() -> DescribeConfigurationRevisionResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# DescribeVpcConnectionResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeVpcConnectionResponseTypeDef


def get_value() -> DescribeVpcConnectionResponseTypeDef:
    return {
        "VpcConnectionArn": ...,
    }


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
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBootstrapBrokersResponseTypeDef

```python
# GetBootstrapBrokersResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetBootstrapBrokersResponseTypeDef


def get_value() -> GetBootstrapBrokersResponseTypeDef:
    return {
        "BootstrapBrokerString": ...,
    }


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
# GetClusterPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetClusterPolicyResponseTypeDef


def get_value() -> GetClusterPolicyResponseTypeDef:
    return {
        "CurrentVersion": ...,
    }


# GetClusterPolicyResponseTypeDef definition

class GetClusterPolicyResponseTypeDef(TypedDict):
    CurrentVersion: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScramSecretsResponseTypeDef

```python
# ListScramSecretsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListScramSecretsResponseTypeDef


def get_value() -> ListScramSecretsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListScramSecretsResponseTypeDef definition

class ListScramSecretsResponseTypeDef(TypedDict):
    SecretArnList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutClusterPolicyResponseTypeDef

```python
# PutClusterPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PutClusterPolicyResponseTypeDef


def get_value() -> PutClusterPolicyResponseTypeDef:
    return {
        "CurrentVersion": ...,
    }


# PutClusterPolicyResponseTypeDef definition

class PutClusterPolicyResponseTypeDef(TypedDict):
    CurrentVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootBrokerResponseTypeDef

```python
# RebootBrokerResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import RebootBrokerResponseTypeDef


def get_value() -> RebootBrokerResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# RebootBrokerResponseTypeDef definition

class RebootBrokerResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerCountResponseTypeDef

```python
# UpdateBrokerCountResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerCountResponseTypeDef


def get_value() -> UpdateBrokerCountResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerCountResponseTypeDef definition

class UpdateBrokerCountResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerStorageResponseTypeDef

```python
# UpdateBrokerStorageResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerStorageResponseTypeDef


def get_value() -> UpdateBrokerStorageResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerStorageResponseTypeDef definition

class UpdateBrokerStorageResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerTypeResponseTypeDef

```python
# UpdateBrokerTypeResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerTypeResponseTypeDef


def get_value() -> UpdateBrokerTypeResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerTypeResponseTypeDef definition

class UpdateBrokerTypeResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigurationResponseTypeDef

```python
# UpdateClusterConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateClusterConfigurationResponseTypeDef


def get_value() -> UpdateClusterConfigurationResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateClusterConfigurationResponseTypeDef definition

class UpdateClusterConfigurationResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterKafkaVersionResponseTypeDef

```python
# UpdateClusterKafkaVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateClusterKafkaVersionResponseTypeDef


def get_value() -> UpdateClusterKafkaVersionResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateClusterKafkaVersionResponseTypeDef definition

class UpdateClusterKafkaVersionResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectivityResponseTypeDef

```python
# UpdateConnectivityResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateConnectivityResponseTypeDef


def get_value() -> UpdateConnectivityResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateConnectivityResponseTypeDef definition

class UpdateConnectivityResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitoringResponseTypeDef

```python
# UpdateMonitoringResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateMonitoringResponseTypeDef


def get_value() -> UpdateMonitoringResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateMonitoringResponseTypeDef definition

class UpdateMonitoringResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationInfoResponseTypeDef

```python
# UpdateReplicationInfoResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateReplicationInfoResponseTypeDef


def get_value() -> UpdateReplicationInfoResponseTypeDef:
    return {
        "ReplicatorArn": ...,
    }


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
# UpdateSecurityResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateSecurityResponseTypeDef


def get_value() -> UpdateSecurityResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateSecurityResponseTypeDef definition

class UpdateSecurityResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStorageResponseTypeDef

```python
# UpdateStorageResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateStorageResponseTypeDef


def get_value() -> UpdateStorageResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateStorageResponseTypeDef definition

class UpdateStorageResponseTypeDef(TypedDict):
    ClusterArn: str,
    ClusterOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAssociateScramSecretResponseTypeDef

```python
# BatchAssociateScramSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretResponseTypeDef


def get_value() -> BatchAssociateScramSecretResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


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
# BatchDisassociateScramSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BatchDisassociateScramSecretResponseTypeDef


def get_value() -> BatchDisassociateScramSecretResponseTypeDef:
    return {
        "ClusterArn": ...,
    }


# BatchDisassociateScramSecretResponseTypeDef definition

class BatchDisassociateScramSecretResponseTypeDef(TypedDict):
    ClusterArn: str,
    UnprocessedScramSecrets: List[UnprocessedScramSecretTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedScramSecretTypeDef](./type_defs.md#unprocessedscramsecrettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationRequestTypeDef

```python
# CreateConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateConfigurationRequestTypeDef


def get_value() -> CreateConfigurationRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateConfigurationRequestTypeDef definition

class CreateConfigurationRequestTypeDef(TypedDict):
    Name: str,
    ServerProperties: BlobTypeDef,
    Description: NotRequired[str],
    KafkaVersions: NotRequired[Sequence[str]],
```

## UpdateConfigurationRequestTypeDef

```python
# UpdateConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateConfigurationRequestTypeDef


def get_value() -> UpdateConfigurationRequestTypeDef:
    return {
        "Arn": ...,
    }


# UpdateConfigurationRequestTypeDef definition

class UpdateConfigurationRequestTypeDef(TypedDict):
    Arn: str,
    ServerProperties: BlobTypeDef,
    Description: NotRequired[str],
```

## BrokerEBSVolumeInfoTypeDef

```python
# BrokerEBSVolumeInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerEBSVolumeInfoTypeDef


def get_value() -> BrokerEBSVolumeInfoTypeDef:
    return {
        "KafkaBrokerNodeId": ...,
    }


# BrokerEBSVolumeInfoTypeDef definition

class BrokerEBSVolumeInfoTypeDef(TypedDict):
    KafkaBrokerNodeId: str,
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    VolumeSizeGB: NotRequired[int],
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## EBSStorageInfoTypeDef

```python
# EBSStorageInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import EBSStorageInfoTypeDef


def get_value() -> EBSStorageInfoTypeDef:
    return {
        "ProvisionedThroughput": ...,
    }


# EBSStorageInfoTypeDef definition

class EBSStorageInfoTypeDef(TypedDict):
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    VolumeSize: NotRequired[int],
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## UpdateStorageRequestTypeDef

```python
# UpdateStorageRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateStorageRequestTypeDef


def get_value() -> UpdateStorageRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateStorageRequestTypeDef definition

class UpdateStorageRequestTypeDef(TypedDict):
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
# BrokerLogsTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerLogsTypeDef


def get_value() -> BrokerLogsTypeDef:
    return {
        "CloudWatchLogs": ...,
    }


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
# BrokerNodeInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerNodeInfoTypeDef


def get_value() -> BrokerNodeInfoTypeDef:
    return {
        "AttachedENIId": ...,
    }


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
# ListClientVpcConnectionsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClientVpcConnectionsResponseTypeDef


def get_value() -> ListClientVpcConnectionsResponseTypeDef:
    return {
        "ClientVpcConnections": ...,
    }


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
# ClusterOperationStepTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationStepTypeDef


def get_value() -> ClusterOperationStepTypeDef:
    return {
        "StepInfo": ...,
    }


# ClusterOperationStepTypeDef definition

class ClusterOperationStepTypeDef(TypedDict):
    StepInfo: NotRequired[ClusterOperationStepInfoTypeDef],  # (1)
    StepName: NotRequired[str],
```

1. See [:material-code-braces: ClusterOperationStepInfoTypeDef](./type_defs.md#clusteroperationstepinfotypedef) 
## ListClusterOperationsV2ResponseTypeDef

```python
# ListClusterOperationsV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsV2ResponseTypeDef


def get_value() -> ListClusterOperationsV2ResponseTypeDef:
    return {
        "ClusterOperationInfoList": ...,
    }


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
# GetCompatibleKafkaVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import GetCompatibleKafkaVersionsResponseTypeDef


def get_value() -> GetCompatibleKafkaVersionsResponseTypeDef:
    return {
        "CompatibleKafkaVersions": ...,
    }


# GetCompatibleKafkaVersionsResponseTypeDef definition

class GetCompatibleKafkaVersionsResponseTypeDef(TypedDict):
    CompatibleKafkaVersions: List[CompatibleKafkaVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompatibleKafkaVersionTypeDef](./type_defs.md#compatiblekafkaversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigurationRequestTypeDef

```python
# UpdateClusterConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateClusterConfigurationRequestTypeDef


def get_value() -> UpdateClusterConfigurationRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateClusterConfigurationRequestTypeDef definition

class UpdateClusterConfigurationRequestTypeDef(TypedDict):
    ClusterArn: str,
    ConfigurationInfo: ConfigurationInfoTypeDef,  # (1)
    CurrentVersion: str,
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
## UpdateClusterKafkaVersionRequestTypeDef

```python
# UpdateClusterKafkaVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateClusterKafkaVersionRequestTypeDef


def get_value() -> UpdateClusterKafkaVersionRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateClusterKafkaVersionRequestTypeDef definition

class UpdateClusterKafkaVersionRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetKafkaVersion: str,
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConfigurationTypeDef


def get_value() -> ConfigurationTypeDef:
    return {
        "Arn": ...,
    }


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
# CreateConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateConfigurationResponseTypeDef


def get_value() -> CreateConfigurationResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# DescribeConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeConfigurationResponseTypeDef


def get_value() -> DescribeConfigurationResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# ListConfigurationRevisionsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationRevisionsResponseTypeDef


def get_value() -> ListConfigurationRevisionsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# UpdateConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateConfigurationResponseTypeDef


def get_value() -> UpdateConfigurationResponseTypeDef:
    return {
        "Arn": ...,
    }


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
# EncryptionInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import EncryptionInfoTypeDef


def get_value() -> EncryptionInfoTypeDef:
    return {
        "EncryptionAtRest": ...,
    }


# EncryptionInfoTypeDef definition

class EncryptionInfoTypeDef(TypedDict):
    EncryptionAtRest: NotRequired[EncryptionAtRestTypeDef],  # (1)
    EncryptionInTransit: NotRequired[EncryptionInTransitTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef) 
2. See [:material-code-braces: EncryptionInTransitTypeDef](./type_defs.md#encryptionintransittypedef) 
## ServerlessSaslTypeDef

```python
# ServerlessSaslTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ServerlessSaslTypeDef


def get_value() -> ServerlessSaslTypeDef:
    return {
        "Iam": ...,
    }


# ServerlessSaslTypeDef definition

class ServerlessSaslTypeDef(TypedDict):
    Iam: NotRequired[IamTypeDef],  # (1)
```

1. See [:material-code-braces: IamTypeDef](./type_defs.md#iamtypedef) 
## KafkaClusterDescriptionTypeDef

```python
# KafkaClusterDescriptionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterDescriptionTypeDef


def get_value() -> KafkaClusterDescriptionTypeDef:
    return {
        "AmazonMskCluster": ...,
    }


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
# ListKafkaVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListKafkaVersionsResponseTypeDef


def get_value() -> ListKafkaVersionsResponseTypeDef:
    return {
        "KafkaVersions": ...,
    }


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
# ListClientVpcConnectionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClientVpcConnectionsRequestPaginateTypeDef


def get_value() -> ListClientVpcConnectionsRequestPaginateTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClientVpcConnectionsRequestPaginateTypeDef definition

class ListClientVpcConnectionsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClusterOperationsRequestPaginateTypeDef

```python
# ListClusterOperationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsRequestPaginateTypeDef


def get_value() -> ListClusterOperationsRequestPaginateTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClusterOperationsRequestPaginateTypeDef definition

class ListClusterOperationsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClusterOperationsV2RequestPaginateTypeDef

```python
# ListClusterOperationsV2RequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsV2RequestPaginateTypeDef


def get_value() -> ListClusterOperationsV2RequestPaginateTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListClusterOperationsV2RequestPaginateTypeDef definition

class ListClusterOperationsV2RequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersRequestPaginateTypeDef


def get_value() -> ListClustersRequestPaginateTypeDef:
    return {
        "ClusterNameFilter": ...,
    }


# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersV2RequestPaginateTypeDef

```python
# ListClustersV2RequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersV2RequestPaginateTypeDef


def get_value() -> ListClustersV2RequestPaginateTypeDef:
    return {
        "ClusterNameFilter": ...,
    }


# ListClustersV2RequestPaginateTypeDef definition

class ListClustersV2RequestPaginateTypeDef(TypedDict):
    ClusterNameFilter: NotRequired[str],
    ClusterTypeFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationRevisionsRequestPaginateTypeDef

```python
# ListConfigurationRevisionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationRevisionsRequestPaginateTypeDef


def get_value() -> ListConfigurationRevisionsRequestPaginateTypeDef:
    return {
        "Arn": ...,
    }


# ListConfigurationRevisionsRequestPaginateTypeDef definition

class ListConfigurationRevisionsRequestPaginateTypeDef(TypedDict):
    Arn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationsRequestPaginateTypeDef

```python
# ListConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationsRequestPaginateTypeDef


def get_value() -> ListConfigurationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListConfigurationsRequestPaginateTypeDef definition

class ListConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKafkaVersionsRequestPaginateTypeDef

```python
# ListKafkaVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListKafkaVersionsRequestPaginateTypeDef


def get_value() -> ListKafkaVersionsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListKafkaVersionsRequestPaginateTypeDef definition

class ListKafkaVersionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodesRequestPaginateTypeDef

```python
# ListNodesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListNodesRequestPaginateTypeDef


def get_value() -> ListNodesRequestPaginateTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListNodesRequestPaginateTypeDef definition

class ListNodesRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReplicatorsRequestPaginateTypeDef

```python
# ListReplicatorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListReplicatorsRequestPaginateTypeDef


def get_value() -> ListReplicatorsRequestPaginateTypeDef:
    return {
        "ReplicatorNameFilter": ...,
    }


# ListReplicatorsRequestPaginateTypeDef definition

class ListReplicatorsRequestPaginateTypeDef(TypedDict):
    ReplicatorNameFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScramSecretsRequestPaginateTypeDef

```python
# ListScramSecretsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListScramSecretsRequestPaginateTypeDef


def get_value() -> ListScramSecretsRequestPaginateTypeDef:
    return {
        "ClusterArn": ...,
    }


# ListScramSecretsRequestPaginateTypeDef definition

class ListScramSecretsRequestPaginateTypeDef(TypedDict):
    ClusterArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVpcConnectionsRequestPaginateTypeDef

```python
# ListVpcConnectionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListVpcConnectionsRequestPaginateTypeDef


def get_value() -> ListVpcConnectionsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListVpcConnectionsRequestPaginateTypeDef definition

class ListVpcConnectionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVpcConnectionsResponseTypeDef

```python
# ListVpcConnectionsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListVpcConnectionsResponseTypeDef


def get_value() -> ListVpcConnectionsResponseTypeDef:
    return {
        "VpcConnections": ...,
    }


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
# PrometheusInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PrometheusInfoTypeDef


def get_value() -> PrometheusInfoTypeDef:
    return {
        "JmxExporter": ...,
    }


# PrometheusInfoTypeDef definition

class PrometheusInfoTypeDef(TypedDict):
    JmxExporter: NotRequired[JmxExporterInfoTypeDef],  # (1)
    NodeExporter: NotRequired[NodeExporterInfoTypeDef],  # (2)
```

1. See [:material-code-braces: JmxExporterInfoTypeDef](./type_defs.md#jmxexporterinfotypedef) 
2. See [:material-code-braces: NodeExporterInfoTypeDef](./type_defs.md#nodeexporterinfotypedef) 
## PrometheusTypeDef

```python
# PrometheusTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import PrometheusTypeDef


def get_value() -> PrometheusTypeDef:
    return {
        "JmxExporter": ...,
    }


# PrometheusTypeDef definition

class PrometheusTypeDef(TypedDict):
    JmxExporter: NotRequired[JmxExporterTypeDef],  # (1)
    NodeExporter: NotRequired[NodeExporterTypeDef],  # (2)
```

1. See [:material-code-braces: JmxExporterTypeDef](./type_defs.md#jmxexportertypedef) 
2. See [:material-code-braces: NodeExporterTypeDef](./type_defs.md#nodeexportertypedef) 
## TopicReplicationOutputTypeDef

```python
# TopicReplicationOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TopicReplicationOutputTypeDef


def get_value() -> TopicReplicationOutputTypeDef:
    return {
        "CopyAccessControlListsForTopics": ...,
    }


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
# TopicReplicationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import TopicReplicationTypeDef


def get_value() -> TopicReplicationTypeDef:
    return {
        "CopyAccessControlListsForTopics": ...,
    }


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
# SaslTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import SaslTypeDef


def get_value() -> SaslTypeDef:
    return {
        "Scram": ...,
    }


# SaslTypeDef definition

class SaslTypeDef(TypedDict):
    Scram: NotRequired[ScramTypeDef],  # (1)
    Iam: NotRequired[IamTypeDef],  # (2)
```

1. See [:material-code-braces: ScramTypeDef](./type_defs.md#scramtypedef) 
2. See [:material-code-braces: IamTypeDef](./type_defs.md#iamtypedef) 
## UpdateReplicationInfoRequestTypeDef

```python
# UpdateReplicationInfoRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateReplicationInfoRequestTypeDef


def get_value() -> UpdateReplicationInfoRequestTypeDef:
    return {
        "CurrentVersion": ...,
    }


# UpdateReplicationInfoRequestTypeDef definition

class UpdateReplicationInfoRequestTypeDef(TypedDict):
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
# VpcConnectionInfoServerlessTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectionInfoServerlessTypeDef


def get_value() -> VpcConnectionInfoServerlessTypeDef:
    return {
        "CreationTime": ...,
    }


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
# VpcConnectionInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectionInfoTypeDef


def get_value() -> VpcConnectionInfoTypeDef:
    return {
        "VpcConnectionArn": ...,
    }


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
# VpcConnectivitySaslTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivitySaslTypeDef


def get_value() -> VpcConnectivitySaslTypeDef:
    return {
        "Scram": ...,
    }


# VpcConnectivitySaslTypeDef definition

class VpcConnectivitySaslTypeDef(TypedDict):
    Scram: NotRequired[VpcConnectivityScramTypeDef],  # (1)
    Iam: NotRequired[VpcConnectivityIamTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConnectivityScramTypeDef](./type_defs.md#vpcconnectivityscramtypedef) 
2. See [:material-code-braces: VpcConnectivityIamTypeDef](./type_defs.md#vpcconnectivityiamtypedef) 
## ReplicatorSummaryTypeDef

```python
# ReplicatorSummaryTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicatorSummaryTypeDef


def get_value() -> ReplicatorSummaryTypeDef:
    return {
        "CreationTime": ...,
    }


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
## UpdateBrokerStorageRequestTypeDef

```python
# UpdateBrokerStorageRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateBrokerStorageRequestTypeDef


def get_value() -> UpdateBrokerStorageRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateBrokerStorageRequestTypeDef definition

class UpdateBrokerStorageRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef],  # (1)
```

1. See [:material-code-braces: BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef) 
## StorageInfoTypeDef

```python
# StorageInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import StorageInfoTypeDef


def get_value() -> StorageInfoTypeDef:
    return {
        "EbsStorageInfo": ...,
    }


# StorageInfoTypeDef definition

class StorageInfoTypeDef(TypedDict):
    EbsStorageInfo: NotRequired[EBSStorageInfoTypeDef],  # (1)
```

1. See [:material-code-braces: EBSStorageInfoTypeDef](./type_defs.md#ebsstorageinfotypedef) 
## LoggingInfoTypeDef

```python
# LoggingInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import LoggingInfoTypeDef


def get_value() -> LoggingInfoTypeDef:
    return {
        "BrokerLogs": ...,
    }


# LoggingInfoTypeDef definition

class LoggingInfoTypeDef(TypedDict):
    BrokerLogs: BrokerLogsTypeDef,  # (1)
```

1. See [:material-code-braces: BrokerLogsTypeDef](./type_defs.md#brokerlogstypedef) 
## NodeInfoTypeDef

```python
# NodeInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import NodeInfoTypeDef


def get_value() -> NodeInfoTypeDef:
    return {
        "AddedToClusterTime": ...,
    }


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
# ListConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListConfigurationsResponseTypeDef


def get_value() -> ListConfigurationsResponseTypeDef:
    return {
        "Configurations": ...,
    }


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
# ServerlessClientAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ServerlessClientAuthenticationTypeDef


def get_value() -> ServerlessClientAuthenticationTypeDef:
    return {
        "Sasl": ...,
    }


# ServerlessClientAuthenticationTypeDef definition

class ServerlessClientAuthenticationTypeDef(TypedDict):
    Sasl: NotRequired[ServerlessSaslTypeDef],  # (1)
```

1. See [:material-code-braces: ServerlessSaslTypeDef](./type_defs.md#serverlesssasltypedef) 
## KafkaClusterTypeDef

```python
# KafkaClusterTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import KafkaClusterTypeDef


def get_value() -> KafkaClusterTypeDef:
    return {
        "AmazonMskCluster": ...,
    }


# KafkaClusterTypeDef definition

class KafkaClusterTypeDef(TypedDict):
    AmazonMskCluster: AmazonMskClusterTypeDef,  # (1)
    VpcConfig: KafkaClusterClientVpcConfigUnionTypeDef,  # (2)
```

1. See [:material-code-braces: AmazonMskClusterTypeDef](./type_defs.md#amazonmskclustertypedef) 
2. See [:material-code-braces: KafkaClusterClientVpcConfigTypeDef](./type_defs.md#kafkaclusterclientvpcconfigtypedef) [:material-code-braces: KafkaClusterClientVpcConfigOutputTypeDef](./type_defs.md#kafkaclusterclientvpcconfigoutputtypedef) 
## OpenMonitoringInfoTypeDef

```python
# OpenMonitoringInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import OpenMonitoringInfoTypeDef


def get_value() -> OpenMonitoringInfoTypeDef:
    return {
        "Prometheus": ...,
    }


# OpenMonitoringInfoTypeDef definition

class OpenMonitoringInfoTypeDef(TypedDict):
    Prometheus: PrometheusInfoTypeDef,  # (1)
```

1. See [:material-code-braces: PrometheusInfoTypeDef](./type_defs.md#prometheusinfotypedef) 
## OpenMonitoringTypeDef

```python
# OpenMonitoringTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import OpenMonitoringTypeDef


def get_value() -> OpenMonitoringTypeDef:
    return {
        "Prometheus": ...,
    }


# OpenMonitoringTypeDef definition

class OpenMonitoringTypeDef(TypedDict):
    Prometheus: PrometheusTypeDef,  # (1)
```

1. See [:material-code-braces: PrometheusTypeDef](./type_defs.md#prometheustypedef) 
## ReplicationInfoDescriptionTypeDef

```python
# ReplicationInfoDescriptionTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationInfoDescriptionTypeDef


def get_value() -> ReplicationInfoDescriptionTypeDef:
    return {
        "ConsumerGroupReplication": ...,
    }


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
# ClientAuthenticationOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClientAuthenticationOutputTypeDef


def get_value() -> ClientAuthenticationOutputTypeDef:
    return {
        "Sasl": ...,
    }


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
# ClientAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClientAuthenticationTypeDef


def get_value() -> ClientAuthenticationTypeDef:
    return {
        "Sasl": ...,
    }


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
# ClusterOperationV2ServerlessTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationV2ServerlessTypeDef


def get_value() -> ClusterOperationV2ServerlessTypeDef:
    return {
        "VpcConnectionInfo": ...,
    }


# ClusterOperationV2ServerlessTypeDef definition

class ClusterOperationV2ServerlessTypeDef(TypedDict):
    VpcConnectionInfo: NotRequired[VpcConnectionInfoServerlessTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConnectionInfoServerlessTypeDef](./type_defs.md#vpcconnectioninfoserverlesstypedef) 
## VpcConnectivityClientAuthenticationTypeDef

```python
# VpcConnectivityClientAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivityClientAuthenticationTypeDef


def get_value() -> VpcConnectivityClientAuthenticationTypeDef:
    return {
        "Sasl": ...,
    }


# VpcConnectivityClientAuthenticationTypeDef definition

class VpcConnectivityClientAuthenticationTypeDef(TypedDict):
    Sasl: NotRequired[VpcConnectivitySaslTypeDef],  # (1)
    Tls: NotRequired[VpcConnectivityTlsTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConnectivitySaslTypeDef](./type_defs.md#vpcconnectivitysasltypedef) 
2. See [:material-code-braces: VpcConnectivityTlsTypeDef](./type_defs.md#vpcconnectivitytlstypedef) 
## ListReplicatorsResponseTypeDef

```python
# ListReplicatorsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListReplicatorsResponseTypeDef


def get_value() -> ListReplicatorsResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListNodesResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListNodesResponseTypeDef


def get_value() -> ListNodesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ServerlessRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ServerlessRequestTypeDef


def get_value() -> ServerlessRequestTypeDef:
    return {
        "VpcConfigs": ...,
    }


# ServerlessRequestTypeDef definition

class ServerlessRequestTypeDef(TypedDict):
    VpcConfigs: Sequence[VpcConfigUnionTypeDef],  # (1)
    ClientAuthentication: NotRequired[ServerlessClientAuthenticationTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
2. See [:material-code-braces: ServerlessClientAuthenticationTypeDef](./type_defs.md#serverlessclientauthenticationtypedef) 
## ServerlessTypeDef

```python
# ServerlessTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ServerlessTypeDef


def get_value() -> ServerlessTypeDef:
    return {
        "VpcConfigs": ...,
    }


# ServerlessTypeDef definition

class ServerlessTypeDef(TypedDict):
    VpcConfigs: List[VpcConfigOutputTypeDef],  # (1)
    ClientAuthentication: NotRequired[ServerlessClientAuthenticationTypeDef],  # (2)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
2. See [:material-code-braces: ServerlessClientAuthenticationTypeDef](./type_defs.md#serverlessclientauthenticationtypedef) 
## UpdateMonitoringRequestTypeDef

```python
# UpdateMonitoringRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateMonitoringRequestTypeDef


def get_value() -> UpdateMonitoringRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateMonitoringRequestTypeDef definition

class UpdateMonitoringRequestTypeDef(TypedDict):
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
# DescribeReplicatorResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeReplicatorResponseTypeDef


def get_value() -> DescribeReplicatorResponseTypeDef:
    return {
        "CreationTime": ...,
    }


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
# ReplicationInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ReplicationInfoTypeDef


def get_value() -> ReplicationInfoTypeDef:
    return {
        "ConsumerGroupReplication": ...,
    }


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
## VpcConnectivityTypeDef

```python
# VpcConnectivityTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import VpcConnectivityTypeDef


def get_value() -> VpcConnectivityTypeDef:
    return {
        "ClientAuthentication": ...,
    }


# VpcConnectivityTypeDef definition

class VpcConnectivityTypeDef(TypedDict):
    ClientAuthentication: NotRequired[VpcConnectivityClientAuthenticationTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConnectivityClientAuthenticationTypeDef](./type_defs.md#vpcconnectivityclientauthenticationtypedef) 
## CreateReplicatorRequestTypeDef

```python
# CreateReplicatorRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateReplicatorRequestTypeDef


def get_value() -> CreateReplicatorRequestTypeDef:
    return {
        "KafkaClusters": ...,
    }


# CreateReplicatorRequestTypeDef definition

class CreateReplicatorRequestTypeDef(TypedDict):
    KafkaClusters: Sequence[KafkaClusterTypeDef],  # (1)
    ReplicationInfoList: Sequence[ReplicationInfoTypeDef],  # (2)
    ReplicatorName: str,
    ServiceExecutionRoleArn: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef) 
2. See [:material-code-braces: ReplicationInfoTypeDef](./type_defs.md#replicationinfotypedef) 
## UpdateSecurityRequestTypeDef

```python
# UpdateSecurityRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateSecurityRequestTypeDef


def get_value() -> UpdateSecurityRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateSecurityRequestTypeDef definition

class UpdateSecurityRequestTypeDef(TypedDict):
    ClusterArn: str,
    CurrentVersion: str,
    ClientAuthentication: NotRequired[ClientAuthenticationUnionTypeDef],  # (1)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (2)
```

1. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) [:material-code-braces: ClientAuthenticationOutputTypeDef](./type_defs.md#clientauthenticationoutputtypedef) 
2. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
## ConnectivityInfoTypeDef

```python
# ConnectivityInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ConnectivityInfoTypeDef


def get_value() -> ConnectivityInfoTypeDef:
    return {
        "PublicAccess": ...,
    }


# ConnectivityInfoTypeDef definition

class ConnectivityInfoTypeDef(TypedDict):
    PublicAccess: NotRequired[PublicAccessTypeDef],  # (1)
    VpcConnectivity: NotRequired[VpcConnectivityTypeDef],  # (2)
```

1. See [:material-code-braces: PublicAccessTypeDef](./type_defs.md#publicaccesstypedef) 
2. See [:material-code-braces: VpcConnectivityTypeDef](./type_defs.md#vpcconnectivitytypedef) 
## BrokerNodeGroupInfoOutputTypeDef

```python
# BrokerNodeGroupInfoOutputTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerNodeGroupInfoOutputTypeDef


def get_value() -> BrokerNodeGroupInfoOutputTypeDef:
    return {
        "BrokerAZDistribution": ...,
    }


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
# BrokerNodeGroupInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import BrokerNodeGroupInfoTypeDef


def get_value() -> BrokerNodeGroupInfoTypeDef:
    return {
        "BrokerAZDistribution": ...,
    }


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
# MutableClusterInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import MutableClusterInfoTypeDef


def get_value() -> MutableClusterInfoTypeDef:
    return {
        "BrokerEBSVolumeInfo": ...,
    }


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
## UpdateConnectivityRequestTypeDef

```python
# UpdateConnectivityRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import UpdateConnectivityRequestTypeDef


def get_value() -> UpdateConnectivityRequestTypeDef:
    return {
        "ClusterArn": ...,
    }


# UpdateConnectivityRequestTypeDef definition

class UpdateConnectivityRequestTypeDef(TypedDict):
    ClusterArn: str,
    ConnectivityInfo: ConnectivityInfoTypeDef,  # (1)
    CurrentVersion: str,
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
## ClusterInfoTypeDef

```python
# ClusterInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterInfoTypeDef


def get_value() -> ClusterInfoTypeDef:
    return {
        "ActiveOperationArn": ...,
    }


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
# ProvisionedTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ProvisionedTypeDef


def get_value() -> ProvisionedTypeDef:
    return {
        "BrokerNodeGroupInfo": ...,
    }


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
## ClusterOperationInfoTypeDef

```python
# ClusterOperationInfoTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationInfoTypeDef


def get_value() -> ClusterOperationInfoTypeDef:
    return {
        "ClientRequestId": ...,
    }


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
# ClusterOperationV2ProvisionedTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationV2ProvisionedTypeDef


def get_value() -> ClusterOperationV2ProvisionedTypeDef:
    return {
        "OperationSteps": ...,
    }


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
# DescribeClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterResponseTypeDef


def get_value() -> DescribeClusterResponseTypeDef:
    return {
        "ClusterInfo": ...,
    }


# DescribeClusterResponseTypeDef definition

class DescribeClusterResponseTypeDef(TypedDict):
    ClusterInfo: ClusterInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterInfoTypeDef](./type_defs.md#clusterinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersResponseTypeDef


def get_value() -> ListClustersResponseTypeDef:
    return {
        "ClusterInfoList": ...,
    }


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
# ClusterTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterTypeDef


def get_value() -> ClusterTypeDef:
    return {
        "ActiveOperationArn": ...,
    }


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
## CreateClusterRequestTypeDef

```python
# CreateClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateClusterRequestTypeDef


def get_value() -> CreateClusterRequestTypeDef:
    return {
        "BrokerNodeGroupInfo": ...,
    }


# CreateClusterRequestTypeDef definition

class CreateClusterRequestTypeDef(TypedDict):
    BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,  # (1)
    ClusterName: str,
    KafkaVersion: str,
    NumberOfBrokerNodes: int,
    ClientAuthentication: NotRequired[ClientAuthenticationUnionTypeDef],  # (2)
    ConfigurationInfo: NotRequired[ConfigurationInfoTypeDef],  # (3)
    EncryptionInfo: NotRequired[EncryptionInfoTypeDef],  # (4)
    EnhancedMonitoring: NotRequired[EnhancedMonitoringType],  # (5)
    OpenMonitoring: NotRequired[OpenMonitoringInfoTypeDef],  # (6)
    LoggingInfo: NotRequired[LoggingInfoTypeDef],  # (7)
    Tags: NotRequired[Mapping[str, str]],
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
## ProvisionedRequestTypeDef

```python
# ProvisionedRequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ProvisionedRequestTypeDef


def get_value() -> ProvisionedRequestTypeDef:
    return {
        "BrokerNodeGroupInfo": ...,
    }


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
# DescribeClusterOperationResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterOperationResponseTypeDef


def get_value() -> DescribeClusterOperationResponseTypeDef:
    return {
        "ClusterOperationInfo": ...,
    }


# DescribeClusterOperationResponseTypeDef definition

class DescribeClusterOperationResponseTypeDef(TypedDict):
    ClusterOperationInfo: ClusterOperationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterOperationInfoTypeDef](./type_defs.md#clusteroperationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClusterOperationsResponseTypeDef

```python
# ListClusterOperationsResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClusterOperationsResponseTypeDef


def get_value() -> ListClusterOperationsResponseTypeDef:
    return {
        "ClusterOperationInfoList": ...,
    }


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
# ClusterOperationV2TypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ClusterOperationV2TypeDef


def get_value() -> ClusterOperationV2TypeDef:
    return {
        "ClusterArn": ...,
    }


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
# DescribeClusterV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterV2ResponseTypeDef


def get_value() -> DescribeClusterV2ResponseTypeDef:
    return {
        "ClusterInfo": ...,
    }


# DescribeClusterV2ResponseTypeDef definition

class DescribeClusterV2ResponseTypeDef(TypedDict):
    ClusterInfo: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersV2ResponseTypeDef

```python
# ListClustersV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import ListClustersV2ResponseTypeDef


def get_value() -> ListClustersV2ResponseTypeDef:
    return {
        "ClusterInfoList": ...,
    }


# ListClustersV2ResponseTypeDef definition

class ListClustersV2ResponseTypeDef(TypedDict):
    ClusterInfoList: List[ClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterV2RequestTypeDef

```python
# CreateClusterV2RequestTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import CreateClusterV2RequestTypeDef


def get_value() -> CreateClusterV2RequestTypeDef:
    return {
        "ClusterName": ...,
    }


# CreateClusterV2RequestTypeDef definition

class CreateClusterV2RequestTypeDef(TypedDict):
    ClusterName: str,
    Tags: NotRequired[Mapping[str, str]],
    Provisioned: NotRequired[ProvisionedRequestTypeDef],  # (1)
    Serverless: NotRequired[ServerlessRequestTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef) 
2. See [:material-code-braces: ServerlessRequestTypeDef](./type_defs.md#serverlessrequesttypedef) 
## DescribeClusterOperationV2ResponseTypeDef

```python
# DescribeClusterOperationV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_kafka.type_defs import DescribeClusterOperationV2ResponseTypeDef


def get_value() -> DescribeClusterOperationV2ResponseTypeDef:
    return {
        "ClusterOperationInfo": ...,
    }


# DescribeClusterOperationV2ResponseTypeDef definition

class DescribeClusterOperationV2ResponseTypeDef(TypedDict):
    ClusterOperationInfo: ClusterOperationV2TypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterOperationV2TypeDef](./type_defs.md#clusteroperationv2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
