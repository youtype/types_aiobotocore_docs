# Type definitions

> [Index](../README.md) > [Detective](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).



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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
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
## ListOrganizationAdminAccountsResponseTypeDef

```python
# ListOrganizationAdminAccountsResponseTypeDef definition

class ListOrganizationAdminAccountsResponseTypeDef(TypedDict):
    Administrators: List[AdministratorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## ListGraphsResponseTypeDef

```python
# ListGraphsResponseTypeDef definition

class ListGraphsResponseTypeDef(TypedDict):
    GraphList: List[GraphTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GraphTypeDef](./type_defs.md#graphtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasourcePackagesResponseTypeDef

```python
# ListDatasourcePackagesResponseTypeDef definition

class ListDatasourcePackagesResponseTypeDef(TypedDict):
    DatasourcePackages: Dict[DatasourcePackageType, DatasourcePackageIngestDetailTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    MemberDetails: List[MemberDetailTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberDetailTypeDef](./type_defs.md#memberdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
