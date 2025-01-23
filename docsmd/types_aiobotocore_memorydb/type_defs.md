# Type definitions

> [Index](../README.md) > [MemoryDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#memorydb)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ACLPendingChangesTypeDef

```python
# ACLPendingChangesTypeDef definition

class ACLPendingChangesTypeDef(TypedDict):
    UserNamesToRemove: NotRequired[List[str]],
    UserNamesToAdd: NotRequired[List[str]],
```

## ACLsUpdateStatusTypeDef

```python
# ACLsUpdateStatusTypeDef definition

class ACLsUpdateStatusTypeDef(TypedDict):
    ACLToApply: NotRequired[str],
```

## AuthenticationModeTypeDef

```python
# AuthenticationModeTypeDef definition

class AuthenticationModeTypeDef(TypedDict):
    Type: NotRequired[InputAuthenticationTypeType],  # (1)
    Passwords: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: InputAuthenticationTypeType](./literals.md#inputauthenticationtypetype) 
## AuthenticationTypeDef

```python
# AuthenticationTypeDef definition

class AuthenticationTypeDef(TypedDict):
    Type: NotRequired[AuthenticationTypeType],  # (1)
    PasswordCount: NotRequired[int],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## ServiceUpdateRequestTypeDef

```python
# ServiceUpdateRequestTypeDef definition

class ServiceUpdateRequestTypeDef(TypedDict):
    ServiceUpdateNameToApply: NotRequired[str],
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

## UnprocessedClusterTypeDef

```python
# UnprocessedClusterTypeDef definition

class UnprocessedClusterTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    ErrorType: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## PendingModifiedServiceUpdateTypeDef

```python
# PendingModifiedServiceUpdateTypeDef definition

class PendingModifiedServiceUpdateTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    Status: NotRequired[ServiceUpdateStatusType],  # (1)
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
```

## SecurityGroupMembershipTypeDef

```python
# SecurityGroupMembershipTypeDef definition

class SecurityGroupMembershipTypeDef(TypedDict):
    SecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ParameterGroupTypeDef

```python
# ParameterGroupTypeDef definition

class ParameterGroupTypeDef(TypedDict):
    Name: NotRequired[str],
    Family: NotRequired[str],
    Description: NotRequired[str],
    ARN: NotRequired[str],
```

## DeleteACLRequestRequestTypeDef

```python
# DeleteACLRequestRequestTypeDef definition

class DeleteACLRequestRequestTypeDef(TypedDict):
    ACLName: str,
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    MultiRegionClusterName: NotRequired[str],
    FinalSnapshotName: NotRequired[str],
```

## DeleteMultiRegionClusterRequestRequestTypeDef

```python
# DeleteMultiRegionClusterRequestRequestTypeDef definition

class DeleteMultiRegionClusterRequestRequestTypeDef(TypedDict):
    MultiRegionClusterName: str,
```

## DeleteParameterGroupRequestRequestTypeDef

```python
# DeleteParameterGroupRequestRequestTypeDef definition

class DeleteParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
```

## DeleteSnapshotRequestRequestTypeDef

```python
# DeleteSnapshotRequestRequestTypeDef definition

class DeleteSnapshotRequestRequestTypeDef(TypedDict):
    SnapshotName: str,
```

## DeleteSubnetGroupRequestRequestTypeDef

```python
# DeleteSubnetGroupRequestRequestTypeDef definition

class DeleteSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    UserName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeACLsRequestRequestTypeDef

```python
# DescribeACLsRequestRequestTypeDef definition

class DescribeACLsRequestRequestTypeDef(TypedDict):
    ACLName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeClustersRequestRequestTypeDef

```python
# DescribeClustersRequestRequestTypeDef definition

class DescribeClustersRequestRequestTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ShowShardDetails: NotRequired[bool],
```

## DescribeEngineVersionsRequestRequestTypeDef

```python
# DescribeEngineVersionsRequestRequestTypeDef definition

class DescribeEngineVersionsRequestRequestTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    ParameterGroupFamily: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    DefaultOnly: NotRequired[bool],
```

## EngineVersionInfoTypeDef

```python
# EngineVersionInfoTypeDef definition

class EngineVersionInfoTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    EnginePatchVersion: NotRequired[str],
    ParameterGroupFamily: NotRequired[str],
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
## DescribeMultiRegionClustersRequestRequestTypeDef

```python
# DescribeMultiRegionClustersRequestRequestTypeDef definition

class DescribeMultiRegionClustersRequestRequestTypeDef(TypedDict):
    MultiRegionClusterName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ShowClusterDetails: NotRequired[bool],
```

## DescribeParameterGroupsRequestRequestTypeDef

```python
# DescribeParameterGroupsRequestRequestTypeDef definition

class DescribeParameterGroupsRequestRequestTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeParametersRequestRequestTypeDef

```python
# DescribeParametersRequestRequestTypeDef definition

class DescribeParametersRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    Description: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    MinimumEngineVersion: NotRequired[str],
```

## DescribeReservedNodesOfferingsRequestRequestTypeDef

```python
# DescribeReservedNodesOfferingsRequestRequestTypeDef definition

class DescribeReservedNodesOfferingsRequestRequestTypeDef(TypedDict):
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[str],
    OfferingType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeReservedNodesRequestRequestTypeDef

```python
# DescribeReservedNodesRequestRequestTypeDef definition

class DescribeReservedNodesRequestRequestTypeDef(TypedDict):
    ReservationId: NotRequired[str],
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[str],
    OfferingType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeServiceUpdatesRequestRequestTypeDef

```python
# DescribeServiceUpdatesRequestRequestTypeDef definition

class DescribeServiceUpdatesRequestRequestTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ClusterNames: NotRequired[Sequence[str]],
    Status: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
## ServiceUpdateTypeDef

```python
# ServiceUpdateTypeDef definition

class ServiceUpdateTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    ServiceUpdateName: NotRequired[str],
    ReleaseDate: NotRequired[datetime],
    Description: NotRequired[str],
    Status: NotRequired[ServiceUpdateStatusType],  # (1)
    Type: NotRequired[ServiceUpdateTypeType],  # (2)
    Engine: NotRequired[str],
    NodesUpdated: NotRequired[str],
    AutoUpdateStartDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-brackets: ServiceUpdateTypeType](./literals.md#serviceupdatetypetype) 
## DescribeSnapshotsRequestRequestTypeDef

```python
# DescribeSnapshotsRequestRequestTypeDef definition

class DescribeSnapshotsRequestRequestTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    SnapshotName: NotRequired[str],
    Source: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ShowDetail: NotRequired[bool],
```

## DescribeSubnetGroupsRequestRequestTypeDef

```python
# DescribeSubnetGroupsRequestRequestTypeDef definition

class DescribeSubnetGroupsRequestRequestTypeDef(TypedDict):
    SubnetGroupName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## FailoverShardRequestRequestTypeDef

```python
# FailoverShardRequestRequestTypeDef definition

class FailoverShardRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    ShardName: str,
```

## ListAllowedMultiRegionClusterUpdatesRequestRequestTypeDef

```python
# ListAllowedMultiRegionClusterUpdatesRequestRequestTypeDef definition

class ListAllowedMultiRegionClusterUpdatesRequestRequestTypeDef(TypedDict):
    MultiRegionClusterName: str,
```

## ListAllowedNodeTypeUpdatesRequestRequestTypeDef

```python
# ListAllowedNodeTypeUpdatesRequestRequestTypeDef definition

class ListAllowedNodeTypeUpdatesRequestRequestTypeDef(TypedDict):
    ClusterName: str,
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RegionalClusterTypeDef

```python
# RegionalClusterTypeDef definition

class RegionalClusterTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    Region: NotRequired[str],
    Status: NotRequired[str],
    ARN: NotRequired[str],
```

## ParameterNameValueTypeDef

```python
# ParameterNameValueTypeDef definition

class ParameterNameValueTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
```

## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    RecurringChargeAmount: NotRequired[float],
    RecurringChargeFrequency: NotRequired[str],
```

## ReplicaConfigurationRequestTypeDef

```python
# ReplicaConfigurationRequestTypeDef definition

class ReplicaConfigurationRequestTypeDef(TypedDict):
    ReplicaCount: NotRequired[int],
```

## ResetParameterGroupRequestRequestTypeDef

```python
# ResetParameterGroupRequestRequestTypeDef definition

class ResetParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    AllParameters: NotRequired[bool],
    ParameterNames: NotRequired[Sequence[str]],
```

## SlotMigrationTypeDef

```python
# SlotMigrationTypeDef definition

class SlotMigrationTypeDef(TypedDict):
    ProgressPercentage: NotRequired[float],
```

## ShardConfigurationRequestTypeDef

```python
# ShardConfigurationRequestTypeDef definition

class ShardConfigurationRequestTypeDef(TypedDict):
    ShardCount: NotRequired[int],
```

## ShardConfigurationTypeDef

```python
# ShardConfigurationTypeDef definition

class ShardConfigurationTypeDef(TypedDict):
    Slots: NotRequired[str],
    ReplicaCount: NotRequired[int],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateACLRequestRequestTypeDef

```python
# UpdateACLRequestRequestTypeDef definition

class UpdateACLRequestRequestTypeDef(TypedDict):
    ACLName: str,
    UserNamesToAdd: NotRequired[Sequence[str]],
    UserNamesToRemove: NotRequired[Sequence[str]],
```

## UpdateSubnetGroupRequestRequestTypeDef

```python
# UpdateSubnetGroupRequestRequestTypeDef definition

class UpdateSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
    Description: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
```

## ACLTypeDef

```python
# ACLTypeDef definition

class ACLTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    UserNames: NotRequired[List[str]],
    MinimumEngineVersion: NotRequired[str],
    PendingChanges: NotRequired[ACLPendingChangesTypeDef],  # (1)
    Clusters: NotRequired[List[str]],
    ARN: NotRequired[str],
```

1. See [:material-code-braces: ACLPendingChangesTypeDef](./type_defs.md#aclpendingchangestypedef) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationMode: NotRequired[AuthenticationModeTypeDef],  # (1)
    AccessString: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    AccessString: NotRequired[str],
    ACLNames: NotRequired[List[str]],
    MinimumEngineVersion: NotRequired[str],
    Authentication: NotRequired[AuthenticationTypeDef],  # (1)
    ARN: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationTypeDef](./type_defs.md#authenticationtypedef) 
## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    Identifier: NotRequired[str],
    AvailabilityZone: NotRequired[AvailabilityZoneTypeDef],  # (1)
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
## BatchUpdateClusterRequestRequestTypeDef

```python
# BatchUpdateClusterRequestRequestTypeDef definition

class BatchUpdateClusterRequestRequestTypeDef(TypedDict):
    ClusterNames: Sequence[str],
    ServiceUpdate: NotRequired[ServiceUpdateRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ServiceUpdateRequestTypeDef](./type_defs.md#serviceupdaterequesttypedef) 
## ListAllowedMultiRegionClusterUpdatesResponseTypeDef

```python
# ListAllowedMultiRegionClusterUpdatesResponseTypeDef definition

class ListAllowedMultiRegionClusterUpdatesResponseTypeDef(TypedDict):
    ScaleUpNodeTypes: List[str],
    ScaleDownNodeTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAllowedNodeTypeUpdatesResponseTypeDef

```python
# ListAllowedNodeTypeUpdatesResponseTypeDef definition

class ListAllowedNodeTypeUpdatesResponseTypeDef(TypedDict):
    ScaleUpNodeTypes: List[str],
    ScaleDownNodeTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    CreateTime: NotRequired[datetime],
    Endpoint: NotRequired[EndpointTypeDef],  # (1)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## CopySnapshotRequestRequestTypeDef

```python
# CopySnapshotRequestRequestTypeDef definition

class CopySnapshotRequestRequestTypeDef(TypedDict):
    SourceSnapshotName: str,
    TargetSnapshotName: str,
    TargetBucket: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateACLRequestRequestTypeDef

```python
# CreateACLRequestRequestTypeDef definition

class CreateACLRequestRequestTypeDef(TypedDict):
    ACLName: str,
    UserNames: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    NodeType: str,
    ACLName: str,
    MultiRegionClusterName: NotRequired[str],
    ParameterGroupName: NotRequired[str],
    Description: NotRequired[str],
    NumShards: NotRequired[int],
    NumReplicasPerShard: NotRequired[int],
    SubnetGroupName: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    MaintenanceWindow: NotRequired[str],
    Port: NotRequired[int],
    SnsTopicArn: NotRequired[str],
    TLSEnabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    SnapshotArns: NotRequired[Sequence[str]],
    SnapshotName: NotRequired[str],
    SnapshotRetentionLimit: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    SnapshotWindow: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    DataTiering: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMultiRegionClusterRequestRequestTypeDef

```python
# CreateMultiRegionClusterRequestRequestTypeDef definition

class CreateMultiRegionClusterRequestRequestTypeDef(TypedDict):
    MultiRegionClusterNameSuffix: str,
    NodeType: str,
    Description: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    MultiRegionParameterGroupName: NotRequired[str],
    NumShards: NotRequired[int],
    TLSEnabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateParameterGroupRequestRequestTypeDef

```python
# CreateParameterGroupRequestRequestTypeDef definition

class CreateParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    Family: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotRequestRequestTypeDef

```python
# CreateSnapshotRequestRequestTypeDef definition

class CreateSnapshotRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    SnapshotName: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSubnetGroupRequestRequestTypeDef

```python
# CreateSubnetGroupRequestRequestTypeDef definition

class CreateSubnetGroupRequestRequestTypeDef(TypedDict):
    SubnetGroupName: str,
    SubnetIds: Sequence[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationMode: AuthenticationModeTypeDef,  # (1)
    AccessString: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseReservedNodesOfferingRequestRequestTypeDef

```python
# PurchaseReservedNodesOfferingRequestRequestTypeDef definition

class PurchaseReservedNodesOfferingRequestRequestTypeDef(TypedDict):
    ReservedNodesOfferingId: str,
    ReservationId: NotRequired[str],
    NodeCount: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceResponseTypeDef

```python
# TagResourceResponseTypeDef definition

class TagResourceResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceResponseTypeDef

```python
# UntagResourceResponseTypeDef definition

class UntagResourceResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
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
## DeleteParameterGroupResponseTypeDef

```python
# DeleteParameterGroupResponseTypeDef definition

class DeleteParameterGroupResponseTypeDef(TypedDict):
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
## ResetParameterGroupResponseTypeDef

```python
# ResetParameterGroupResponseTypeDef definition

class ResetParameterGroupResponseTypeDef(TypedDict):
    ParameterGroup: ParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## DescribeACLsRequestPaginateTypeDef

```python
# DescribeACLsRequestPaginateTypeDef definition

class DescribeACLsRequestPaginateTypeDef(TypedDict):
    ACLName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClustersRequestPaginateTypeDef

```python
# DescribeClustersRequestPaginateTypeDef definition

class DescribeClustersRequestPaginateTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    ShowShardDetails: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineVersionsRequestPaginateTypeDef

```python
# DescribeEngineVersionsRequestPaginateTypeDef definition

class DescribeEngineVersionsRequestPaginateTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    ParameterGroupFamily: NotRequired[str],
    DefaultOnly: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMultiRegionClustersRequestPaginateTypeDef

```python
# DescribeMultiRegionClustersRequestPaginateTypeDef definition

class DescribeMultiRegionClustersRequestPaginateTypeDef(TypedDict):
    MultiRegionClusterName: NotRequired[str],
    ShowClusterDetails: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParameterGroupsRequestPaginateTypeDef

```python
# DescribeParameterGroupsRequestPaginateTypeDef definition

class DescribeParameterGroupsRequestPaginateTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeParametersRequestPaginateTypeDef

```python
# DescribeParametersRequestPaginateTypeDef definition

class DescribeParametersRequestPaginateTypeDef(TypedDict):
    ParameterGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedNodesOfferingsRequestPaginateTypeDef

```python
# DescribeReservedNodesOfferingsRequestPaginateTypeDef definition

class DescribeReservedNodesOfferingsRequestPaginateTypeDef(TypedDict):
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[str],
    OfferingType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedNodesRequestPaginateTypeDef

```python
# DescribeReservedNodesRequestPaginateTypeDef definition

class DescribeReservedNodesRequestPaginateTypeDef(TypedDict):
    ReservationId: NotRequired[str],
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[str],
    OfferingType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServiceUpdatesRequestPaginateTypeDef

```python
# DescribeServiceUpdatesRequestPaginateTypeDef definition

class DescribeServiceUpdatesRequestPaginateTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ClusterNames: NotRequired[Sequence[str]],
    Status: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSnapshotsRequestPaginateTypeDef

```python
# DescribeSnapshotsRequestPaginateTypeDef definition

class DescribeSnapshotsRequestPaginateTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    SnapshotName: NotRequired[str],
    Source: NotRequired[str],
    ShowDetail: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSubnetGroupsRequestPaginateTypeDef

```python
# DescribeSubnetGroupsRequestPaginateTypeDef definition

class DescribeSubnetGroupsRequestPaginateTypeDef(TypedDict):
    SubnetGroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineVersionsResponseTypeDef

```python
# DescribeEngineVersionsResponseTypeDef definition

class DescribeEngineVersionsResponseTypeDef(TypedDict):
    EngineVersions: List[EngineVersionInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngineVersionInfoTypeDef](./type_defs.md#engineversioninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## DescribeServiceUpdatesResponseTypeDef

```python
# DescribeServiceUpdatesResponseTypeDef definition

class DescribeServiceUpdatesResponseTypeDef(TypedDict):
    ServiceUpdates: List[ServiceUpdateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceUpdateTypeDef](./type_defs.md#serviceupdatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUsersRequestPaginateTypeDef

```python
# DescribeUsersRequestPaginateTypeDef definition

class DescribeUsersRequestPaginateTypeDef(TypedDict):
    UserName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUsersRequestRequestTypeDef

```python
# DescribeUsersRequestRequestTypeDef definition

class DescribeUsersRequestRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## MultiRegionClusterTypeDef

```python
# MultiRegionClusterTypeDef definition

class MultiRegionClusterTypeDef(TypedDict):
    MultiRegionClusterName: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[str],
    NodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    NumberOfShards: NotRequired[int],
    Clusters: NotRequired[List[RegionalClusterTypeDef]],  # (1)
    MultiRegionParameterGroupName: NotRequired[str],
    TLSEnabled: NotRequired[bool],
    ARN: NotRequired[str],
```

1. See [:material-code-braces: RegionalClusterTypeDef](./type_defs.md#regionalclustertypedef) 
## UpdateParameterGroupRequestRequestTypeDef

```python
# UpdateParameterGroupRequestRequestTypeDef definition

class UpdateParameterGroupRequestRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    ParameterNameValues: Sequence[ParameterNameValueTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef) 
## ReservedNodeTypeDef

```python
# ReservedNodeTypeDef definition

class ReservedNodeTypeDef(TypedDict):
    ReservationId: NotRequired[str],
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    NodeCount: NotRequired[int],
    OfferingType: NotRequired[str],
    State: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
    ARN: NotRequired[str],
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReservedNodesOfferingTypeDef

```python
# ReservedNodesOfferingTypeDef definition

class ReservedNodesOfferingTypeDef(TypedDict):
    ReservedNodesOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    OfferingType: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReshardingStatusTypeDef

```python
# ReshardingStatusTypeDef definition

class ReshardingStatusTypeDef(TypedDict):
    SlotMigration: NotRequired[SlotMigrationTypeDef],  # (1)
```

1. See [:material-code-braces: SlotMigrationTypeDef](./type_defs.md#slotmigrationtypedef) 
## UpdateClusterRequestRequestTypeDef

```python
# UpdateClusterRequestRequestTypeDef definition

class UpdateClusterRequestRequestTypeDef(TypedDict):
    ClusterName: str,
    Description: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    MaintenanceWindow: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SnsTopicStatus: NotRequired[str],
    ParameterGroupName: NotRequired[str],
    SnapshotWindow: NotRequired[str],
    SnapshotRetentionLimit: NotRequired[int],
    NodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    ReplicaConfiguration: NotRequired[ReplicaConfigurationRequestTypeDef],  # (1)
    ShardConfiguration: NotRequired[ShardConfigurationRequestTypeDef],  # (2)
    ACLName: NotRequired[str],
```

1. See [:material-code-braces: ReplicaConfigurationRequestTypeDef](./type_defs.md#replicaconfigurationrequesttypedef) 
2. See [:material-code-braces: ShardConfigurationRequestTypeDef](./type_defs.md#shardconfigurationrequesttypedef) 
## UpdateMultiRegionClusterRequestRequestTypeDef

```python
# UpdateMultiRegionClusterRequestRequestTypeDef definition

class UpdateMultiRegionClusterRequestRequestTypeDef(TypedDict):
    MultiRegionClusterName: str,
    NodeType: NotRequired[str],
    Description: NotRequired[str],
    EngineVersion: NotRequired[str],
    ShardConfiguration: NotRequired[ShardConfigurationRequestTypeDef],  # (1)
    MultiRegionParameterGroupName: NotRequired[str],
    UpdateStrategy: NotRequired[UpdateStrategyType],  # (2)
```

1. See [:material-code-braces: ShardConfigurationRequestTypeDef](./type_defs.md#shardconfigurationrequesttypedef) 
2. See [:material-code-brackets: UpdateStrategyType](./literals.md#updatestrategytype) 
## ShardDetailTypeDef

```python
# ShardDetailTypeDef definition

class ShardDetailTypeDef(TypedDict):
    Name: NotRequired[str],
    Configuration: NotRequired[ShardConfigurationTypeDef],  # (1)
    Size: NotRequired[str],
    SnapshotCreationTime: NotRequired[datetime],
```

1. See [:material-code-braces: ShardConfigurationTypeDef](./type_defs.md#shardconfigurationtypedef) 
## CreateACLResponseTypeDef

```python
# CreateACLResponseTypeDef definition

class CreateACLResponseTypeDef(TypedDict):
    ACL: ACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ACLTypeDef](./type_defs.md#acltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteACLResponseTypeDef

```python
# DeleteACLResponseTypeDef definition

class DeleteACLResponseTypeDef(TypedDict):
    ACL: ACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ACLTypeDef](./type_defs.md#acltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeACLsResponseTypeDef

```python
# DescribeACLsResponseTypeDef definition

class DescribeACLsResponseTypeDef(TypedDict):
    ACLs: List[ACLTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ACLTypeDef](./type_defs.md#acltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateACLResponseTypeDef

```python
# UpdateACLResponseTypeDef definition

class UpdateACLResponseTypeDef(TypedDict):
    ACL: ACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ACLTypeDef](./type_defs.md#acltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteUserResponseTypeDef

```python
# DeleteUserResponseTypeDef definition

class DeleteUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUsersResponseTypeDef

```python
# DescribeUsersResponseTypeDef definition

class DescribeUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubnetGroupTypeDef

```python
# SubnetGroupTypeDef definition

class SubnetGroupTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    VpcId: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
    ARN: NotRequired[str],
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
## ShardTypeDef

```python
# ShardTypeDef definition

class ShardTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    Slots: NotRequired[str],
    Nodes: NotRequired[List[NodeTypeDef]],  # (1)
    NumberOfNodes: NotRequired[int],
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
## CreateMultiRegionClusterResponseTypeDef

```python
# CreateMultiRegionClusterResponseTypeDef definition

class CreateMultiRegionClusterResponseTypeDef(TypedDict):
    MultiRegionCluster: MultiRegionClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiRegionClusterTypeDef](./type_defs.md#multiregionclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMultiRegionClusterResponseTypeDef

```python
# DeleteMultiRegionClusterResponseTypeDef definition

class DeleteMultiRegionClusterResponseTypeDef(TypedDict):
    MultiRegionCluster: MultiRegionClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiRegionClusterTypeDef](./type_defs.md#multiregionclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMultiRegionClustersResponseTypeDef

```python
# DescribeMultiRegionClustersResponseTypeDef definition

class DescribeMultiRegionClustersResponseTypeDef(TypedDict):
    MultiRegionClusters: List[MultiRegionClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MultiRegionClusterTypeDef](./type_defs.md#multiregionclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMultiRegionClusterResponseTypeDef

```python
# UpdateMultiRegionClusterResponseTypeDef definition

class UpdateMultiRegionClusterResponseTypeDef(TypedDict):
    MultiRegionCluster: MultiRegionClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiRegionClusterTypeDef](./type_defs.md#multiregionclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservedNodesResponseTypeDef

```python
# DescribeReservedNodesResponseTypeDef definition

class DescribeReservedNodesResponseTypeDef(TypedDict):
    ReservedNodes: List[ReservedNodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseReservedNodesOfferingResponseTypeDef

```python
# PurchaseReservedNodesOfferingResponseTypeDef definition

class PurchaseReservedNodesOfferingResponseTypeDef(TypedDict):
    ReservedNode: ReservedNodeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservedNodesOfferingsResponseTypeDef

```python
# DescribeReservedNodesOfferingsResponseTypeDef definition

class DescribeReservedNodesOfferingsResponseTypeDef(TypedDict):
    ReservedNodesOfferings: List[ReservedNodesOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReservedNodesOfferingTypeDef](./type_defs.md#reservednodesofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterPendingUpdatesTypeDef

```python
# ClusterPendingUpdatesTypeDef definition

class ClusterPendingUpdatesTypeDef(TypedDict):
    Resharding: NotRequired[ReshardingStatusTypeDef],  # (1)
    ACLs: NotRequired[ACLsUpdateStatusTypeDef],  # (2)
    ServiceUpdates: NotRequired[List[PendingModifiedServiceUpdateTypeDef]],  # (3)
```

1. See [:material-code-braces: ReshardingStatusTypeDef](./type_defs.md#reshardingstatustypedef) 
2. See [:material-code-braces: ACLsUpdateStatusTypeDef](./type_defs.md#aclsupdatestatustypedef) 
3. See [:material-code-braces: PendingModifiedServiceUpdateTypeDef](./type_defs.md#pendingmodifiedserviceupdatetypedef) 
## ClusterConfigurationTypeDef

```python
# ClusterConfigurationTypeDef definition

class ClusterConfigurationTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    NodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    MaintenanceWindow: NotRequired[str],
    TopicArn: NotRequired[str],
    Port: NotRequired[int],
    ParameterGroupName: NotRequired[str],
    SubnetGroupName: NotRequired[str],
    VpcId: NotRequired[str],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    NumShards: NotRequired[int],
    Shards: NotRequired[List[ShardDetailTypeDef]],  # (1)
    MultiRegionParameterGroupName: NotRequired[str],
    MultiRegionClusterName: NotRequired[str],
```

1. See [:material-code-braces: ShardDetailTypeDef](./type_defs.md#sharddetailtypedef) 
## CreateSubnetGroupResponseTypeDef

```python
# CreateSubnetGroupResponseTypeDef definition

class CreateSubnetGroupResponseTypeDef(TypedDict):
    SubnetGroup: SubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubnetGroupTypeDef](./type_defs.md#subnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSubnetGroupResponseTypeDef

```python
# DeleteSubnetGroupResponseTypeDef definition

class DeleteSubnetGroupResponseTypeDef(TypedDict):
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
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[str],
    PendingUpdates: NotRequired[ClusterPendingUpdatesTypeDef],  # (1)
    MultiRegionClusterName: NotRequired[str],
    NumberOfShards: NotRequired[int],
    Shards: NotRequired[List[ShardTypeDef]],  # (2)
    AvailabilityMode: NotRequired[AZStatusType],  # (3)
    ClusterEndpoint: NotRequired[EndpointTypeDef],  # (4)
    NodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    EnginePatchVersion: NotRequired[str],
    ParameterGroupName: NotRequired[str],
    ParameterGroupStatus: NotRequired[str],
    SecurityGroups: NotRequired[List[SecurityGroupMembershipTypeDef]],  # (5)
    SubnetGroupName: NotRequired[str],
    TLSEnabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    ARN: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SnsTopicStatus: NotRequired[str],
    SnapshotRetentionLimit: NotRequired[int],
    MaintenanceWindow: NotRequired[str],
    SnapshotWindow: NotRequired[str],
    ACLName: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    DataTiering: NotRequired[DataTieringStatusType],  # (6)
```

1. See [:material-code-braces: ClusterPendingUpdatesTypeDef](./type_defs.md#clusterpendingupdatestypedef) 
2. See [:material-code-braces: ShardTypeDef](./type_defs.md#shardtypedef) 
3. See [:material-code-brackets: AZStatusType](./literals.md#azstatustype) 
4. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
5. See [:material-code-braces: SecurityGroupMembershipTypeDef](./type_defs.md#securitygroupmembershiptypedef) 
6. See [:material-code-brackets: DataTieringStatusType](./literals.md#datatieringstatustype) 
## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    Source: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ARN: NotRequired[str],
    ClusterConfiguration: NotRequired[ClusterConfigurationTypeDef],  # (1)
    DataTiering: NotRequired[DataTieringStatusType],  # (2)
```

1. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
2. See [:material-code-brackets: DataTieringStatusType](./literals.md#datatieringstatustype) 
## BatchUpdateClusterResponseTypeDef

```python
# BatchUpdateClusterResponseTypeDef definition

class BatchUpdateClusterResponseTypeDef(TypedDict):
    ProcessedClusters: List[ClusterTypeDef],  # (1)
    UnprocessedClusters: List[UnprocessedClusterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: UnprocessedClusterTypeDef](./type_defs.md#unprocessedclustertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
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
## FailoverShardResponseTypeDef

```python
# FailoverShardResponseTypeDef definition

class FailoverShardResponseTypeDef(TypedDict):
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
## CopySnapshotResponseTypeDef

```python
# CopySnapshotResponseTypeDef definition

class CopySnapshotResponseTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSnapshotResponseTypeDef

```python
# CreateSnapshotResponseTypeDef definition

class CreateSnapshotResponseTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSnapshotResponseTypeDef

```python
# DeleteSnapshotResponseTypeDef definition

class DeleteSnapshotResponseTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSnapshotsResponseTypeDef

```python
# DescribeSnapshotsResponseTypeDef definition

class DescribeSnapshotsResponseTypeDef(TypedDict):
    Snapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
