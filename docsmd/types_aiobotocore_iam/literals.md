# Literals

> [Index](../README.md) > [IAM](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## AccessAdvisorUsageGranularityTypeType

```python
# AccessAdvisorUsageGranularityTypeType usage example

from types_aiobotocore_iam.literals import AccessAdvisorUsageGranularityTypeType

def get_value() -> AccessAdvisorUsageGranularityTypeType:
    return "ACTION_LEVEL"
```

```python
# AccessAdvisorUsageGranularityTypeType definition

AccessAdvisorUsageGranularityTypeType = Literal[
    "ACTION_LEVEL",
    "SERVICE_LEVEL",
]
```
## ContextKeyTypeEnumType

```python
# ContextKeyTypeEnumType usage example

from types_aiobotocore_iam.literals import ContextKeyTypeEnumType

def get_value() -> ContextKeyTypeEnumType:
    return "binary"
```

```python
# ContextKeyTypeEnumType definition

ContextKeyTypeEnumType = Literal[
    "binary",
    "binaryList",
    "boolean",
    "booleanList",
    "date",
    "dateList",
    "ip",
    "ipList",
    "numeric",
    "numericList",
    "string",
    "stringList",
]
```
## DeletionTaskStatusTypeType

```python
# DeletionTaskStatusTypeType usage example

from types_aiobotocore_iam.literals import DeletionTaskStatusTypeType

def get_value() -> DeletionTaskStatusTypeType:
    return "FAILED"
```

```python
# DeletionTaskStatusTypeType definition

DeletionTaskStatusTypeType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "NOT_STARTED",
    "SUCCEEDED",
]
```
## EntityTypeType

```python
# EntityTypeType usage example

from types_aiobotocore_iam.literals import EntityTypeType

def get_value() -> EntityTypeType:
    return "AWSManagedPolicy"
```

```python
# EntityTypeType definition

EntityTypeType = Literal[
    "AWSManagedPolicy",
    "Group",
    "LocalManagedPolicy",
    "Role",
    "User",
]
```
## GetAccountAuthorizationDetailsPaginatorName

```python
# GetAccountAuthorizationDetailsPaginatorName usage example

from types_aiobotocore_iam.literals import GetAccountAuthorizationDetailsPaginatorName

def get_value() -> GetAccountAuthorizationDetailsPaginatorName:
    return "get_account_authorization_details"
```

```python
# GetAccountAuthorizationDetailsPaginatorName definition

GetAccountAuthorizationDetailsPaginatorName = Literal[
    "get_account_authorization_details",
]
```
## GetGroupPaginatorName

```python
# GetGroupPaginatorName usage example

from types_aiobotocore_iam.literals import GetGroupPaginatorName

def get_value() -> GetGroupPaginatorName:
    return "get_group"
```

```python
# GetGroupPaginatorName definition

GetGroupPaginatorName = Literal[
    "get_group",
]
```
## InstanceProfileExistsWaiterName

```python
# InstanceProfileExistsWaiterName usage example

from types_aiobotocore_iam.literals import InstanceProfileExistsWaiterName

def get_value() -> InstanceProfileExistsWaiterName:
    return "instance_profile_exists"
```

```python
# InstanceProfileExistsWaiterName definition

InstanceProfileExistsWaiterName = Literal[
    "instance_profile_exists",
]
```
## ListAccessKeysPaginatorName

```python
# ListAccessKeysPaginatorName usage example

from types_aiobotocore_iam.literals import ListAccessKeysPaginatorName

def get_value() -> ListAccessKeysPaginatorName:
    return "list_access_keys"
```

```python
# ListAccessKeysPaginatorName definition

ListAccessKeysPaginatorName = Literal[
    "list_access_keys",
]
```
## ListAccountAliasesPaginatorName

```python
# ListAccountAliasesPaginatorName usage example

from types_aiobotocore_iam.literals import ListAccountAliasesPaginatorName

def get_value() -> ListAccountAliasesPaginatorName:
    return "list_account_aliases"
```

```python
# ListAccountAliasesPaginatorName definition

ListAccountAliasesPaginatorName = Literal[
    "list_account_aliases",
]
```
## ListAttachedGroupPoliciesPaginatorName

```python
# ListAttachedGroupPoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListAttachedGroupPoliciesPaginatorName

def get_value() -> ListAttachedGroupPoliciesPaginatorName:
    return "list_attached_group_policies"
```

```python
# ListAttachedGroupPoliciesPaginatorName definition

ListAttachedGroupPoliciesPaginatorName = Literal[
    "list_attached_group_policies",
]
```
## ListAttachedRolePoliciesPaginatorName

```python
# ListAttachedRolePoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListAttachedRolePoliciesPaginatorName

def get_value() -> ListAttachedRolePoliciesPaginatorName:
    return "list_attached_role_policies"
```

```python
# ListAttachedRolePoliciesPaginatorName definition

ListAttachedRolePoliciesPaginatorName = Literal[
    "list_attached_role_policies",
]
```
## ListAttachedUserPoliciesPaginatorName

```python
# ListAttachedUserPoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListAttachedUserPoliciesPaginatorName

def get_value() -> ListAttachedUserPoliciesPaginatorName:
    return "list_attached_user_policies"
```

```python
# ListAttachedUserPoliciesPaginatorName definition

ListAttachedUserPoliciesPaginatorName = Literal[
    "list_attached_user_policies",
]
```
## ListEntitiesForPolicyPaginatorName

```python
# ListEntitiesForPolicyPaginatorName usage example

from types_aiobotocore_iam.literals import ListEntitiesForPolicyPaginatorName

def get_value() -> ListEntitiesForPolicyPaginatorName:
    return "list_entities_for_policy"
```

```python
# ListEntitiesForPolicyPaginatorName definition

ListEntitiesForPolicyPaginatorName = Literal[
    "list_entities_for_policy",
]
```
## ListGroupPoliciesPaginatorName

```python
# ListGroupPoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListGroupPoliciesPaginatorName

def get_value() -> ListGroupPoliciesPaginatorName:
    return "list_group_policies"
```

```python
# ListGroupPoliciesPaginatorName definition

ListGroupPoliciesPaginatorName = Literal[
    "list_group_policies",
]
```
## ListGroupsForUserPaginatorName

```python
# ListGroupsForUserPaginatorName usage example

from types_aiobotocore_iam.literals import ListGroupsForUserPaginatorName

def get_value() -> ListGroupsForUserPaginatorName:
    return "list_groups_for_user"
```

```python
# ListGroupsForUserPaginatorName definition

ListGroupsForUserPaginatorName = Literal[
    "list_groups_for_user",
]
```
## ListGroupsPaginatorName

```python
# ListGroupsPaginatorName usage example

from types_aiobotocore_iam.literals import ListGroupsPaginatorName

def get_value() -> ListGroupsPaginatorName:
    return "list_groups"
```

```python
# ListGroupsPaginatorName definition

ListGroupsPaginatorName = Literal[
    "list_groups",
]
```
## ListInstanceProfileTagsPaginatorName

```python
# ListInstanceProfileTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListInstanceProfileTagsPaginatorName

def get_value() -> ListInstanceProfileTagsPaginatorName:
    return "list_instance_profile_tags"
```

```python
# ListInstanceProfileTagsPaginatorName definition

ListInstanceProfileTagsPaginatorName = Literal[
    "list_instance_profile_tags",
]
```
## ListInstanceProfilesForRolePaginatorName

```python
# ListInstanceProfilesForRolePaginatorName usage example

from types_aiobotocore_iam.literals import ListInstanceProfilesForRolePaginatorName

def get_value() -> ListInstanceProfilesForRolePaginatorName:
    return "list_instance_profiles_for_role"
```

```python
# ListInstanceProfilesForRolePaginatorName definition

ListInstanceProfilesForRolePaginatorName = Literal[
    "list_instance_profiles_for_role",
]
```
## ListInstanceProfilesPaginatorName

```python
# ListInstanceProfilesPaginatorName usage example

from types_aiobotocore_iam.literals import ListInstanceProfilesPaginatorName

def get_value() -> ListInstanceProfilesPaginatorName:
    return "list_instance_profiles"
```

```python
# ListInstanceProfilesPaginatorName definition

ListInstanceProfilesPaginatorName = Literal[
    "list_instance_profiles",
]
```
## ListMFADeviceTagsPaginatorName

```python
# ListMFADeviceTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListMFADeviceTagsPaginatorName

def get_value() -> ListMFADeviceTagsPaginatorName:
    return "list_mfa_device_tags"
```

```python
# ListMFADeviceTagsPaginatorName definition

ListMFADeviceTagsPaginatorName = Literal[
    "list_mfa_device_tags",
]
```
## ListMFADevicesPaginatorName

```python
# ListMFADevicesPaginatorName usage example

from types_aiobotocore_iam.literals import ListMFADevicesPaginatorName

def get_value() -> ListMFADevicesPaginatorName:
    return "list_mfa_devices"
```

```python
# ListMFADevicesPaginatorName definition

ListMFADevicesPaginatorName = Literal[
    "list_mfa_devices",
]
```
## ListOpenIDConnectProviderTagsPaginatorName

```python
# ListOpenIDConnectProviderTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListOpenIDConnectProviderTagsPaginatorName

def get_value() -> ListOpenIDConnectProviderTagsPaginatorName:
    return "list_open_id_connect_provider_tags"
```

```python
# ListOpenIDConnectProviderTagsPaginatorName definition

ListOpenIDConnectProviderTagsPaginatorName = Literal[
    "list_open_id_connect_provider_tags",
]
```
## ListPoliciesPaginatorName

```python
# ListPoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListPoliciesPaginatorName

def get_value() -> ListPoliciesPaginatorName:
    return "list_policies"
```

```python
# ListPoliciesPaginatorName definition

ListPoliciesPaginatorName = Literal[
    "list_policies",
]
```
## ListPolicyTagsPaginatorName

```python
# ListPolicyTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListPolicyTagsPaginatorName

def get_value() -> ListPolicyTagsPaginatorName:
    return "list_policy_tags"
```

```python
# ListPolicyTagsPaginatorName definition

ListPolicyTagsPaginatorName = Literal[
    "list_policy_tags",
]
```
## ListPolicyVersionsPaginatorName

```python
# ListPolicyVersionsPaginatorName usage example

from types_aiobotocore_iam.literals import ListPolicyVersionsPaginatorName

def get_value() -> ListPolicyVersionsPaginatorName:
    return "list_policy_versions"
```

```python
# ListPolicyVersionsPaginatorName definition

ListPolicyVersionsPaginatorName = Literal[
    "list_policy_versions",
]
```
## ListRolePoliciesPaginatorName

```python
# ListRolePoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListRolePoliciesPaginatorName

def get_value() -> ListRolePoliciesPaginatorName:
    return "list_role_policies"
```

```python
# ListRolePoliciesPaginatorName definition

ListRolePoliciesPaginatorName = Literal[
    "list_role_policies",
]
```
## ListRoleTagsPaginatorName

```python
# ListRoleTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListRoleTagsPaginatorName

def get_value() -> ListRoleTagsPaginatorName:
    return "list_role_tags"
```

```python
# ListRoleTagsPaginatorName definition

ListRoleTagsPaginatorName = Literal[
    "list_role_tags",
]
```
## ListRolesPaginatorName

```python
# ListRolesPaginatorName usage example

from types_aiobotocore_iam.literals import ListRolesPaginatorName

def get_value() -> ListRolesPaginatorName:
    return "list_roles"
```

```python
# ListRolesPaginatorName definition

ListRolesPaginatorName = Literal[
    "list_roles",
]
```
## ListSAMLProviderTagsPaginatorName

```python
# ListSAMLProviderTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListSAMLProviderTagsPaginatorName

def get_value() -> ListSAMLProviderTagsPaginatorName:
    return "list_saml_provider_tags"
```

```python
# ListSAMLProviderTagsPaginatorName definition

ListSAMLProviderTagsPaginatorName = Literal[
    "list_saml_provider_tags",
]
```
## ListSSHPublicKeysPaginatorName

```python
# ListSSHPublicKeysPaginatorName usage example

from types_aiobotocore_iam.literals import ListSSHPublicKeysPaginatorName

def get_value() -> ListSSHPublicKeysPaginatorName:
    return "list_ssh_public_keys"
```

```python
# ListSSHPublicKeysPaginatorName definition

ListSSHPublicKeysPaginatorName = Literal[
    "list_ssh_public_keys",
]
```
## ListServerCertificateTagsPaginatorName

```python
# ListServerCertificateTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListServerCertificateTagsPaginatorName

def get_value() -> ListServerCertificateTagsPaginatorName:
    return "list_server_certificate_tags"
```

```python
# ListServerCertificateTagsPaginatorName definition

ListServerCertificateTagsPaginatorName = Literal[
    "list_server_certificate_tags",
]
```
## ListServerCertificatesPaginatorName

```python
# ListServerCertificatesPaginatorName usage example

from types_aiobotocore_iam.literals import ListServerCertificatesPaginatorName

def get_value() -> ListServerCertificatesPaginatorName:
    return "list_server_certificates"
```

```python
# ListServerCertificatesPaginatorName definition

ListServerCertificatesPaginatorName = Literal[
    "list_server_certificates",
]
```
## ListSigningCertificatesPaginatorName

```python
# ListSigningCertificatesPaginatorName usage example

from types_aiobotocore_iam.literals import ListSigningCertificatesPaginatorName

def get_value() -> ListSigningCertificatesPaginatorName:
    return "list_signing_certificates"
```

```python
# ListSigningCertificatesPaginatorName definition

ListSigningCertificatesPaginatorName = Literal[
    "list_signing_certificates",
]
```
## ListUserPoliciesPaginatorName

```python
# ListUserPoliciesPaginatorName usage example

from types_aiobotocore_iam.literals import ListUserPoliciesPaginatorName

def get_value() -> ListUserPoliciesPaginatorName:
    return "list_user_policies"
```

```python
# ListUserPoliciesPaginatorName definition

ListUserPoliciesPaginatorName = Literal[
    "list_user_policies",
]
```
## ListUserTagsPaginatorName

```python
# ListUserTagsPaginatorName usage example

from types_aiobotocore_iam.literals import ListUserTagsPaginatorName

def get_value() -> ListUserTagsPaginatorName:
    return "list_user_tags"
```

```python
# ListUserTagsPaginatorName definition

ListUserTagsPaginatorName = Literal[
    "list_user_tags",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example

from types_aiobotocore_iam.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition

ListUsersPaginatorName = Literal[
    "list_users",
]
```
## ListVirtualMFADevicesPaginatorName

```python
# ListVirtualMFADevicesPaginatorName usage example

from types_aiobotocore_iam.literals import ListVirtualMFADevicesPaginatorName

def get_value() -> ListVirtualMFADevicesPaginatorName:
    return "list_virtual_mfa_devices"
```

```python
# ListVirtualMFADevicesPaginatorName definition

ListVirtualMFADevicesPaginatorName = Literal[
    "list_virtual_mfa_devices",
]
```
## PermissionsBoundaryAttachmentTypeType

```python
# PermissionsBoundaryAttachmentTypeType usage example

from types_aiobotocore_iam.literals import PermissionsBoundaryAttachmentTypeType

def get_value() -> PermissionsBoundaryAttachmentTypeType:
    return "PermissionsBoundaryPolicy"
```

```python
# PermissionsBoundaryAttachmentTypeType definition

PermissionsBoundaryAttachmentTypeType = Literal[
    "PermissionsBoundaryPolicy",
]
```
## PolicyEvaluationDecisionTypeType

```python
# PolicyEvaluationDecisionTypeType usage example

from types_aiobotocore_iam.literals import PolicyEvaluationDecisionTypeType

def get_value() -> PolicyEvaluationDecisionTypeType:
    return "allowed"
```

```python
# PolicyEvaluationDecisionTypeType definition

PolicyEvaluationDecisionTypeType = Literal[
    "allowed",
    "explicitDeny",
    "implicitDeny",
]
```
## PolicyExistsWaiterName

```python
# PolicyExistsWaiterName usage example

from types_aiobotocore_iam.literals import PolicyExistsWaiterName

def get_value() -> PolicyExistsWaiterName:
    return "policy_exists"
```

```python
# PolicyExistsWaiterName definition

PolicyExistsWaiterName = Literal[
    "policy_exists",
]
```
## PolicySourceTypeType

```python
# PolicySourceTypeType usage example

from types_aiobotocore_iam.literals import PolicySourceTypeType

def get_value() -> PolicySourceTypeType:
    return "aws-managed"
```

```python
# PolicySourceTypeType definition

PolicySourceTypeType = Literal[
    "aws-managed",
    "group",
    "none",
    "resource",
    "role",
    "user",
    "user-managed",
]
```
## PolicyUsageTypeType

```python
# PolicyUsageTypeType usage example

from types_aiobotocore_iam.literals import PolicyUsageTypeType

def get_value() -> PolicyUsageTypeType:
    return "PermissionsBoundary"
```

```python
# PolicyUsageTypeType definition

PolicyUsageTypeType = Literal[
    "PermissionsBoundary",
    "PermissionsPolicy",
]
```
## ReportFormatTypeType

```python
# ReportFormatTypeType usage example

from types_aiobotocore_iam.literals import ReportFormatTypeType

def get_value() -> ReportFormatTypeType:
    return "text/csv"
```

```python
# ReportFormatTypeType definition

ReportFormatTypeType = Literal[
    "text/csv",
]
```
## ReportStateTypeType

```python
# ReportStateTypeType usage example

from types_aiobotocore_iam.literals import ReportStateTypeType

def get_value() -> ReportStateTypeType:
    return "COMPLETE"
```

```python
# ReportStateTypeType definition

ReportStateTypeType = Literal[
    "COMPLETE",
    "INPROGRESS",
    "STARTED",
]
```
## RoleExistsWaiterName

```python
# RoleExistsWaiterName usage example

from types_aiobotocore_iam.literals import RoleExistsWaiterName

def get_value() -> RoleExistsWaiterName:
    return "role_exists"
```

```python
# RoleExistsWaiterName definition

RoleExistsWaiterName = Literal[
    "role_exists",
]
```
## SimulateCustomPolicyPaginatorName

```python
# SimulateCustomPolicyPaginatorName usage example

from types_aiobotocore_iam.literals import SimulateCustomPolicyPaginatorName

def get_value() -> SimulateCustomPolicyPaginatorName:
    return "simulate_custom_policy"
```

```python
# SimulateCustomPolicyPaginatorName definition

SimulateCustomPolicyPaginatorName = Literal[
    "simulate_custom_policy",
]
```
## SimulatePrincipalPolicyPaginatorName

```python
# SimulatePrincipalPolicyPaginatorName usage example

from types_aiobotocore_iam.literals import SimulatePrincipalPolicyPaginatorName

def get_value() -> SimulatePrincipalPolicyPaginatorName:
    return "simulate_principal_policy"
```

```python
# SimulatePrincipalPolicyPaginatorName definition

SimulatePrincipalPolicyPaginatorName = Literal[
    "simulate_principal_policy",
]
```
## UserExistsWaiterName

```python
# UserExistsWaiterName usage example

from types_aiobotocore_iam.literals import UserExistsWaiterName

def get_value() -> UserExistsWaiterName:
    return "user_exists"
```

```python
# UserExistsWaiterName definition

UserExistsWaiterName = Literal[
    "user_exists",
]
```
## assignmentStatusTypeType

```python
# assignmentStatusTypeType usage example

from types_aiobotocore_iam.literals import assignmentStatusTypeType

def get_value() -> assignmentStatusTypeType:
    return "Any"
```

```python
# assignmentStatusTypeType definition

assignmentStatusTypeType = Literal[
    "Any",
    "Assigned",
    "Unassigned",
]
```
## encodingTypeType

```python
# encodingTypeType usage example

from types_aiobotocore_iam.literals import encodingTypeType

def get_value() -> encodingTypeType:
    return "PEM"
```

```python
# encodingTypeType definition

encodingTypeType = Literal[
    "PEM",
    "SSH",
]
```
## globalEndpointTokenVersionType

```python
# globalEndpointTokenVersionType usage example

from types_aiobotocore_iam.literals import globalEndpointTokenVersionType

def get_value() -> globalEndpointTokenVersionType:
    return "v1Token"
```

```python
# globalEndpointTokenVersionType definition

globalEndpointTokenVersionType = Literal[
    "v1Token",
    "v2Token",
]
```
## jobStatusTypeType

```python
# jobStatusTypeType usage example

from types_aiobotocore_iam.literals import jobStatusTypeType

def get_value() -> jobStatusTypeType:
    return "COMPLETED"
```

```python
# jobStatusTypeType definition

jobStatusTypeType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## policyOwnerEntityTypeType

```python
# policyOwnerEntityTypeType usage example

from types_aiobotocore_iam.literals import policyOwnerEntityTypeType

def get_value() -> policyOwnerEntityTypeType:
    return "GROUP"
```

```python
# policyOwnerEntityTypeType definition

policyOwnerEntityTypeType = Literal[
    "GROUP",
    "ROLE",
    "USER",
]
```
## policyScopeTypeType

```python
# policyScopeTypeType usage example

from types_aiobotocore_iam.literals import policyScopeTypeType

def get_value() -> policyScopeTypeType:
    return "AWS"
```

```python
# policyScopeTypeType definition

policyScopeTypeType = Literal[
    "All",
    "AWS",
    "Local",
]
```
## policyTypeType

```python
# policyTypeType usage example

from types_aiobotocore_iam.literals import policyTypeType

def get_value() -> policyTypeType:
    return "INLINE"
```

```python
# policyTypeType definition

policyTypeType = Literal[
    "INLINE",
    "MANAGED",
]
```
## sortKeyTypeType

```python
# sortKeyTypeType usage example

from types_aiobotocore_iam.literals import sortKeyTypeType

def get_value() -> sortKeyTypeType:
    return "LAST_AUTHENTICATED_TIME_ASCENDING"
```

```python
# sortKeyTypeType definition

sortKeyTypeType = Literal[
    "LAST_AUTHENTICATED_TIME_ASCENDING",
    "LAST_AUTHENTICATED_TIME_DESCENDING",
    "SERVICE_NAMESPACE_ASCENDING",
    "SERVICE_NAMESPACE_DESCENDING",
]
```
## statusTypeType

```python
# statusTypeType usage example

from types_aiobotocore_iam.literals import statusTypeType

def get_value() -> statusTypeType:
    return "Active"
```

```python
# statusTypeType definition

statusTypeType = Literal[
    "Active",
    "Inactive",
]
```
## summaryKeyTypeType

```python
# summaryKeyTypeType usage example

from types_aiobotocore_iam.literals import summaryKeyTypeType

def get_value() -> summaryKeyTypeType:
    return "AccessKeysPerUserQuota"
```

```python
# summaryKeyTypeType definition

summaryKeyTypeType = Literal[
    "AccessKeysPerUserQuota",
    "AccountAccessKeysPresent",
    "AccountMFAEnabled",
    "AccountSigningCertificatesPresent",
    "AttachedPoliciesPerGroupQuota",
    "AttachedPoliciesPerRoleQuota",
    "AttachedPoliciesPerUserQuota",
    "GlobalEndpointTokenVersion",
    "GroupPolicySizeQuota",
    "Groups",
    "GroupsPerUserQuota",
    "GroupsQuota",
    "MFADevices",
    "MFADevicesInUse",
    "Policies",
    "PoliciesQuota",
    "PolicySizeQuota",
    "PolicyVersionsInUse",
    "PolicyVersionsInUseQuota",
    "ServerCertificates",
    "ServerCertificatesQuota",
    "SigningCertificatesPerUserQuota",
    "UserPolicySizeQuota",
    "Users",
    "UsersQuota",
    "VersionsPerPolicyQuota",
]
```
## IAMServiceName

```python
# IAMServiceName usage example

from types_aiobotocore_iam.literals import IAMServiceName

def get_value() -> IAMServiceName:
    return "iam"
```

```python
# IAMServiceName definition

IAMServiceName = Literal[
    "iam",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_iam.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_iam.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_iam.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_account_authorization_details"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_account_authorization_details",
    "get_group",
    "list_access_keys",
    "list_account_aliases",
    "list_attached_group_policies",
    "list_attached_role_policies",
    "list_attached_user_policies",
    "list_entities_for_policy",
    "list_group_policies",
    "list_groups",
    "list_groups_for_user",
    "list_instance_profile_tags",
    "list_instance_profiles",
    "list_instance_profiles_for_role",
    "list_mfa_device_tags",
    "list_mfa_devices",
    "list_open_id_connect_provider_tags",
    "list_policies",
    "list_policy_tags",
    "list_policy_versions",
    "list_role_policies",
    "list_role_tags",
    "list_roles",
    "list_saml_provider_tags",
    "list_server_certificate_tags",
    "list_server_certificates",
    "list_signing_certificates",
    "list_ssh_public_keys",
    "list_user_policies",
    "list_user_tags",
    "list_users",
    "list_virtual_mfa_devices",
    "simulate_custom_policy",
    "simulate_principal_policy",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_iam.literals import WaiterName

def get_value() -> WaiterName:
    return "instance_profile_exists"
```

```python
# WaiterName definition

WaiterName = Literal[
    "instance_profile_exists",
    "policy_exists",
    "role_exists",
    "user_exists",
]
```
