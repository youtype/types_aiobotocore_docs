# Type definitions

> [Index](../README.md) > [Detective](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AcceptInvitationRequestRequestTypeDef

```python
# AcceptInvitationRequestRequestTypeDef definition

class AcceptInvitationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
```

## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    AccountId: str,
    EmailAddress: str,
```

## AdministratorTypeDef

```python
# AdministratorTypeDef definition

class AdministratorTypeDef(TypedDict):
    AccountId: NotRequired[str],
    GraphArn: NotRequired[str],
    DelegationTime: NotRequired[datetime],
```

## BatchGetGraphMemberDatasourcesRequestRequestTypeDef

```python
# BatchGetGraphMemberDatasourcesRequestRequestTypeDef definition

class BatchGetGraphMemberDatasourcesRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    AccountIds: Sequence[str],
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

## UnprocessedAccountTypeDef

```python
# UnprocessedAccountTypeDef definition

class UnprocessedAccountTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Reason: NotRequired[str],
```

## BatchGetMembershipDatasourcesRequestRequestTypeDef

```python
# BatchGetMembershipDatasourcesRequestRequestTypeDef definition

class BatchGetMembershipDatasourcesRequestRequestTypeDef(TypedDict):
    GraphArns: Sequence[str],
```

## UnprocessedGraphTypeDef

```python
# UnprocessedGraphTypeDef definition

class UnprocessedGraphTypeDef(TypedDict):
    GraphArn: NotRequired[str],
    Reason: NotRequired[str],
```

## CreateGraphRequestRequestTypeDef

```python
# CreateGraphRequestRequestTypeDef definition

class CreateGraphRequestRequestTypeDef(TypedDict):
    Tags: NotRequired[Mapping[str, str]],
```

## TimestampForCollectionTypeDef

```python
# TimestampForCollectionTypeDef definition

class TimestampForCollectionTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
```

## DatasourcePackageUsageInfoTypeDef

```python
# DatasourcePackageUsageInfoTypeDef definition

class DatasourcePackageUsageInfoTypeDef(TypedDict):
    VolumeUsageInBytes: NotRequired[int],
    VolumeUsageUpdateTime: NotRequired[datetime],
```

## DeleteGraphRequestRequestTypeDef

```python
# DeleteGraphRequestRequestTypeDef definition

class DeleteGraphRequestRequestTypeDef(TypedDict):
    GraphArn: str,
```

## DeleteMembersRequestRequestTypeDef

```python
# DeleteMembersRequestRequestTypeDef definition

class DeleteMembersRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    AccountIds: Sequence[str],
```

## DescribeOrganizationConfigurationRequestRequestTypeDef

```python
# DescribeOrganizationConfigurationRequestRequestTypeDef definition

class DescribeOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
```

## DisassociateMembershipRequestRequestTypeDef

```python
# DisassociateMembershipRequestRequestTypeDef definition

class DisassociateMembershipRequestRequestTypeDef(TypedDict):
    GraphArn: str,
```

## EnableOrganizationAdminAccountRequestRequestTypeDef

```python
# EnableOrganizationAdminAccountRequestRequestTypeDef definition

class EnableOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## StringFilterTypeDef

```python
# StringFilterTypeDef definition

class StringFilterTypeDef(TypedDict):
    Value: str,
```

## FlaggedIpAddressDetailTypeDef

```python
# FlaggedIpAddressDetailTypeDef definition

class FlaggedIpAddressDetailTypeDef(TypedDict):
    IpAddress: NotRequired[str],
    Reason: NotRequired[ReasonType],  # (1)
```

1. See [:material-code-brackets: ReasonType](./literals.md#reasontype) 
## GetInvestigationRequestRequestTypeDef

```python
# GetInvestigationRequestRequestTypeDef definition

class GetInvestigationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    InvestigationId: str,
```

## GetMembersRequestRequestTypeDef

```python
# GetMembersRequestRequestTypeDef definition

class GetMembersRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    AccountIds: Sequence[str],
```

## GraphTypeDef

```python
# GraphTypeDef definition

class GraphTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

## ImpossibleTravelDetailTypeDef

```python
# ImpossibleTravelDetailTypeDef definition

class ImpossibleTravelDetailTypeDef(TypedDict):
    StartingIpAddress: NotRequired[str],
    EndingIpAddress: NotRequired[str],
    StartingLocation: NotRequired[str],
    EndingLocation: NotRequired[str],
    HourlyTimeDelta: NotRequired[int],
```

## NewAsoDetailTypeDef

```python
# NewAsoDetailTypeDef definition

class NewAsoDetailTypeDef(TypedDict):
    Aso: NotRequired[str],
    IsNewForEntireAccount: NotRequired[bool],
```

## NewGeolocationDetailTypeDef

```python
# NewGeolocationDetailTypeDef definition

class NewGeolocationDetailTypeDef(TypedDict):
    Location: NotRequired[str],
    IpAddress: NotRequired[str],
    IsNewForEntireAccount: NotRequired[bool],
```

## NewUserAgentDetailTypeDef

```python
# NewUserAgentDetailTypeDef definition

class NewUserAgentDetailTypeDef(TypedDict):
    UserAgent: NotRequired[str],
    IsNewForEntireAccount: NotRequired[bool],
```

## RelatedFindingDetailTypeDef

```python
# RelatedFindingDetailTypeDef definition

class RelatedFindingDetailTypeDef(TypedDict):
    Arn: NotRequired[str],
    Type: NotRequired[str],
    IpAddress: NotRequired[str],
```

## RelatedFindingGroupDetailTypeDef

```python
# RelatedFindingGroupDetailTypeDef definition

class RelatedFindingGroupDetailTypeDef(TypedDict):
    Id: NotRequired[str],
```

## TTPsObservedDetailTypeDef

```python
# TTPsObservedDetailTypeDef definition

class TTPsObservedDetailTypeDef(TypedDict):
    Tactic: NotRequired[str],
    Technique: NotRequired[str],
    Procedure: NotRequired[str],
    IpAddress: NotRequired[str],
    APIName: NotRequired[str],
    APISuccessCount: NotRequired[int],
    APIFailureCount: NotRequired[int],
```

## InvestigationDetailTypeDef

```python
# InvestigationDetailTypeDef definition

class InvestigationDetailTypeDef(TypedDict):
    InvestigationId: NotRequired[str],
    Severity: NotRequired[SeverityType],  # (1)
    Status: NotRequired[StatusType],  # (2)
    State: NotRequired[StateType],  # (3)
    CreatedTime: NotRequired[datetime],
    EntityArn: NotRequired[str],
    EntityType: NotRequired[EntityTypeType],  # (4)
```

1. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
4. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## ListDatasourcePackagesRequestRequestTypeDef

```python
# ListDatasourcePackagesRequestRequestTypeDef definition

class ListDatasourcePackagesRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGraphsRequestRequestTypeDef

```python
# ListGraphsRequestRequestTypeDef definition

class ListGraphsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIndicatorsRequestRequestTypeDef

```python
# ListIndicatorsRequestRequestTypeDef definition

class ListIndicatorsRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    InvestigationId: str,
    IndicatorType: NotRequired[IndicatorTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: IndicatorTypeType](./literals.md#indicatortypetype) 
## SortCriteriaTypeDef

```python
# SortCriteriaTypeDef definition

class SortCriteriaTypeDef(TypedDict):
    Field: NotRequired[FieldType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: FieldType](./literals.md#fieldtype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListInvitationsRequestRequestTypeDef

```python
# ListInvitationsRequestRequestTypeDef definition

class ListInvitationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMembersRequestRequestTypeDef

```python
# ListMembersRequestRequestTypeDef definition

class ListMembersRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListOrganizationAdminAccountsRequestRequestTypeDef

```python
# ListOrganizationAdminAccountsRequestRequestTypeDef definition

class ListOrganizationAdminAccountsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RejectInvitationRequestRequestTypeDef

```python
# RejectInvitationRequestRequestTypeDef definition

class RejectInvitationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
```

## StartMonitoringMemberRequestRequestTypeDef

```python
# StartMonitoringMemberRequestRequestTypeDef definition

class StartMonitoringMemberRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    AccountId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateDatasourcePackagesRequestRequestTypeDef

```python
# UpdateDatasourcePackagesRequestRequestTypeDef definition

class UpdateDatasourcePackagesRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    DatasourcePackages: Sequence[DatasourcePackageType],  # (1)
```

1. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) 
## UpdateInvestigationStateRequestRequestTypeDef

```python
# UpdateInvestigationStateRequestRequestTypeDef definition

class UpdateInvestigationStateRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    InvestigationId: str,
    State: StateType,  # (1)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
## UpdateOrganizationConfigurationRequestRequestTypeDef

```python
# UpdateOrganizationConfigurationRequestRequestTypeDef definition

class UpdateOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    AutoEnable: NotRequired[bool],
```

## CreateMembersRequestRequestTypeDef

```python
# CreateMembersRequestRequestTypeDef definition

class CreateMembersRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    Accounts: Sequence[AccountTypeDef],  # (1)
    Message: NotRequired[str],
    DisableEmailNotification: NotRequired[bool],
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
## CreateGraphResponseTypeDef

```python
# CreateGraphResponseTypeDef definition

class CreateGraphResponseTypeDef(TypedDict):
    GraphArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigurationResponseTypeDef

```python
# DescribeOrganizationConfigurationResponseTypeDef definition

class DescribeOrganizationConfigurationResponseTypeDef(TypedDict):
    AutoEnable: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInvestigationResponseTypeDef

```python
# GetInvestigationResponseTypeDef definition

class GetInvestigationResponseTypeDef(TypedDict):
    GraphArn: str,
    InvestigationId: str,
    EntityArn: str,
    EntityType: EntityTypeType,  # (1)
    CreatedTime: datetime,
    ScopeStartTime: datetime,
    ScopeEndTime: datetime,
    Status: StatusType,  # (2)
    Severity: SeverityType,  # (3)
    State: StateType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
4. See [:material-code-brackets: StateType](./literals.md#statetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationAdminAccountsResponseTypeDef

```python
# ListOrganizationAdminAccountsResponseTypeDef definition

class ListOrganizationAdminAccountsResponseTypeDef(TypedDict):
    Administrators: List[AdministratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AdministratorTypeDef](./type_defs.md#administratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInvestigationResponseTypeDef

```python
# StartInvestigationResponseTypeDef definition

class StartInvestigationResponseTypeDef(TypedDict):
    InvestigationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMembersResponseTypeDef

```python
# DeleteMembersResponseTypeDef definition

class DeleteMembersResponseTypeDef(TypedDict):
    AccountIds: List[str],
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasourcePackageIngestDetailTypeDef

```python
# DatasourcePackageIngestDetailTypeDef definition

class DatasourcePackageIngestDetailTypeDef(TypedDict):
    DatasourcePackageIngestState: NotRequired[DatasourcePackageIngestStateType],  # (1)
    LastIngestStateChange: NotRequired[Dict[DatasourcePackageIngestStateType, TimestampForCollectionTypeDef]],  # (2)
```

1. See [:material-code-brackets: DatasourcePackageIngestStateType](./literals.md#datasourcepackageingeststatetype) 
2. See [:material-code-brackets: DatasourcePackageIngestStateType](./literals.md#datasourcepackageingeststatetype) [:material-code-braces: TimestampForCollectionTypeDef](./type_defs.md#timestampforcollectiontypedef) 
## MembershipDatasourcesTypeDef

```python
# MembershipDatasourcesTypeDef definition

class MembershipDatasourcesTypeDef(TypedDict):
    AccountId: NotRequired[str],
    GraphArn: NotRequired[str],
    DatasourcePackageIngestHistory: NotRequired[Dict[DatasourcePackageType, Dict[DatasourcePackageIngestStateType, TimestampForCollectionTypeDef]]],  # (1)
```

1. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) [:material-code-brackets: DatasourcePackageIngestStateType](./literals.md#datasourcepackageingeststatetype) [:material-code-braces: TimestampForCollectionTypeDef](./type_defs.md#timestampforcollectiontypedef) 
## MemberDetailTypeDef

```python
# MemberDetailTypeDef definition

class MemberDetailTypeDef(TypedDict):
    AccountId: NotRequired[str],
    EmailAddress: NotRequired[str],
    GraphArn: NotRequired[str],
    MasterId: NotRequired[str],
    AdministratorId: NotRequired[str],
    Status: NotRequired[MemberStatusType],  # (1)
    DisabledReason: NotRequired[MemberDisabledReasonType],  # (2)
    InvitedTime: NotRequired[datetime],
    UpdatedTime: NotRequired[datetime],
    VolumeUsageInBytes: NotRequired[int],
    VolumeUsageUpdatedTime: NotRequired[datetime],
    PercentOfGraphUtilization: NotRequired[float],
    PercentOfGraphUtilizationUpdatedTime: NotRequired[datetime],
    InvitationType: NotRequired[InvitationTypeType],  # (3)
    VolumeUsageByDatasourcePackage: NotRequired[Dict[DatasourcePackageType, DatasourcePackageUsageInfoTypeDef]],  # (4)
    DatasourcePackageIngestStates: NotRequired[Dict[DatasourcePackageType, DatasourcePackageIngestStateType]],  # (5)
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-brackets: MemberDisabledReasonType](./literals.md#memberdisabledreasontype) 
3. See [:material-code-brackets: InvitationTypeType](./literals.md#invitationtypetype) 
4. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) [:material-code-braces: DatasourcePackageUsageInfoTypeDef](./type_defs.md#datasourcepackageusageinfotypedef) 
5. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) [:material-code-brackets: DatasourcePackageIngestStateType](./literals.md#datasourcepackageingeststatetype) 
## DateFilterTypeDef

```python
# DateFilterTypeDef definition

class DateFilterTypeDef(TypedDict):
    StartInclusive: TimestampTypeDef,
    EndInclusive: TimestampTypeDef,
```

## StartInvestigationRequestRequestTypeDef

```python
# StartInvestigationRequestRequestTypeDef definition

class StartInvestigationRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    EntityArn: str,
    ScopeStartTime: TimestampTypeDef,
    ScopeEndTime: TimestampTypeDef,
```

## ListGraphsResponseTypeDef

```python
# ListGraphsResponseTypeDef definition

class ListGraphsResponseTypeDef(TypedDict):
    GraphList: List[GraphTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GraphTypeDef](./type_defs.md#graphtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndicatorDetailTypeDef

```python
# IndicatorDetailTypeDef definition

class IndicatorDetailTypeDef(TypedDict):
    TTPsObservedDetail: NotRequired[TTPsObservedDetailTypeDef],  # (1)
    ImpossibleTravelDetail: NotRequired[ImpossibleTravelDetailTypeDef],  # (2)
    FlaggedIpAddressDetail: NotRequired[FlaggedIpAddressDetailTypeDef],  # (3)
    NewGeolocationDetail: NotRequired[NewGeolocationDetailTypeDef],  # (4)
    NewAsoDetail: NotRequired[NewAsoDetailTypeDef],  # (5)
    NewUserAgentDetail: NotRequired[NewUserAgentDetailTypeDef],  # (6)
    RelatedFindingDetail: NotRequired[RelatedFindingDetailTypeDef],  # (7)
    RelatedFindingGroupDetail: NotRequired[RelatedFindingGroupDetailTypeDef],  # (8)
```

1. See [:material-code-braces: TTPsObservedDetailTypeDef](./type_defs.md#ttpsobserveddetailtypedef) 
2. See [:material-code-braces: ImpossibleTravelDetailTypeDef](./type_defs.md#impossibletraveldetailtypedef) 
3. See [:material-code-braces: FlaggedIpAddressDetailTypeDef](./type_defs.md#flaggedipaddressdetailtypedef) 
4. See [:material-code-braces: NewGeolocationDetailTypeDef](./type_defs.md#newgeolocationdetailtypedef) 
5. See [:material-code-braces: NewAsoDetailTypeDef](./type_defs.md#newasodetailtypedef) 
6. See [:material-code-braces: NewUserAgentDetailTypeDef](./type_defs.md#newuseragentdetailtypedef) 
7. See [:material-code-braces: RelatedFindingDetailTypeDef](./type_defs.md#relatedfindingdetailtypedef) 
8. See [:material-code-braces: RelatedFindingGroupDetailTypeDef](./type_defs.md#relatedfindinggroupdetailtypedef) 
## ListInvestigationsResponseTypeDef

```python
# ListInvestigationsResponseTypeDef definition

class ListInvestigationsResponseTypeDef(TypedDict):
    InvestigationDetails: List[InvestigationDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InvestigationDetailTypeDef](./type_defs.md#investigationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasourcePackagesResponseTypeDef

```python
# ListDatasourcePackagesResponseTypeDef definition

class ListDatasourcePackagesResponseTypeDef(TypedDict):
    DatasourcePackages: Dict[DatasourcePackageType, DatasourcePackageIngestDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) [:material-code-braces: DatasourcePackageIngestDetailTypeDef](./type_defs.md#datasourcepackageingestdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetGraphMemberDatasourcesResponseTypeDef

```python
# BatchGetGraphMemberDatasourcesResponseTypeDef definition

class BatchGetGraphMemberDatasourcesResponseTypeDef(TypedDict):
    MemberDatasources: List[MembershipDatasourcesTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MembershipDatasourcesTypeDef](./type_defs.md#membershipdatasourcestypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetMembershipDatasourcesResponseTypeDef

```python
# BatchGetMembershipDatasourcesResponseTypeDef definition

class BatchGetMembershipDatasourcesResponseTypeDef(TypedDict):
    MembershipDatasources: List[MembershipDatasourcesTypeDef],  # (1)
    UnprocessedGraphs: List[UnprocessedGraphTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MembershipDatasourcesTypeDef](./type_defs.md#membershipdatasourcestypedef) 
2. See [:material-code-braces: UnprocessedGraphTypeDef](./type_defs.md#unprocessedgraphtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembersResponseTypeDef

```python
# CreateMembersResponseTypeDef definition

class CreateMembersResponseTypeDef(TypedDict):
    Members: List[MemberDetailTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMembersResponseTypeDef

```python
# GetMembersResponseTypeDef definition

class GetMembersResponseTypeDef(TypedDict):
    MemberDetails: List[MemberDetailTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInvitationsResponseTypeDef

```python
# ListInvitationsResponseTypeDef definition

class ListInvitationsResponseTypeDef(TypedDict):
    Invitations: List[MemberDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    MemberDetails: List[MemberDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    Severity: NotRequired[StringFilterTypeDef],  # (1)
    Status: NotRequired[StringFilterTypeDef],  # (1)
    State: NotRequired[StringFilterTypeDef],  # (1)
    EntityArn: NotRequired[StringFilterTypeDef],  # (1)
    CreatedTime: NotRequired[DateFilterTypeDef],  # (5)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
## IndicatorTypeDef

```python
# IndicatorTypeDef definition

class IndicatorTypeDef(TypedDict):
    IndicatorType: NotRequired[IndicatorTypeType],  # (1)
    IndicatorDetail: NotRequired[IndicatorDetailTypeDef],  # (2)
```

1. See [:material-code-brackets: IndicatorTypeType](./literals.md#indicatortypetype) 
2. See [:material-code-braces: IndicatorDetailTypeDef](./type_defs.md#indicatordetailtypedef) 
## ListInvestigationsRequestRequestTypeDef

```python
# ListInvestigationsRequestRequestTypeDef definition

class ListInvestigationsRequestRequestTypeDef(TypedDict):
    GraphArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## ListIndicatorsResponseTypeDef

```python
# ListIndicatorsResponseTypeDef definition

class ListIndicatorsResponseTypeDef(TypedDict):
    GraphArn: str,
    InvestigationId: str,
    Indicators: List[IndicatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndicatorTypeDef](./type_defs.md#indicatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
