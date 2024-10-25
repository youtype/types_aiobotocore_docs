# Type definitions

> [Index](../README.md) > [Shield](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
    type annotations stubs module [types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ResponseActionOutputTypeDef

```python
# ResponseActionOutputTypeDef definition

class ResponseActionOutputTypeDef(TypedDict):
    Block: NotRequired[Dict[str, Any]],
    Count: NotRequired[Dict[str, Any]],
```

## AssociateDRTLogBucketRequestRequestTypeDef

```python
# AssociateDRTLogBucketRequestRequestTypeDef definition

class AssociateDRTLogBucketRequestRequestTypeDef(TypedDict):
    LogBucket: str,
```

## AssociateDRTRoleRequestRequestTypeDef

```python
# AssociateDRTRoleRequestRequestTypeDef definition

class AssociateDRTRoleRequestRequestTypeDef(TypedDict):
    RoleArn: str,
```

## AssociateHealthCheckRequestRequestTypeDef

```python
# AssociateHealthCheckRequestRequestTypeDef definition

class AssociateHealthCheckRequestRequestTypeDef(TypedDict):
    ProtectionId: str,
    HealthCheckArn: str,
```

## EmergencyContactTypeDef

```python
# EmergencyContactTypeDef definition

class EmergencyContactTypeDef(TypedDict):
    EmailAddress: str,
    PhoneNumber: NotRequired[str],
    ContactNotes: NotRequired[str],
```

## MitigationTypeDef

```python
# MitigationTypeDef definition

class MitigationTypeDef(TypedDict):
    MitigationName: NotRequired[str],
```

## SummarizedCounterTypeDef

```python
# SummarizedCounterTypeDef definition

class SummarizedCounterTypeDef(TypedDict):
    Name: NotRequired[str],
    Max: NotRequired[float],
    Average: NotRequired[float],
    Sum: NotRequired[float],
    N: NotRequired[int],
    Unit: NotRequired[str],
```

## ContributorTypeDef

```python
# ContributorTypeDef definition

class ContributorTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[int],
```

## AttackVectorDescriptionTypeDef

```python
# AttackVectorDescriptionTypeDef definition

class AttackVectorDescriptionTypeDef(TypedDict):
    VectorType: str,
```

## AttackVolumeStatisticsTypeDef

```python
# AttackVolumeStatisticsTypeDef definition

class AttackVolumeStatisticsTypeDef(TypedDict):
    Max: float,
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

## DeleteProtectionGroupRequestRequestTypeDef

```python
# DeleteProtectionGroupRequestRequestTypeDef definition

class DeleteProtectionGroupRequestRequestTypeDef(TypedDict):
    ProtectionGroupId: str,
```

## DeleteProtectionRequestRequestTypeDef

```python
# DeleteProtectionRequestRequestTypeDef definition

class DeleteProtectionRequestRequestTypeDef(TypedDict):
    ProtectionId: str,
```

## DescribeAttackRequestRequestTypeDef

```python
# DescribeAttackRequestRequestTypeDef definition

class DescribeAttackRequestRequestTypeDef(TypedDict):
    AttackId: str,
```

## TimeRangeOutputTypeDef

```python
# TimeRangeOutputTypeDef definition

class TimeRangeOutputTypeDef(TypedDict):
    FromInclusive: NotRequired[datetime],
    ToExclusive: NotRequired[datetime],
```

## DescribeProtectionGroupRequestRequestTypeDef

```python
# DescribeProtectionGroupRequestRequestTypeDef definition

class DescribeProtectionGroupRequestRequestTypeDef(TypedDict):
    ProtectionGroupId: str,
```

## ProtectionGroupTypeDef

```python
# ProtectionGroupTypeDef definition

class ProtectionGroupTypeDef(TypedDict):
    ProtectionGroupId: str,
    Aggregation: ProtectionGroupAggregationType,  # (1)
    Pattern: ProtectionGroupPatternType,  # (2)
    Members: List[str],
    ResourceType: NotRequired[ProtectedResourceTypeType],  # (3)
    ProtectionGroupArn: NotRequired[str],
```

1. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
2. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
3. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
## DescribeProtectionRequestRequestTypeDef

```python
# DescribeProtectionRequestRequestTypeDef definition

class DescribeProtectionRequestRequestTypeDef(TypedDict):
    ProtectionId: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## DisableApplicationLayerAutomaticResponseRequestRequestTypeDef

```python
# DisableApplicationLayerAutomaticResponseRequestRequestTypeDef definition

class DisableApplicationLayerAutomaticResponseRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DisassociateDRTLogBucketRequestRequestTypeDef

```python
# DisassociateDRTLogBucketRequestRequestTypeDef definition

class DisassociateDRTLogBucketRequestRequestTypeDef(TypedDict):
    LogBucket: str,
```

## DisassociateHealthCheckRequestRequestTypeDef

```python
# DisassociateHealthCheckRequestRequestTypeDef definition

class DisassociateHealthCheckRequestRequestTypeDef(TypedDict):
    ProtectionId: str,
    HealthCheckArn: str,
```

## ResponseActionTypeDef

```python
# ResponseActionTypeDef definition

class ResponseActionTypeDef(TypedDict):
    Block: NotRequired[Mapping[str, Any]],
    Count: NotRequired[Mapping[str, Any]],
```

## InclusionProtectionFiltersTypeDef

```python
# InclusionProtectionFiltersTypeDef definition

class InclusionProtectionFiltersTypeDef(TypedDict):
    ResourceArns: NotRequired[Sequence[str]],
    ProtectionNames: NotRequired[Sequence[str]],
    ResourceTypes: NotRequired[Sequence[ProtectedResourceTypeType]],  # (1)
```

1. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
## InclusionProtectionGroupFiltersTypeDef

```python
# InclusionProtectionGroupFiltersTypeDef definition

class InclusionProtectionGroupFiltersTypeDef(TypedDict):
    ProtectionGroupIds: NotRequired[Sequence[str]],
    Patterns: NotRequired[Sequence[ProtectionGroupPatternType]],  # (1)
    ResourceTypes: NotRequired[Sequence[ProtectedResourceTypeType]],  # (2)
    Aggregations: NotRequired[Sequence[ProtectionGroupAggregationType]],  # (3)
```

1. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
2. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
3. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
## LimitTypeDef

```python
# LimitTypeDef definition

class LimitTypeDef(TypedDict):
    Type: NotRequired[str],
    Max: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListResourcesInProtectionGroupRequestRequestTypeDef

```python
# ListResourcesInProtectionGroupRequestRequestTypeDef definition

class ListResourcesInProtectionGroupRequestRequestTypeDef(TypedDict):
    ProtectionGroupId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ProtectionGroupArbitraryPatternLimitsTypeDef

```python
# ProtectionGroupArbitraryPatternLimitsTypeDef definition

class ProtectionGroupArbitraryPatternLimitsTypeDef(TypedDict):
    MaxMembers: int,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateProtectionGroupRequestRequestTypeDef

```python
# UpdateProtectionGroupRequestRequestTypeDef definition

class UpdateProtectionGroupRequestRequestTypeDef(TypedDict):
    ProtectionGroupId: str,
    Aggregation: ProtectionGroupAggregationType,  # (1)
    Pattern: ProtectionGroupPatternType,  # (2)
    ResourceType: NotRequired[ProtectedResourceTypeType],  # (3)
    Members: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
2. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
3. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
## UpdateSubscriptionRequestRequestTypeDef

```python
# UpdateSubscriptionRequestRequestTypeDef definition

class UpdateSubscriptionRequestRequestTypeDef(TypedDict):
    AutoRenew: NotRequired[AutoRenewType],  # (1)
```

1. See [:material-code-brackets: AutoRenewType](./literals.md#autorenewtype) 
## ApplicationLayerAutomaticResponseConfigurationTypeDef

```python
# ApplicationLayerAutomaticResponseConfigurationTypeDef definition

class ApplicationLayerAutomaticResponseConfigurationTypeDef(TypedDict):
    Status: ApplicationLayerAutomaticResponseStatusType,  # (1)
    Action: ResponseActionOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: ApplicationLayerAutomaticResponseStatusType](./literals.md#applicationlayerautomaticresponsestatustype) 
2. See [:material-code-braces: ResponseActionOutputTypeDef](./type_defs.md#responseactionoutputtypedef) 
## AssociateProactiveEngagementDetailsRequestRequestTypeDef

```python
# AssociateProactiveEngagementDetailsRequestRequestTypeDef definition

class AssociateProactiveEngagementDetailsRequestRequestTypeDef(TypedDict):
    EmergencyContactList: Sequence[EmergencyContactTypeDef],  # (1)
```

1. See [:material-code-braces: EmergencyContactTypeDef](./type_defs.md#emergencycontacttypedef) 
## UpdateEmergencyContactSettingsRequestRequestTypeDef

```python
# UpdateEmergencyContactSettingsRequestRequestTypeDef definition

class UpdateEmergencyContactSettingsRequestRequestTypeDef(TypedDict):
    EmergencyContactList: NotRequired[Sequence[EmergencyContactTypeDef]],  # (1)
```

1. See [:material-code-braces: EmergencyContactTypeDef](./type_defs.md#emergencycontacttypedef) 
## SummarizedAttackVectorTypeDef

```python
# SummarizedAttackVectorTypeDef definition

class SummarizedAttackVectorTypeDef(TypedDict):
    VectorType: str,
    VectorCounters: NotRequired[List[SummarizedCounterTypeDef]],  # (1)
```

1. See [:material-code-braces: SummarizedCounterTypeDef](./type_defs.md#summarizedcountertypedef) 
## AttackPropertyTypeDef

```python
# AttackPropertyTypeDef definition

class AttackPropertyTypeDef(TypedDict):
    AttackLayer: NotRequired[AttackLayerType],  # (1)
    AttackPropertyIdentifier: NotRequired[AttackPropertyIdentifierType],  # (2)
    TopContributors: NotRequired[List[ContributorTypeDef]],  # (3)
    Unit: NotRequired[UnitType],  # (4)
    Total: NotRequired[int],
```

1. See [:material-code-brackets: AttackLayerType](./literals.md#attacklayertype) 
2. See [:material-code-brackets: AttackPropertyIdentifierType](./literals.md#attackpropertyidentifiertype) 
3. See [:material-code-braces: ContributorTypeDef](./type_defs.md#contributortypedef) 
4. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## AttackSummaryTypeDef

```python
# AttackSummaryTypeDef definition

class AttackSummaryTypeDef(TypedDict):
    AttackId: NotRequired[str],
    ResourceArn: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    AttackVectors: NotRequired[List[AttackVectorDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: AttackVectorDescriptionTypeDef](./type_defs.md#attackvectordescriptiontypedef) 
## AttackVolumeTypeDef

```python
# AttackVolumeTypeDef definition

class AttackVolumeTypeDef(TypedDict):
    BitsPerSecond: NotRequired[AttackVolumeStatisticsTypeDef],  # (1)
    PacketsPerSecond: NotRequired[AttackVolumeStatisticsTypeDef],  # (1)
    RequestsPerSecond: NotRequired[AttackVolumeStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: AttackVolumeStatisticsTypeDef](./type_defs.md#attackvolumestatisticstypedef) 
2. See [:material-code-braces: AttackVolumeStatisticsTypeDef](./type_defs.md#attackvolumestatisticstypedef) 
3. See [:material-code-braces: AttackVolumeStatisticsTypeDef](./type_defs.md#attackvolumestatisticstypedef) 
## CreateProtectionGroupRequestRequestTypeDef

```python
# CreateProtectionGroupRequestRequestTypeDef definition

class CreateProtectionGroupRequestRequestTypeDef(TypedDict):
    ProtectionGroupId: str,
    Aggregation: ProtectionGroupAggregationType,  # (1)
    Pattern: ProtectionGroupPatternType,  # (2)
    ResourceType: NotRequired[ProtectedResourceTypeType],  # (3)
    Members: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: ProtectionGroupAggregationType](./literals.md#protectiongroupaggregationtype) 
2. See [:material-code-brackets: ProtectionGroupPatternType](./literals.md#protectiongrouppatterntype) 
3. See [:material-code-brackets: ProtectedResourceTypeType](./literals.md#protectedresourcetypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProtectionRequestRequestTypeDef

```python
# CreateProtectionRequestRequestTypeDef definition

class CreateProtectionRequestRequestTypeDef(TypedDict):
    Name: str,
    ResourceArn: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProtectionResponseTypeDef

```python
# CreateProtectionResponseTypeDef definition

class CreateProtectionResponseTypeDef(TypedDict):
    ProtectionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDRTAccessResponseTypeDef

```python
# DescribeDRTAccessResponseTypeDef definition

class DescribeDRTAccessResponseTypeDef(TypedDict):
    RoleArn: str,
    LogBucketList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEmergencyContactSettingsResponseTypeDef

```python
# DescribeEmergencyContactSettingsResponseTypeDef definition

class DescribeEmergencyContactSettingsResponseTypeDef(TypedDict):
    EmergencyContactList: List[EmergencyContactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmergencyContactTypeDef](./type_defs.md#emergencycontacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionStateResponseTypeDef

```python
# GetSubscriptionStateResponseTypeDef definition

class GetSubscriptionStateResponseTypeDef(TypedDict):
    SubscriptionState: SubscriptionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SubscriptionStateType](./literals.md#subscriptionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesInProtectionGroupResponseTypeDef

```python
# ListResourcesInProtectionGroupResponseTypeDef definition

class ListResourcesInProtectionGroupResponseTypeDef(TypedDict):
    ResourceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProtectionGroupResponseTypeDef

```python
# DescribeProtectionGroupResponseTypeDef definition

class DescribeProtectionGroupResponseTypeDef(TypedDict):
    ProtectionGroup: ProtectionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectionGroupTypeDef](./type_defs.md#protectiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectionGroupsResponseTypeDef

```python
# ListProtectionGroupsResponseTypeDef definition

class ListProtectionGroupsResponseTypeDef(TypedDict):
    ProtectionGroups: List[ProtectionGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectionGroupTypeDef](./type_defs.md#protectiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableApplicationLayerAutomaticResponseRequestRequestTypeDef

```python
# EnableApplicationLayerAutomaticResponseRequestRequestTypeDef definition

class EnableApplicationLayerAutomaticResponseRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Action: ResponseActionTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseActionTypeDef](./type_defs.md#responseactiontypedef) 
## UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef

```python
# UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef definition

class UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Action: ResponseActionTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseActionTypeDef](./type_defs.md#responseactiontypedef) 
## ListProtectionsRequestRequestTypeDef

```python
# ListProtectionsRequestRequestTypeDef definition

class ListProtectionsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    InclusionFilters: NotRequired[InclusionProtectionFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: InclusionProtectionFiltersTypeDef](./type_defs.md#inclusionprotectionfilterstypedef) 
## ListProtectionGroupsRequestRequestTypeDef

```python
# ListProtectionGroupsRequestRequestTypeDef definition

class ListProtectionGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    InclusionFilters: NotRequired[InclusionProtectionGroupFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: InclusionProtectionGroupFiltersTypeDef](./type_defs.md#inclusionprotectiongroupfilterstypedef) 
## ProtectionLimitsTypeDef

```python
# ProtectionLimitsTypeDef definition

class ProtectionLimitsTypeDef(TypedDict):
    ProtectedResourceTypeLimits: List[LimitTypeDef],  # (1)
```

1. See [:material-code-braces: LimitTypeDef](./type_defs.md#limittypedef) 
## ListProtectionsRequestListProtectionsPaginateTypeDef

```python
# ListProtectionsRequestListProtectionsPaginateTypeDef definition

class ListProtectionsRequestListProtectionsPaginateTypeDef(TypedDict):
    InclusionFilters: NotRequired[InclusionProtectionFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InclusionProtectionFiltersTypeDef](./type_defs.md#inclusionprotectionfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ProtectionGroupPatternTypeLimitsTypeDef

```python
# ProtectionGroupPatternTypeLimitsTypeDef definition

class ProtectionGroupPatternTypeLimitsTypeDef(TypedDict):
    ArbitraryPatternLimits: ProtectionGroupArbitraryPatternLimitsTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectionGroupArbitraryPatternLimitsTypeDef](./type_defs.md#protectiongrouparbitrarypatternlimitstypedef) 
## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    FromInclusive: NotRequired[TimestampTypeDef],
    ToExclusive: NotRequired[TimestampTypeDef],
```

## ProtectionTypeDef

```python
# ProtectionTypeDef definition

class ProtectionTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    ResourceArn: NotRequired[str],
    HealthCheckIds: NotRequired[List[str]],
    ProtectionArn: NotRequired[str],
    ApplicationLayerAutomaticResponseConfiguration: NotRequired[ApplicationLayerAutomaticResponseConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationLayerAutomaticResponseConfigurationTypeDef](./type_defs.md#applicationlayerautomaticresponseconfigurationtypedef) 
## SubResourceSummaryTypeDef

```python
# SubResourceSummaryTypeDef definition

class SubResourceSummaryTypeDef(TypedDict):
    Type: NotRequired[SubResourceTypeType],  # (1)
    Id: NotRequired[str],
    AttackVectors: NotRequired[List[SummarizedAttackVectorTypeDef]],  # (2)
    Counters: NotRequired[List[SummarizedCounterTypeDef]],  # (3)
```

1. See [:material-code-brackets: SubResourceTypeType](./literals.md#subresourcetypetype) 
2. See [:material-code-braces: SummarizedAttackVectorTypeDef](./type_defs.md#summarizedattackvectortypedef) 
3. See [:material-code-braces: SummarizedCounterTypeDef](./type_defs.md#summarizedcountertypedef) 
## ListAttacksResponseTypeDef

```python
# ListAttacksResponseTypeDef definition

class ListAttacksResponseTypeDef(TypedDict):
    AttackSummaries: List[AttackSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttackSummaryTypeDef](./type_defs.md#attacksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttackStatisticsDataItemTypeDef

```python
# AttackStatisticsDataItemTypeDef definition

class AttackStatisticsDataItemTypeDef(TypedDict):
    AttackCount: int,
    AttackVolume: NotRequired[AttackVolumeTypeDef],  # (1)
```

1. See [:material-code-braces: AttackVolumeTypeDef](./type_defs.md#attackvolumetypedef) 
## ProtectionGroupLimitsTypeDef

```python
# ProtectionGroupLimitsTypeDef definition

class ProtectionGroupLimitsTypeDef(TypedDict):
    MaxProtectionGroups: int,
    PatternTypeLimits: ProtectionGroupPatternTypeLimitsTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectionGroupPatternTypeLimitsTypeDef](./type_defs.md#protectiongrouppatterntypelimitstypedef) 
## ListAttacksRequestListAttacksPaginateTypeDef

```python
# ListAttacksRequestListAttacksPaginateTypeDef definition

class ListAttacksRequestListAttacksPaginateTypeDef(TypedDict):
    ResourceArns: NotRequired[Sequence[str]],
    StartTime: NotRequired[TimeRangeTypeDef],  # (1)
    EndTime: NotRequired[TimeRangeTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttacksRequestRequestTypeDef

```python
# ListAttacksRequestRequestTypeDef definition

class ListAttacksRequestRequestTypeDef(TypedDict):
    ResourceArns: NotRequired[Sequence[str]],
    StartTime: NotRequired[TimeRangeTypeDef],  # (1)
    EndTime: NotRequired[TimeRangeTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## DescribeProtectionResponseTypeDef

```python
# DescribeProtectionResponseTypeDef definition

class DescribeProtectionResponseTypeDef(TypedDict):
    Protection: ProtectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectionTypeDef](./type_defs.md#protectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtectionsResponseTypeDef

```python
# ListProtectionsResponseTypeDef definition

class ListProtectionsResponseTypeDef(TypedDict):
    Protections: List[ProtectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectionTypeDef](./type_defs.md#protectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttackDetailTypeDef

```python
# AttackDetailTypeDef definition

class AttackDetailTypeDef(TypedDict):
    AttackId: NotRequired[str],
    ResourceArn: NotRequired[str],
    SubResources: NotRequired[List[SubResourceSummaryTypeDef]],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    AttackCounters: NotRequired[List[SummarizedCounterTypeDef]],  # (2)
    AttackProperties: NotRequired[List[AttackPropertyTypeDef]],  # (3)
    Mitigations: NotRequired[List[MitigationTypeDef]],  # (4)
```

1. See [:material-code-braces: SubResourceSummaryTypeDef](./type_defs.md#subresourcesummarytypedef) 
2. See [:material-code-braces: SummarizedCounterTypeDef](./type_defs.md#summarizedcountertypedef) 
3. See [:material-code-braces: AttackPropertyTypeDef](./type_defs.md#attackpropertytypedef) 
4. See [:material-code-braces: MitigationTypeDef](./type_defs.md#mitigationtypedef) 
## DescribeAttackStatisticsResponseTypeDef

```python
# DescribeAttackStatisticsResponseTypeDef definition

class DescribeAttackStatisticsResponseTypeDef(TypedDict):
    TimeRange: TimeRangeOutputTypeDef,  # (1)
    DataItems: List[AttackStatisticsDataItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TimeRangeOutputTypeDef](./type_defs.md#timerangeoutputtypedef) 
2. See [:material-code-braces: AttackStatisticsDataItemTypeDef](./type_defs.md#attackstatisticsdataitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionLimitsTypeDef

```python
# SubscriptionLimitsTypeDef definition

class SubscriptionLimitsTypeDef(TypedDict):
    ProtectionLimits: ProtectionLimitsTypeDef,  # (1)
    ProtectionGroupLimits: ProtectionGroupLimitsTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectionLimitsTypeDef](./type_defs.md#protectionlimitstypedef) 
2. See [:material-code-braces: ProtectionGroupLimitsTypeDef](./type_defs.md#protectiongrouplimitstypedef) 
## DescribeAttackResponseTypeDef

```python
# DescribeAttackResponseTypeDef definition

class DescribeAttackResponseTypeDef(TypedDict):
    Attack: AttackDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttackDetailTypeDef](./type_defs.md#attackdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    SubscriptionLimits: SubscriptionLimitsTypeDef,  # (4)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    TimeCommitmentInSeconds: NotRequired[int],
    AutoRenew: NotRequired[AutoRenewType],  # (1)
    Limits: NotRequired[List[LimitTypeDef]],  # (2)
    ProactiveEngagementStatus: NotRequired[ProactiveEngagementStatusType],  # (3)
    SubscriptionArn: NotRequired[str],
```

1. See [:material-code-brackets: AutoRenewType](./literals.md#autorenewtype) 
2. See [:material-code-braces: LimitTypeDef](./type_defs.md#limittypedef) 
3. See [:material-code-brackets: ProactiveEngagementStatusType](./literals.md#proactiveengagementstatustype) 
4. See [:material-code-braces: SubscriptionLimitsTypeDef](./type_defs.md#subscriptionlimitstypedef) 
## DescribeSubscriptionResponseTypeDef

```python
# DescribeSubscriptionResponseTypeDef definition

class DescribeSubscriptionResponseTypeDef(TypedDict):
    Subscription: SubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
