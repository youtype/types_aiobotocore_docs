# Type definitions

> [Index](../README.md) > [SSOAdmin](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).



## AccessControlAttributeValueTypeDef

```python
# AccessControlAttributeValueTypeDef definition

class AccessControlAttributeValueTypeDef(TypedDict):
    Source: Sequence[str],
```

## AccountAssignmentOperationStatusMetadataTypeDef

```python
# AccountAssignmentOperationStatusMetadataTypeDef definition

class AccountAssignmentOperationStatusMetadataTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
    RequestId: NotRequired[str],
    CreatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## AccountAssignmentOperationStatusTypeDef

```python
# AccountAssignmentOperationStatusTypeDef definition

class AccountAssignmentOperationStatusTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
    RequestId: NotRequired[str],
    FailureReason: NotRequired[str],
    TargetId: NotRequired[str],
    TargetType: NotRequired[TargetTypeType],  # (2)
    PermissionSetArn: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (3)
    PrincipalId: NotRequired[str],
    CreatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## AccountAssignmentTypeDef

```python
# AccountAssignmentTypeDef definition

class AccountAssignmentTypeDef(TypedDict):
    AccountId: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
    PrincipalId: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## CustomerManagedPolicyReferenceTypeDef

```python
# CustomerManagedPolicyReferenceTypeDef definition

class CustomerManagedPolicyReferenceTypeDef(TypedDict):
    Name: str,
    Path: NotRequired[str],
```

## AttachManagedPolicyToPermissionSetRequestRequestTypeDef

```python
# AttachManagedPolicyToPermissionSetRequestRequestTypeDef definition

class AttachManagedPolicyToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    ManagedPolicyArn: str,
```

## AttachedManagedPolicyTypeDef

```python
# AttachedManagedPolicyTypeDef definition

class AttachedManagedPolicyTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## CreateAccountAssignmentRequestRequestTypeDef

```python
# CreateAccountAssignmentRequestRequestTypeDef definition

class CreateAccountAssignmentRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    TargetId: str,
    TargetType: TargetTypeType,  # (1)
    PermissionSetArn: str,
    PrincipalType: PrincipalTypeType,  # (2)
    PrincipalId: str,
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## PermissionSetTypeDef

```python
# PermissionSetTypeDef definition

class PermissionSetTypeDef(TypedDict):
    Name: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    Description: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    SessionDuration: NotRequired[str],
    RelayState: NotRequired[str],
```

## DeleteAccountAssignmentRequestRequestTypeDef

```python
# DeleteAccountAssignmentRequestRequestTypeDef definition

class DeleteAccountAssignmentRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    TargetId: str,
    TargetType: TargetTypeType,  # (1)
    PermissionSetArn: str,
    PrincipalType: PrincipalTypeType,  # (2)
    PrincipalId: str,
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef

```python
# DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef definition

class DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DeletePermissionSetRequestRequestTypeDef

```python
# DeletePermissionSetRequestRequestTypeDef definition

class DeletePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef

```python
# DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef definition

class DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DescribeAccountAssignmentCreationStatusRequestRequestTypeDef

```python
# DescribeAccountAssignmentCreationStatusRequestRequestTypeDef definition

class DescribeAccountAssignmentCreationStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    AccountAssignmentCreationRequestId: str,
```

## DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef

```python
# DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef definition

class DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    AccountAssignmentDeletionRequestId: str,
```

## DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
```

## DescribePermissionSetProvisioningStatusRequestRequestTypeDef

```python
# DescribePermissionSetProvisioningStatusRequestRequestTypeDef definition

class DescribePermissionSetProvisioningStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ProvisionPermissionSetRequestId: str,
```

## PermissionSetProvisioningStatusTypeDef

```python
# PermissionSetProvisioningStatusTypeDef definition

class PermissionSetProvisioningStatusTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
    RequestId: NotRequired[str],
    AccountId: NotRequired[str],
    PermissionSetArn: NotRequired[str],
    FailureReason: NotRequired[str],
    CreatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## DescribePermissionSetRequestRequestTypeDef

```python
# DescribePermissionSetRequestRequestTypeDef definition

class DescribePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## DetachManagedPolicyFromPermissionSetRequestRequestTypeDef

```python
# DetachManagedPolicyFromPermissionSetRequestRequestTypeDef definition

class DetachManagedPolicyFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    ManagedPolicyArn: str,
```

## GetInlinePolicyForPermissionSetRequestRequestTypeDef

```python
# GetInlinePolicyForPermissionSetRequestRequestTypeDef definition

class GetInlinePolicyForPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef

```python
# GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef definition

class GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
```

## InstanceMetadataTypeDef

```python
# InstanceMetadataTypeDef definition

class InstanceMetadataTypeDef(TypedDict):
    InstanceArn: NotRequired[str],
    IdentityStoreId: NotRequired[str],
```

## OperationStatusFilterTypeDef

```python
# OperationStatusFilterTypeDef definition

class OperationStatusFilterTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountAssignmentsRequestRequestTypeDef

```python
# ListAccountAssignmentsRequestRequestTypeDef definition

class ListAccountAssignmentsRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    AccountId: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAccountsForProvisionedPermissionSetRequestRequestTypeDef

```python
# ListAccountsForProvisionedPermissionSetRequestRequestTypeDef definition

class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
## ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListManagedPoliciesInPermissionSetRequestRequestTypeDef

```python
# ListManagedPoliciesInPermissionSetRequestRequestTypeDef definition

class ListManagedPoliciesInPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PermissionSetProvisioningStatusMetadataTypeDef

```python
# PermissionSetProvisioningStatusMetadataTypeDef definition

