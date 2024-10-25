# Type definitions

> [Index](../README.md) > [ParallelComputingService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).



## SlurmCustomSettingTypeDef

```python
# SlurmCustomSettingTypeDef definition

class SlurmCustomSettingTypeDef(TypedDict):
    parameterName: str,
    parameterValue: str,
```

## SlurmAuthKeyTypeDef

```python
# SlurmAuthKeyTypeDef definition

class SlurmAuthKeyTypeDef(TypedDict):
    secretArn: str,
    secretVersion: str,
```

## ClusterSummaryTypeDef

```python
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
# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## NetworkingTypeDef

```python
# NetworkingTypeDef definition

class NetworkingTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
```

## SchedulerTypeDef

```python
# SchedulerTypeDef definition

class SchedulerTypeDef(TypedDict):
    type: SchedulerTypeType,  # (1)
    version: str,
```

1. See [:material-code-brackets: SchedulerTypeType](./literals.md#schedulertypetype) 
## ComputeNodeGroupConfigurationTypeDef

```python
# ComputeNodeGroupConfigurationTypeDef definition

class ComputeNodeGroupConfigurationTypeDef(TypedDict):
    computeNodeGroupId: NotRequired[str],
```

## ComputeNodeGroupSummaryTypeDef

```python
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
# CustomLaunchTemplateTypeDef definition

class CustomLaunchTemplateTypeDef(TypedDict):
    id: str,
    version: str,
```

## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    instanceType: NotRequired[str],
```

## ScalingConfigurationTypeDef

```python
# ScalingConfigurationTypeDef definition

class ScalingConfigurationTypeDef(TypedDict):
    minInstanceCount: int,
    maxInstanceCount: int,
```

## SpotOptionsTypeDef

```python
# SpotOptionsTypeDef definition

class SpotOptionsTypeDef(TypedDict):
    allocationStrategy: NotRequired[SpotAllocationStrategyType],  # (1)
```

