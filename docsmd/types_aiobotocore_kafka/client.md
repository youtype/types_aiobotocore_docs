# KafkaClient

> [Index](../README.md) > [Kafka](./README.md) > KafkaClient

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## KafkaClient

Type annotations and code completion for `#!python session.create_client("kafka")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client)

```python
# KafkaClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kafka.client import KafkaClient

session = get_session()
async with session.create_client("kafka") as client:
    client: KafkaClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kafka").exceptions` structure.

```python
# KafkaClient.exceptions usage example

async with session.create_client("kafka") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# KafkaClient usage type checking example

from types_aiobotocore_kafka.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("kafka").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("kafka").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("kafka").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### batch\_associate\_scram\_secret

Associates one or more Scram Secrets with an Amazon MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").batch_associate_scram_secret` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/batch_associate_scram_secret.html)

```python
# batch_associate_scram_secret method definition

await def batch_associate_scram_secret(
    self,
    *,
    ClusterArn: str,
    SecretArnList: Sequence[str],
) -> BatchAssociateScramSecretResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef) 


```python
# batch_associate_scram_secret method usage example with argument unpacking

kwargs: BatchAssociateScramSecretRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "SecretArnList": ...,
}

parent.batch_associate_scram_secret(**kwargs)
```

1. See [:material-code-braces: BatchAssociateScramSecretRequestRequestTypeDef](./type_defs.md#batchassociatescramsecretrequestrequesttypedef) 

### create\_cluster

Creates a new MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/create_cluster.html)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,  # (1)
    ClusterName: str,
    KafkaVersion: str,
    NumberOfBrokerNodes: int,
    ClientAuthentication: ClientAuthenticationTypeDef = ...,  # (2)
    ConfigurationInfo: ConfigurationInfoTypeDef = ...,  # (3)
    EncryptionInfo: EncryptionInfoTypeDef = ...,  # (4)
    EnhancedMonitoring: EnhancedMonitoringType = ...,  # (5)
    OpenMonitoring: OpenMonitoringInfoTypeDef = ...,  # (6)
    LoggingInfo: LoggingInfoTypeDef = ...,  # (7)
    Tags: Mapping[str, str] = ...,
    StorageMode: StorageModeType = ...,  # (8)
) -> CreateClusterResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: BrokerNodeGroupInfoTypeDef](./type_defs.md#brokernodegroupinfotypedef) 
2. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) 
3. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
4. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
5. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
6. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
7. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
8. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
9. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestRequestTypeDef = {  # (1)
    "BrokerNodeGroupInfo": ...,
    "ClusterName": ...,
    "KafkaVersion": ...,
    "NumberOfBrokerNodes": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef) 

### create\_cluster\_v2

Creates a new MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").create_cluster_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/create_cluster_v2.html)

```python
# create_cluster_v2 method definition

