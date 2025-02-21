# Type definitions

> [Index](../README.md) > [ParallelComputingService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).



## SlurmCustomSettingTypeDef

```python
# SlurmCustomSettingTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import SlurmCustomSettingTypeDef


def get_value() -> SlurmCustomSettingTypeDef:
    return {
        "parameterName": ...,
    }


# SlurmCustomSettingTypeDef definition

class SlurmCustomSettingTypeDef(TypedDict):
    parameterName: str,
    parameterValue: str,
```

## SlurmAuthKeyTypeDef

```python
# SlurmAuthKeyTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import SlurmAuthKeyTypeDef


def get_value() -> SlurmAuthKeyTypeDef:
    return {
        "secretArn": ...,
    }


# SlurmAuthKeyTypeDef definition

class SlurmAuthKeyTypeDef(TypedDict):
    secretArn: str,
    secretVersion: str,
```

## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ClusterSummaryTypeDef


def get_value() -> ClusterSummaryTypeDef:
    return {
        "name": ...,
    }


# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    createdAt: datetime,
    modifiedAt: datetime,
    status: ClusterStatusType,  # (1)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
## EndpointTypeDef

```python
# EndpointTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import EndpointTypeDef


def get_value() -> EndpointTypeDef:
    return {
        "type": ...,
    }


# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    type: EndpointTypeType,  # (1)
    privateIpAddress: str,
    port: str,
    publicIpAddress: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ErrorInfoTypeDef


def get_value() -> ErrorInfoTypeDef:
    return {
        "code": ...,
    }


# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## NetworkingTypeDef

```python
# NetworkingTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import NetworkingTypeDef


def get_value() -> NetworkingTypeDef:
    return {
        "subnetIds": ...,
    }


# NetworkingTypeDef definition

class NetworkingTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
```

## SchedulerTypeDef

```python
# SchedulerTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import SchedulerTypeDef


def get_value() -> SchedulerTypeDef:
    return {
        "type": ...,
    }


# SchedulerTypeDef definition

class SchedulerTypeDef(TypedDict):
    type: SchedulerTypeType,  # (1)
    version: str,
```

1. See [:material-code-brackets: SchedulerTypeType](./literals.md#schedulertypetype) 
## ComputeNodeGroupConfigurationTypeDef

```python
# ComputeNodeGroupConfigurationTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ComputeNodeGroupConfigurationTypeDef


def get_value() -> ComputeNodeGroupConfigurationTypeDef:
    return {
        "computeNodeGroupId": ...,
    }


# ComputeNodeGroupConfigurationTypeDef definition

class ComputeNodeGroupConfigurationTypeDef(TypedDict):
    computeNodeGroupId: NotRequired[str],
```

## ComputeNodeGroupSummaryTypeDef

```python
# ComputeNodeGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ComputeNodeGroupSummaryTypeDef


def get_value() -> ComputeNodeGroupSummaryTypeDef:
    return {
        "name": ...,
    }


# ComputeNodeGroupSummaryTypeDef definition

class ComputeNodeGroupSummaryTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    clusterId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    status: ComputeNodeGroupStatusType,  # (1)
```

1. See [:material-code-brackets: ComputeNodeGroupStatusType](./literals.md#computenodegroupstatustype) 
## CustomLaunchTemplateTypeDef

```python
# CustomLaunchTemplateTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CustomLaunchTemplateTypeDef


def get_value() -> CustomLaunchTemplateTypeDef:
    return {
        "id": ...,
    }


# CustomLaunchTemplateTypeDef definition

class CustomLaunchTemplateTypeDef(TypedDict):
    id: str,
    version: str,
```

## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import InstanceConfigTypeDef


def get_value() -> InstanceConfigTypeDef:
    return {
        "instanceType": ...,
    }


# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    instanceType: NotRequired[str],
```

## ScalingConfigurationTypeDef

```python
# ScalingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ScalingConfigurationTypeDef


def get_value() -> ScalingConfigurationTypeDef:
    return {
        "minInstanceCount": ...,
    }


# ScalingConfigurationTypeDef definition

class ScalingConfigurationTypeDef(TypedDict):
    minInstanceCount: int,
    maxInstanceCount: int,
```

## SpotOptionsTypeDef

```python
# SpotOptionsTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import SpotOptionsTypeDef


def get_value() -> SpotOptionsTypeDef:
    return {
        "allocationStrategy": ...,
    }


# SpotOptionsTypeDef definition

class SpotOptionsTypeDef(TypedDict):
    allocationStrategy: NotRequired[SpotAllocationStrategyType],  # (1)
```