1. See [:material-code-brackets: SpotAllocationStrategyType](./literals.md#spotallocationstrategytype) 
## NetworkingRequestTypeDef

```python
# NetworkingRequestTypeDef definition

class NetworkingRequestTypeDef(TypedDict):
    subnetIds: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
```

## SchedulerRequestTypeDef

```python
# SchedulerRequestTypeDef definition

class SchedulerRequestTypeDef(TypedDict):
    type: SchedulerTypeType,  # (1)
    version: str,
```

1. See [:material-code-brackets: SchedulerTypeType](./literals.md#schedulertypetype) 
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

## ScalingConfigurationRequestTypeDef

```python
# ScalingConfigurationRequestTypeDef definition

class ScalingConfigurationRequestTypeDef(TypedDict):
    minInstanceCount: int,
    maxInstanceCount: int,
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    clientToken: NotRequired[str],
```

## DeleteComputeNodeGroupRequestRequestTypeDef

```python
# DeleteComputeNodeGroupRequestRequestTypeDef definition

class DeleteComputeNodeGroupRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
    clientToken: NotRequired[str],
```

## DeleteQueueRequestRequestTypeDef

```python
# DeleteQueueRequestRequestTypeDef definition

class DeleteQueueRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
    clientToken: NotRequired[str],
```

## GetClusterRequestRequestTypeDef

```python
# GetClusterRequestRequestTypeDef definition

class GetClusterRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
```

## GetComputeNodeGroupRequestRequestTypeDef

```python
# GetComputeNodeGroupRequestRequestTypeDef definition

class GetComputeNodeGroupRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
```

## GetQueueRequestRequestTypeDef

```python
# GetQueueRequestRequestTypeDef definition

class GetQueueRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListClustersRequestRequestTypeDef

```python
# ListClustersRequestRequestTypeDef definition

class ListClustersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListComputeNodeGroupsRequestRequestTypeDef

```python
# ListComputeNodeGroupsRequestRequestTypeDef definition

class ListComputeNodeGroupsRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListQueuesRequestRequestTypeDef

```python
# ListQueuesRequestRequestTypeDef definition

class ListQueuesRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueSummaryTypeDef

```python
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
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterComputeNodeGroupInstanceRequestRequestTypeDef

```python
# RegisterComputeNodeGroupInstanceRequestRequestTypeDef definition

class RegisterComputeNodeGroupInstanceRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    bootstrapId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## ClusterSlurmConfigurationRequestTypeDef

```python
# ClusterSlurmConfigurationRequestTypeDef definition

class ClusterSlurmConfigurationRequestTypeDef(TypedDict):
    scaleDownIdleTimeInSeconds: NotRequired[int],
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ComputeNodeGroupSlurmConfigurationRequestTypeDef

```python
# ComputeNodeGroupSlurmConfigurationRequestTypeDef definition

class ComputeNodeGroupSlurmConfigurationRequestTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ComputeNodeGroupSlurmConfigurationTypeDef

```python
# ComputeNodeGroupSlurmConfigurationTypeDef definition

class ComputeNodeGroupSlurmConfigurationTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[List[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef

```python
# UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef definition

class UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef(TypedDict):
    slurmCustomSettings: NotRequired[Sequence[SlurmCustomSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
## ClusterSlurmConfigurationTypeDef

```python
# ClusterSlurmConfigurationTypeDef definition

class ClusterSlurmConfigurationTypeDef(TypedDict):
    scaleDownIdleTimeInSeconds: NotRequired[int],
    slurmCustomSettings: NotRequired[List[SlurmCustomSettingTypeDef]],  # (1)
    authKey: NotRequired[SlurmAuthKeyTypeDef],  # (2)
```

1. See [:material-code-braces: SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef) 
2. See [:material-code-braces: SlurmAuthKeyTypeDef](./type_defs.md#slurmauthkeytypedef) 
## CreateQueueRequestRequestTypeDef

```python
# CreateQueueRequestRequestTypeDef definition

class CreateQueueRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueName: str,
    computeNodeGroupConfigurations: NotRequired[Sequence[ComputeNodeGroupConfigurationTypeDef]],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
## QueueTypeDef

```python
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
## UpdateQueueRequestRequestTypeDef

```python
# UpdateQueueRequestRequestTypeDef definition

class UpdateQueueRequestRequestTypeDef(TypedDict):
    clusterIdentifier: str,
    queueIdentifier: str,
    computeNodeGroupConfigurations: NotRequired[Sequence[ComputeNodeGroupConfigurationTypeDef]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
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
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterComputeNodeGroupInstanceResponseTypeDef

```python
# RegisterComputeNodeGroupInstanceResponseTypeDef definition

class RegisterComputeNodeGroupInstanceResponseTypeDef(TypedDict):
    nodeID: str,
    sharedSecret: str,
    endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersRequestListClustersPaginateTypeDef

```python
# ListClustersRequestListClustersPaginateTypeDef definition

class ListClustersRequestListClustersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComputeNodeGroupsRequestListComputeNodeGroupsPaginateTypeDef

```python
# ListComputeNodeGroupsRequestListComputeNodeGroupsPaginateTypeDef definition

class ListComputeNodeGroupsRequestListComputeNodeGroupsPaginateTypeDef(TypedDict):
    clusterIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestListQueuesPaginateTypeDef

```python
# ListQueuesRequestListQueuesPaginateTypeDef definition

class ListQueuesRequestListQueuesPaginateTypeDef(TypedDict):
    clusterIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    queues: List[QueueSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
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
## CreateComputeNodeGroupRequestRequestTypeDef

```python
# CreateComputeNodeGroupRequestRequestTypeDef definition

class CreateComputeNodeGroupRequestRequestTypeDef(TypedDict):
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
## UpdateComputeNodeGroupRequestRequestTypeDef

```python
# UpdateComputeNodeGroupRequestRequestTypeDef definition

class UpdateComputeNodeGroupRequestRequestTypeDef(TypedDict):
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
# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueResponseTypeDef

```python
# GetQueueResponseTypeDef definition

class GetQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQueueResponseTypeDef

```python
# UpdateQueueResponseTypeDef definition

class UpdateQueueResponseTypeDef(TypedDict):
    queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComputeNodeGroupResponseTypeDef

```python
# CreateComputeNodeGroupResponseTypeDef definition

class CreateComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComputeNodeGroupResponseTypeDef

```python
# GetComputeNodeGroupResponseTypeDef definition

class GetComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComputeNodeGroupResponseTypeDef

```python
# UpdateComputeNodeGroupResponseTypeDef definition

class UpdateComputeNodeGroupResponseTypeDef(TypedDict):
    computeNodeGroup: ComputeNodeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClusterResponseTypeDef

```python
# GetClusterResponseTypeDef definition

class GetClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
