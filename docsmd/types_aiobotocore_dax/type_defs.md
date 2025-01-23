# Type definitions

> [Index](../README.md) > [DAX](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#dax)
    type annotations stubs module [types-aiobotocore-dax](https://pypi.org/project/types-aiobotocore-dax/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
    URL: NotRequired[str],
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    TopicArn: NotRequired[str],
    TopicStatus: NotRequired[str],
```

## ParameterGroupStatusTypeDef

```python
# ParameterGroupStatusTypeDef definition

class ParameterGroupStatusTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
    NodeIdsToReboot: NotRequired[List[str]],
```

## SSEDescriptionTypeDef

```python
# SSEDescriptionTypeDef definition

class SSEDescriptionTypeDef(TypedDict):
    Status: NotRequired[SSEStatusType],  # (1)
```

1. See [:material-code-brackets: SSEStatusType](./literals.md#ssestatustype) 
## SecurityGroupMembershipTypeDef

```python
# SecurityGroupMembershipTypeDef definition

class SecurityGroupMembershipTypeDef(TypedDict):
    SecurityGroupIdentifier: NotRequired[str],
    Status: NotRequired[str],
```

## SSESpecificationTypeDef

```python
# SSESpecificationTypeDef definition

class SSESpecificationTypeDef(TypedDict):
    Enabled: bool,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
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

## CreateParameterGroupRequestRequestTypeDef

```python
# CreateParameterGroupRequestRequestTypeDef definition

class CreateParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    Description: NotRequired[str],
```

## ParameterGroupTypeDef

```python
# ParameterGroupTypeDef definition

class ParameterGroupTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    Description: NotRequired[str],
```

## CreateSubnetGroupRequestRequestTypeDef

```python
# CreateSubnetGroupRequestRequestTypeDef definition

class CreateSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
    SubnetIds: Sequence[str],
    Description: NotRequired[str],
```

## DecreaseReplicationFactorRequestRequestTypeDef

```python
# DecreaseReplicationFactorRequestRequestTypeDef definition

class DecreaseReplicationFactorRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    NewReplicationFactor: int,
    AvailabilityZones: NotRequired[Sequence[str]],
    NodeIdsToRemove: NotRequired[Sequence[str]],
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
```

## DeleteParameterGroupRequestRequestTypeDef

```python
# DeleteParameterGroupRequestRequestTypeDef definition

class DeleteParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
```

## DeleteSubnetGroupRequestRequestTypeDef

```python
# DeleteSubnetGroupRequestRequestTypeDef definition

class DeleteSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeClustersRequestRequestTypeDef

```python
# DescribeClustersRequestRequestTypeDef definition

class DescribeClustersRequestRequestTypeDef(TypedDict):
    ClusterNames: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeDefaultParametersRequestRequestTypeDef

```python
# DescribeDefaultParametersRequestRequestTypeDef definition

class DescribeDefaultParametersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    SourceName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    Message: NotRequired[str],
    Date: NotRequired[datetime],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## DescribeParameterGroupsRequestRequestTypeDef

```python
# DescribeParameterGroupsRequestRequestTypeDef definition

class DescribeParameterGroupsRequestRequestTypeDef(TypedDict):
    ParameterGroupNames: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeParametersRequestRequestTypeDef

```python
# DescribeParametersRequestRequestTypeDef definition

class DescribeParametersRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    Source: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeSubnetGroupsRequestRequestTypeDef

```python
# DescribeSubnetGroupsRequestRequestTypeDef definition

class DescribeSubnetGroupsRequestRequestTypeDef(TypedDict):
    SubnetGroupNames: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## IncreaseReplicationFactorRequestRequestTypeDef

```python
# IncreaseReplicationFactorRequestRequestTypeDef definition

class IncreaseReplicationFactorRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    NewReplicationFactor: int,
    AvailabilityZones: NotRequired[Sequence[str]],
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceName: str,
    NextToken: NotRequired[str],
```

## NodeTypeSpecificValueTypeDef

```python
# NodeTypeSpecificValueTypeDef definition

class NodeTypeSpecificValueTypeDef(TypedDict):
    NodeType: NotRequired[str],
    Value: NotRequired[str],
```

## ParameterNameValueTypeDef

```python
# ParameterNameValueTypeDef definition

class ParameterNameValueTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
```

## RebootNodeRequestRequestTypeDef

```python
# RebootNodeRequestRequestTypeDef definition

class RebootNodeRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    NodeId: str,
```

## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceName: str,
    TagKeys: Sequence[str],
```

## UpdateClusterRequestRequestTypeDef

```python
# UpdateClusterRequestRequestTypeDef definition

class UpdateClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    Description: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    NotificationTopicArn: NotRequired[str],
    NotificationTopicStatus: NotRequired[str],
    ParameterGroupName: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## UpdateSubnetGroupRequestRequestTypeDef

```python
# UpdateSubnetGroupRequestRequestTypeDef definition

class UpdateSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
    Description: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
```

## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    NodeId: NotRequired[str],
    Endpoint: NotRequired[EndpointTypeDef],  # (1)
    NodeCreateTime: NotRequired[datetime],
    AvailabilityZone: NotRequired[str],
    NodeStatus: NotRequired[str],
    ParameterGroupStatus: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    NodeType: str,
    ReplicationFactor: int,
    IamRoleArn: str,
    Description: NotRequired[str],
    AvailabilityZones: NotRequired[Sequence[str]],
    SubnetGroupName: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    PreferredMaintenanceWindow: NotRequired[str],
    NotificationTopicArn: NotRequired[str],
    ParameterGroupName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (2)
    ClusterEndpointEncryptionType: NotRequired[ClusterEndpointEncryptionTypeType],  # (3)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
3. See [:material-code-brackets: ClusterEndpointEncryptionTypeType](./literals.md#clusterendpointencryptiontypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteParameterGroupResponseTypeDef

```python
# DeleteParameterGroupResponseTypeDef definition

class DeleteParameterGroupResponseTypeDef(TypedDict):
    DeletionMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSubnetGroupResponseTypeDef

```python
# DeleteSubnetGroupResponseTypeDef definition

class DeleteSubnetGroupResponseTypeDef(TypedDict):
    DeletionMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceResponseTypeDef

```python
# TagResourceResponseTypeDef definition

class TagResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceResponseTypeDef

```python
# UntagResourceResponseTypeDef definition

class UntagResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateParameterGroupResponseTypeDef

```python
# CreateParameterGroupResponseTypeDef definition

class CreateParameterGroupResponseTypeDef(TypedDict):
    ParameterGroup: ParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterGroupTypeDef](./type_defs.md#parametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeParameterGroupsResponseTypeDef

```python
# DescribeParameterGroupsResponseTypeDef definition

class DescribeParameterGroupsResponseTypeDef(TypedDict):
    ParameterGroups: List[ParameterGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterGroupTypeDef](./type_defs.md#parametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateParameterGroupResponseTypeDef

```python
# UpdateParameterGroupResponseTypeDef definition

class UpdateParameterGroupResponseTypeDef(TypedDict):
    ParameterGroup: ParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterGroupTypeDef](./type_defs.md#parametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClustersRequestPaginateTypeDef

```python
# DescribeClustersRequestPaginateTypeDef definition

class DescribeClustersRequestPaginateTypeDef(TypedDict):
    ClusterNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDefaultParametersRequestPaginateTypeDef

```python
# DescribeDefaultParametersRequestPaginateTypeDef definition

class DescribeDefaultParametersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParameterGroupsRequestPaginateTypeDef

```python
# DescribeParameterGroupsRequestPaginateTypeDef definition

class DescribeParameterGroupsRequestPaginateTypeDef(TypedDict):
    ParameterGroupNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParametersRequestPaginateTypeDef

```python
# DescribeParametersRequestPaginateTypeDef definition

class DescribeParametersRequestPaginateTypeDef(TypedDict):
    ParameterGroupName: str,
    Source: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSubnetGroupsRequestPaginateTypeDef

```python
# DescribeSubnetGroupsRequestPaginateTypeDef definition

class DescribeSubnetGroupsRequestPaginateTypeDef(TypedDict):
    SubnetGroupNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsRequestPaginateTypeDef

```python
# ListTagsRequestPaginateTypeDef definition

class ListTagsRequestPaginateTypeDef(TypedDict):
    ResourceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestPaginateTypeDef

```python
# DescribeEventsRequestPaginateTypeDef definition

class DescribeEventsRequestPaginateTypeDef(TypedDict):
    SourceName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestRequestTypeDef

```python
# DescribeEventsRequestRequestTypeDef definition

class DescribeEventsRequestRequestTypeDef(TypedDict):
    SourceName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## DescribeEventsResponseTypeDef

```python
# DescribeEventsResponseTypeDef definition

class DescribeEventsResponseTypeDef(TypedDict):
    Events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterType: NotRequired[ParameterTypeType],  # (1)
    ParameterValue: NotRequired[str],
    NodeTypeSpecificValues: NotRequired[List[NodeTypeSpecificValueTypeDef]],  # (2)
    Description: NotRequired[str],
    Source: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[IsModifiableType],  # (3)
    ChangeType: NotRequired[ChangeTypeType],  # (4)
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: NodeTypeSpecificValueTypeDef](./type_defs.md#nodetypespecificvaluetypedef) 
3. See [:material-code-brackets: IsModifiableType](./literals.md#ismodifiabletype) 
4. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## UpdateParameterGroupRequestRequestTypeDef

```python
# UpdateParameterGroupRequestRequestTypeDef definition

class UpdateParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    ParameterNameValues: Sequence[ParameterNameValueTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef) 
## SubnetGroupTypeDef

```python
# SubnetGroupTypeDef definition

class SubnetGroupTypeDef(TypedDict):
    SubnetGroupName: NotRequired[str],
    Description: NotRequired[str],
    VpcId: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    Description: NotRequired[str],
    ClusterArn: NotRequired[str],
    TotalNodes: NotRequired[int],
    ActiveNodes: NotRequired[int],
    NodeType: NotRequired[str],
    Status: NotRequired[str],
    ClusterDiscoveryEndpoint: NotRequired[EndpointTypeDef],  # (1)
    NodeIdsToRemove: NotRequired[List[str]],
    Nodes: NotRequired[List[NodeTypeDef]],  # (2)
    PreferredMaintenanceWindow: NotRequired[str],
    NotificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (3)
    SubnetGroup: NotRequired[str],
    SecurityGroups: NotRequired[List[SecurityGroupMembershipTypeDef]],  # (4)
    IamRoleArn: NotRequired[str],
    ParameterGroup: NotRequired[ParameterGroupStatusTypeDef],  # (5)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (6)
    ClusterEndpointEncryptionType: NotRequired[ClusterEndpointEncryptionTypeType],  # (7)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
3. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
4. See [:material-code-braces: SecurityGroupMembershipTypeDef](./type_defs.md#securitygroupmembershiptypedef) 
5. See [:material-code-braces: ParameterGroupStatusTypeDef](./type_defs.md#parametergroupstatustypedef) 
6. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
7. See [:material-code-brackets: ClusterEndpointEncryptionTypeType](./literals.md#clusterendpointencryptiontypetype) 
## DescribeDefaultParametersResponseTypeDef

```python
# DescribeDefaultParametersResponseTypeDef definition

class DescribeDefaultParametersResponseTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeParametersResponseTypeDef

```python
# DescribeParametersResponseTypeDef definition

class DescribeParametersResponseTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubnetGroupResponseTypeDef

```python
# CreateSubnetGroupResponseTypeDef definition

class CreateSubnetGroupResponseTypeDef(TypedDict):
    SubnetGroup: SubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubnetGroupTypeDef](./type_defs.md#subnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSubnetGroupsResponseTypeDef

```python
# DescribeSubnetGroupsResponseTypeDef definition

class DescribeSubnetGroupsResponseTypeDef(TypedDict):
    SubnetGroups: List[SubnetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubnetGroupTypeDef](./type_defs.md#subnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSubnetGroupResponseTypeDef

```python
# UpdateSubnetGroupResponseTypeDef definition

class UpdateSubnetGroupResponseTypeDef(TypedDict):
    SubnetGroup: SubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubnetGroupTypeDef](./type_defs.md#subnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecreaseReplicationFactorResponseTypeDef

```python
# DecreaseReplicationFactorResponseTypeDef definition

class DecreaseReplicationFactorResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClustersResponseTypeDef

```python
# DescribeClustersResponseTypeDef definition

class DescribeClustersResponseTypeDef(TypedDict):
    Clusters: List[ClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncreaseReplicationFactorResponseTypeDef

```python
# IncreaseReplicationFactorResponseTypeDef definition

class IncreaseReplicationFactorResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootNodeResponseTypeDef

```python
# RebootNodeResponseTypeDef definition

class RebootNodeResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterResponseTypeDef

```python
# UpdateClusterResponseTypeDef definition

class UpdateClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