1. See [:material-code-brackets: SpotAllocationStrategyType](./literals.md#spotallocationstrategytype) 
## NetworkingRequestTypeDef

```python
# NetworkingRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import NetworkingRequestTypeDef


def get_value() -> NetworkingRequestTypeDef:
    return {
        "subnetIds": ...,
    }


# NetworkingRequestTypeDef definition

class NetworkingRequestTypeDef(TypedDict):
    subnetIds: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
```

## SchedulerRequestTypeDef

```python
# SchedulerRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import SchedulerRequestTypeDef


def get_value() -> SchedulerRequestTypeDef:
    return {
        "type": ...,
    }


# SchedulerRequestTypeDef definition

class SchedulerRequestTypeDef(TypedDict):
    type: SchedulerTypeType,  # (1)
    version: str,
```

1. See [:material-code-brackets: SchedulerTypeType](./literals.md#schedulertypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ResponseMetadataTypeDef


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

## ScalingConfigurationRequestTypeDef

```python
# ScalingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ScalingConfigurationRequestTypeDef


def get_value() -> ScalingConfigurationRequestTypeDef:
    return {
        "minInstanceCount": ...,
    }


# ScalingConfigurationRequestTypeDef definition

class ScalingConfigurationRequestTypeDef(TypedDict):
    minInstanceCount: int,
    maxInstanceCount: int,
```

## DeleteClusterRequestTypeDef

```python
# DeleteClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import DeleteClusterRequestTypeDef


def get_value() -> DeleteClusterRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# DeleteClusterRequestTypeDef definition

class DeleteClusterRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    clientToken: NotRequired[str],
```

## DeleteComputeNodeGroupRequestTypeDef

```python
# DeleteComputeNodeGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import DeleteComputeNodeGroupRequestTypeDef


def get_value() -> DeleteComputeNodeGroupRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# DeleteComputeNodeGroupRequestTypeDef definition

class DeleteComputeNodeGroupRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
    clientToken: NotRequired[str],
```

## DeleteQueueRequestTypeDef

```python
# DeleteQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import DeleteQueueRequestTypeDef


def get_value() -> DeleteQueueRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# DeleteQueueRequestTypeDef definition

class DeleteQueueRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
    clientToken: NotRequired[str],
```

## GetClusterRequestTypeDef

```python
# GetClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetClusterRequestTypeDef


def get_value() -> GetClusterRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# GetClusterRequestTypeDef definition

class GetClusterRequestTypeDef(TypedDict):
    clusterIdentifier: str,
```

## GetComputeNodeGroupRequestTypeDef

```python
# GetComputeNodeGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetComputeNodeGroupRequestTypeDef


def get_value() -> GetComputeNodeGroupRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# GetComputeNodeGroupRequestTypeDef definition

class GetComputeNodeGroupRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
```

## GetQueueRequestTypeDef

```python
# GetQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetQueueRequestTypeDef


def get_value() -> GetQueueRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# GetQueueRequestTypeDef definition

class GetQueueRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import PaginatorConfigTypeDef


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

## ListClustersRequestTypeDef

```python
# ListClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListClustersRequestTypeDef


def get_value() -> ListClustersRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListClustersRequestTypeDef definition

class ListClustersRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListComputeNodeGroupsRequestTypeDef

```python
# ListComputeNodeGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListComputeNodeGroupsRequestTypeDef


def get_value() -> ListComputeNodeGroupsRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# ListComputeNodeGroupsRequestTypeDef definition

class ListComputeNodeGroupsRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListQueuesRequestTypeDef

```python
# ListQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListQueuesRequestTypeDef


def get_value() -> ListQueuesRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# ListQueuesRequestTypeDef definition

class ListQueuesRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueSummaryTypeDef

```python
# QueueSummaryTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import QueueSummaryTypeDef


def get_value() -> QueueSummaryTypeDef:
    return {
        "name": ...,
    }


# QueueSummaryTypeDef definition

class QueueSummaryTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    clusterId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    status: QueueStatusType,  # (1)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterComputeNodeGroupInstanceRequestTypeDef

```python
# RegisterComputeNodeGroupInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import RegisterComputeNodeGroupInstanceRequestTypeDef


def get_value() -> RegisterComputeNodeGroupInstanceRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# RegisterComputeNodeGroupInstanceRequestTypeDef definition

class RegisterComputeNodeGroupInstanceRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    bootstrapId: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## ClusterSlurmConfigurationRequestTypeDef

```python
# ClusterSlurmConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ClusterSlurmConfigurationRequestTypeDef


def get_value() -> ClusterSlurmConfigurationRequestTypeDef:
    return {
        "scaleDownIdleTimeInSeconds": ...,
    }


# ClusterSlurmConfigurationRequestTypeDef definition

class ClusterSlurmConfigurationRequestTypeDef(TypedDict):
    scaleDownIdleTimeInSeconds: NotRequired[int],
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ComputeNodeGroupSlurmConfigurationRequestTypeDef

```python
# ComputeNodeGroupSlurmConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ComputeNodeGroupSlurmConfigurationRequestTypeDef


def get_value() -> ComputeNodeGroupSlurmConfigurationRequestTypeDef:
    return {
        "slurmCustomSettings": ...,
    }


# ComputeNodeGroupSlurmConfigurationRequestTypeDef definition

class ComputeNodeGroupSlurmConfigurationRequestTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ComputeNodeGroupSlurmConfigurationTypeDef

```python
# ComputeNodeGroupSlurmConfigurationTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ComputeNodeGroupSlurmConfigurationTypeDef


def get_value() -> ComputeNodeGroupSlurmConfigurationTypeDef:
    return {
        "slurmCustomSettings": ...,
    }


# ComputeNodeGroupSlurmConfigurationTypeDef definition

class ComputeNodeGroupSlurmConfigurationTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[List[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef

```python
# UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef


def get_value() -> UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef:
    return {
        "slurmCustomSettings": ...,
    }


# UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef definition

class UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ClusterSlurmConfigurationTypeDef

```python
# ClusterSlurmConfigurationTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ClusterSlurmConfigurationTypeDef


def get_value() -> ClusterSlurmConfigurationTypeDef:
    return {
        "scaleDownIdleTimeInSeconds": ...,
    }


# ClusterSlurmConfigurationTypeDef definition

class ClusterSlurmConfigurationTypeDef(TypedDict):
    scaleDownIdleTimeInSeconds: NotRequired[int],
    slurmCustomSettings: NotRequired[List[SlurmCustomSettingTypeDef]],  # (1)
    authKey: NotRequired[SlurmAuthKeyTypeDef],  # (2)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
2. See [:material-code-braces: SlurmAuthKeyTypeDef](./type_defs.md#slurmauthkeytypedef) 
## CreateQueueRequestTypeDef

```python
# CreateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateQueueRequestTypeDef


def get_value() -> CreateQueueRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# CreateQueueRequestTypeDef definition

class CreateQueueRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueName: str,
    computeNodeGroupConfigurations: NotRequired[Sequence[ComputeNodeGroupConfigurationTypeDef]],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
## QueueTypeDef

```python
# QueueTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import QueueTypeDef


def get_value() -> QueueTypeDef:
    return {
        "name": ...,
    }


# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    clusterId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    status: QueueStatusType,  # (1)
    computeNodeGroupConfigurations: List[ComputeNodeGroupConfigurationTypeDef],  # (2)
    errorInfo: NotRequired[List[ErrorInfoTypeDef]],  # (3)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
3. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
## UpdateQueueRequestTypeDef

```python
# UpdateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UpdateQueueRequestTypeDef


def get_value() -> UpdateQueueRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# UpdateQueueRequestTypeDef definition

class UpdateQueueRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
    computeNodeGroupConfigurations: NotRequired[Sequence[ComputeNodeGroupConfigurationTypeDef]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListClustersResponseTypeDef


def get_value() -> ListClustersResponseTypeDef:
    return {
        "clusters": ...,
    }


# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusters: List[ClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComputeNodeGroupsResponseTypeDef

```python
# ListComputeNodeGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListComputeNodeGroupsResponseTypeDef


def get_value() -> ListComputeNodeGroupsResponseTypeDef:
    return {
        "computeNodeGroups": ...,
    }


# ListComputeNodeGroupsResponseTypeDef definition

class ListComputeNodeGroupsResponseTypeDef(TypedDict):
    computeNodeGroups: List[ComputeNodeGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ComputeNodeGroupSummaryTypeDef](./type_defs.md#computenodegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterComputeNodeGroupInstanceResponseTypeDef

```python
# RegisterComputeNodeGroupInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import RegisterComputeNodeGroupInstanceResponseTypeDef


def get_value() -> RegisterComputeNodeGroupInstanceResponseTypeDef:
    return {
        "nodeID": ...,
    }


# RegisterComputeNodeGroupInstanceResponseTypeDef definition

class RegisterComputeNodeGroupInstanceResponseTypeDef(TypedDict):
    nodeID: str,
    sharedSecret: str,
    endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListClustersRequestPaginateTypeDef


def get_value() -> ListClustersRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComputeNodeGroupsRequestPaginateTypeDef

```python
# ListComputeNodeGroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListComputeNodeGroupsRequestPaginateTypeDef


def get_value() -> ListComputeNodeGroupsRequestPaginateTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# ListComputeNodeGroupsRequestPaginateTypeDef definition

class ListComputeNodeGroupsRequestPaginateTypeDef(TypedDict):
    clusterIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestPaginateTypeDef

```python
# ListQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListQueuesRequestPaginateTypeDef


def get_value() -> ListQueuesRequestPaginateTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# ListQueuesRequestPaginateTypeDef definition

class ListQueuesRequestPaginateTypeDef(TypedDict):
    clusterIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ListQueuesResponseTypeDef


def get_value() -> ListQueuesResponseTypeDef:
    return {
        "queues": ...,
    }


# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    queues: List[QueueSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterRequestTypeDef

```python
# CreateClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateClusterRequestTypeDef


def get_value() -> CreateClusterRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreateClusterRequestTypeDef definition

class CreateClusterRequestTypeDef(TypedDict):
    clusterName: str,
    scheduler: SchedulerRequestTypeDef,  # (1)
    size: SizeType,  # (2)
    networking: NetworkingRequestTypeDef,  # (3)
    slurmConfiguration: NotRequired[ClusterSlurmConfigurationRequestTypeDef],  # (4)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SchedulerRequestTypeDef](./type_defs.md#schedulerrequesttypedef) 
2. See [:material-code-brackets: SizeType](./literals.md#sizetype) 
3. See [:material-code-braces: NetworkingRequestTypeDef](./type_defs.md#networkingrequesttypedef) 
4. See [:material-code-braces: ClusterSlurmConfigurationRequestTypeDef](./type_defs.md#clusterslurmconfigurationrequesttypedef) 
## CreateComputeNodeGroupRequestTypeDef

```python
# CreateComputeNodeGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateComputeNodeGroupRequestTypeDef


def get_value() -> CreateComputeNodeGroupRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# CreateComputeNodeGroupRequestTypeDef definition

class CreateComputeNodeGroupRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupName: str,
    subnetIds: Sequence[str],
    customLaunchTemplate: CustomLaunchTemplateTypeDef,  # (1)
    iamInstanceProfileArn: str,
    scalingConfiguration: ScalingConfigurationRequestTypeDef,  # (2)
    instanceConfigs: Sequence[InstanceConfigTypeDef],  # (3)
    amiId: NotRequired[str],
    purchaseOption: NotRequired[PurchaseOptionType],  # (4)
    spotOptions: NotRequired[SpotOptionsTypeDef],  # (5)
    slurmConfiguration: NotRequired[ComputeNodeGroupSlurmConfigurationRequestTypeDef],  # (6)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef) 
2. See [:material-code-braces: ScalingConfigurationRequestTypeDef](./type_defs.md#scalingconfigurationrequesttypedef) 
3. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
4. See [:material-code-brackets: PurchaseOptionType](./literals.md#purchaseoptiontype) 
5. See [:material-code-braces: SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef) 
6. See [:material-code-braces: ComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#computenodegroupslurmconfigurationrequesttypedef) 
## ComputeNodeGroupTypeDef

```python
# ComputeNodeGroupTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ComputeNodeGroupTypeDef


def get_value() -> ComputeNodeGroupTypeDef:
    return {
        "name": ...,
    }


# ComputeNodeGroupTypeDef definition

class ComputeNodeGroupTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    clusterId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    status: ComputeNodeGroupStatusType,  # (1)
    subnetIds: List[str],
    customLaunchTemplate: CustomLaunchTemplateTypeDef,  # (3)
    iamInstanceProfileArn: str,
    scalingConfiguration: ScalingConfigurationTypeDef,  # (4)
    instanceConfigs: List[InstanceConfigTypeDef],  # (5)
    amiId: NotRequired[str],
    purchaseOption: NotRequired[PurchaseOptionType],  # (2)
    spotOptions: NotRequired[SpotOptionsTypeDef],  # (6)
    slurmConfiguration: NotRequired[ComputeNodeGroupSlurmConfigurationTypeDef],  # (7)
    errorInfo: NotRequired[List[ErrorInfoTypeDef]],  # (8)
```

1. See [:material-code-brackets: ComputeNodeGroupStatusType](./literals.md#computenodegroupstatustype) 
2. See [:material-code-brackets: PurchaseOptionType](./literals.md#purchaseoptiontype) 
3. See [:material-code-braces: CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef) 
4. See [:material-code-braces: ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef) 
5. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
6. See [:material-code-braces: SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef) 
7. See [:material-code-braces: ComputeNodeGroupSlurmConfigurationTypeDef](./type_defs.md#computenodegroupslurmconfigurationtypedef) 
8. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
## UpdateComputeNodeGroupRequestTypeDef

```python
# UpdateComputeNodeGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UpdateComputeNodeGroupRequestTypeDef


def get_value() -> UpdateComputeNodeGroupRequestTypeDef:
    return {
        "clusterIdentifier": ...,
    }


# UpdateComputeNodeGroupRequestTypeDef definition

class UpdateComputeNodeGroupRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
    amiId: NotRequired[str],
    subnetIds: NotRequired[Sequence[str]],
    customLaunchTemplate: NotRequired[CustomLaunchTemplateTypeDef],  # (1)
    purchaseOption: NotRequired[PurchaseOptionType],  # (2)
    spotOptions: NotRequired[SpotOptionsTypeDef],  # (3)
    scalingConfiguration: NotRequired[ScalingConfigurationRequestTypeDef],  # (4)
    iamInstanceProfileArn: NotRequired[str],
    slurmConfiguration: NotRequired[UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef],  # (5)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef) 
2. See [:material-code-brackets: PurchaseOptionType](./literals.md#purchaseoptiontype) 
3. See [:material-code-braces: SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef) 
4. See [:material-code-braces: ScalingConfigurationRequestTypeDef](./type_defs.md#scalingconfigurationrequesttypedef) 
5. See [:material-code-braces: UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#updatecomputenodegroupslurmconfigurationrequesttypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import ClusterTypeDef


def get_value() -> ClusterTypeDef:
    return {
        "name": ...,
    }


# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    createdAt: datetime,
    modifiedAt: datetime,
    scheduler: SchedulerTypeDef,  # (2)
    size: SizeType,  # (3)
    networking: NetworkingTypeDef,  # (5)
    slurmConfiguration: NotRequired[ClusterSlurmConfigurationTypeDef],  # (4)
    endpoints: NotRequired[List[EndpointTypeDef]],  # (6)
    errorInfo: NotRequired[List[ErrorInfoTypeDef]],  # (7)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: SchedulerTypeDef](./type_defs.md#schedulertypedef) 
3. See [:material-code-brackets: SizeType](./literals.md#sizetype) 
4. See [:material-code-braces: ClusterSlurmConfigurationTypeDef](./type_defs.md#clusterslurmconfigurationtypedef) 
5. See [:material-code-braces: NetworkingTypeDef](./type_defs.md#networkingtypedef) 
6. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
7. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateQueueResponseTypeDef


def get_value() -> CreateQueueResponseTypeDef:
    return {
        "queue": ...,
    }


# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueResponseTypeDef

```python
# GetQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetQueueResponseTypeDef


def get_value() -> GetQueueResponseTypeDef:
    return {
        "queue": ...,
    }


# GetQueueResponseTypeDef definition

class GetQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQueueResponseTypeDef

```python
# UpdateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UpdateQueueResponseTypeDef


def get_value() -> UpdateQueueResponseTypeDef:
    return {
        "queue": ...,
    }


# UpdateQueueResponseTypeDef definition

class UpdateQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComputeNodeGroupResponseTypeDef

```python
# CreateComputeNodeGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateComputeNodeGroupResponseTypeDef


def get_value() -> CreateComputeNodeGroupResponseTypeDef:
    return {
        "computeNodeGroup": ...,
    }


# CreateComputeNodeGroupResponseTypeDef definition

class CreateComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComputeNodeGroupResponseTypeDef

```python
# GetComputeNodeGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetComputeNodeGroupResponseTypeDef


def get_value() -> GetComputeNodeGroupResponseTypeDef:
    return {
        "computeNodeGroup": ...,
    }


# GetComputeNodeGroupResponseTypeDef definition

class GetComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComputeNodeGroupResponseTypeDef

```python
# UpdateComputeNodeGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import UpdateComputeNodeGroupResponseTypeDef


def get_value() -> UpdateComputeNodeGroupResponseTypeDef:
    return {
        "computeNodeGroup": ...,
    }


# UpdateComputeNodeGroupResponseTypeDef definition

class UpdateComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import CreateClusterResponseTypeDef


def get_value() -> CreateClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterResponseTypeDef

```python
# GetClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_pcs.type_defs import GetClusterResponseTypeDef


def get_value() -> GetClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# GetClusterResponseTypeDef definition

class GetClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