await def create_cluster_v2(
    self,
    *,
    ClusterName: str,
    Tags: Mapping[str, str] = ...,
    Provisioned: ProvisionedRequestTypeDef = ...,  # (1)
    Serverless: ServerlessRequestTypeDef = ...,  # (2)
) -> CreateClusterV2ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ProvisionedRequestTypeDef](./type_defs.md#provisionedrequesttypedef) 
2. See [:material-code-braces: ServerlessRequestTypeDef](./type_defs.md#serverlessrequesttypedef) 
3. See [:material-code-braces: CreateClusterV2ResponseTypeDef](./type_defs.md#createclusterv2responsetypedef) 


```python
# create_cluster_v2 method usage example with argument unpacking

kwargs: CreateClusterV2RequestRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.create_cluster_v2(**kwargs)
```

1. See [:material-code-braces: CreateClusterV2RequestRequestTypeDef](./type_defs.md#createclusterv2requestrequesttypedef) 

### create\_configuration

Creates a new MSK configuration.

Type annotations and code completion for `#!python session.create_client("kafka").create_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/create_configuration.html)

```python
# create_configuration method definition

await def create_configuration(
    self,
    *,
    Name: str,
    ServerProperties: BlobTypeDef,
    Description: str = ...,
    KafkaVersions: Sequence[str] = ...,
) -> CreateConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateConfigurationResponseTypeDef](./type_defs.md#createconfigurationresponsetypedef) 


```python
# create_configuration method usage example with argument unpacking

kwargs: CreateConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ServerProperties": ...,
}

parent.create_configuration(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationRequestRequestTypeDef](./type_defs.md#createconfigurationrequestrequesttypedef) 

### create\_replicator

Creates the replicator.

Type annotations and code completion for `#!python session.create_client("kafka").create_replicator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/create_replicator.html)

```python
# create_replicator method definition

await def create_replicator(
    self,
    *,
    KafkaClusters: Sequence[KafkaClusterTypeDef],  # (1)
    ReplicationInfoList: Sequence[ReplicationInfoTypeDef],  # (2)
    ReplicatorName: str,
    ServiceExecutionRoleArn: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateReplicatorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef) 
2. See [:material-code-braces: ReplicationInfoTypeDef](./type_defs.md#replicationinfotypedef) 
3. See [:material-code-braces: CreateReplicatorResponseTypeDef](./type_defs.md#createreplicatorresponsetypedef) 


```python
# create_replicator method usage example with argument unpacking

kwargs: CreateReplicatorRequestRequestTypeDef = {  # (1)
    "KafkaClusters": ...,
    "ReplicationInfoList": ...,
    "ReplicatorName": ...,
    "ServiceExecutionRoleArn": ...,
}

parent.create_replicator(**kwargs)
```

1. See [:material-code-braces: CreateReplicatorRequestRequestTypeDef](./type_defs.md#createreplicatorrequestrequesttypedef) 

### create\_vpc\_connection

Creates a new MSK VPC connection.

Type annotations and code completion for `#!python session.create_client("kafka").create_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/create_vpc_connection.html)

```python
# create_vpc_connection method definition

await def create_vpc_connection(
    self,
    *,
    TargetClusterArn: str,
    Authentication: str,
    VpcId: str,
    ClientSubnets: Sequence[str],
    SecurityGroups: Sequence[str],
    Tags: Mapping[str, str] = ...,
) -> CreateVpcConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVpcConnectionResponseTypeDef](./type_defs.md#createvpcconnectionresponsetypedef) 


```python
# create_vpc_connection method usage example with argument unpacking

kwargs: CreateVpcConnectionRequestRequestTypeDef = {  # (1)
    "TargetClusterArn": ...,
    "Authentication": ...,
    "VpcId": ...,
    "ClientSubnets": ...,
    "SecurityGroups": ...,
}

parent.create_vpc_connection(**kwargs)
```

1. See [:material-code-braces: CreateVpcConnectionRequestRequestTypeDef](./type_defs.md#createvpcconnectionrequestrequesttypedef) 

### delete\_cluster

Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
request.

Type annotations and code completion for `#!python session.create_client("kafka").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/delete_cluster.html)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str = ...,
) -> DeleteClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef) 

### delete\_cluster\_policy

Deletes the MSK cluster policy specified by the Amazon Resource Name (ARN) in
the request.

Type annotations and code completion for `#!python session.create_client("kafka").delete_cluster_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/delete_cluster_policy.html)

```python
# delete_cluster_policy method definition

await def delete_cluster_policy(
    self,
    *,
    ClusterArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_cluster_policy method usage example with argument unpacking

kwargs: DeleteClusterPolicyRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.delete_cluster_policy(**kwargs)
```

1. See [:material-code-braces: DeleteClusterPolicyRequestRequestTypeDef](./type_defs.md#deleteclusterpolicyrequestrequesttypedef) 

### delete\_configuration

Deletes an MSK Configuration.

Type annotations and code completion for `#!python session.create_client("kafka").delete_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/delete_configuration.html)

```python
# delete_configuration method definition

await def delete_configuration(
    self,
    *,
    Arn: str,
) -> DeleteConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteConfigurationResponseTypeDef](./type_defs.md#deleteconfigurationresponsetypedef) 


```python
# delete_configuration method usage example with argument unpacking

kwargs: DeleteConfigurationRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationRequestRequestTypeDef](./type_defs.md#deleteconfigurationrequestrequesttypedef) 

### delete\_replicator

Deletes a replicator.

Type annotations and code completion for `#!python session.create_client("kafka").delete_replicator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/delete_replicator.html)

```python
# delete_replicator method definition

await def delete_replicator(
    self,
    *,
    ReplicatorArn: str,
    CurrentVersion: str = ...,
) -> DeleteReplicatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReplicatorResponseTypeDef](./type_defs.md#deletereplicatorresponsetypedef) 


```python
# delete_replicator method usage example with argument unpacking

kwargs: DeleteReplicatorRequestRequestTypeDef = {  # (1)
    "ReplicatorArn": ...,
}

parent.delete_replicator(**kwargs)
```

1. See [:material-code-braces: DeleteReplicatorRequestRequestTypeDef](./type_defs.md#deletereplicatorrequestrequesttypedef) 

### delete\_vpc\_connection

Deletes a MSK VPC connection.

Type annotations and code completion for `#!python session.create_client("kafka").delete_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/delete_vpc_connection.html)

```python
# delete_vpc_connection method definition

await def delete_vpc_connection(
    self,
    *,
    Arn: str,
) -> DeleteVpcConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVpcConnectionResponseTypeDef](./type_defs.md#deletevpcconnectionresponsetypedef) 


```python
# delete_vpc_connection method usage example with argument unpacking

kwargs: DeleteVpcConnectionRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DeleteVpcConnectionRequestRequestTypeDef](./type_defs.md#deletevpcconnectionrequestrequesttypedef) 

### describe\_cluster

Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
specified in the request.

Type annotations and code completion for `#!python session.create_client("kafka").describe_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_cluster.html)

```python
# describe_cluster method definition

await def describe_cluster(
    self,
    *,
    ClusterArn: str,
) -> DescribeClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef) 


```python
# describe_cluster method usage example with argument unpacking

kwargs: DescribeClusterRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.describe_cluster(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef) 

### describe\_cluster\_v2

Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
specified in the request.

Type annotations and code completion for `#!python session.create_client("kafka").describe_cluster_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_cluster_v2.html)

```python
# describe_cluster_v2 method definition

await def describe_cluster_v2(
    self,
    *,
    ClusterArn: str,
) -> DescribeClusterV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterV2ResponseTypeDef](./type_defs.md#describeclusterv2responsetypedef) 


```python
# describe_cluster_v2 method usage example with argument unpacking

kwargs: DescribeClusterV2RequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.describe_cluster_v2(**kwargs)
```

1. See [:material-code-braces: DescribeClusterV2RequestRequestTypeDef](./type_defs.md#describeclusterv2requestrequesttypedef) 

### describe\_cluster\_operation

Returns a description of the cluster operation specified by the ARN.

Type annotations and code completion for `#!python session.create_client("kafka").describe_cluster_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_cluster_operation.html)

```python
# describe_cluster_operation method definition

await def describe_cluster_operation(
    self,
    *,
    ClusterOperationArn: str,
) -> DescribeClusterOperationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterOperationResponseTypeDef](./type_defs.md#describeclusteroperationresponsetypedef) 


```python
# describe_cluster_operation method usage example with argument unpacking

kwargs: DescribeClusterOperationRequestRequestTypeDef = {  # (1)
    "ClusterOperationArn": ...,
}

parent.describe_cluster_operation(**kwargs)
```

1. See [:material-code-braces: DescribeClusterOperationRequestRequestTypeDef](./type_defs.md#describeclusteroperationrequestrequesttypedef) 

### describe\_cluster\_operation\_v2

Returns a description of the cluster operation specified by the ARN.

Type annotations and code completion for `#!python session.create_client("kafka").describe_cluster_operation_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_cluster_operation_v2.html)

```python
# describe_cluster_operation_v2 method definition

await def describe_cluster_operation_v2(
    self,
    *,
    ClusterOperationArn: str,
) -> DescribeClusterOperationV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterOperationV2ResponseTypeDef](./type_defs.md#describeclusteroperationv2responsetypedef) 


```python
# describe_cluster_operation_v2 method usage example with argument unpacking

kwargs: DescribeClusterOperationV2RequestRequestTypeDef = {  # (1)
    "ClusterOperationArn": ...,
}

parent.describe_cluster_operation_v2(**kwargs)
```

1. See [:material-code-braces: DescribeClusterOperationV2RequestRequestTypeDef](./type_defs.md#describeclusteroperationv2requestrequesttypedef) 

### describe\_configuration

Returns a description of this MSK configuration.

Type annotations and code completion for `#!python session.create_client("kafka").describe_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_configuration.html)

```python
# describe_configuration method definition

await def describe_configuration(
    self,
    *,
    Arn: str,
) -> DescribeConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationResponseTypeDef](./type_defs.md#describeconfigurationresponsetypedef) 


```python
# describe_configuration method usage example with argument unpacking

kwargs: DescribeConfigurationRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.describe_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationRequestRequestTypeDef](./type_defs.md#describeconfigurationrequestrequesttypedef) 

### describe\_configuration\_revision

Returns a description of this revision of the configuration.

Type annotations and code completion for `#!python session.create_client("kafka").describe_configuration_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_configuration_revision.html)

```python
# describe_configuration_revision method definition

await def describe_configuration_revision(
    self,
    *,
    Arn: str,
    Revision: int,
) -> DescribeConfigurationRevisionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationRevisionResponseTypeDef](./type_defs.md#describeconfigurationrevisionresponsetypedef) 


```python
# describe_configuration_revision method usage example with argument unpacking

kwargs: DescribeConfigurationRevisionRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "Revision": ...,
}

parent.describe_configuration_revision(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationRevisionRequestRequestTypeDef](./type_defs.md#describeconfigurationrevisionrequestrequesttypedef) 

### describe\_replicator

Describes a replicator.

Type annotations and code completion for `#!python session.create_client("kafka").describe_replicator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_replicator.html)

```python
# describe_replicator method definition

await def describe_replicator(
    self,
    *,
    ReplicatorArn: str,
) -> DescribeReplicatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplicatorResponseTypeDef](./type_defs.md#describereplicatorresponsetypedef) 


```python
# describe_replicator method usage example with argument unpacking

kwargs: DescribeReplicatorRequestRequestTypeDef = {  # (1)
    "ReplicatorArn": ...,
}

parent.describe_replicator(**kwargs)
```

1. See [:material-code-braces: DescribeReplicatorRequestRequestTypeDef](./type_defs.md#describereplicatorrequestrequesttypedef) 

### describe\_vpc\_connection

Returns a description of this MSK VPC connection.

Type annotations and code completion for `#!python session.create_client("kafka").describe_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/describe_vpc_connection.html)

```python
# describe_vpc_connection method definition

await def describe_vpc_connection(
    self,
    *,
    Arn: str,
) -> DescribeVpcConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVpcConnectionResponseTypeDef](./type_defs.md#describevpcconnectionresponsetypedef) 


```python
# describe_vpc_connection method usage example with argument unpacking

kwargs: DescribeVpcConnectionRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.describe_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DescribeVpcConnectionRequestRequestTypeDef](./type_defs.md#describevpcconnectionrequestrequesttypedef) 

### batch\_disassociate\_scram\_secret

Disassociates one or more Scram Secrets from an Amazon MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").batch_disassociate_scram_secret` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/batch_disassociate_scram_secret.html)

```python
# batch_disassociate_scram_secret method definition

await def batch_disassociate_scram_secret(
    self,
    *,
    ClusterArn: str,
    SecretArnList: Sequence[str],
) -> BatchDisassociateScramSecretResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisassociateScramSecretResponseTypeDef](./type_defs.md#batchdisassociatescramsecretresponsetypedef) 


```python
# batch_disassociate_scram_secret method usage example with argument unpacking

kwargs: BatchDisassociateScramSecretRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "SecretArnList": ...,
}

parent.batch_disassociate_scram_secret(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateScramSecretRequestRequestTypeDef](./type_defs.md#batchdisassociatescramsecretrequestrequesttypedef) 

### get\_bootstrap\_brokers

A list of brokers that a client application can use to bootstrap.

Type annotations and code completion for `#!python session.create_client("kafka").get_bootstrap_brokers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/get_bootstrap_brokers.html)

```python
# get_bootstrap_brokers method definition

await def get_bootstrap_brokers(
    self,
    *,
    ClusterArn: str,
) -> GetBootstrapBrokersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBootstrapBrokersResponseTypeDef](./type_defs.md#getbootstrapbrokersresponsetypedef) 


```python
# get_bootstrap_brokers method usage example with argument unpacking

kwargs: GetBootstrapBrokersRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.get_bootstrap_brokers(**kwargs)
```

1. See [:material-code-braces: GetBootstrapBrokersRequestRequestTypeDef](./type_defs.md#getbootstrapbrokersrequestrequesttypedef) 

### get\_compatible\_kafka\_versions

Gets the Apache Kafka versions to which you can update the MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").get_compatible_kafka_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/get_compatible_kafka_versions.html)

```python
# get_compatible_kafka_versions method definition

await def get_compatible_kafka_versions(
    self,
    *,
    ClusterArn: str = ...,
) -> GetCompatibleKafkaVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCompatibleKafkaVersionsResponseTypeDef](./type_defs.md#getcompatiblekafkaversionsresponsetypedef) 


```python
# get_compatible_kafka_versions method usage example with argument unpacking

kwargs: GetCompatibleKafkaVersionsRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.get_compatible_kafka_versions(**kwargs)
```

1. See [:material-code-braces: GetCompatibleKafkaVersionsRequestRequestTypeDef](./type_defs.md#getcompatiblekafkaversionsrequestrequesttypedef) 

### get\_cluster\_policy

Get the MSK cluster policy specified by the Amazon Resource Name (ARN) in the
request.

Type annotations and code completion for `#!python session.create_client("kafka").get_cluster_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/get_cluster_policy.html)

```python
# get_cluster_policy method definition

await def get_cluster_policy(
    self,
    *,
    ClusterArn: str,
) -> GetClusterPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterPolicyResponseTypeDef](./type_defs.md#getclusterpolicyresponsetypedef) 


```python
# get_cluster_policy method usage example with argument unpacking

kwargs: GetClusterPolicyRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.get_cluster_policy(**kwargs)
```

1. See [:material-code-braces: GetClusterPolicyRequestRequestTypeDef](./type_defs.md#getclusterpolicyrequestrequesttypedef) 

### list\_cluster\_operations

Returns a list of all the operations that have been performed on the specified
MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").list_cluster_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_cluster_operations.html)

```python
# list_cluster_operations method definition

await def list_cluster_operations(
    self,
    *,
    ClusterArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClusterOperationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef) 


```python
# list_cluster_operations method usage example with argument unpacking

kwargs: ListClusterOperationsRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.list_cluster_operations(**kwargs)
```

1. See [:material-code-braces: ListClusterOperationsRequestRequestTypeDef](./type_defs.md#listclusteroperationsrequestrequesttypedef) 

### list\_cluster\_operations\_v2

Returns a list of all the operations that have been performed on the specified
MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").list_cluster_operations_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_cluster_operations_v2.html)

```python
# list_cluster_operations_v2 method definition

await def list_cluster_operations_v2(
    self,
    *,
    ClusterArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClusterOperationsV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClusterOperationsV2ResponseTypeDef](./type_defs.md#listclusteroperationsv2responsetypedef) 


```python
# list_cluster_operations_v2 method usage example with argument unpacking

kwargs: ListClusterOperationsV2RequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.list_cluster_operations_v2(**kwargs)
```

1. See [:material-code-braces: ListClusterOperationsV2RequestRequestTypeDef](./type_defs.md#listclusteroperationsv2requestrequesttypedef) 

### list\_clusters

Returns a list of all the MSK clusters in the current Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_clusters.html)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    ClusterNameFilter: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersRequestRequestTypeDef = {  # (1)
    "ClusterNameFilter": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef) 

### list\_clusters\_v2

Returns a list of all the MSK clusters in the current Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_clusters_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_clusters_v2.html)

```python
# list_clusters_v2 method definition

await def list_clusters_v2(
    self,
    *,
    ClusterNameFilter: str = ...,
    ClusterTypeFilter: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClustersV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersV2ResponseTypeDef](./type_defs.md#listclustersv2responsetypedef) 


```python
# list_clusters_v2 method usage example with argument unpacking

kwargs: ListClustersV2RequestRequestTypeDef = {  # (1)
    "ClusterNameFilter": ...,
}

parent.list_clusters_v2(**kwargs)
```

1. See [:material-code-braces: ListClustersV2RequestRequestTypeDef](./type_defs.md#listclustersv2requestrequesttypedef) 

### list\_configuration\_revisions

Returns a list of all the MSK configurations in this Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_configuration_revisions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_configuration_revisions.html)

```python
# list_configuration_revisions method definition

await def list_configuration_revisions(
    self,
    *,
    Arn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConfigurationRevisionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfigurationRevisionsResponseTypeDef](./type_defs.md#listconfigurationrevisionsresponsetypedef) 


```python
# list_configuration_revisions method usage example with argument unpacking

kwargs: ListConfigurationRevisionsRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_configuration_revisions(**kwargs)
```

1. See [:material-code-braces: ListConfigurationRevisionsRequestRequestTypeDef](./type_defs.md#listconfigurationrevisionsrequestrequesttypedef) 

### list\_configurations

Returns a list of all the MSK configurations in this Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_configurations.html)

```python
# list_configurations method definition

await def list_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


```python
# list_configurations method usage example with argument unpacking

kwargs: ListConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_configurations(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef) 

### list\_kafka\_versions

Returns a list of Apache Kafka versions.

Type annotations and code completion for `#!python session.create_client("kafka").list_kafka_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_kafka_versions.html)

```python
# list_kafka_versions method definition

await def list_kafka_versions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListKafkaVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKafkaVersionsResponseTypeDef](./type_defs.md#listkafkaversionsresponsetypedef) 


```python
# list_kafka_versions method usage example with argument unpacking

kwargs: ListKafkaVersionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_kafka_versions(**kwargs)
```

1. See [:material-code-braces: ListKafkaVersionsRequestRequestTypeDef](./type_defs.md#listkafkaversionsrequestrequesttypedef) 

### list\_nodes

Returns a list of the broker nodes in the cluster.

Type annotations and code completion for `#!python session.create_client("kafka").list_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_nodes.html)

```python
# list_nodes method definition

await def list_nodes(
    self,
    *,
    ClusterArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


```python
# list_nodes method usage example with argument unpacking

kwargs: ListNodesRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.list_nodes(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef) 

### list\_replicators

Lists the replicators.

Type annotations and code completion for `#!python session.create_client("kafka").list_replicators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_replicators.html)

```python
# list_replicators method definition

await def list_replicators(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ReplicatorNameFilter: str = ...,
) -> ListReplicatorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReplicatorsResponseTypeDef](./type_defs.md#listreplicatorsresponsetypedef) 


```python
# list_replicators method usage example with argument unpacking

kwargs: ListReplicatorsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_replicators(**kwargs)
```

1. See [:material-code-braces: ListReplicatorsRequestRequestTypeDef](./type_defs.md#listreplicatorsrequestrequesttypedef) 

### list\_scram\_secrets

Returns a list of the Scram Secrets associated with an Amazon MSK cluster.

Type annotations and code completion for `#!python session.create_client("kafka").list_scram_secrets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_scram_secrets.html)

```python
# list_scram_secrets method definition

await def list_scram_secrets(
    self,
    *,
    ClusterArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListScramSecretsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScramSecretsResponseTypeDef](./type_defs.md#listscramsecretsresponsetypedef) 


```python
# list_scram_secrets method usage example with argument unpacking

kwargs: ListScramSecretsRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.list_scram_secrets(**kwargs)
```

1. See [:material-code-braces: ListScramSecretsRequestRequestTypeDef](./type_defs.md#listscramsecretsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags associated with the specified resource.

Type annotations and code completion for `#!python session.create_client("kafka").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_client\_vpc\_connections

Returns a list of all the VPC connections in this Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_client_vpc_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_client_vpc_connections.html)

```python
# list_client_vpc_connections method definition

await def list_client_vpc_connections(
    self,
    *,
    ClusterArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClientVpcConnectionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef) 


```python
# list_client_vpc_connections method usage example with argument unpacking

kwargs: ListClientVpcConnectionsRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.list_client_vpc_connections(**kwargs)
```

1. See [:material-code-braces: ListClientVpcConnectionsRequestRequestTypeDef](./type_defs.md#listclientvpcconnectionsrequestrequesttypedef) 

### list\_vpc\_connections

Returns a list of all the VPC connections in this Region.

Type annotations and code completion for `#!python session.create_client("kafka").list_vpc_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/list_vpc_connections.html)

```python
# list_vpc_connections method definition

await def list_vpc_connections(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListVpcConnectionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVpcConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef) 


```python
# list_vpc_connections method usage example with argument unpacking

kwargs: ListVpcConnectionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_vpc_connections(**kwargs)
```

1. See [:material-code-braces: ListVpcConnectionsRequestRequestTypeDef](./type_defs.md#listvpcconnectionsrequestrequesttypedef) 

### reject\_client\_vpc\_connection

Returns empty response.

Type annotations and code completion for `#!python session.create_client("kafka").reject_client_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/reject_client_vpc_connection.html)

```python
# reject_client_vpc_connection method definition

await def reject_client_vpc_connection(
    self,
    *,
    ClusterArn: str,
    VpcConnectionArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# reject_client_vpc_connection method usage example with argument unpacking

kwargs: RejectClientVpcConnectionRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "VpcConnectionArn": ...,
}

parent.reject_client_vpc_connection(**kwargs)
```

1. See [:material-code-braces: RejectClientVpcConnectionRequestRequestTypeDef](./type_defs.md#rejectclientvpcconnectionrequestrequesttypedef) 

### put\_cluster\_policy

Creates or updates the MSK cluster policy specified by the cluster Amazon
Resource Name (ARN) in the request.

Type annotations and code completion for `#!python session.create_client("kafka").put_cluster_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/put_cluster_policy.html)

```python
# put_cluster_policy method definition

await def put_cluster_policy(
    self,
    *,
    ClusterArn: str,
    Policy: str,
    CurrentVersion: str = ...,
) -> PutClusterPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutClusterPolicyResponseTypeDef](./type_defs.md#putclusterpolicyresponsetypedef) 


```python
# put_cluster_policy method usage example with argument unpacking

kwargs: PutClusterPolicyRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "Policy": ...,
}

parent.put_cluster_policy(**kwargs)
```

1. See [:material-code-braces: PutClusterPolicyRequestRequestTypeDef](./type_defs.md#putclusterpolicyrequestrequesttypedef) 

### reboot\_broker

Reboots brokers.

Type annotations and code completion for `#!python session.create_client("kafka").reboot_broker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/reboot_broker.html)

```python
# reboot_broker method definition

await def reboot_broker(
    self,
    *,
    BrokerIds: Sequence[str],
    ClusterArn: str,
) -> RebootBrokerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RebootBrokerResponseTypeDef](./type_defs.md#rebootbrokerresponsetypedef) 


```python
# reboot_broker method usage example with argument unpacking

kwargs: RebootBrokerRequestRequestTypeDef = {  # (1)
    "BrokerIds": ...,
    "ClusterArn": ...,
}

parent.reboot_broker(**kwargs)
```

1. See [:material-code-braces: RebootBrokerRequestRequestTypeDef](./type_defs.md#rebootbrokerrequestrequesttypedef) 

### tag\_resource

Adds tags to the specified MSK resource.

Type annotations and code completion for `#!python session.create_client("kafka").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the tags associated with the keys that are provided in the query.

Type annotations and code completion for `#!python session.create_client("kafka").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_broker\_count

Updates the number of broker nodes in the cluster.

Type annotations and code completion for `#!python session.create_client("kafka").update_broker_count` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_broker_count.html)

```python
# update_broker_count method definition

await def update_broker_count(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    TargetNumberOfBrokerNodes: int,
) -> UpdateBrokerCountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBrokerCountResponseTypeDef](./type_defs.md#updatebrokercountresponsetypedef) 


```python
# update_broker_count method usage example with argument unpacking

kwargs: UpdateBrokerCountRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
    "TargetNumberOfBrokerNodes": ...,
}

parent.update_broker_count(**kwargs)
```

1. See [:material-code-braces: UpdateBrokerCountRequestRequestTypeDef](./type_defs.md#updatebrokercountrequestrequesttypedef) 

### update\_broker\_type

Updates EC2 instance type.

Type annotations and code completion for `#!python session.create_client("kafka").update_broker_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_broker_type.html)

```python
# update_broker_type method definition

await def update_broker_type(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    TargetInstanceType: str,
) -> UpdateBrokerTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBrokerTypeResponseTypeDef](./type_defs.md#updatebrokertyperesponsetypedef) 


```python
# update_broker_type method usage example with argument unpacking

kwargs: UpdateBrokerTypeRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
    "TargetInstanceType": ...,
}

parent.update_broker_type(**kwargs)
```

1. See [:material-code-braces: UpdateBrokerTypeRequestRequestTypeDef](./type_defs.md#updatebrokertyperequestrequesttypedef) 

### update\_broker\_storage

Updates the EBS storage associated with MSK brokers.

Type annotations and code completion for `#!python session.create_client("kafka").update_broker_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_broker_storage.html)

```python
# update_broker_storage method definition

await def update_broker_storage(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    TargetBrokerEBSVolumeInfo: Sequence[BrokerEBSVolumeInfoTypeDef],  # (1)
) -> UpdateBrokerStorageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BrokerEBSVolumeInfoTypeDef](./type_defs.md#brokerebsvolumeinfotypedef) 
2. See [:material-code-braces: UpdateBrokerStorageResponseTypeDef](./type_defs.md#updatebrokerstorageresponsetypedef) 


```python
# update_broker_storage method usage example with argument unpacking

kwargs: UpdateBrokerStorageRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
    "TargetBrokerEBSVolumeInfo": ...,
}

parent.update_broker_storage(**kwargs)
```

1. See [:material-code-braces: UpdateBrokerStorageRequestRequestTypeDef](./type_defs.md#updatebrokerstoragerequestrequesttypedef) 

### update\_configuration

Updates an MSK configuration.

Type annotations and code completion for `#!python session.create_client("kafka").update_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_configuration.html)

```python
# update_configuration method definition

await def update_configuration(
    self,
    *,
    Arn: str,
    ServerProperties: BlobTypeDef,
    Description: str = ...,
) -> UpdateConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateConfigurationResponseTypeDef](./type_defs.md#updateconfigurationresponsetypedef) 


```python
# update_configuration method usage example with argument unpacking

kwargs: UpdateConfigurationRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "ServerProperties": ...,
}

parent.update_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef) 

### update\_connectivity

Updates the cluster's connectivity configuration.

Type annotations and code completion for `#!python session.create_client("kafka").update_connectivity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_connectivity.html)

```python
# update_connectivity method definition

await def update_connectivity(
    self,
    *,
    ClusterArn: str,
    ConnectivityInfo: ConnectivityInfoTypeDef,  # (1)
    CurrentVersion: str,
) -> UpdateConnectivityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
2. See [:material-code-braces: UpdateConnectivityResponseTypeDef](./type_defs.md#updateconnectivityresponsetypedef) 


```python
# update_connectivity method usage example with argument unpacking

kwargs: UpdateConnectivityRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "ConnectivityInfo": ...,
    "CurrentVersion": ...,
}

parent.update_connectivity(**kwargs)
```

1. See [:material-code-braces: UpdateConnectivityRequestRequestTypeDef](./type_defs.md#updateconnectivityrequestrequesttypedef) 

### update\_cluster\_configuration

Updates the cluster with the configuration that is specified in the request
body.

Type annotations and code completion for `#!python session.create_client("kafka").update_cluster_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_cluster_configuration.html)

```python
# update_cluster_configuration method definition

await def update_cluster_configuration(
    self,
    *,
    ClusterArn: str,
    ConfigurationInfo: ConfigurationInfoTypeDef,  # (1)
    CurrentVersion: str,
) -> UpdateClusterConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
2. See [:material-code-braces: UpdateClusterConfigurationResponseTypeDef](./type_defs.md#updateclusterconfigurationresponsetypedef) 


```python
# update_cluster_configuration method usage example with argument unpacking

kwargs: UpdateClusterConfigurationRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "ConfigurationInfo": ...,
    "CurrentVersion": ...,
}

parent.update_cluster_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateClusterConfigurationRequestRequestTypeDef](./type_defs.md#updateclusterconfigurationrequestrequesttypedef) 

### update\_cluster\_kafka\_version

Updates the Apache Kafka version for the cluster.

Type annotations and code completion for `#!python session.create_client("kafka").update_cluster_kafka_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_cluster_kafka_version.html)

```python
# update_cluster_kafka_version method definition

await def update_cluster_kafka_version(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    TargetKafkaVersion: str,
    ConfigurationInfo: ConfigurationInfoTypeDef = ...,  # (1)
) -> UpdateClusterKafkaVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationInfoTypeDef](./type_defs.md#configurationinfotypedef) 
2. See [:material-code-braces: UpdateClusterKafkaVersionResponseTypeDef](./type_defs.md#updateclusterkafkaversionresponsetypedef) 


```python
# update_cluster_kafka_version method usage example with argument unpacking

kwargs: UpdateClusterKafkaVersionRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
    "TargetKafkaVersion": ...,
}

parent.update_cluster_kafka_version(**kwargs)
```

1. See [:material-code-braces: UpdateClusterKafkaVersionRequestRequestTypeDef](./type_defs.md#updateclusterkafkaversionrequestrequesttypedef) 

### update\_monitoring

Updates the monitoring settings for the cluster.

Type annotations and code completion for `#!python session.create_client("kafka").update_monitoring` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_monitoring.html)

```python
# update_monitoring method definition

await def update_monitoring(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    EnhancedMonitoring: EnhancedMonitoringType = ...,  # (1)
    OpenMonitoring: OpenMonitoringInfoTypeDef = ...,  # (2)
    LoggingInfo: LoggingInfoTypeDef = ...,  # (3)
) -> UpdateMonitoringResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: EnhancedMonitoringType](./literals.md#enhancedmonitoringtype) 
2. See [:material-code-braces: OpenMonitoringInfoTypeDef](./type_defs.md#openmonitoringinfotypedef) 
3. See [:material-code-braces: LoggingInfoTypeDef](./type_defs.md#logginginfotypedef) 
4. See [:material-code-braces: UpdateMonitoringResponseTypeDef](./type_defs.md#updatemonitoringresponsetypedef) 


```python
# update_monitoring method usage example with argument unpacking

kwargs: UpdateMonitoringRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
}

parent.update_monitoring(**kwargs)
```

1. See [:material-code-braces: UpdateMonitoringRequestRequestTypeDef](./type_defs.md#updatemonitoringrequestrequesttypedef) 

### update\_replication\_info

Updates replication info of a replicator.

Type annotations and code completion for `#!python session.create_client("kafka").update_replication_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_replication_info.html)

```python
# update_replication_info method definition

await def update_replication_info(
    self,
    *,
    CurrentVersion: str,
    ReplicatorArn: str,
    SourceKafkaClusterArn: str,
    TargetKafkaClusterArn: str,
    ConsumerGroupReplication: ConsumerGroupReplicationUpdateTypeDef = ...,  # (1)
    TopicReplication: TopicReplicationUpdateTypeDef = ...,  # (2)
) -> UpdateReplicationInfoResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConsumerGroupReplicationUpdateTypeDef](./type_defs.md#consumergroupreplicationupdatetypedef) 
2. See [:material-code-braces: TopicReplicationUpdateTypeDef](./type_defs.md#topicreplicationupdatetypedef) 
3. See [:material-code-braces: UpdateReplicationInfoResponseTypeDef](./type_defs.md#updatereplicationinforesponsetypedef) 


```python
# update_replication_info method usage example with argument unpacking

kwargs: UpdateReplicationInfoRequestRequestTypeDef = {  # (1)
    "CurrentVersion": ...,
    "ReplicatorArn": ...,
    "SourceKafkaClusterArn": ...,
    "TargetKafkaClusterArn": ...,
}

parent.update_replication_info(**kwargs)
```

1. See [:material-code-braces: UpdateReplicationInfoRequestRequestTypeDef](./type_defs.md#updatereplicationinforequestrequesttypedef) 

### update\_security

Updates the security settings for the cluster.

Type annotations and code completion for `#!python session.create_client("kafka").update_security` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_security.html)

```python
# update_security method definition

await def update_security(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    ClientAuthentication: ClientAuthenticationTypeDef = ...,  # (1)
    EncryptionInfo: EncryptionInfoTypeDef = ...,  # (2)
) -> UpdateSecurityResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ClientAuthenticationTypeDef](./type_defs.md#clientauthenticationtypedef) 
2. See [:material-code-braces: EncryptionInfoTypeDef](./type_defs.md#encryptioninfotypedef) 
3. See [:material-code-braces: UpdateSecurityResponseTypeDef](./type_defs.md#updatesecurityresponsetypedef) 


```python
# update_security method usage example with argument unpacking

kwargs: UpdateSecurityRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
}

parent.update_security(**kwargs)
```

1. See [:material-code-braces: UpdateSecurityRequestRequestTypeDef](./type_defs.md#updatesecurityrequestrequesttypedef) 

### update\_storage

Updates cluster broker volume size (or) sets cluster storage mode to TIERED.

Type annotations and code completion for `#!python session.create_client("kafka").update_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka/client/update_storage.html)

```python
# update_storage method definition

await def update_storage(
    self,
    *,
    ClusterArn: str,
    CurrentVersion: str,
    ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,  # (1)
    StorageMode: StorageModeType = ...,  # (2)
    VolumeSizeGB: int = ...,
) -> UpdateStorageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
2. See [:material-code-brackets: StorageModeType](./literals.md#storagemodetype) 
3. See [:material-code-braces: UpdateStorageResponseTypeDef](./type_defs.md#updatestorageresponsetypedef) 


```python
# update_storage method usage example with argument unpacking

kwargs: UpdateStorageRequestRequestTypeDef = {  # (1)
    "ClusterArn": ...,
    "CurrentVersion": ...,
}

parent.update_storage(**kwargs)
```

1. See [:material-code-braces: UpdateStorageRequestRequestTypeDef](./type_defs.md#updatestoragerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kafka").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "KafkaClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kafka").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("kafka").get_paginator` method with overloads.

- `client.get_paginator("list_client_vpc_connections")` -> [ListClientVpcConnectionsPaginator](./paginators.md#listclientvpcconnectionspaginator)
- `client.get_paginator("list_cluster_operations")` -> [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
- `client.get_paginator("list_cluster_operations_v2")` -> [ListClusterOperationsV2Paginator](./paginators.md#listclusteroperationsv2paginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_clusters_v2")` -> [ListClustersV2Paginator](./paginators.md#listclustersv2paginator)
- `client.get_paginator("list_configuration_revisions")` -> [ListConfigurationRevisionsPaginator](./paginators.md#listconfigurationrevisionspaginator)
- `client.get_paginator("list_configurations")` -> [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
- `client.get_paginator("list_kafka_versions")` -> [ListKafkaVersionsPaginator](./paginators.md#listkafkaversionspaginator)
- `client.get_paginator("list_nodes")` -> [ListNodesPaginator](./paginators.md#listnodespaginator)
- `client.get_paginator("list_replicators")` -> [ListReplicatorsPaginator](./paginators.md#listreplicatorspaginator)
- `client.get_paginator("list_scram_secrets")` -> [ListScramSecretsPaginator](./paginators.md#listscramsecretspaginator)
- `client.get_paginator("list_vpc_connections")` -> [ListVpcConnectionsPaginator](./paginators.md#listvpcconnectionspaginator)



