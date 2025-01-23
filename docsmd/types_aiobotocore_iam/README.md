# IAM module

> [Index](../README.md) > IAM


!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#iam)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IAM` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IAM` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iam]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iam]'

# standalone installation
python -m pip install types-aiobotocore-iam
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iam
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IAMClient

Type annotations and code completion for  `#!python session.create_client("iam")` as [IAMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client)

```python
# IAMClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iam.client import IAMClient


session = get_session()
async with session.create_client("iam") as client:
    client: IAMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iam").get_paginator("...")`.

```python
# GetAccountAuthorizationDetailsPaginator usage example

from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator

def get_get_account_authorization_details_paginator() -> GetAccountAuthorizationDetailsPaginator:
    return client.get_paginator("get_account_authorization_details"))
```

- [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
- [GetGroupPaginator](./paginators.md#getgrouppaginator)
- [ListAccessKeysPaginator](./paginators.md#listaccesskeyspaginator)
- [ListAccountAliasesPaginator](./paginators.md#listaccountaliasespaginator)
- [ListAttachedGroupPoliciesPaginator](./paginators.md#listattachedgrouppoliciespaginator)
- [ListAttachedRolePoliciesPaginator](./paginators.md#listattachedrolepoliciespaginator)
- [ListAttachedUserPoliciesPaginator](./paginators.md#listattacheduserpoliciespaginator)
- [ListEntitiesForPolicyPaginator](./paginators.md#listentitiesforpolicypaginator)
- [ListGroupPoliciesPaginator](./paginators.md#listgrouppoliciespaginator)
- [ListGroupsForUserPaginator](./paginators.md#listgroupsforuserpaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListInstanceProfileTagsPaginator](./paginators.md#listinstanceprofiletagspaginator)
- [ListInstanceProfilesForRolePaginator](./paginators.md#listinstanceprofilesforrolepaginator)
- [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
- [ListMFADeviceTagsPaginator](./paginators.md#listmfadevicetagspaginator)
- [ListMFADevicesPaginator](./paginators.md#listmfadevicespaginator)
- [ListOpenIDConnectProviderTagsPaginator](./paginators.md#listopenidconnectprovidertagspaginator)
- [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- [ListPolicyTagsPaginator](./paginators.md#listpolicytagspaginator)
- [ListPolicyVersionsPaginator](./paginators.md#listpolicyversionspaginator)
- [ListRolePoliciesPaginator](./paginators.md#listrolepoliciespaginator)
- [ListRoleTagsPaginator](./paginators.md#listroletagspaginator)
- [ListRolesPaginator](./paginators.md#listrolespaginator)
- [ListSAMLProviderTagsPaginator](./paginators.md#listsamlprovidertagspaginator)
- [ListSSHPublicKeysPaginator](./paginators.md#listsshpublickeyspaginator)
- [ListServerCertificateTagsPaginator](./paginators.md#listservercertificatetagspaginator)
- [ListServerCertificatesPaginator](./paginators.md#listservercertificatespaginator)
- [ListSigningCertificatesPaginator](./paginators.md#listsigningcertificatespaginator)
- [ListUserPoliciesPaginator](./paginators.md#listuserpoliciespaginator)
- [ListUserTagsPaginator](./paginators.md#listusertagspaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)
- [ListVirtualMFADevicesPaginator](./paginators.md#listvirtualmfadevicespaginator)
- [SimulateCustomPolicyPaginator](./paginators.md#simulatecustompolicypaginator)
- [SimulatePrincipalPolicyPaginator](./paginators.md#simulateprincipalpolicypaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("iam").get_waiter("...")`.

```python
# InstanceProfileExistsWaiter usage example

from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter

def get_instance_profile_exists_waiter() -> InstanceProfileExistsWaiter:
    return Session().client("iam").get_waiter("instance_profile_exists")
```

- [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)
- [PolicyExistsWaiter](./waiters.md#policyexistswaiter)
- [RoleExistsWaiter](./waiters.md#roleexistswaiter)
- [UserExistsWaiter](./waiters.md#userexistswaiter)




## IAMServiceResource

Type annotations and code completion for `#!python session.resource("iam")` as
[IAMServiceResource](./service_resource.md#iamserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam/service-resource/index.html)

```python
# IAMServiceResource usage example

from types_aiobotocore_iam.service_resource import IAMServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("iam").*`.

```python
# ServiceResourceGroupsCollection usage example

from types_aiobotocore_iam.service_resource import ServiceResourceGroupsCollection

def get_collection() -> ServiceResourceGroupsCollection:
    return resource.groups
```

- [ServiceResourceGroupsCollection](./service_resource.md#serviceresourcegroupscollection)
- [ServiceResourceInstanceProfilesCollection](./service_resource.md#serviceresourceinstanceprofilescollection)
- [ServiceResourcePoliciesCollection](./service_resource.md#serviceresourcepoliciescollection)
- [ServiceResourceRolesCollection](./service_resource.md#serviceresourcerolescollection)
- [ServiceResourceSamlProvidersCollection](./service_resource.md#serviceresourcesamlproviderscollection)
- [ServiceResourceServerCertificatesCollection](./service_resource.md#serviceresourceservercertificatescollection)
- [ServiceResourceUsersCollection](./service_resource.md#serviceresourceuserscollection)
- [ServiceResourceVirtualMfaDevicesCollection](./service_resource.md#serviceresourcevirtualmfadevicescollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("iam").*`.

```python
# AccessKey usage example

from types_aiobotocore_iam.service_resource import AccessKey

def get_resource() -> AccessKey:
    return resource.AccessKey(...)
```

- [AccessKey](./service_resource.md#accesskey)
- [AccessKeyPair](./service_resource.md#accesskeypair)
- [AccountPasswordPolicy](./service_resource.md#accountpasswordpolicy)
- [AccountSummary](./service_resource.md#accountsummary)
- [AssumeRolePolicy](./service_resource.md#assumerolepolicy)
- [CurrentUser](./service_resource.md#currentuser)
- [Group](./service_resource.md#group)
- [GroupPolicy](./service_resource.md#grouppolicy)
- [InstanceProfile](./service_resource.md#instanceprofile)
- [LoginProfile](./service_resource.md#loginprofile)
- [MfaDevice](./service_resource.md#mfadevice)
- [Policy](./service_resource.md#policy)
- [PolicyVersion](./service_resource.md#policyversion)
- [Role](./service_resource.md#role)
- [RolePolicy](./service_resource.md#rolepolicy)
- [SamlProvider](./service_resource.md#samlprovider)
- [ServerCertificate](./service_resource.md#servercertificate)
- [SigningCertificate](./service_resource.md#signingcertificate)
- [User](./service_resource.md#user)
- [UserPolicy](./service_resource.md#userpolicy)
- [VirtualMfaDevice](./service_resource.md#virtualmfadevice)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessAdvisorUsageGranularityTypeType usage example

from types_aiobotocore_iam.literals import AccessAdvisorUsageGranularityTypeType

def get_value() -> AccessAdvisorUsageGranularityTypeType:
    return "ACTION_LEVEL"
```

- [AccessAdvisorUsageGranularityTypeType](./literals.md#accessadvisorusagegranularitytypetype)
- [AssignmentStatusTypeType](./literals.md#assignmentstatustypetype)
- [ContextKeyTypeEnumType](./literals.md#contextkeytypeenumtype)
- [DeletionTaskStatusTypeType](./literals.md#deletiontaskstatustypetype)
- [EncodingTypeType](./literals.md#encodingtypetype)
- [EntityTypeType](./literals.md#entitytypetype)
- [FeatureTypeType](./literals.md#featuretypetype)
- [GetAccountAuthorizationDetailsPaginatorName](./literals.md#getaccountauthorizationdetailspaginatorname)
- [GetGroupPaginatorName](./literals.md#getgrouppaginatorname)
- [GlobalEndpointTokenVersionType](./literals.md#globalendpointtokenversiontype)
- [InstanceProfileExistsWaiterName](./literals.md#instanceprofileexistswaitername)
- [JobStatusTypeType](./literals.md#jobstatustypetype)
- [ListAccessKeysPaginatorName](./literals.md#listaccesskeyspaginatorname)
- [ListAccountAliasesPaginatorName](./literals.md#listaccountaliasespaginatorname)
- [ListAttachedGroupPoliciesPaginatorName](./literals.md#listattachedgrouppoliciespaginatorname)
- [ListAttachedRolePoliciesPaginatorName](./literals.md#listattachedrolepoliciespaginatorname)
- [ListAttachedUserPoliciesPaginatorName](./literals.md#listattacheduserpoliciespaginatorname)
- [ListEntitiesForPolicyPaginatorName](./literals.md#listentitiesforpolicypaginatorname)
- [ListGroupPoliciesPaginatorName](./literals.md#listgrouppoliciespaginatorname)
- [ListGroupsForUserPaginatorName](./literals.md#listgroupsforuserpaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListInstanceProfileTagsPaginatorName](./literals.md#listinstanceprofiletagspaginatorname)
- [ListInstanceProfilesForRolePaginatorName](./literals.md#listinstanceprofilesforrolepaginatorname)
- [ListInstanceProfilesPaginatorName](./literals.md#listinstanceprofilespaginatorname)
- [ListMFADeviceTagsPaginatorName](./literals.md#listmfadevicetagspaginatorname)
- [ListMFADevicesPaginatorName](./literals.md#listmfadevicespaginatorname)
- [ListOpenIDConnectProviderTagsPaginatorName](./literals.md#listopenidconnectprovidertagspaginatorname)
- [ListPoliciesPaginatorName](./literals.md#listpoliciespaginatorname)
- [ListPolicyTagsPaginatorName](./literals.md#listpolicytagspaginatorname)
- [ListPolicyVersionsPaginatorName](./literals.md#listpolicyversionspaginatorname)
- [ListRolePoliciesPaginatorName](./literals.md#listrolepoliciespaginatorname)
- [ListRoleTagsPaginatorName](./literals.md#listroletagspaginatorname)
- [ListRolesPaginatorName](./literals.md#listrolespaginatorname)
- [ListSAMLProviderTagsPaginatorName](./literals.md#listsamlprovidertagspaginatorname)
- [ListSSHPublicKeysPaginatorName](./literals.md#listsshpublickeyspaginatorname)
- [ListServerCertificateTagsPaginatorName](./literals.md#listservercertificatetagspaginatorname)
- [ListServerCertificatesPaginatorName](./literals.md#listservercertificatespaginatorname)
- [ListSigningCertificatesPaginatorName](./literals.md#listsigningcertificatespaginatorname)
- [ListUserPoliciesPaginatorName](./literals.md#listuserpoliciespaginatorname)
- [ListUserTagsPaginatorName](./literals.md#listusertagspaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [ListVirtualMFADevicesPaginatorName](./literals.md#listvirtualmfadevicespaginatorname)
- [PermissionsBoundaryAttachmentTypeType](./literals.md#permissionsboundaryattachmenttypetype)
- [PolicyEvaluationDecisionTypeType](./literals.md#policyevaluationdecisiontypetype)
- [PolicyExistsWaiterName](./literals.md#policyexistswaitername)
- [PolicyOwnerEntityTypeType](./literals.md#policyownerentitytypetype)
- [PolicyScopeTypeType](./literals.md#policyscopetypetype)
- [PolicySourceTypeType](./literals.md#policysourcetypetype)
- [PolicyTypeType](./literals.md#policytypetype)
- [PolicyUsageTypeType](./literals.md#policyusagetypetype)
- [ReportFormatTypeType](./literals.md#reportformattypetype)
- [ReportStateTypeType](./literals.md#reportstatetypetype)
- [RoleExistsWaiterName](./literals.md#roleexistswaitername)
- [SimulateCustomPolicyPaginatorName](./literals.md#simulatecustompolicypaginatorname)
- [SimulatePrincipalPolicyPaginatorName](./literals.md#simulateprincipalpolicypaginatorname)
- [SortKeyTypeType](./literals.md#sortkeytypetype)
- [StatusTypeType](./literals.md#statustypetype)
- [SummaryKeyTypeType](./literals.md#summarykeytypetype)
- [UserExistsWaiterName](./literals.md#userexistswaitername)
- [IAMServiceName](./literals.md#iamservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessDetailTypeDef](./type_defs.md#accessdetailtypedef)
- [AccessKeyLastUsedTypeDef](./type_defs.md#accesskeylastusedtypedef)
- [AccessKeyMetadataTypeDef](./type_defs.md#accesskeymetadatatypedef)
- [AccessKeyTypeDef](./type_defs.md#accesskeytypedef)
- [AddClientIDToOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#addclientidtoopenidconnectproviderrequestrequesttypedef)
- [AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef](./type_defs.md#addroletoinstanceprofilerequestinstanceprofileaddroletypedef)
- [AddRoleToInstanceProfileRequestRequestTypeDef](./type_defs.md#addroletoinstanceprofilerequestrequesttypedef)
- [AddUserToGroupRequestGroupAddUserTypeDef](./type_defs.md#addusertogrouprequestgroupaddusertypedef)
- [AddUserToGroupRequestRequestTypeDef](./type_defs.md#addusertogrouprequestrequesttypedef)
- [AddUserToGroupRequestUserAddGroupTypeDef](./type_defs.md#addusertogrouprequestuseraddgrouptypedef)
- [AttachGroupPolicyRequestGroupAttachPolicyTypeDef](./type_defs.md#attachgrouppolicyrequestgroupattachpolicytypedef)
- [AttachGroupPolicyRequestPolicyAttachGroupTypeDef](./type_defs.md#attachgrouppolicyrequestpolicyattachgrouptypedef)
- [AttachGroupPolicyRequestRequestTypeDef](./type_defs.md#attachgrouppolicyrequestrequesttypedef)
- [AttachRolePolicyRequestPolicyAttachRoleTypeDef](./type_defs.md#attachrolepolicyrequestpolicyattachroletypedef)
- [AttachRolePolicyRequestRequestTypeDef](./type_defs.md#attachrolepolicyrequestrequesttypedef)
- [AttachRolePolicyRequestRoleAttachPolicyTypeDef](./type_defs.md#attachrolepolicyrequestroleattachpolicytypedef)
- [AttachUserPolicyRequestPolicyAttachUserTypeDef](./type_defs.md#attachuserpolicyrequestpolicyattachusertypedef)
- [AttachUserPolicyRequestRequestTypeDef](./type_defs.md#attachuserpolicyrequestrequesttypedef)
- [AttachUserPolicyRequestUserAttachPolicyTypeDef](./type_defs.md#attachuserpolicyrequestuserattachpolicytypedef)
- [AttachedPermissionsBoundaryTypeDef](./type_defs.md#attachedpermissionsboundarytypedef)
- [AttachedPolicyTypeDef](./type_defs.md#attachedpolicytypedef)
- [ChangePasswordRequestRequestTypeDef](./type_defs.md#changepasswordrequestrequesttypedef)
- [ChangePasswordRequestServiceResourceChangePasswordTypeDef](./type_defs.md#changepasswordrequestserviceresourcechangepasswordtypedef)
- [ContextEntryTypeDef](./type_defs.md#contextentrytypedef)
- [CreateAccessKeyRequestRequestTypeDef](./type_defs.md#createaccesskeyrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateAccountAliasRequestRequestTypeDef](./type_defs.md#createaccountaliasrequestrequesttypedef)
- [CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef](./type_defs.md#createaccountaliasrequestserviceresourcecreateaccountaliastypedef)
- [CreateGroupRequestGroupCreateTypeDef](./type_defs.md#creategrouprequestgroupcreatetypedef)
- [CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef)
- [CreateGroupRequestServiceResourceCreateGroupTypeDef](./type_defs.md#creategrouprequestserviceresourcecreategrouptypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateLoginProfileRequestLoginProfileCreateTypeDef](./type_defs.md#createloginprofilerequestloginprofilecreatetypedef)
- [CreateLoginProfileRequestRequestTypeDef](./type_defs.md#createloginprofilerequestrequesttypedef)
- [CreateLoginProfileRequestUserCreateLoginProfileTypeDef](./type_defs.md#createloginprofilerequestusercreateloginprofiletypedef)
- [LoginProfileTypeDef](./type_defs.md#loginprofiletypedef)
- [CreatePolicyVersionRequestPolicyCreateVersionTypeDef](./type_defs.md#createpolicyversionrequestpolicycreateversiontypedef)
- [CreatePolicyVersionRequestRequestTypeDef](./type_defs.md#createpolicyversionrequestrequesttypedef)
- [CreateServiceLinkedRoleRequestRequestTypeDef](./type_defs.md#createservicelinkedrolerequestrequesttypedef)
- [CreateServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#createservicespecificcredentialrequestrequesttypedef)
- [ServiceSpecificCredentialTypeDef](./type_defs.md#servicespecificcredentialtypedef)
- [DeactivateMFADeviceRequestRequestTypeDef](./type_defs.md#deactivatemfadevicerequestrequesttypedef)
- [DeleteAccessKeyRequestRequestTypeDef](./type_defs.md#deleteaccesskeyrequestrequesttypedef)
- [DeleteAccountAliasRequestRequestTypeDef](./type_defs.md#deleteaccountaliasrequestrequesttypedef)
- [DeleteGroupPolicyRequestRequestTypeDef](./type_defs.md#deletegrouppolicyrequestrequesttypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteInstanceProfileRequestRequestTypeDef](./type_defs.md#deleteinstanceprofilerequestrequesttypedef)
- [DeleteLoginProfileRequestRequestTypeDef](./type_defs.md#deleteloginprofilerequestrequesttypedef)
- [DeleteOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#deleteopenidconnectproviderrequestrequesttypedef)
- [DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef)
- [DeletePolicyVersionRequestRequestTypeDef](./type_defs.md#deletepolicyversionrequestrequesttypedef)
- [DeleteRolePermissionsBoundaryRequestRequestTypeDef](./type_defs.md#deleterolepermissionsboundaryrequestrequesttypedef)
- [DeleteRolePolicyRequestRequestTypeDef](./type_defs.md#deleterolepolicyrequestrequesttypedef)
- [DeleteRoleRequestRequestTypeDef](./type_defs.md#deleterolerequestrequesttypedef)
- [DeleteSAMLProviderRequestRequestTypeDef](./type_defs.md#deletesamlproviderrequestrequesttypedef)
- [DeleteSSHPublicKeyRequestRequestTypeDef](./type_defs.md#deletesshpublickeyrequestrequesttypedef)
- [DeleteServerCertificateRequestRequestTypeDef](./type_defs.md#deleteservercertificaterequestrequesttypedef)
- [DeleteServiceLinkedRoleRequestRequestTypeDef](./type_defs.md#deleteservicelinkedrolerequestrequesttypedef)
- [DeleteServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#deleteservicespecificcredentialrequestrequesttypedef)
- [DeleteSigningCertificateRequestRequestTypeDef](./type_defs.md#deletesigningcertificaterequestrequesttypedef)
- [DeleteUserPermissionsBoundaryRequestRequestTypeDef](./type_defs.md#deleteuserpermissionsboundaryrequestrequesttypedef)
- [DeleteUserPolicyRequestRequestTypeDef](./type_defs.md#deleteuserpolicyrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteVirtualMFADeviceRequestRequestTypeDef](./type_defs.md#deletevirtualmfadevicerequestrequesttypedef)
- [RoleUsageTypeTypeDef](./type_defs.md#roleusagetypetypedef)
- [DetachGroupPolicyRequestGroupDetachPolicyTypeDef](./type_defs.md#detachgrouppolicyrequestgroupdetachpolicytypedef)
- [DetachGroupPolicyRequestPolicyDetachGroupTypeDef](./type_defs.md#detachgrouppolicyrequestpolicydetachgrouptypedef)
- [DetachGroupPolicyRequestRequestTypeDef](./type_defs.md#detachgrouppolicyrequestrequesttypedef)
- [DetachRolePolicyRequestPolicyDetachRoleTypeDef](./type_defs.md#detachrolepolicyrequestpolicydetachroletypedef)
- [DetachRolePolicyRequestRequestTypeDef](./type_defs.md#detachrolepolicyrequestrequesttypedef)
- [DetachRolePolicyRequestRoleDetachPolicyTypeDef](./type_defs.md#detachrolepolicyrequestroledetachpolicytypedef)
- [DetachUserPolicyRequestPolicyDetachUserTypeDef](./type_defs.md#detachuserpolicyrequestpolicydetachusertypedef)
- [DetachUserPolicyRequestRequestTypeDef](./type_defs.md#detachuserpolicyrequestrequesttypedef)
- [DetachUserPolicyRequestUserDetachPolicyTypeDef](./type_defs.md#detachuserpolicyrequestuserdetachpolicytypedef)
- [EnableMFADeviceRequestMfaDeviceAssociateTypeDef](./type_defs.md#enablemfadevicerequestmfadeviceassociatetypedef)
- [EnableMFADeviceRequestRequestTypeDef](./type_defs.md#enablemfadevicerequestrequesttypedef)
- [EnableMFADeviceRequestUserEnableMfaTypeDef](./type_defs.md#enablemfadevicerequestuserenablemfatypedef)
- [EntityInfoTypeDef](./type_defs.md#entityinfotypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [OrganizationsDecisionDetailTypeDef](./type_defs.md#organizationsdecisiondetailtypedef)
- [PermissionsBoundaryDecisionDetailTypeDef](./type_defs.md#permissionsboundarydecisiondetailtypedef)
- [GenerateOrganizationsAccessReportRequestRequestTypeDef](./type_defs.md#generateorganizationsaccessreportrequestrequesttypedef)
- [GenerateServiceLastAccessedDetailsRequestRequestTypeDef](./type_defs.md#generateservicelastaccesseddetailsrequestrequesttypedef)
- [GetAccessKeyLastUsedRequestRequestTypeDef](./type_defs.md#getaccesskeylastusedrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetAccountAuthorizationDetailsRequestRequestTypeDef](./type_defs.md#getaccountauthorizationdetailsrequestrequesttypedef)
- [PasswordPolicyTypeDef](./type_defs.md#passwordpolicytypedef)
- [GetContextKeysForCustomPolicyRequestRequestTypeDef](./type_defs.md#getcontextkeysforcustompolicyrequestrequesttypedef)
- [GetContextKeysForPrincipalPolicyRequestRequestTypeDef](./type_defs.md#getcontextkeysforprincipalpolicyrequestrequesttypedef)
- [GetGroupPolicyRequestRequestTypeDef](./type_defs.md#getgrouppolicyrequestrequesttypedef)
- [GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef)
- [GetInstanceProfileRequestRequestTypeDef](./type_defs.md#getinstanceprofilerequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetLoginProfileRequestRequestTypeDef](./type_defs.md#getloginprofilerequestrequesttypedef)
- [GetMFADeviceRequestRequestTypeDef](./type_defs.md#getmfadevicerequestrequesttypedef)
- [GetOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#getopenidconnectproviderrequestrequesttypedef)
- [GetOrganizationsAccessReportRequestRequestTypeDef](./type_defs.md#getorganizationsaccessreportrequestrequesttypedef)
- [GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef)
- [GetPolicyVersionRequestRequestTypeDef](./type_defs.md#getpolicyversionrequestrequesttypedef)
- [GetRolePolicyRequestRequestTypeDef](./type_defs.md#getrolepolicyrequestrequesttypedef)
- [GetRoleRequestRequestTypeDef](./type_defs.md#getrolerequestrequesttypedef)
- [GetSAMLProviderRequestRequestTypeDef](./type_defs.md#getsamlproviderrequestrequesttypedef)
- [GetSSHPublicKeyRequestRequestTypeDef](./type_defs.md#getsshpublickeyrequestrequesttypedef)
- [SSHPublicKeyTypeDef](./type_defs.md#sshpublickeytypedef)
- [GetServerCertificateRequestRequestTypeDef](./type_defs.md#getservercertificaterequestrequesttypedef)
- [GetServiceLastAccessedDetailsRequestRequestTypeDef](./type_defs.md#getservicelastaccesseddetailsrequestrequesttypedef)
- [GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef](./type_defs.md#getservicelastaccesseddetailswithentitiesrequestrequesttypedef)
- [GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef](./type_defs.md#getservicelinkedroledeletionstatusrequestrequesttypedef)
- [GetUserPolicyRequestRequestTypeDef](./type_defs.md#getuserpolicyrequestrequesttypedef)
- [GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef)
- [ListAccessKeysRequestRequestTypeDef](./type_defs.md#listaccesskeysrequestrequesttypedef)
- [ListAccountAliasesRequestRequestTypeDef](./type_defs.md#listaccountaliasesrequestrequesttypedef)
- [ListAttachedGroupPoliciesRequestRequestTypeDef](./type_defs.md#listattachedgrouppoliciesrequestrequesttypedef)
- [ListAttachedRolePoliciesRequestRequestTypeDef](./type_defs.md#listattachedrolepoliciesrequestrequesttypedef)
- [ListAttachedUserPoliciesRequestRequestTypeDef](./type_defs.md#listattacheduserpoliciesrequestrequesttypedef)
- [ListEntitiesForPolicyRequestRequestTypeDef](./type_defs.md#listentitiesforpolicyrequestrequesttypedef)
- [PolicyGroupTypeDef](./type_defs.md#policygrouptypedef)
- [PolicyRoleTypeDef](./type_defs.md#policyroletypedef)
- [PolicyUserTypeDef](./type_defs.md#policyusertypedef)
- [ListGroupPoliciesRequestRequestTypeDef](./type_defs.md#listgrouppoliciesrequestrequesttypedef)
- [ListGroupsForUserRequestRequestTypeDef](./type_defs.md#listgroupsforuserrequestrequesttypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListInstanceProfileTagsRequestRequestTypeDef](./type_defs.md#listinstanceprofiletagsrequestrequesttypedef)
- [ListInstanceProfilesForRoleRequestRequestTypeDef](./type_defs.md#listinstanceprofilesforrolerequestrequesttypedef)
- [ListInstanceProfilesRequestRequestTypeDef](./type_defs.md#listinstanceprofilesrequestrequesttypedef)
- [ListMFADeviceTagsRequestRequestTypeDef](./type_defs.md#listmfadevicetagsrequestrequesttypedef)
- [ListMFADevicesRequestRequestTypeDef](./type_defs.md#listmfadevicesrequestrequesttypedef)
- [MFADeviceTypeDef](./type_defs.md#mfadevicetypedef)
- [ListOpenIDConnectProviderTagsRequestRequestTypeDef](./type_defs.md#listopenidconnectprovidertagsrequestrequesttypedef)
- [OpenIDConnectProviderListEntryTypeDef](./type_defs.md#openidconnectproviderlistentrytypedef)
- [PolicyGrantingServiceAccessTypeDef](./type_defs.md#policygrantingserviceaccesstypedef)
- [ListPoliciesGrantingServiceAccessRequestRequestTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessrequestrequesttypedef)
- [ListPoliciesRequestRequestTypeDef](./type_defs.md#listpoliciesrequestrequesttypedef)
- [ListPolicyTagsRequestRequestTypeDef](./type_defs.md#listpolicytagsrequestrequesttypedef)
- [ListPolicyVersionsRequestRequestTypeDef](./type_defs.md#listpolicyversionsrequestrequesttypedef)
- [ListRolePoliciesRequestRequestTypeDef](./type_defs.md#listrolepoliciesrequestrequesttypedef)
- [ListRoleTagsRequestRequestTypeDef](./type_defs.md#listroletagsrequestrequesttypedef)
- [ListRolesRequestRequestTypeDef](./type_defs.md#listrolesrequestrequesttypedef)
- [ListSAMLProviderTagsRequestRequestTypeDef](./type_defs.md#listsamlprovidertagsrequestrequesttypedef)
- [SAMLProviderListEntryTypeDef](./type_defs.md#samlproviderlistentrytypedef)
- [ListSSHPublicKeysRequestRequestTypeDef](./type_defs.md#listsshpublickeysrequestrequesttypedef)
- [SSHPublicKeyMetadataTypeDef](./type_defs.md#sshpublickeymetadatatypedef)
- [ListServerCertificateTagsRequestRequestTypeDef](./type_defs.md#listservercertificatetagsrequestrequesttypedef)
- [ListServerCertificatesRequestRequestTypeDef](./type_defs.md#listservercertificatesrequestrequesttypedef)
- [ServerCertificateMetadataTypeDef](./type_defs.md#servercertificatemetadatatypedef)
- [ListServiceSpecificCredentialsRequestRequestTypeDef](./type_defs.md#listservicespecificcredentialsrequestrequesttypedef)
- [ServiceSpecificCredentialMetadataTypeDef](./type_defs.md#servicespecificcredentialmetadatatypedef)
- [ListSigningCertificatesRequestRequestTypeDef](./type_defs.md#listsigningcertificatesrequestrequesttypedef)
- [SigningCertificateTypeDef](./type_defs.md#signingcertificatetypedef)
- [ListUserPoliciesRequestRequestTypeDef](./type_defs.md#listuserpoliciesrequestrequesttypedef)
- [ListUserTagsRequestRequestTypeDef](./type_defs.md#listusertagsrequestrequesttypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListVirtualMFADevicesRequestRequestTypeDef](./type_defs.md#listvirtualmfadevicesrequestrequesttypedef)
- [PolicyDocumentStatementTypeDef](./type_defs.md#policydocumentstatementtypedef)
- [PositionTypeDef](./type_defs.md#positiontypedef)
- [PutGroupPolicyRequestGroupCreatePolicyTypeDef](./type_defs.md#putgrouppolicyrequestgroupcreatepolicytypedef)
- [PutGroupPolicyRequestGroupPolicyPutTypeDef](./type_defs.md#putgrouppolicyrequestgrouppolicyputtypedef)
- [PutGroupPolicyRequestRequestTypeDef](./type_defs.md#putgrouppolicyrequestrequesttypedef)
- [PutRolePermissionsBoundaryRequestRequestTypeDef](./type_defs.md#putrolepermissionsboundaryrequestrequesttypedef)
- [PutRolePolicyRequestRequestTypeDef](./type_defs.md#putrolepolicyrequestrequesttypedef)
- [PutRolePolicyRequestRolePolicyPutTypeDef](./type_defs.md#putrolepolicyrequestrolepolicyputtypedef)
- [PutUserPermissionsBoundaryRequestRequestTypeDef](./type_defs.md#putuserpermissionsboundaryrequestrequesttypedef)
- [PutUserPolicyRequestRequestTypeDef](./type_defs.md#putuserpolicyrequestrequesttypedef)
- [PutUserPolicyRequestUserCreatePolicyTypeDef](./type_defs.md#putuserpolicyrequestusercreatepolicytypedef)
- [PutUserPolicyRequestUserPolicyPutTypeDef](./type_defs.md#putuserpolicyrequestuserpolicyputtypedef)
- [RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#removeclientidfromopenidconnectproviderrequestrequesttypedef)
- [RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef](./type_defs.md#removerolefrominstanceprofilerequestinstanceprofileremoveroletypedef)
- [RemoveRoleFromInstanceProfileRequestRequestTypeDef](./type_defs.md#removerolefrominstanceprofilerequestrequesttypedef)
- [RemoveUserFromGroupRequestGroupRemoveUserTypeDef](./type_defs.md#removeuserfromgrouprequestgroupremoveusertypedef)
- [RemoveUserFromGroupRequestRequestTypeDef](./type_defs.md#removeuserfromgrouprequestrequesttypedef)
- [RemoveUserFromGroupRequestUserRemoveGroupTypeDef](./type_defs.md#removeuserfromgrouprequestuserremovegrouptypedef)
- [ResetServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#resetservicespecificcredentialrequestrequesttypedef)
- [ResyncMFADeviceRequestMfaDeviceResyncTypeDef](./type_defs.md#resyncmfadevicerequestmfadeviceresynctypedef)
- [ResyncMFADeviceRequestRequestTypeDef](./type_defs.md#resyncmfadevicerequestrequesttypedef)
- [RoleLastUsedTypeDef](./type_defs.md#rolelastusedtypedef)
- [TrackedActionLastAccessedTypeDef](./type_defs.md#trackedactionlastaccessedtypedef)
- [SetDefaultPolicyVersionRequestRequestTypeDef](./type_defs.md#setdefaultpolicyversionrequestrequesttypedef)
- [SetSecurityTokenServicePreferencesRequestRequestTypeDef](./type_defs.md#setsecuritytokenservicepreferencesrequestrequesttypedef)
- [UntagInstanceProfileRequestRequestTypeDef](./type_defs.md#untaginstanceprofilerequestrequesttypedef)
- [UntagMFADeviceRequestRequestTypeDef](./type_defs.md#untagmfadevicerequestrequesttypedef)
- [UntagOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#untagopenidconnectproviderrequestrequesttypedef)
- [UntagPolicyRequestRequestTypeDef](./type_defs.md#untagpolicyrequestrequesttypedef)
- [UntagRoleRequestRequestTypeDef](./type_defs.md#untagrolerequestrequesttypedef)
- [UntagSAMLProviderRequestRequestTypeDef](./type_defs.md#untagsamlproviderrequestrequesttypedef)
- [UntagServerCertificateRequestRequestTypeDef](./type_defs.md#untagservercertificaterequestrequesttypedef)
- [UntagUserRequestRequestTypeDef](./type_defs.md#untaguserrequestrequesttypedef)
- [UpdateAccessKeyRequestAccessKeyActivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeyactivatetypedef)
- [UpdateAccessKeyRequestAccessKeyDeactivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeydeactivatetypedef)
- [UpdateAccessKeyRequestAccessKeyPairActivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeypairactivatetypedef)
- [UpdateAccessKeyRequestAccessKeyPairDeactivateTypeDef](./type_defs.md#updateaccesskeyrequestaccesskeypairdeactivatetypedef)
- [UpdateAccessKeyRequestRequestTypeDef](./type_defs.md#updateaccesskeyrequestrequesttypedef)
- [UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestaccountpasswordpolicyupdatetypedef)
- [UpdateAccountPasswordPolicyRequestRequestTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestrequesttypedef)
- [UpdateAccountPasswordPolicyRequestServiceResourceCreateAccountPasswordPolicyTypeDef](./type_defs.md#updateaccountpasswordpolicyrequestserviceresourcecreateaccountpasswordpolicytypedef)
- [UpdateAssumeRolePolicyRequestAssumeRolePolicyUpdateTypeDef](./type_defs.md#updateassumerolepolicyrequestassumerolepolicyupdatetypedef)
- [UpdateAssumeRolePolicyRequestRequestTypeDef](./type_defs.md#updateassumerolepolicyrequestrequesttypedef)
- [UpdateGroupRequestGroupUpdateTypeDef](./type_defs.md#updategrouprequestgroupupdatetypedef)
- [UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef)
- [UpdateLoginProfileRequestLoginProfileUpdateTypeDef](./type_defs.md#updateloginprofilerequestloginprofileupdatetypedef)
- [UpdateLoginProfileRequestRequestTypeDef](./type_defs.md#updateloginprofilerequestrequesttypedef)
- [UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef](./type_defs.md#updateopenidconnectproviderthumbprintrequestrequesttypedef)
- [UpdateRoleDescriptionRequestRequestTypeDef](./type_defs.md#updateroledescriptionrequestrequesttypedef)
- [UpdateRoleRequestRequestTypeDef](./type_defs.md#updaterolerequestrequesttypedef)
- [UpdateSAMLProviderRequestRequestTypeDef](./type_defs.md#updatesamlproviderrequestrequesttypedef)
- [UpdateSAMLProviderRequestSamlProviderUpdateTypeDef](./type_defs.md#updatesamlproviderrequestsamlproviderupdatetypedef)
- [UpdateSSHPublicKeyRequestRequestTypeDef](./type_defs.md#updatesshpublickeyrequestrequesttypedef)
- [UpdateServerCertificateRequestRequestTypeDef](./type_defs.md#updateservercertificaterequestrequesttypedef)
- [UpdateServerCertificateRequestServerCertificateUpdateTypeDef](./type_defs.md#updateservercertificaterequestservercertificateupdatetypedef)
- [UpdateServiceSpecificCredentialRequestRequestTypeDef](./type_defs.md#updateservicespecificcredentialrequestrequesttypedef)
- [UpdateSigningCertificateRequestRequestTypeDef](./type_defs.md#updatesigningcertificaterequestrequesttypedef)
- [UpdateSigningCertificateRequestSigningCertificateActivateTypeDef](./type_defs.md#updatesigningcertificaterequestsigningcertificateactivatetypedef)
- [UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef](./type_defs.md#updatesigningcertificaterequestsigningcertificatedeactivatetypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [UpdateUserRequestUserUpdateTypeDef](./type_defs.md#updateuserrequestuserupdatetypedef)
- [UploadSSHPublicKeyRequestRequestTypeDef](./type_defs.md#uploadsshpublickeyrequestrequesttypedef)
- [UploadSigningCertificateRequestRequestTypeDef](./type_defs.md#uploadsigningcertificaterequestrequesttypedef)
- [UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef](./type_defs.md#uploadsigningcertificaterequestserviceresourcecreatesigningcertificatetypedef)
- [SimulateCustomPolicyRequestRequestTypeDef](./type_defs.md#simulatecustompolicyrequestrequesttypedef)
- [SimulatePrincipalPolicyRequestRequestTypeDef](./type_defs.md#simulateprincipalpolicyrequestrequesttypedef)
- [CreateAccessKeyResponseTypeDef](./type_defs.md#createaccesskeyresponsetypedef)
- [DeleteServiceLinkedRoleResponseTypeDef](./type_defs.md#deleteservicelinkedroleresponsetypedef)
- [DisableOrganizationsRootCredentialsManagementResponseTypeDef](./type_defs.md#disableorganizationsrootcredentialsmanagementresponsetypedef)
- [DisableOrganizationsRootSessionsResponseTypeDef](./type_defs.md#disableorganizationsrootsessionsresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EnableOrganizationsRootCredentialsManagementResponseTypeDef](./type_defs.md#enableorganizationsrootcredentialsmanagementresponsetypedef)
- [EnableOrganizationsRootSessionsResponseTypeDef](./type_defs.md#enableorganizationsrootsessionsresponsetypedef)
- [GenerateCredentialReportResponseTypeDef](./type_defs.md#generatecredentialreportresponsetypedef)
- [GenerateOrganizationsAccessReportResponseTypeDef](./type_defs.md#generateorganizationsaccessreportresponsetypedef)
- [GenerateServiceLastAccessedDetailsResponseTypeDef](./type_defs.md#generateservicelastaccesseddetailsresponsetypedef)
- [GetAccessKeyLastUsedResponseTypeDef](./type_defs.md#getaccesskeylastusedresponsetypedef)
- [GetAccountSummaryResponseTypeDef](./type_defs.md#getaccountsummaryresponsetypedef)
- [GetContextKeysForPolicyResponseTypeDef](./type_defs.md#getcontextkeysforpolicyresponsetypedef)
- [GetCredentialReportResponseTypeDef](./type_defs.md#getcredentialreportresponsetypedef)
- [GetMFADeviceResponseTypeDef](./type_defs.md#getmfadeviceresponsetypedef)
- [ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef)
- [ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef)
- [ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef)
- [ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef)
- [ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef)
- [ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef)
- [ListOrganizationsFeaturesResponseTypeDef](./type_defs.md#listorganizationsfeaturesresponsetypedef)
- [ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef)
- [ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef)
- [UpdateSAMLProviderResponseTypeDef](./type_defs.md#updatesamlproviderresponsetypedef)
- [CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)
- [ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [CreateInstanceProfileRequestRequestTypeDef](./type_defs.md#createinstanceprofilerequestrequesttypedef)
- [CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef](./type_defs.md#createinstanceprofilerequestserviceresourcecreateinstanceprofiletypedef)
- [CreateOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#createopenidconnectproviderrequestrequesttypedef)
- [CreateOpenIDConnectProviderResponseTypeDef](./type_defs.md#createopenidconnectproviderresponsetypedef)
- [CreatePolicyRequestRequestTypeDef](./type_defs.md#createpolicyrequestrequesttypedef)
- [CreatePolicyRequestServiceResourceCreatePolicyTypeDef](./type_defs.md#createpolicyrequestserviceresourcecreatepolicytypedef)
- [CreateRoleRequestRequestTypeDef](./type_defs.md#createrolerequestrequesttypedef)
- [CreateRoleRequestServiceResourceCreateRoleTypeDef](./type_defs.md#createrolerequestserviceresourcecreateroletypedef)
- [CreateSAMLProviderRequestRequestTypeDef](./type_defs.md#createsamlproviderrequestrequesttypedef)
- [CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef](./type_defs.md#createsamlproviderrequestserviceresourcecreatesamlprovidertypedef)
- [CreateSAMLProviderResponseTypeDef](./type_defs.md#createsamlproviderresponsetypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [CreateUserRequestServiceResourceCreateUserTypeDef](./type_defs.md#createuserrequestserviceresourcecreateusertypedef)
- [CreateUserRequestUserCreateTypeDef](./type_defs.md#createuserrequestusercreatetypedef)
- [CreateVirtualMFADeviceRequestRequestTypeDef](./type_defs.md#createvirtualmfadevicerequestrequesttypedef)
- [CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef](./type_defs.md#createvirtualmfadevicerequestserviceresourcecreatevirtualmfadevicetypedef)
- [GetOpenIDConnectProviderResponseTypeDef](./type_defs.md#getopenidconnectproviderresponsetypedef)
- [GetSAMLProviderResponseTypeDef](./type_defs.md#getsamlproviderresponsetypedef)
- [ListInstanceProfileTagsResponseTypeDef](./type_defs.md#listinstanceprofiletagsresponsetypedef)
- [ListMFADeviceTagsResponseTypeDef](./type_defs.md#listmfadevicetagsresponsetypedef)
- [ListOpenIDConnectProviderTagsResponseTypeDef](./type_defs.md#listopenidconnectprovidertagsresponsetypedef)
- [ListPolicyTagsResponseTypeDef](./type_defs.md#listpolicytagsresponsetypedef)
- [ListRoleTagsResponseTypeDef](./type_defs.md#listroletagsresponsetypedef)
- [ListSAMLProviderTagsResponseTypeDef](./type_defs.md#listsamlprovidertagsresponsetypedef)
- [ListServerCertificateTagsResponseTypeDef](./type_defs.md#listservercertificatetagsresponsetypedef)
- [ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef)
- [PolicyTypeDef](./type_defs.md#policytypedef)
- [TagInstanceProfileRequestRequestTypeDef](./type_defs.md#taginstanceprofilerequestrequesttypedef)
- [TagMFADeviceRequestRequestTypeDef](./type_defs.md#tagmfadevicerequestrequesttypedef)
- [TagOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#tagopenidconnectproviderrequestrequesttypedef)
- [TagPolicyRequestRequestTypeDef](./type_defs.md#tagpolicyrequestrequesttypedef)
- [TagRoleRequestRequestTypeDef](./type_defs.md#tagrolerequestrequesttypedef)
- [TagSAMLProviderRequestRequestTypeDef](./type_defs.md#tagsamlproviderrequestrequesttypedef)
- [TagServerCertificateRequestRequestTypeDef](./type_defs.md#tagservercertificaterequestrequesttypedef)
- [TagUserRequestRequestTypeDef](./type_defs.md#taguserrequestrequesttypedef)
- [UploadServerCertificateRequestRequestTypeDef](./type_defs.md#uploadservercertificaterequestrequesttypedef)
- [UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef](./type_defs.md#uploadservercertificaterequestserviceresourcecreateservercertificatetypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [CreateLoginProfileResponseTypeDef](./type_defs.md#createloginprofileresponsetypedef)
- [GetLoginProfileResponseTypeDef](./type_defs.md#getloginprofileresponsetypedef)
- [CreateServiceSpecificCredentialResponseTypeDef](./type_defs.md#createservicespecificcredentialresponsetypedef)
- [ResetServiceSpecificCredentialResponseTypeDef](./type_defs.md#resetservicespecificcredentialresponsetypedef)
- [DeletionTaskFailureReasonTypeTypeDef](./type_defs.md#deletiontaskfailurereasontypetypedef)
- [EntityDetailsTypeDef](./type_defs.md#entitydetailstypedef)
- [GetOrganizationsAccessReportResponseTypeDef](./type_defs.md#getorganizationsaccessreportresponsetypedef)
- [GetAccountAuthorizationDetailsRequestPaginateTypeDef](./type_defs.md#getaccountauthorizationdetailsrequestpaginatetypedef)
- [GetGroupRequestPaginateTypeDef](./type_defs.md#getgrouprequestpaginatetypedef)
- [ListAccessKeysRequestPaginateTypeDef](./type_defs.md#listaccesskeysrequestpaginatetypedef)
- [ListAccountAliasesRequestPaginateTypeDef](./type_defs.md#listaccountaliasesrequestpaginatetypedef)
- [ListAttachedGroupPoliciesRequestPaginateTypeDef](./type_defs.md#listattachedgrouppoliciesrequestpaginatetypedef)
- [ListAttachedRolePoliciesRequestPaginateTypeDef](./type_defs.md#listattachedrolepoliciesrequestpaginatetypedef)
- [ListAttachedUserPoliciesRequestPaginateTypeDef](./type_defs.md#listattacheduserpoliciesrequestpaginatetypedef)
- [ListEntitiesForPolicyRequestPaginateTypeDef](./type_defs.md#listentitiesforpolicyrequestpaginatetypedef)
- [ListGroupPoliciesRequestPaginateTypeDef](./type_defs.md#listgrouppoliciesrequestpaginatetypedef)
- [ListGroupsForUserRequestPaginateTypeDef](./type_defs.md#listgroupsforuserrequestpaginatetypedef)
- [ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef)
- [ListInstanceProfileTagsRequestPaginateTypeDef](./type_defs.md#listinstanceprofiletagsrequestpaginatetypedef)
- [ListInstanceProfilesForRoleRequestPaginateTypeDef](./type_defs.md#listinstanceprofilesforrolerequestpaginatetypedef)
- [ListInstanceProfilesRequestPaginateTypeDef](./type_defs.md#listinstanceprofilesrequestpaginatetypedef)
- [ListMFADeviceTagsRequestPaginateTypeDef](./type_defs.md#listmfadevicetagsrequestpaginatetypedef)
- [ListMFADevicesRequestPaginateTypeDef](./type_defs.md#listmfadevicesrequestpaginatetypedef)
- [ListOpenIDConnectProviderTagsRequestPaginateTypeDef](./type_defs.md#listopenidconnectprovidertagsrequestpaginatetypedef)
- [ListPoliciesRequestPaginateTypeDef](./type_defs.md#listpoliciesrequestpaginatetypedef)
- [ListPolicyTagsRequestPaginateTypeDef](./type_defs.md#listpolicytagsrequestpaginatetypedef)
- [ListPolicyVersionsRequestPaginateTypeDef](./type_defs.md#listpolicyversionsrequestpaginatetypedef)
- [ListRolePoliciesRequestPaginateTypeDef](./type_defs.md#listrolepoliciesrequestpaginatetypedef)
- [ListRoleTagsRequestPaginateTypeDef](./type_defs.md#listroletagsrequestpaginatetypedef)
- [ListRolesRequestPaginateTypeDef](./type_defs.md#listrolesrequestpaginatetypedef)
- [ListSAMLProviderTagsRequestPaginateTypeDef](./type_defs.md#listsamlprovidertagsrequestpaginatetypedef)
- [ListSSHPublicKeysRequestPaginateTypeDef](./type_defs.md#listsshpublickeysrequestpaginatetypedef)
- [ListServerCertificateTagsRequestPaginateTypeDef](./type_defs.md#listservercertificatetagsrequestpaginatetypedef)
- [ListServerCertificatesRequestPaginateTypeDef](./type_defs.md#listservercertificatesrequestpaginatetypedef)
- [ListSigningCertificatesRequestPaginateTypeDef](./type_defs.md#listsigningcertificatesrequestpaginatetypedef)
- [ListUserPoliciesRequestPaginateTypeDef](./type_defs.md#listuserpoliciesrequestpaginatetypedef)
- [ListUserTagsRequestPaginateTypeDef](./type_defs.md#listusertagsrequestpaginatetypedef)
- [ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
- [ListVirtualMFADevicesRequestPaginateTypeDef](./type_defs.md#listvirtualmfadevicesrequestpaginatetypedef)
- [SimulateCustomPolicyRequestPaginateTypeDef](./type_defs.md#simulatecustompolicyrequestpaginatetypedef)
- [SimulatePrincipalPolicyRequestPaginateTypeDef](./type_defs.md#simulateprincipalpolicyrequestpaginatetypedef)
- [GetAccountPasswordPolicyResponseTypeDef](./type_defs.md#getaccountpasswordpolicyresponsetypedef)
- [GetInstanceProfileRequestWaitTypeDef](./type_defs.md#getinstanceprofilerequestwaittypedef)
- [GetPolicyRequestWaitTypeDef](./type_defs.md#getpolicyrequestwaittypedef)
- [GetRoleRequestWaitTypeDef](./type_defs.md#getrolerequestwaittypedef)
- [GetUserRequestWaitTypeDef](./type_defs.md#getuserrequestwaittypedef)
- [GetSSHPublicKeyResponseTypeDef](./type_defs.md#getsshpublickeyresponsetypedef)
- [UploadSSHPublicKeyResponseTypeDef](./type_defs.md#uploadsshpublickeyresponsetypedef)
- [ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef)
- [ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef)
- [ListOpenIDConnectProvidersResponseTypeDef](./type_defs.md#listopenidconnectprovidersresponsetypedef)
- [ListPoliciesGrantingServiceAccessEntryTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessentrytypedef)
- [ListSAMLProvidersResponseTypeDef](./type_defs.md#listsamlprovidersresponsetypedef)
- [ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef)
- [ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef)
- [ServerCertificateTypeDef](./type_defs.md#servercertificatetypedef)
- [UploadServerCertificateResponseTypeDef](./type_defs.md#uploadservercertificateresponsetypedef)
- [ListServiceSpecificCredentialsResponseTypeDef](./type_defs.md#listservicespecificcredentialsresponsetypedef)
- [ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef)
- [UploadSigningCertificateResponseTypeDef](./type_defs.md#uploadsigningcertificateresponsetypedef)
- [PolicyDocumentDictTypeDef](./type_defs.md#policydocumentdicttypedef)
- [StatementTypeDef](./type_defs.md#statementtypedef)
- [ServiceLastAccessedTypeDef](./type_defs.md#servicelastaccessedtypedef)
- [CreatePolicyResponseTypeDef](./type_defs.md#createpolicyresponsetypedef)
- [GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)
- [ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [VirtualMFADeviceTypeDef](./type_defs.md#virtualmfadevicetypedef)
- [GetServiceLinkedRoleDeletionStatusResponseTypeDef](./type_defs.md#getservicelinkedroledeletionstatusresponsetypedef)
- [GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef](./type_defs.md#getservicelastaccesseddetailswithentitiesresponsetypedef)
- [ListPoliciesGrantingServiceAccessResponseTypeDef](./type_defs.md#listpoliciesgrantingserviceaccessresponsetypedef)
- [GetServerCertificateResponseTypeDef](./type_defs.md#getservercertificateresponsetypedef)
- [PolicyDocumentTypeDef](./type_defs.md#policydocumenttypedef)
- [ResourceSpecificResultTypeDef](./type_defs.md#resourcespecificresulttypedef)
- [GetServiceLastAccessedDetailsResponseTypeDef](./type_defs.md#getservicelastaccesseddetailsresponsetypedef)
- [CreateVirtualMFADeviceResponseTypeDef](./type_defs.md#createvirtualmfadeviceresponsetypedef)
- [ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef)
- [GetGroupPolicyResponseTypeDef](./type_defs.md#getgrouppolicyresponsetypedef)
- [GetRolePolicyResponseTypeDef](./type_defs.md#getrolepolicyresponsetypedef)
- [GetUserPolicyResponseTypeDef](./type_defs.md#getuserpolicyresponsetypedef)
- [PolicyDetailTypeDef](./type_defs.md#policydetailtypedef)
- [PolicyVersionTypeDef](./type_defs.md#policyversiontypedef)
- [RoleTypeDef](./type_defs.md#roletypedef)
- [EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef)
- [GroupDetailTypeDef](./type_defs.md#groupdetailtypedef)
- [UserDetailTypeDef](./type_defs.md#userdetailtypedef)
- [CreatePolicyVersionResponseTypeDef](./type_defs.md#createpolicyversionresponsetypedef)
- [GetPolicyVersionResponseTypeDef](./type_defs.md#getpolicyversionresponsetypedef)
- [ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef)
- [ManagedPolicyDetailTypeDef](./type_defs.md#managedpolicydetailtypedef)
- [CreateRoleResponseTypeDef](./type_defs.md#createroleresponsetypedef)
- [CreateServiceLinkedRoleResponseTypeDef](./type_defs.md#createservicelinkedroleresponsetypedef)
- [GetRoleResponseTypeDef](./type_defs.md#getroleresponsetypedef)
- [InstanceProfileTypeDef](./type_defs.md#instanceprofiletypedef)
- [ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef)
- [UpdateRoleDescriptionResponseTypeDef](./type_defs.md#updateroledescriptionresponsetypedef)
- [SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef)
- [CreateInstanceProfileResponseTypeDef](./type_defs.md#createinstanceprofileresponsetypedef)
- [GetInstanceProfileResponseTypeDef](./type_defs.md#getinstanceprofileresponsetypedef)
- [ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef)
- [ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef)
- [RoleDetailTypeDef](./type_defs.md#roledetailtypedef)
- [GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef)

