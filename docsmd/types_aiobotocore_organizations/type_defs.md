# Type definitions

> [Index](../README.md) > [Organizations](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
    type annotations stubs module [types-aiobotocore-organizations](https://pypi.org/project/types-aiobotocore-organizations/).



## AcceptHandshakeRequestRequestTypeDef

```python
# AcceptHandshakeRequestRequestTypeDef definition

class AcceptHandshakeRequestRequestTypeDef(TypedDict):
    HandshakeId: str,
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

## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Email: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[AccountStatusType],  # (1)
    JoinedMethod: NotRequired[AccountJoinedMethodType],  # (2)
    JoinedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
2. See [:material-code-brackets: AccountJoinedMethodType](./literals.md#accountjoinedmethodtype) 
## AttachPolicyRequestRequestTypeDef

```python
# AttachPolicyRequestRequestTypeDef definition

class AttachPolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    TargetId: str,
```

## CancelHandshakeRequestRequestTypeDef

```python
# CancelHandshakeRequestRequestTypeDef definition

class CancelHandshakeRequestRequestTypeDef(TypedDict):
    HandshakeId: str,
```

## ChildTypeDef

```python
# ChildTypeDef definition

class ChildTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[ChildTypeType],  # (1)
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype) 
## CloseAccountRequestRequestTypeDef

```python
# CloseAccountRequestRequestTypeDef definition

class CloseAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateAccountStatusTypeDef

```python
# CreateAccountStatusTypeDef definition

class CreateAccountStatusTypeDef(TypedDict):
    Id: NotRequired[str],
    AccountName: NotRequired[str],
    State: NotRequired[CreateAccountStateType],  # (1)
    RequestedTimestamp: NotRequired[datetime],
    CompletedTimestamp: NotRequired[datetime],
    AccountId: NotRequired[str],
    GovCloudAccountId: NotRequired[str],
    FailureReason: NotRequired[CreateAccountFailureReasonType],  # (2)
```

1. See [:material-code-brackets: CreateAccountStateType](./literals.md#createaccountstatetype) 
2. See [:material-code-brackets: CreateAccountFailureReasonType](./literals.md#createaccountfailurereasontype) 
## CreateOrganizationRequestRequestTypeDef

```python
# CreateOrganizationRequestRequestTypeDef definition

class CreateOrganizationRequestRequestTypeDef(TypedDict):
    FeatureSet: NotRequired[OrganizationFeatureSetType],  # (1)
```

1. See [:material-code-brackets: OrganizationFeatureSetType](./literals.md#organizationfeaturesettype) 
## OrganizationalUnitTypeDef

```python
# OrganizationalUnitTypeDef definition

class OrganizationalUnitTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## DeclineHandshakeRequestRequestTypeDef

```python
# DeclineHandshakeRequestRequestTypeDef definition

class DeclineHandshakeRequestRequestTypeDef(TypedDict):
    HandshakeId: str,
```

## DelegatedAdministratorTypeDef

```python
# DelegatedAdministratorTypeDef definition

class DelegatedAdministratorTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Email: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[AccountStatusType],  # (1)
    JoinedMethod: NotRequired[AccountJoinedMethodType],  # (2)
    JoinedTimestamp: NotRequired[datetime],
    DelegationEnabledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
2. See [:material-code-brackets: AccountJoinedMethodType](./literals.md#accountjoinedmethodtype) 
## DelegatedServiceTypeDef

```python
# DelegatedServiceTypeDef definition

class DelegatedServiceTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    DelegationEnabledDate: NotRequired[datetime],
```

## DeleteOrganizationalUnitRequestRequestTypeDef

```python
# DeleteOrganizationalUnitRequestRequestTypeDef definition

class DeleteOrganizationalUnitRequestRequestTypeDef(TypedDict):
    OrganizationalUnitId: str,
```

## DeletePolicyRequestRequestTypeDef

```python
# DeletePolicyRequestRequestTypeDef definition

class DeletePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
```

## DeregisterDelegatedAdministratorRequestRequestTypeDef

```python
# DeregisterDelegatedAdministratorRequestRequestTypeDef definition

class DeregisterDelegatedAdministratorRequestRequestTypeDef(TypedDict):
    AccountId: str,
    ServicePrincipal: str,
```

## DescribeAccountRequestRequestTypeDef

```python
# DescribeAccountRequestRequestTypeDef definition

class DescribeAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## DescribeCreateAccountStatusRequestRequestTypeDef

```python
# DescribeCreateAccountStatusRequestRequestTypeDef definition

class DescribeCreateAccountStatusRequestRequestTypeDef(TypedDict):
    CreateAccountRequestId: str,
```

## DescribeEffectivePolicyRequestRequestTypeDef

```python
# DescribeEffectivePolicyRequestRequestTypeDef definition

class DescribeEffectivePolicyRequestRequestTypeDef(TypedDict):
    PolicyType: EffectivePolicyTypeType,  # (1)
    TargetId: NotRequired[str],
```

1. See [:material-code-brackets: EffectivePolicyTypeType](./literals.md#effectivepolicytypetype) 
## EffectivePolicyTypeDef

```python
# EffectivePolicyTypeDef definition

class EffectivePolicyTypeDef(TypedDict):
    PolicyContent: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[datetime],
    TargetId: NotRequired[str],
    PolicyType: NotRequired[EffectivePolicyTypeType],  # (1)
```

1. See [:material-code-brackets: EffectivePolicyTypeType](./literals.md#effectivepolicytypetype) 
## DescribeHandshakeRequestRequestTypeDef

```python
# DescribeHandshakeRequestRequestTypeDef definition

class DescribeHandshakeRequestRequestTypeDef(TypedDict):
    HandshakeId: str,
```

## DescribeOrganizationalUnitRequestRequestTypeDef

```python
# DescribeOrganizationalUnitRequestRequestTypeDef definition

class DescribeOrganizationalUnitRequestRequestTypeDef(TypedDict):
    OrganizationalUnitId: str,
```

## DescribePolicyRequestRequestTypeDef

```python
# DescribePolicyRequestRequestTypeDef definition

class DescribePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
```

## DetachPolicyRequestRequestTypeDef

```python
# DetachPolicyRequestRequestTypeDef definition

class DetachPolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    TargetId: str,
```

## DisableAWSServiceAccessRequestRequestTypeDef

```python
# DisableAWSServiceAccessRequestRequestTypeDef definition

class DisableAWSServiceAccessRequestRequestTypeDef(TypedDict):
    ServicePrincipal: str,
```

## DisablePolicyTypeRequestRequestTypeDef

```python
# DisablePolicyTypeRequestRequestTypeDef definition

class DisablePolicyTypeRequestRequestTypeDef(TypedDict):
    RootId: str,
    PolicyType: PolicyTypeType,  # (1)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## EnableAWSServiceAccessRequestRequestTypeDef

```python
# EnableAWSServiceAccessRequestRequestTypeDef definition

class EnableAWSServiceAccessRequestRequestTypeDef(TypedDict):
    ServicePrincipal: str,
```

## EnablePolicyTypeRequestRequestTypeDef

```python
# EnablePolicyTypeRequestRequestTypeDef definition

class EnablePolicyTypeRequestRequestTypeDef(TypedDict):
    RootId: str,
    PolicyType: PolicyTypeType,  # (1)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## EnabledServicePrincipalTypeDef

```python
# EnabledServicePrincipalTypeDef definition

class EnabledServicePrincipalTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    DateEnabled: NotRequired[datetime],
```

## HandshakeFilterTypeDef

```python
# HandshakeFilterTypeDef definition

class HandshakeFilterTypeDef(TypedDict):
    ActionType: NotRequired[ActionTypeType],  # (1)
    ParentHandshakeId: NotRequired[str],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## HandshakePartyTypeDef

```python
# HandshakePartyTypeDef definition

class HandshakePartyTypeDef(TypedDict):
    Id: str,
    Type: HandshakePartyTypeType,  # (1)
```

1. See [:material-code-brackets: HandshakePartyTypeType](./literals.md#handshakepartytypetype) 
## HandshakeResourcePaginatorTypeDef

```python
# HandshakeResourcePaginatorTypeDef definition

class HandshakeResourcePaginatorTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[HandshakeResourceTypeType],  # (1)
    Resources: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-brackets: HandshakeResourceTypeType](./literals.md#handshakeresourcetypetype) 
## HandshakeResourceTypeDef

```python
# HandshakeResourceTypeDef definition

class HandshakeResourceTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[HandshakeResourceTypeType],  # (1)
    Resources: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-brackets: HandshakeResourceTypeType](./literals.md#handshakeresourcetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAWSServiceAccessForOrganizationRequestRequestTypeDef

```python
# ListAWSServiceAccessForOrganizationRequestRequestTypeDef definition

class ListAWSServiceAccessForOrganizationRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAccountsForParentRequestRequestTypeDef

```python
# ListAccountsForParentRequestRequestTypeDef definition

class ListAccountsForParentRequestRequestTypeDef(TypedDict):
    ParentId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAccountsRequestRequestTypeDef

```python
# ListAccountsRequestRequestTypeDef definition

class ListAccountsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListChildrenRequestRequestTypeDef

```python
# ListChildrenRequestRequestTypeDef definition

class ListChildrenRequestRequestTypeDef(TypedDict):
    ParentId: str,
    ChildType: ChildTypeType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype) 
## ListCreateAccountStatusRequestRequestTypeDef

```python
# ListCreateAccountStatusRequestRequestTypeDef definition

class ListCreateAccountStatusRequestRequestTypeDef(TypedDict):
    States: NotRequired[Sequence[CreateAccountStateType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: CreateAccountStateType](./literals.md#createaccountstatetype) 
## ListDelegatedAdministratorsRequestRequestTypeDef

```python
# ListDelegatedAdministratorsRequestRequestTypeDef definition

class ListDelegatedAdministratorsRequestRequestTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDelegatedServicesForAccountRequestRequestTypeDef

```python
# ListDelegatedServicesForAccountRequestRequestTypeDef definition

class ListDelegatedServicesForAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListOrganizationalUnitsForParentRequestRequestTypeDef

```python
# ListOrganizationalUnitsForParentRequestRequestTypeDef definition

class ListOrganizationalUnitsForParentRequestRequestTypeDef(TypedDict):
    ParentId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListParentsRequestRequestTypeDef

```python
# ListParentsRequestRequestTypeDef definition

class ListParentsRequestRequestTypeDef(TypedDict):
    ChildId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ParentTypeDef

```python
# ParentTypeDef definition

class ParentTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[ParentTypeType],  # (1)
```

1. See [:material-code-brackets: ParentTypeType](./literals.md#parenttypetype) 
## ListPoliciesForTargetRequestRequestTypeDef

```python
# ListPoliciesForTargetRequestRequestTypeDef definition

class ListPoliciesForTargetRequestRequestTypeDef(TypedDict):
    TargetId: str,
    Filter: PolicyTypeType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## PolicySummaryTypeDef

```python
# PolicySummaryTypeDef definition

class PolicySummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[PolicyTypeType],  # (1)
    AwsManaged: NotRequired[bool],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## ListPoliciesRequestRequestTypeDef

```python
# ListPoliciesRequestRequestTypeDef definition

class ListPoliciesRequestRequestTypeDef(TypedDict):
    Filter: PolicyTypeType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## ListRootsRequestRequestTypeDef

```python
# ListRootsRequestRequestTypeDef definition

class ListRootsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    NextToken: NotRequired[str],
```

## ListTargetsForPolicyRequestRequestTypeDef

```python
# ListTargetsForPolicyRequestRequestTypeDef definition

class ListTargetsForPolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PolicyTargetSummaryTypeDef

```python
# PolicyTargetSummaryTypeDef definition

class PolicyTargetSummaryTypeDef(TypedDict):
    TargetId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[TargetTypeType],  # (1)
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## MoveAccountRequestRequestTypeDef

```python
# MoveAccountRequestRequestTypeDef definition

class MoveAccountRequestRequestTypeDef(TypedDict):
    AccountId: str,
    SourceParentId: str,
    DestinationParentId: str,
```

## PolicyTypeSummaryTypeDef

```python
# PolicyTypeSummaryTypeDef definition

class PolicyTypeSummaryTypeDef(TypedDict):
    Type: NotRequired[PolicyTypeType],  # (1)
    Status: NotRequired[PolicyTypeStatusType],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: PolicyTypeStatusType](./literals.md#policytypestatustype) 
## RegisterDelegatedAdministratorRequestRequestTypeDef

```python
# RegisterDelegatedAdministratorRequestRequestTypeDef definition

class RegisterDelegatedAdministratorRequestRequestTypeDef(TypedDict):
    AccountId: str,
    ServicePrincipal: str,
```

## RemoveAccountFromOrganizationRequestRequestTypeDef

```python
# RemoveAccountFromOrganizationRequestRequestTypeDef definition

class RemoveAccountFromOrganizationRequestRequestTypeDef(TypedDict):
    AccountId: str,
```

## ResourcePolicySummaryTypeDef

```python
# ResourcePolicySummaryTypeDef definition

class ResourcePolicySummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagKeys: Sequence[str],
```

## UpdateOrganizationalUnitRequestRequestTypeDef

```python
# UpdateOrganizationalUnitRequestRequestTypeDef definition

class UpdateOrganizationalUnitRequestRequestTypeDef(TypedDict):
    OrganizationalUnitId: str,
    Name: NotRequired[str],
```

## UpdatePolicyRequestRequestTypeDef

```python
# UpdatePolicyRequestRequestTypeDef definition

class UpdatePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Content: NotRequired[str],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountResponseTypeDef

```python
# DescribeAccountResponseTypeDef definition

class DescribeAccountResponseTypeDef(TypedDict):
    Account: AccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsForParentResponseTypeDef

```python
# ListAccountsForParentResponseTypeDef definition

class ListAccountsForParentResponseTypeDef(TypedDict):
    Accounts: List[AccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsResponseTypeDef

```python
# ListAccountsResponseTypeDef definition

class ListAccountsResponseTypeDef(TypedDict):
    Accounts: List[AccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChildrenResponseTypeDef

```python
# ListChildrenResponseTypeDef definition

class ListChildrenResponseTypeDef(TypedDict):
    Children: List[ChildTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChildTypeDef](./type_defs.md#childtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccountRequestRequestTypeDef

```python
# CreateAccountRequestRequestTypeDef definition

class CreateAccountRequestRequestTypeDef(TypedDict):
    Email: str,
    AccountName: str,
    RoleName: NotRequired[str],
    IamUserAccessToBilling: NotRequired[IAMUserAccessToBillingType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IAMUserAccessToBillingType](./literals.md#iamuseraccesstobillingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateGovCloudAccountRequestRequestTypeDef

```python
# CreateGovCloudAccountRequestRequestTypeDef definition

class CreateGovCloudAccountRequestRequestTypeDef(TypedDict):
    Email: str,
    AccountName: str,
    RoleName: NotRequired[str],
    IamUserAccessToBilling: NotRequired[IAMUserAccessToBillingType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IAMUserAccessToBillingType](./literals.md#iamuseraccesstobillingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOrganizationalUnitRequestRequestTypeDef

```python
# CreateOrganizationalUnitRequestRequestTypeDef definition

class CreateOrganizationalUnitRequestRequestTypeDef(TypedDict):
    ParentId: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePolicyRequestRequestTypeDef

```python
# CreatePolicyRequestRequestTypeDef definition

class CreatePolicyRequestRequestTypeDef(TypedDict):
    Content: str,
    Description: str,
    Name: str,
    Type: PolicyTypeType,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    Content: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAccountResponseTypeDef

```python
# CreateAccountResponseTypeDef definition

class CreateAccountResponseTypeDef(TypedDict):
    CreateAccountStatus: CreateAccountStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateAccountStatusTypeDef](./type_defs.md#createaccountstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGovCloudAccountResponseTypeDef

```python
# CreateGovCloudAccountResponseTypeDef definition

class CreateGovCloudAccountResponseTypeDef(TypedDict):
    CreateAccountStatus: CreateAccountStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateAccountStatusTypeDef](./type_defs.md#createaccountstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCreateAccountStatusResponseTypeDef

```python
# DescribeCreateAccountStatusResponseTypeDef definition

class DescribeCreateAccountStatusResponseTypeDef(TypedDict):
    CreateAccountStatus: CreateAccountStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateAccountStatusTypeDef](./type_defs.md#createaccountstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCreateAccountStatusResponseTypeDef

```python
# ListCreateAccountStatusResponseTypeDef definition

class ListCreateAccountStatusResponseTypeDef(TypedDict):
    CreateAccountStatuses: List[CreateAccountStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CreateAccountStatusTypeDef](./type_defs.md#createaccountstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOrganizationalUnitResponseTypeDef

```python
# CreateOrganizationalUnitResponseTypeDef definition

class CreateOrganizationalUnitResponseTypeDef(TypedDict):
    OrganizationalUnit: OrganizationalUnitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationalUnitTypeDef](./type_defs.md#organizationalunittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationalUnitResponseTypeDef

```python
# DescribeOrganizationalUnitResponseTypeDef definition

class DescribeOrganizationalUnitResponseTypeDef(TypedDict):
    OrganizationalUnit: OrganizationalUnitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationalUnitTypeDef](./type_defs.md#organizationalunittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationalUnitsForParentResponseTypeDef

```python
# ListOrganizationalUnitsForParentResponseTypeDef definition

class ListOrganizationalUnitsForParentResponseTypeDef(TypedDict):
    OrganizationalUnits: List[OrganizationalUnitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationalUnitTypeDef](./type_defs.md#organizationalunittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOrganizationalUnitResponseTypeDef

```python
# UpdateOrganizationalUnitResponseTypeDef definition

class UpdateOrganizationalUnitResponseTypeDef(TypedDict):
    OrganizationalUnit: OrganizationalUnitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationalUnitTypeDef](./type_defs.md#organizationalunittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDelegatedAdministratorsResponseTypeDef

```python
# ListDelegatedAdministratorsResponseTypeDef definition

class ListDelegatedAdministratorsResponseTypeDef(TypedDict):
    DelegatedAdministrators: List[DelegatedAdministratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DelegatedAdministratorTypeDef](./type_defs.md#delegatedadministratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDelegatedServicesForAccountResponseTypeDef

```python
# ListDelegatedServicesForAccountResponseTypeDef definition

class ListDelegatedServicesForAccountResponseTypeDef(TypedDict):
    DelegatedServices: List[DelegatedServiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DelegatedServiceTypeDef](./type_defs.md#delegatedservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEffectivePolicyResponseTypeDef

```python
# DescribeEffectivePolicyResponseTypeDef definition

class DescribeEffectivePolicyResponseTypeDef(TypedDict):
    EffectivePolicy: EffectivePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EffectivePolicyTypeDef](./type_defs.md#effectivepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAWSServiceAccessForOrganizationResponseTypeDef

```python
# ListAWSServiceAccessForOrganizationResponseTypeDef definition

class ListAWSServiceAccessForOrganizationResponseTypeDef(TypedDict):
    EnabledServicePrincipals: List[EnabledServicePrincipalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EnabledServicePrincipalTypeDef](./type_defs.md#enabledserviceprincipaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHandshakesForAccountRequestRequestTypeDef

```python
# ListHandshakesForAccountRequestRequestTypeDef definition

class ListHandshakesForAccountRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[HandshakeFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
## ListHandshakesForOrganizationRequestRequestTypeDef

```python
# ListHandshakesForOrganizationRequestRequestTypeDef definition

class ListHandshakesForOrganizationRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[HandshakeFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
## InviteAccountToOrganizationRequestRequestTypeDef

```python
# InviteAccountToOrganizationRequestRequestTypeDef definition

class InviteAccountToOrganizationRequestRequestTypeDef(TypedDict):
    Target: HandshakePartyTypeDef,  # (1)
    Notes: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: HandshakePartyTypeDef](./type_defs.md#handshakepartytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## HandshakePaginatorTypeDef

```python
# HandshakePaginatorTypeDef definition

class HandshakePaginatorTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Parties: NotRequired[List[HandshakePartyTypeDef]],  # (1)
    State: NotRequired[HandshakeStateType],  # (2)
    RequestedTimestamp: NotRequired[datetime],
    ExpirationTimestamp: NotRequired[datetime],
    Action: NotRequired[ActionTypeType],  # (3)
    Resources: NotRequired[List[HandshakeResourcePaginatorTypeDef]],  # (4)
```

1. See [:material-code-braces: HandshakePartyTypeDef](./type_defs.md#handshakepartytypedef) 
2. See [:material-code-brackets: HandshakeStateType](./literals.md#handshakestatetype) 
3. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
4. See [:material-code-braces: HandshakeResourcePaginatorTypeDef](./type_defs.md#handshakeresourcepaginatortypedef) 
## HandshakeTypeDef

```python
# HandshakeTypeDef definition

class HandshakeTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Parties: NotRequired[List[HandshakePartyTypeDef]],  # (1)
    State: NotRequired[HandshakeStateType],  # (2)
    RequestedTimestamp: NotRequired[datetime],
    ExpirationTimestamp: NotRequired[datetime],
    Action: NotRequired[ActionTypeType],  # (3)
    Resources: NotRequired[List[HandshakeResourceTypeDef]],  # (4)
```

1. See [:material-code-braces: HandshakePartyTypeDef](./type_defs.md#handshakepartytypedef) 
2. See [:material-code-brackets: HandshakeStateType](./literals.md#handshakestatetype) 
3. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
4. See [:material-code-braces: HandshakeResourceTypeDef](./type_defs.md#handshakeresourcetypedef) 
## ListAWSServiceAccessForOrganizationRequestListAWSServiceAccessForOrganizationPaginateTypeDef

```python
# ListAWSServiceAccessForOrganizationRequestListAWSServiceAccessForOrganizationPaginateTypeDef definition

class ListAWSServiceAccessForOrganizationRequestListAWSServiceAccessForOrganizationPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountsForParentRequestListAccountsForParentPaginateTypeDef

```python
# ListAccountsForParentRequestListAccountsForParentPaginateTypeDef definition

class ListAccountsForParentRequestListAccountsForParentPaginateTypeDef(TypedDict):
    ParentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountsRequestListAccountsPaginateTypeDef

```python
# ListAccountsRequestListAccountsPaginateTypeDef definition

class ListAccountsRequestListAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChildrenRequestListChildrenPaginateTypeDef

```python
# ListChildrenRequestListChildrenPaginateTypeDef definition

class ListChildrenRequestListChildrenPaginateTypeDef(TypedDict):
    ParentId: str,
    ChildType: ChildTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCreateAccountStatusRequestListCreateAccountStatusPaginateTypeDef

```python
# ListCreateAccountStatusRequestListCreateAccountStatusPaginateTypeDef definition

class ListCreateAccountStatusRequestListCreateAccountStatusPaginateTypeDef(TypedDict):
    States: NotRequired[Sequence[CreateAccountStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CreateAccountStateType](./literals.md#createaccountstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDelegatedAdministratorsRequestListDelegatedAdministratorsPaginateTypeDef

```python
# ListDelegatedAdministratorsRequestListDelegatedAdministratorsPaginateTypeDef definition

class ListDelegatedAdministratorsRequestListDelegatedAdministratorsPaginateTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDelegatedServicesForAccountRequestListDelegatedServicesForAccountPaginateTypeDef

```python
# ListDelegatedServicesForAccountRequestListDelegatedServicesForAccountPaginateTypeDef definition

class ListDelegatedServicesForAccountRequestListDelegatedServicesForAccountPaginateTypeDef(TypedDict):
    AccountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHandshakesForAccountRequestListHandshakesForAccountPaginateTypeDef

```python
# ListHandshakesForAccountRequestListHandshakesForAccountPaginateTypeDef definition

class ListHandshakesForAccountRequestListHandshakesForAccountPaginateTypeDef(TypedDict):
    Filter: NotRequired[HandshakeFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHandshakesForOrganizationRequestListHandshakesForOrganizationPaginateTypeDef

```python
# ListHandshakesForOrganizationRequestListHandshakesForOrganizationPaginateTypeDef definition

class ListHandshakesForOrganizationRequestListHandshakesForOrganizationPaginateTypeDef(TypedDict):
    Filter: NotRequired[HandshakeFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationalUnitsForParentRequestListOrganizationalUnitsForParentPaginateTypeDef

```python
# ListOrganizationalUnitsForParentRequestListOrganizationalUnitsForParentPaginateTypeDef definition

class ListOrganizationalUnitsForParentRequestListOrganizationalUnitsForParentPaginateTypeDef(TypedDict):
    ParentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListParentsRequestListParentsPaginateTypeDef

```python
# ListParentsRequestListParentsPaginateTypeDef definition

class ListParentsRequestListParentsPaginateTypeDef(TypedDict):
    ChildId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesForTargetRequestListPoliciesForTargetPaginateTypeDef

```python
# ListPoliciesForTargetRequestListPoliciesForTargetPaginateTypeDef definition

class ListPoliciesForTargetRequestListPoliciesForTargetPaginateTypeDef(TypedDict):
    TargetId: str,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesRequestListPoliciesPaginateTypeDef

```python
# ListPoliciesRequestListPoliciesPaginateTypeDef definition

class ListPoliciesRequestListPoliciesPaginateTypeDef(TypedDict):
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRootsRequestListRootsPaginateTypeDef

```python
# ListRootsRequestListRootsPaginateTypeDef definition

class ListRootsRequestListRootsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef

```python
# ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef definition

class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(TypedDict):
    PolicyId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListParentsResponseTypeDef

```python
# ListParentsResponseTypeDef definition

class ListParentsResponseTypeDef(TypedDict):
    Parents: List[ParentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParentTypeDef](./type_defs.md#parenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesForTargetResponseTypeDef

```python
# ListPoliciesForTargetResponseTypeDef definition

class ListPoliciesForTargetResponseTypeDef(TypedDict):
    Policies: List[PolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicySummaryTypeDef](./type_defs.md#policysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPoliciesResponseTypeDef

```python
# ListPoliciesResponseTypeDef definition

class ListPoliciesResponseTypeDef(TypedDict):
    Policies: List[PolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicySummaryTypeDef](./type_defs.md#policysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    PolicySummary: NotRequired[PolicySummaryTypeDef],  # (1)
    Content: NotRequired[str],
```

1. See [:material-code-braces: PolicySummaryTypeDef](./type_defs.md#policysummarytypedef) 
## ListTargetsForPolicyResponseTypeDef

```python
# ListTargetsForPolicyResponseTypeDef definition

class ListTargetsForPolicyResponseTypeDef(TypedDict):
    Targets: List[PolicyTargetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyTargetSummaryTypeDef](./type_defs.md#policytargetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrganizationTypeDef

```python
# OrganizationTypeDef definition

class OrganizationTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    FeatureSet: NotRequired[OrganizationFeatureSetType],  # (1)
    MasterAccountArn: NotRequired[str],
    MasterAccountId: NotRequired[str],
    MasterAccountEmail: NotRequired[str],
    AvailablePolicyTypes: NotRequired[List[PolicyTypeSummaryTypeDef]],  # (2)
```

1. See [:material-code-brackets: OrganizationFeatureSetType](./literals.md#organizationfeaturesettype) 
2. See [:material-code-braces: PolicyTypeSummaryTypeDef](./type_defs.md#policytypesummarytypedef) 
## RootTypeDef

```python
# RootTypeDef definition

class RootTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    PolicyTypes: NotRequired[List[PolicyTypeSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyTypeSummaryTypeDef](./type_defs.md#policytypesummarytypedef) 
## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    ResourcePolicySummary: NotRequired[ResourcePolicySummaryTypeDef],  # (1)
    Content: NotRequired[str],
```

1. See [:material-code-braces: ResourcePolicySummaryTypeDef](./type_defs.md#resourcepolicysummarytypedef) 
## ListHandshakesForAccountResponsePaginatorTypeDef

```python
# ListHandshakesForAccountResponsePaginatorTypeDef definition

class ListHandshakesForAccountResponsePaginatorTypeDef(TypedDict):
    Handshakes: List[HandshakePaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HandshakePaginatorTypeDef](./type_defs.md#handshakepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHandshakesForOrganizationResponsePaginatorTypeDef

```python
# ListHandshakesForOrganizationResponsePaginatorTypeDef definition

class ListHandshakesForOrganizationResponsePaginatorTypeDef(TypedDict):
    Handshakes: List[HandshakePaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HandshakePaginatorTypeDef](./type_defs.md#handshakepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptHandshakeResponseTypeDef

```python
# AcceptHandshakeResponseTypeDef definition

class AcceptHandshakeResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelHandshakeResponseTypeDef

```python
# CancelHandshakeResponseTypeDef definition

class CancelHandshakeResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeclineHandshakeResponseTypeDef

```python
# DeclineHandshakeResponseTypeDef definition

class DeclineHandshakeResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHandshakeResponseTypeDef

```python
# DescribeHandshakeResponseTypeDef definition

class DescribeHandshakeResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableAllFeaturesResponseTypeDef

```python
# EnableAllFeaturesResponseTypeDef definition

class EnableAllFeaturesResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InviteAccountToOrganizationResponseTypeDef

```python
# InviteAccountToOrganizationResponseTypeDef definition

class InviteAccountToOrganizationResponseTypeDef(TypedDict):
    Handshake: HandshakeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHandshakesForAccountResponseTypeDef

```python
# ListHandshakesForAccountResponseTypeDef definition

class ListHandshakesForAccountResponseTypeDef(TypedDict):
    Handshakes: List[HandshakeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHandshakesForOrganizationResponseTypeDef

```python
# ListHandshakesForOrganizationResponseTypeDef definition

class ListHandshakesForOrganizationResponseTypeDef(TypedDict):
    Handshakes: List[HandshakeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HandshakeTypeDef](./type_defs.md#handshaketypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePolicyResponseTypeDef

```python
# CreatePolicyResponseTypeDef definition

class CreatePolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePolicyResponseTypeDef

```python
# DescribePolicyResponseTypeDef definition

class DescribePolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePolicyResponseTypeDef

```python
# UpdatePolicyResponseTypeDef definition

class UpdatePolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOrganizationResponseTypeDef

```python
# CreateOrganizationResponseTypeDef definition

class CreateOrganizationResponseTypeDef(TypedDict):
    Organization: OrganizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationTypeDef](./type_defs.md#organizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationResponseTypeDef

```python
# DescribeOrganizationResponseTypeDef definition

class DescribeOrganizationResponseTypeDef(TypedDict):
    Organization: OrganizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationTypeDef](./type_defs.md#organizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisablePolicyTypeResponseTypeDef

```python
# DisablePolicyTypeResponseTypeDef definition

class DisablePolicyTypeResponseTypeDef(TypedDict):
    Root: RootTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RootTypeDef](./type_defs.md#roottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnablePolicyTypeResponseTypeDef

```python
# EnablePolicyTypeResponseTypeDef definition

class EnablePolicyTypeResponseTypeDef(TypedDict):
    Root: RootTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RootTypeDef](./type_defs.md#roottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRootsResponseTypeDef

```python
# ListRootsResponseTypeDef definition

class ListRootsResponseTypeDef(TypedDict):
    Roots: List[RootTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RootTypeDef](./type_defs.md#roottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePolicyResponseTypeDef

```python
# DescribeResourcePolicyResponseTypeDef definition

class DescribeResourcePolicyResponseTypeDef(TypedDict):
    ResourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    ResourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