class PermissionSetProvisioningStatusMetadataTypeDef(TypedDict):
    Status: NotRequired[StatusValuesType],  # (1)
    RequestId: NotRequired[str],
    CreatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusValuesType](./literals.md#statusvaluestype) 
## ListPermissionSetsProvisionedToAccountRequestRequestTypeDef

```python
# ListPermissionSetsProvisionedToAccountRequestRequestTypeDef definition

class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    AccountId: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
## ListPermissionSetsRequestRequestTypeDef

```python
# ListPermissionSetsRequestRequestTypeDef definition

class ListPermissionSetsRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ResourceArn: str,
    NextToken: NotRequired[str],
```

## ProvisionPermissionSetRequestRequestTypeDef

```python
# ProvisionPermissionSetRequestRequestTypeDef definition

class ProvisionPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    TargetType: ProvisionTargetTypeType,  # (1)
    TargetId: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionTargetTypeType](./literals.md#provisiontargettypetype) 
## PutInlinePolicyToPermissionSetRequestRequestTypeDef

```python
# PutInlinePolicyToPermissionSetRequestRequestTypeDef definition

class PutInlinePolicyToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    InlinePolicy: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdatePermissionSetRequestRequestTypeDef

```python
# UpdatePermissionSetRequestRequestTypeDef definition

class UpdatePermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    Description: NotRequired[str],
    SessionDuration: NotRequired[str],
    RelayState: NotRequired[str],
```

## AccessControlAttributeTypeDef

```python
# AccessControlAttributeTypeDef definition

class AccessControlAttributeTypeDef(TypedDict):
    Key: str,
    Value: AccessControlAttributeValueTypeDef,  # (1)
```

1. See [:material-code-braces: AccessControlAttributeValueTypeDef](./type_defs.md#accesscontrolattributevaluetypedef) 
## AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef

```python
# AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef definition

class AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef

```python
# DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef definition

class DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    CustomerManagedPolicyReference: CustomerManagedPolicyReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## PermissionsBoundaryTypeDef

```python
# PermissionsBoundaryTypeDef definition

class PermissionsBoundaryTypeDef(TypedDict):
    CustomerManagedPolicyReference: NotRequired[CustomerManagedPolicyReferenceTypeDef],  # (1)
    ManagedPolicyArn: NotRequired[str],
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
## CreateAccountAssignmentResponseTypeDef

```python
# CreateAccountAssignmentResponseTypeDef definition

class CreateAccountAssignmentResponseTypeDef(TypedDict):
    AccountAssignmentCreationStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountAssignmentResponseTypeDef

```python
# DeleteAccountAssignmentResponseTypeDef definition

class DeleteAccountAssignmentResponseTypeDef(TypedDict):
    AccountAssignmentDeletionStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAssignmentCreationStatusResponseTypeDef

```python
# DescribeAccountAssignmentCreationStatusResponseTypeDef definition

class DescribeAccountAssignmentCreationStatusResponseTypeDef(TypedDict):
    AccountAssignmentCreationStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAssignmentDeletionStatusResponseTypeDef

```python
# DescribeAccountAssignmentDeletionStatusResponseTypeDef definition

class DescribeAccountAssignmentDeletionStatusResponseTypeDef(TypedDict):
    AccountAssignmentDeletionStatus: AccountAssignmentOperationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusTypeDef](./type_defs.md#accountassignmentoperationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInlinePolicyForPermissionSetResponseTypeDef

```python
# GetInlinePolicyForPermissionSetResponseTypeDef definition

class GetInlinePolicyForPermissionSetResponseTypeDef(TypedDict):
    InlinePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentCreationStatusResponseTypeDef

```python
# ListAccountAssignmentCreationStatusResponseTypeDef definition

class ListAccountAssignmentCreationStatusResponseTypeDef(TypedDict):
    AccountAssignmentsCreationStatus: List[AccountAssignmentOperationStatusMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusMetadataTypeDef](./type_defs.md#accountassignmentoperationstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentDeletionStatusResponseTypeDef

```python
# ListAccountAssignmentDeletionStatusResponseTypeDef definition

class ListAccountAssignmentDeletionStatusResponseTypeDef(TypedDict):
    AccountAssignmentsDeletionStatus: List[AccountAssignmentOperationStatusMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentOperationStatusMetadataTypeDef](./type_defs.md#accountassignmentoperationstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentsResponseTypeDef

```python
# ListAccountAssignmentsResponseTypeDef definition

class ListAccountAssignmentsResponseTypeDef(TypedDict):
    AccountAssignments: List[AccountAssignmentTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAssignmentTypeDef](./type_defs.md#accountassignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsForProvisionedPermissionSetResponseTypeDef

```python
# ListAccountsForProvisionedPermissionSetResponseTypeDef definition

class ListAccountsForProvisionedPermissionSetResponseTypeDef(TypedDict):
    AccountIds: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef(TypedDict):
    CustomerManagedPolicyReferences: List[CustomerManagedPolicyReferenceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomerManagedPolicyReferenceTypeDef](./type_defs.md#customermanagedpolicyreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedPoliciesInPermissionSetResponseTypeDef

```python
# ListManagedPoliciesInPermissionSetResponseTypeDef definition

class ListManagedPoliciesInPermissionSetResponseTypeDef(TypedDict):
    AttachedManagedPolicies: List[AttachedManagedPolicyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachedManagedPolicyTypeDef](./type_defs.md#attachedmanagedpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionSetsProvisionedToAccountResponseTypeDef

```python
# ListPermissionSetsProvisionedToAccountResponseTypeDef definition

class ListPermissionSetsProvisionedToAccountResponseTypeDef(TypedDict):
    NextToken: str,
    PermissionSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionSetsResponseTypeDef

```python
# ListPermissionSetsResponseTypeDef definition

class ListPermissionSetsResponseTypeDef(TypedDict):
    PermissionSets: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePermissionSetRequestRequestTypeDef

```python
# CreatePermissionSetRequestRequestTypeDef definition

class CreatePermissionSetRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceArn: str,
    Description: NotRequired[str],
    SessionDuration: NotRequired[str],
    RelayState: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePermissionSetResponseTypeDef

```python
# CreatePermissionSetResponseTypeDef definition

class CreatePermissionSetResponseTypeDef(TypedDict):
    PermissionSet: PermissionSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetTypeDef](./type_defs.md#permissionsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionSetResponseTypeDef

```python
# DescribePermissionSetResponseTypeDef definition

class DescribePermissionSetResponseTypeDef(TypedDict):
    PermissionSet: PermissionSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetTypeDef](./type_defs.md#permissionsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionSetProvisioningStatusResponseTypeDef

```python
# DescribePermissionSetProvisioningStatusResponseTypeDef definition

class DescribePermissionSetProvisioningStatusResponseTypeDef(TypedDict):
    PermissionSetProvisioningStatus: PermissionSetProvisioningStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetProvisioningStatusTypeDef](./type_defs.md#permissionsetprovisioningstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionPermissionSetResponseTypeDef

```python
# ProvisionPermissionSetResponseTypeDef definition

class ProvisionPermissionSetResponseTypeDef(TypedDict):
    PermissionSetProvisioningStatus: PermissionSetProvisioningStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetProvisioningStatusTypeDef](./type_defs.md#permissionsetprovisioningstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    Instances: List[InstanceMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceMetadataTypeDef](./type_defs.md#instancemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountAssignmentCreationStatusRequestRequestTypeDef

```python
# ListAccountAssignmentCreationStatusRequestRequestTypeDef definition

class ListAccountAssignmentCreationStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListAccountAssignmentDeletionStatusRequestRequestTypeDef

```python
# ListAccountAssignmentDeletionStatusRequestRequestTypeDef definition

class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListPermissionSetProvisioningStatusRequestRequestTypeDef

```python
# ListPermissionSetProvisioningStatusRequestRequestTypeDef definition

class ListPermissionSetProvisioningStatusRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
## ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef

```python
# ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef definition

class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef

```python
# ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef definition

class ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef

```python
# ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef definition

class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(TypedDict):
    InstanceArn: str,
    AccountId: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef

```python
# ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef definition

class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef

```python
# ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef definition

class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestListInstancesPaginateTypeDef

```python
# ListInstancesRequestListInstancesPaginateTypeDef definition

class ListInstancesRequestListInstancesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef

```python
# ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef definition

class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef

```python
# ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef definition

class ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef(TypedDict):
    InstanceArn: str,
    Filter: NotRequired[OperationStatusFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef

```python
# ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef definition

class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(TypedDict):
    InstanceArn: str,
    AccountId: str,
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetsRequestListPermissionSetsPaginateTypeDef

```python
# ListPermissionSetsRequestListPermissionSetsPaginateTypeDef definition

class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(TypedDict):
    InstanceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    InstanceArn: str,
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionSetProvisioningStatusResponseTypeDef

```python
# ListPermissionSetProvisioningStatusResponseTypeDef definition

class ListPermissionSetProvisioningStatusResponseTypeDef(TypedDict):
    PermissionSetsProvisioningStatus: List[PermissionSetProvisioningStatusMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionSetProvisioningStatusMetadataTypeDef](./type_defs.md#permissionsetprovisioningstatusmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceAccessControlAttributeConfigurationTypeDef

```python
# InstanceAccessControlAttributeConfigurationTypeDef definition

class InstanceAccessControlAttributeConfigurationTypeDef(TypedDict):
    AccessControlAttributes: Sequence[AccessControlAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: AccessControlAttributeTypeDef](./type_defs.md#accesscontrolattributetypedef) 
## GetPermissionsBoundaryForPermissionSetResponseTypeDef

```python
# GetPermissionsBoundaryForPermissionSetResponseTypeDef definition

class GetPermissionsBoundaryForPermissionSetResponseTypeDef(TypedDict):
    PermissionsBoundary: PermissionsBoundaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionsBoundaryTypeDef](./type_defs.md#permissionsboundarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef

```python
# PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef definition

class PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    PermissionSetArn: str,
    PermissionsBoundary: PermissionsBoundaryTypeDef,  # (1)
```

1. See [:material-code-braces: PermissionsBoundaryTypeDef](./type_defs.md#permissionsboundarytypedef) 
## CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 
## DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef

```python
# DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef definition

class DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef(TypedDict):
    Status: InstanceAccessControlAttributeConfigurationStatusType,  # (1)
    StatusReason: str,
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: InstanceAccessControlAttributeConfigurationStatusType](./literals.md#instanceaccesscontrolattributeconfigurationstatustype) 
2. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef

```python
# UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef definition

class UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef(TypedDict):
    InstanceArn: str,
    InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceAccessControlAttributeConfigurationTypeDef](./type_defs.md#instanceaccesscontrolattributeconfigurationtypedef) 
