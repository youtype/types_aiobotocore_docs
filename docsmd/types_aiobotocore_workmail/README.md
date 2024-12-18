# WorkMail module

> [Index](../README.md) > WorkMail


!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#workmail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkMail` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkMail` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workmail]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workmail]'

# standalone installation
python -m pip install types-aiobotocore-workmail
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workmail
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkMailClient

Type annotations and code completion for  `#!python session.create_client("workmail")` as [WorkMailClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client)

```python
# WorkMailClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmail.client import WorkMailClient


session = get_session()
async with session.create_client("workmail") as client:
    client: WorkMailClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("workmail").get_paginator("...")`.

```python
# ListAliasesPaginator usage example

from types_aiobotocore_workmail.paginator import ListAliasesPaginator

def get_list_aliases_paginator() -> ListAliasesPaginator:
    return client.get_paginator("list_aliases"))
```

- [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- [ListAvailabilityConfigurationsPaginator](./paginators.md#listavailabilityconfigurationspaginator)
- [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListMailboxPermissionsPaginator](./paginators.md#listmailboxpermissionspaginator)
- [ListOrganizationsPaginator](./paginators.md#listorganizationspaginator)
- [ListPersonalAccessTokensPaginator](./paginators.md#listpersonalaccesstokenspaginator)
- [ListResourceDelegatesPaginator](./paginators.md#listresourcedelegatespaginator)
- [ListResourcesPaginator](./paginators.md#listresourcespaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessControlRuleEffectType usage example

from types_aiobotocore_workmail.literals import AccessControlRuleEffectType

def get_value() -> AccessControlRuleEffectType:
    return "ALLOW"
```

- [AccessControlRuleEffectType](./literals.md#accesscontrolruleeffecttype)
- [AccessEffectType](./literals.md#accesseffecttype)
- [AvailabilityProviderTypeType](./literals.md#availabilityprovidertypetype)
- [DnsRecordVerificationStatusType](./literals.md#dnsrecordverificationstatustype)
- [EntityStateType](./literals.md#entitystatetype)
- [EntityTypeType](./literals.md#entitytypetype)
- [FolderNameType](./literals.md#foldernametype)
- [IdentityProviderAuthenticationModeType](./literals.md#identityproviderauthenticationmodetype)
- [ImpersonationRoleTypeType](./literals.md#impersonationroletypetype)
- [ListAliasesPaginatorName](./literals.md#listaliasespaginatorname)
- [ListAvailabilityConfigurationsPaginatorName](./literals.md#listavailabilityconfigurationspaginatorname)
- [ListGroupMembersPaginatorName](./literals.md#listgroupmemberspaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListMailboxPermissionsPaginatorName](./literals.md#listmailboxpermissionspaginatorname)
- [ListOrganizationsPaginatorName](./literals.md#listorganizationspaginatorname)
- [ListPersonalAccessTokensPaginatorName](./literals.md#listpersonalaccesstokenspaginatorname)
- [ListResourceDelegatesPaginatorName](./literals.md#listresourcedelegatespaginatorname)
- [ListResourcesPaginatorName](./literals.md#listresourcespaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [MailboxExportJobStateType](./literals.md#mailboxexportjobstatetype)
- [MemberTypeType](./literals.md#membertypetype)
- [MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype)
- [PermissionTypeType](./literals.md#permissiontypetype)
- [PersonalAccessTokenConfigurationStatusType](./literals.md#personalaccesstokenconfigurationstatustype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RetentionActionType](./literals.md#retentionactiontype)
- [UserRoleType](./literals.md#userroletype)
- [WorkMailServiceName](./literals.md#workmailservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessControlRuleTypeDef](./type_defs.md#accesscontrolruletypedef)
- [AssociateDelegateToResourceRequestRequestTypeDef](./type_defs.md#associatedelegatetoresourcerequestrequesttypedef)
- [AssociateMemberToGroupRequestRequestTypeDef](./type_defs.md#associatemembertogrouprequestrequesttypedef)
- [AssumeImpersonationRoleRequestRequestTypeDef](./type_defs.md#assumeimpersonationrolerequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef)
- [RedactedEwsAvailabilityProviderTypeDef](./type_defs.md#redactedewsavailabilityprovidertypedef)
- [BookingOptionsTypeDef](./type_defs.md#bookingoptionstypedef)
- [CancelMailboxExportJobRequestRequestTypeDef](./type_defs.md#cancelmailboxexportjobrequestrequesttypedef)
- [CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef)
- [EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef)
- [CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef)
- [CreateIdentityCenterApplicationRequestRequestTypeDef](./type_defs.md#createidentitycenterapplicationrequestrequesttypedef)
- [CreateMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#createmobiledeviceaccessrulerequestrequesttypedef)
- [DomainTypeDef](./type_defs.md#domaintypedef)
- [CreateResourceRequestRequestTypeDef](./type_defs.md#createresourcerequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [DelegateTypeDef](./type_defs.md#delegatetypedef)
- [DeleteAccessControlRuleRequestRequestTypeDef](./type_defs.md#deleteaccesscontrolrulerequestrequesttypedef)
- [DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef)
- [DeleteAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#deleteavailabilityconfigurationrequestrequesttypedef)
- [DeleteEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#deleteemailmonitoringconfigurationrequestrequesttypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteIdentityCenterApplicationRequestRequestTypeDef](./type_defs.md#deleteidentitycenterapplicationrequestrequesttypedef)
- [DeleteIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#deleteidentityproviderconfigurationrequestrequesttypedef)
- [DeleteImpersonationRoleRequestRequestTypeDef](./type_defs.md#deleteimpersonationrolerequestrequesttypedef)
- [DeleteMailboxPermissionsRequestRequestTypeDef](./type_defs.md#deletemailboxpermissionsrequestrequesttypedef)
- [DeleteMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#deletemobiledeviceaccessoverriderequestrequesttypedef)
- [DeleteMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#deletemobiledeviceaccessrulerequestrequesttypedef)
- [DeleteOrganizationRequestRequestTypeDef](./type_defs.md#deleteorganizationrequestrequesttypedef)
- [DeletePersonalAccessTokenRequestRequestTypeDef](./type_defs.md#deletepersonalaccesstokenrequestrequesttypedef)
- [DeleteResourceRequestRequestTypeDef](./type_defs.md#deleteresourcerequestrequesttypedef)
- [DeleteRetentionPolicyRequestRequestTypeDef](./type_defs.md#deleteretentionpolicyrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeregisterFromWorkMailRequestRequestTypeDef](./type_defs.md#deregisterfromworkmailrequestrequesttypedef)
- [DeregisterMailDomainRequestRequestTypeDef](./type_defs.md#deregistermaildomainrequestrequesttypedef)
- [DescribeEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#describeemailmonitoringconfigurationrequestrequesttypedef)
- [DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef)
- [DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef)
- [DescribeIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#describeidentityproviderconfigurationrequestrequesttypedef)
- [IdentityCenterConfigurationTypeDef](./type_defs.md#identitycenterconfigurationtypedef)
- [PersonalAccessTokenConfigurationTypeDef](./type_defs.md#personalaccesstokenconfigurationtypedef)
- [DescribeInboundDmarcSettingsRequestRequestTypeDef](./type_defs.md#describeinbounddmarcsettingsrequestrequesttypedef)
- [DescribeMailboxExportJobRequestRequestTypeDef](./type_defs.md#describemailboxexportjobrequestrequesttypedef)
- [DescribeOrganizationRequestRequestTypeDef](./type_defs.md#describeorganizationrequestrequesttypedef)
- [DescribeResourceRequestRequestTypeDef](./type_defs.md#describeresourcerequestrequesttypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DisassociateDelegateFromResourceRequestRequestTypeDef](./type_defs.md#disassociatedelegatefromresourcerequestrequesttypedef)
- [DisassociateMemberFromGroupRequestRequestTypeDef](./type_defs.md#disassociatememberfromgrouprequestrequesttypedef)
- [DnsRecordTypeDef](./type_defs.md#dnsrecordtypedef)
- [FolderConfigurationTypeDef](./type_defs.md#folderconfigurationtypedef)
- [GetAccessControlEffectRequestRequestTypeDef](./type_defs.md#getaccesscontroleffectrequestrequesttypedef)
- [GetDefaultRetentionPolicyRequestRequestTypeDef](./type_defs.md#getdefaultretentionpolicyrequestrequesttypedef)
- [GetImpersonationRoleEffectRequestRequestTypeDef](./type_defs.md#getimpersonationroleeffectrequestrequesttypedef)
- [ImpersonationMatchedRuleTypeDef](./type_defs.md#impersonationmatchedruletypedef)
- [GetImpersonationRoleRequestRequestTypeDef](./type_defs.md#getimpersonationrolerequestrequesttypedef)
- [ImpersonationRuleOutputTypeDef](./type_defs.md#impersonationruleoutputtypedef)
- [GetMailDomainRequestRequestTypeDef](./type_defs.md#getmaildomainrequestrequesttypedef)
- [GetMailboxDetailsRequestRequestTypeDef](./type_defs.md#getmailboxdetailsrequestrequesttypedef)
- [GetMobileDeviceAccessEffectRequestRequestTypeDef](./type_defs.md#getmobiledeviceaccesseffectrequestrequesttypedef)
- [MobileDeviceAccessMatchedRuleTypeDef](./type_defs.md#mobiledeviceaccessmatchedruletypedef)
- [GetMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#getmobiledeviceaccessoverriderequestrequesttypedef)
- [GetPersonalAccessTokenMetadataRequestRequestTypeDef](./type_defs.md#getpersonalaccesstokenmetadatarequestrequesttypedef)
- [GroupIdentifierTypeDef](./type_defs.md#groupidentifiertypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ImpersonationRoleTypeDef](./type_defs.md#impersonationroletypedef)
- [ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef)
- [ListAccessControlRulesRequestRequestTypeDef](./type_defs.md#listaccesscontrolrulesrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef)
- [ListAvailabilityConfigurationsRequestRequestTypeDef](./type_defs.md#listavailabilityconfigurationsrequestrequesttypedef)
- [ListGroupMembersRequestRequestTypeDef](./type_defs.md#listgroupmembersrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [ListGroupsFiltersTypeDef](./type_defs.md#listgroupsfilterstypedef)
- [ListGroupsForEntityFiltersTypeDef](./type_defs.md#listgroupsforentityfilterstypedef)
- [ListImpersonationRolesRequestRequestTypeDef](./type_defs.md#listimpersonationrolesrequestrequesttypedef)
- [ListMailDomainsRequestRequestTypeDef](./type_defs.md#listmaildomainsrequestrequesttypedef)
- [MailDomainSummaryTypeDef](./type_defs.md#maildomainsummarytypedef)
- [ListMailboxExportJobsRequestRequestTypeDef](./type_defs.md#listmailboxexportjobsrequestrequesttypedef)
- [MailboxExportJobTypeDef](./type_defs.md#mailboxexportjobtypedef)
- [ListMailboxPermissionsRequestRequestTypeDef](./type_defs.md#listmailboxpermissionsrequestrequesttypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [ListMobileDeviceAccessOverridesRequestRequestTypeDef](./type_defs.md#listmobiledeviceaccessoverridesrequestrequesttypedef)
- [MobileDeviceAccessOverrideTypeDef](./type_defs.md#mobiledeviceaccessoverridetypedef)
- [ListMobileDeviceAccessRulesRequestRequestTypeDef](./type_defs.md#listmobiledeviceaccessrulesrequestrequesttypedef)
- [MobileDeviceAccessRuleTypeDef](./type_defs.md#mobiledeviceaccessruletypedef)
- [ListOrganizationsRequestRequestTypeDef](./type_defs.md#listorganizationsrequestrequesttypedef)
- [OrganizationSummaryTypeDef](./type_defs.md#organizationsummarytypedef)
- [ListPersonalAccessTokensRequestRequestTypeDef](./type_defs.md#listpersonalaccesstokensrequestrequesttypedef)
- [PersonalAccessTokenSummaryTypeDef](./type_defs.md#personalaccesstokensummarytypedef)
- [ListResourceDelegatesRequestRequestTypeDef](./type_defs.md#listresourcedelegatesrequestrequesttypedef)
- [ListResourcesFiltersTypeDef](./type_defs.md#listresourcesfilterstypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ListUsersFiltersTypeDef](./type_defs.md#listusersfilterstypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [PutAccessControlRuleRequestRequestTypeDef](./type_defs.md#putaccesscontrolrulerequestrequesttypedef)
- [PutEmailMonitoringConfigurationRequestRequestTypeDef](./type_defs.md#putemailmonitoringconfigurationrequestrequesttypedef)
- [PutInboundDmarcSettingsRequestRequestTypeDef](./type_defs.md#putinbounddmarcsettingsrequestrequesttypedef)
- [PutMailboxPermissionsRequestRequestTypeDef](./type_defs.md#putmailboxpermissionsrequestrequesttypedef)
- [PutMobileDeviceAccessOverrideRequestRequestTypeDef](./type_defs.md#putmobiledeviceaccessoverriderequestrequesttypedef)
- [RegisterMailDomainRequestRequestTypeDef](./type_defs.md#registermaildomainrequestrequesttypedef)
- [RegisterToWorkMailRequestRequestTypeDef](./type_defs.md#registertoworkmailrequestrequesttypedef)
- [ResetPasswordRequestRequestTypeDef](./type_defs.md#resetpasswordrequestrequesttypedef)
- [StartMailboxExportJobRequestRequestTypeDef](./type_defs.md#startmailboxexportjobrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDefaultMailDomainRequestRequestTypeDef](./type_defs.md#updatedefaultmaildomainrequestrequesttypedef)
- [UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef)
- [UpdateMailboxQuotaRequestRequestTypeDef](./type_defs.md#updatemailboxquotarequestrequesttypedef)
- [UpdateMobileDeviceAccessRuleRequestRequestTypeDef](./type_defs.md#updatemobiledeviceaccessrulerequestrequesttypedef)
- [UpdatePrimaryEmailAddressRequestRequestTypeDef](./type_defs.md#updateprimaryemailaddressrequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [AssumeImpersonationRoleResponseTypeDef](./type_defs.md#assumeimpersonationroleresponsetypedef)
- [CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)
- [CreateIdentityCenterApplicationResponseTypeDef](./type_defs.md#createidentitycenterapplicationresponsetypedef)
- [CreateImpersonationRoleResponseTypeDef](./type_defs.md#createimpersonationroleresponsetypedef)
- [CreateMobileDeviceAccessRuleResponseTypeDef](./type_defs.md#createmobiledeviceaccessruleresponsetypedef)
- [CreateOrganizationResponseTypeDef](./type_defs.md#createorganizationresponsetypedef)
- [CreateResourceResponseTypeDef](./type_defs.md#createresourceresponsetypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [DeleteOrganizationResponseTypeDef](./type_defs.md#deleteorganizationresponsetypedef)
- [DescribeEmailMonitoringConfigurationResponseTypeDef](./type_defs.md#describeemailmonitoringconfigurationresponsetypedef)
- [DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef)
- [DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef)
- [DescribeInboundDmarcSettingsResponseTypeDef](./type_defs.md#describeinbounddmarcsettingsresponsetypedef)
- [DescribeMailboxExportJobResponseTypeDef](./type_defs.md#describemailboxexportjobresponsetypedef)
- [DescribeOrganizationResponseTypeDef](./type_defs.md#describeorganizationresponsetypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [GetAccessControlEffectResponseTypeDef](./type_defs.md#getaccesscontroleffectresponsetypedef)
- [GetMailboxDetailsResponseTypeDef](./type_defs.md#getmailboxdetailsresponsetypedef)
- [GetMobileDeviceAccessOverrideResponseTypeDef](./type_defs.md#getmobiledeviceaccessoverrideresponsetypedef)
- [GetPersonalAccessTokenMetadataResponseTypeDef](./type_defs.md#getpersonalaccesstokenmetadataresponsetypedef)
- [ListAccessControlRulesResponseTypeDef](./type_defs.md#listaccesscontrolrulesresponsetypedef)
- [ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef)
- [StartMailboxExportJobResponseTypeDef](./type_defs.md#startmailboxexportjobresponsetypedef)
- [TestAvailabilityConfigurationResponseTypeDef](./type_defs.md#testavailabilityconfigurationresponsetypedef)
- [AvailabilityConfigurationTypeDef](./type_defs.md#availabilityconfigurationtypedef)
- [DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef)
- [UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef)
- [CreateAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#createavailabilityconfigurationrequestrequesttypedef)
- [TestAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#testavailabilityconfigurationrequestrequesttypedef)
- [UpdateAvailabilityConfigurationRequestRequestTypeDef](./type_defs.md#updateavailabilityconfigurationrequestrequesttypedef)
- [CreateOrganizationRequestRequestTypeDef](./type_defs.md#createorganizationrequestrequesttypedef)
- [ListResourceDelegatesResponseTypeDef](./type_defs.md#listresourcedelegatesresponsetypedef)
- [DescribeIdentityProviderConfigurationResponseTypeDef](./type_defs.md#describeidentityproviderconfigurationresponsetypedef)
- [PutIdentityProviderConfigurationRequestRequestTypeDef](./type_defs.md#putidentityproviderconfigurationrequestrequesttypedef)
- [GetMailDomainResponseTypeDef](./type_defs.md#getmaildomainresponsetypedef)
- [GetDefaultRetentionPolicyResponseTypeDef](./type_defs.md#getdefaultretentionpolicyresponsetypedef)
- [PutRetentionPolicyRequestRequestTypeDef](./type_defs.md#putretentionpolicyrequestrequesttypedef)
- [GetImpersonationRoleEffectResponseTypeDef](./type_defs.md#getimpersonationroleeffectresponsetypedef)
- [GetImpersonationRoleResponseTypeDef](./type_defs.md#getimpersonationroleresponsetypedef)
- [GetMobileDeviceAccessEffectResponseTypeDef](./type_defs.md#getmobiledeviceaccesseffectresponsetypedef)
- [ListGroupsForEntityResponseTypeDef](./type_defs.md#listgroupsforentityresponsetypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [ListImpersonationRolesResponseTypeDef](./type_defs.md#listimpersonationrolesresponsetypedef)
- [ImpersonationRuleUnionTypeDef](./type_defs.md#impersonationruleuniontypedef)
- [UpdateImpersonationRoleRequestRequestTypeDef](./type_defs.md#updateimpersonationrolerequestrequesttypedef)
- [ListAliasesRequestListAliasesPaginateTypeDef](./type_defs.md#listaliasesrequestlistaliasespaginatetypedef)
- [ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef](./type_defs.md#listavailabilityconfigurationsrequestlistavailabilityconfigurationspaginatetypedef)
- [ListGroupMembersRequestListGroupMembersPaginateTypeDef](./type_defs.md#listgroupmembersrequestlistgroupmemberspaginatetypedef)
- [ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef](./type_defs.md#listmailboxpermissionsrequestlistmailboxpermissionspaginatetypedef)
- [ListOrganizationsRequestListOrganizationsPaginateTypeDef](./type_defs.md#listorganizationsrequestlistorganizationspaginatetypedef)
- [ListPersonalAccessTokensRequestListPersonalAccessTokensPaginateTypeDef](./type_defs.md#listpersonalaccesstokensrequestlistpersonalaccesstokenspaginatetypedef)
- [ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef](./type_defs.md#listresourcedelegatesrequestlistresourcedelegatespaginatetypedef)
- [ListGroupMembersResponseTypeDef](./type_defs.md#listgroupmembersresponsetypedef)
- [ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListGroupsForEntityRequestRequestTypeDef](./type_defs.md#listgroupsforentityrequestrequesttypedef)
- [ListMailDomainsResponseTypeDef](./type_defs.md#listmaildomainsresponsetypedef)
- [ListMailboxExportJobsResponseTypeDef](./type_defs.md#listmailboxexportjobsresponsetypedef)
- [ListMailboxPermissionsResponseTypeDef](./type_defs.md#listmailboxpermissionsresponsetypedef)
- [ListMobileDeviceAccessOverridesResponseTypeDef](./type_defs.md#listmobiledeviceaccessoverridesresponsetypedef)
- [ListMobileDeviceAccessRulesResponseTypeDef](./type_defs.md#listmobiledeviceaccessrulesresponsetypedef)
- [ListOrganizationsResponseTypeDef](./type_defs.md#listorganizationsresponsetypedef)
- [ListPersonalAccessTokensResponseTypeDef](./type_defs.md#listpersonalaccesstokensresponsetypedef)
- [ListResourcesRequestListResourcesPaginateTypeDef](./type_defs.md#listresourcesrequestlistresourcespaginatetypedef)
- [ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef)
- [ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [ListAvailabilityConfigurationsResponseTypeDef](./type_defs.md#listavailabilityconfigurationsresponsetypedef)
- [CreateImpersonationRoleRequestRequestTypeDef](./type_defs.md#createimpersonationrolerequestrequesttypedef)

