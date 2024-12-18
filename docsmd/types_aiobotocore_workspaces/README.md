# WorkSpaces module

> [Index](../README.md) > WorkSpaces


!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkSpaces` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkSpaces` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workspaces]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workspaces]'

# standalone installation
python -m pip install types-aiobotocore-workspaces
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workspaces
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkSpacesClient

Type annotations and code completion for  `#!python session.create_client("workspaces")` as [WorkSpacesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# WorkSpacesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces.client import WorkSpacesClient


session = get_session()
async with session.create_client("workspaces") as client:
    client: WorkSpacesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("workspaces").get_paginator("...")`.

```python
# DescribeAccountModificationsPaginator usage example

from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator

def get_describe_account_modifications_paginator() -> DescribeAccountModificationsPaginator:
    return client.get_paginator("describe_account_modifications"))
```

- [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
- [DescribeIpGroupsPaginator](./paginators.md#describeipgroupspaginator)
- [DescribeWorkspaceBundlesPaginator](./paginators.md#describeworkspacebundlespaginator)
- [DescribeWorkspaceDirectoriesPaginator](./paginators.md#describeworkspacedirectoriespaginator)
- [DescribeWorkspaceImagesPaginator](./paginators.md#describeworkspaceimagespaginator)
- [DescribeWorkspacesConnectionStatusPaginator](./paginators.md#describeworkspacesconnectionstatuspaginator)
- [DescribeWorkspacesPaginator](./paginators.md#describeworkspacespaginator)
- [ListAccountLinksPaginator](./paginators.md#listaccountlinkspaginator)
- [ListAvailableManagementCidrRangesPaginator](./paginators.md#listavailablemanagementcidrrangespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessPropertyValueType usage example

from types_aiobotocore_workspaces.literals import AccessPropertyValueType

def get_value() -> AccessPropertyValueType:
    return "ALLOW"
```

- [AccessPropertyValueType](./literals.md#accesspropertyvaluetype)
- [AccountLinkStatusEnumType](./literals.md#accountlinkstatusenumtype)
- [ApplicationAssociatedResourceTypeType](./literals.md#applicationassociatedresourcetypetype)
- [ApplicationSettingsStatusEnumType](./literals.md#applicationsettingsstatusenumtype)
- [ApplicationType](./literals.md#applicationtype)
- [AssociationErrorCodeType](./literals.md#associationerrorcodetype)
- [AssociationStateType](./literals.md#associationstatetype)
- [AssociationStatusType](./literals.md#associationstatustype)
- [AuthenticationTypeType](./literals.md#authenticationtypetype)
- [BundleAssociatedResourceTypeType](./literals.md#bundleassociatedresourcetypetype)
- [BundleTypeType](./literals.md#bundletypetype)
- [CertificateBasedAuthStatusEnumType](./literals.md#certificatebasedauthstatusenumtype)
- [ClientDeviceTypeType](./literals.md#clientdevicetypetype)
- [ComputeType](./literals.md#computetype)
- [ConnectionAliasStateType](./literals.md#connectionaliasstatetype)
- [ConnectionStateType](./literals.md#connectionstatetype)
- [DataReplicationType](./literals.md#datareplicationtype)
- [DedicatedTenancyAccountTypeType](./literals.md#dedicatedtenancyaccounttypetype)
- [DedicatedTenancyModificationStateEnumType](./literals.md#dedicatedtenancymodificationstateenumtype)
- [DedicatedTenancySupportEnumType](./literals.md#dedicatedtenancysupportenumtype)
- [DedicatedTenancySupportResultEnumType](./literals.md#dedicatedtenancysupportresultenumtype)
- [DeletableCertificateBasedAuthPropertyType](./literals.md#deletablecertificatebasedauthpropertytype)
- [DeletableSamlPropertyType](./literals.md#deletablesamlpropertytype)
- [DescribeAccountModificationsPaginatorName](./literals.md#describeaccountmodificationspaginatorname)
- [DescribeIpGroupsPaginatorName](./literals.md#describeipgroupspaginatorname)
- [DescribeWorkspaceBundlesPaginatorName](./literals.md#describeworkspacebundlespaginatorname)
- [DescribeWorkspaceDirectoriesFilterNameType](./literals.md#describeworkspacedirectoriesfilternametype)
- [DescribeWorkspaceDirectoriesPaginatorName](./literals.md#describeworkspacedirectoriespaginatorname)
- [DescribeWorkspaceImagesPaginatorName](./literals.md#describeworkspaceimagespaginatorname)
- [DescribeWorkspacesConnectionStatusPaginatorName](./literals.md#describeworkspacesconnectionstatuspaginatorname)
- [DescribeWorkspacesPaginatorName](./literals.md#describeworkspacespaginatorname)
- [DescribeWorkspacesPoolsFilterNameType](./literals.md#describeworkspacespoolsfilternametype)
- [DescribeWorkspacesPoolsFilterOperatorType](./literals.md#describeworkspacespoolsfilteroperatortype)
- [ImageAssociatedResourceTypeType](./literals.md#imageassociatedresourcetypetype)
- [ImageTypeType](./literals.md#imagetypetype)
- [ListAccountLinksPaginatorName](./literals.md#listaccountlinkspaginatorname)
- [ListAvailableManagementCidrRangesPaginatorName](./literals.md#listavailablemanagementcidrrangespaginatorname)
- [LogUploadEnumType](./literals.md#loguploadenumtype)
- [ModificationResourceEnumType](./literals.md#modificationresourceenumtype)
- [ModificationStateEnumType](./literals.md#modificationstateenumtype)
- [OperatingSystemNameType](./literals.md#operatingsystemnametype)
- [OperatingSystemTypeType](./literals.md#operatingsystemtypetype)
- [ProtocolType](./literals.md#protocoltype)
- [ReconnectEnumType](./literals.md#reconnectenumtype)
- [RunningModeType](./literals.md#runningmodetype)
- [SamlStatusEnumType](./literals.md#samlstatusenumtype)
- [SessionConnectionStateType](./literals.md#sessionconnectionstatetype)
- [StandbyWorkspaceRelationshipTypeType](./literals.md#standbyworkspacerelationshiptypetype)
- [StorageConnectorStatusEnumType](./literals.md#storageconnectorstatusenumtype)
- [StorageConnectorTypeEnumType](./literals.md#storageconnectortypeenumtype)
- [StreamingExperiencePreferredProtocolEnumType](./literals.md#streamingexperiencepreferredprotocolenumtype)
- [TargetWorkspaceStateType](./literals.md#targetworkspacestatetype)
- [TenancyType](./literals.md#tenancytype)
- [UserIdentityTypeType](./literals.md#useridentitytypetype)
- [UserSettingActionEnumType](./literals.md#usersettingactionenumtype)
- [UserSettingPermissionEnumType](./literals.md#usersettingpermissionenumtype)
- [WorkSpaceApplicationLicenseTypeType](./literals.md#workspaceapplicationlicensetypetype)
- [WorkSpaceApplicationStateType](./literals.md#workspaceapplicationstatetype)
- [WorkSpaceAssociatedResourceTypeType](./literals.md#workspaceassociatedresourcetypetype)
- [WorkspaceBundleStateType](./literals.md#workspacebundlestatetype)
- [WorkspaceDirectoryStateType](./literals.md#workspacedirectorystatetype)
- [WorkspaceDirectoryTypeType](./literals.md#workspacedirectorytypetype)
- [WorkspaceImageErrorDetailCodeType](./literals.md#workspaceimageerrordetailcodetype)
- [WorkspaceImageIngestionProcessType](./literals.md#workspaceimageingestionprocesstype)
- [WorkspaceImageRequiredTenancyType](./literals.md#workspaceimagerequiredtenancytype)
- [WorkspaceImageStateType](./literals.md#workspaceimagestatetype)
- [WorkspaceStateType](./literals.md#workspacestatetype)
- [WorkspaceTypeType](./literals.md#workspacetypetype)
- [WorkspacesPoolErrorCodeType](./literals.md#workspacespoolerrorcodetype)
- [WorkspacesPoolStateType](./literals.md#workspacespoolstatetype)
- [WorkSpacesServiceName](./literals.md#workspacesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#acceptaccountlinkinvitationrequestrequesttypedef)
- [AccountLinkTypeDef](./type_defs.md#accountlinktypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AccountModificationTypeDef](./type_defs.md#accountmodificationtypedef)
- [ActiveDirectoryConfigTypeDef](./type_defs.md#activedirectoryconfigtypedef)
- [AssociationStateReasonTypeDef](./type_defs.md#associationstatereasontypedef)
- [ApplicationSettingsRequestTypeDef](./type_defs.md#applicationsettingsrequesttypedef)
- [ApplicationSettingsResponseTypeDef](./type_defs.md#applicationsettingsresponsetypedef)
- [AssociateConnectionAliasRequestRequestTypeDef](./type_defs.md#associateconnectionaliasrequestrequesttypedef)
- [AssociateIpGroupsRequestRequestTypeDef](./type_defs.md#associateipgroupsrequestrequesttypedef)
- [AssociateWorkspaceApplicationRequestRequestTypeDef](./type_defs.md#associateworkspaceapplicationrequestrequesttypedef)
- [IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CapacityStatusTypeDef](./type_defs.md#capacitystatustypedef)
- [CapacityTypeDef](./type_defs.md#capacitytypedef)
- [CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef)
- [ClientPropertiesTypeDef](./type_defs.md#clientpropertiestypedef)
- [ComputeTypeTypeDef](./type_defs.md#computetypetypedef)
- [ConnectClientAddInTypeDef](./type_defs.md#connectclientaddintypedef)
- [ConnectionAliasAssociationTypeDef](./type_defs.md#connectionaliasassociationtypedef)
- [ConnectionAliasPermissionTypeDef](./type_defs.md#connectionaliaspermissiontypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#createaccountlinkinvitationrequestrequesttypedef)
- [CreateConnectClientAddInRequestRequestTypeDef](./type_defs.md#createconnectclientaddinrequestrequesttypedef)
- [PendingCreateStandbyWorkspacesRequestTypeDef](./type_defs.md#pendingcreatestandbyworkspacesrequesttypedef)
- [RootStorageTypeDef](./type_defs.md#rootstoragetypedef)
- [UserStorageTypeDef](./type_defs.md#userstoragetypedef)
- [OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef)
- [TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef)
- [DataReplicationSettingsTypeDef](./type_defs.md#datareplicationsettingstypedef)
- [DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef)
- [DefaultWorkspaceCreationPropertiesTypeDef](./type_defs.md#defaultworkspacecreationpropertiestypedef)
- [DeleteAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#deleteaccountlinkinvitationrequestrequesttypedef)
- [DeleteClientBrandingRequestRequestTypeDef](./type_defs.md#deleteclientbrandingrequestrequesttypedef)
- [DeleteConnectClientAddInRequestRequestTypeDef](./type_defs.md#deleteconnectclientaddinrequestrequesttypedef)
- [DeleteConnectionAliasRequestRequestTypeDef](./type_defs.md#deleteconnectionaliasrequestrequesttypedef)
- [DeleteIpGroupRequestRequestTypeDef](./type_defs.md#deleteipgrouprequestrequesttypedef)
- [DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef)
- [DeleteWorkspaceBundleRequestRequestTypeDef](./type_defs.md#deleteworkspacebundlerequestrequesttypedef)
- [DeleteWorkspaceImageRequestRequestTypeDef](./type_defs.md#deleteworkspaceimagerequestrequesttypedef)
- [DeployWorkspaceApplicationsRequestRequestTypeDef](./type_defs.md#deployworkspaceapplicationsrequestrequesttypedef)
- [DeregisterWorkspaceDirectoryRequestRequestTypeDef](./type_defs.md#deregisterworkspacedirectoryrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAccountModificationsRequestRequestTypeDef](./type_defs.md#describeaccountmodificationsrequestrequesttypedef)
- [DescribeApplicationAssociationsRequestRequestTypeDef](./type_defs.md#describeapplicationassociationsrequestrequesttypedef)
- [DescribeApplicationsRequestRequestTypeDef](./type_defs.md#describeapplicationsrequestrequesttypedef)
- [WorkSpaceApplicationTypeDef](./type_defs.md#workspaceapplicationtypedef)
- [DescribeBundleAssociationsRequestRequestTypeDef](./type_defs.md#describebundleassociationsrequestrequesttypedef)
- [DescribeClientBrandingRequestRequestTypeDef](./type_defs.md#describeclientbrandingrequestrequesttypedef)
- [IosClientBrandingAttributesTypeDef](./type_defs.md#iosclientbrandingattributestypedef)
- [DescribeClientPropertiesRequestRequestTypeDef](./type_defs.md#describeclientpropertiesrequestrequesttypedef)
- [DescribeConnectClientAddInsRequestRequestTypeDef](./type_defs.md#describeconnectclientaddinsrequestrequesttypedef)
- [DescribeConnectionAliasPermissionsRequestRequestTypeDef](./type_defs.md#describeconnectionaliaspermissionsrequestrequesttypedef)
- [DescribeConnectionAliasesRequestRequestTypeDef](./type_defs.md#describeconnectionaliasesrequestrequesttypedef)
- [DescribeImageAssociationsRequestRequestTypeDef](./type_defs.md#describeimageassociationsrequestrequesttypedef)
- [DescribeIpGroupsRequestRequestTypeDef](./type_defs.md#describeipgroupsrequestrequesttypedef)
- [DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef)
- [DescribeWorkspaceAssociationsRequestRequestTypeDef](./type_defs.md#describeworkspaceassociationsrequestrequesttypedef)
- [DescribeWorkspaceBundlesRequestRequestTypeDef](./type_defs.md#describeworkspacebundlesrequestrequesttypedef)
- [DescribeWorkspaceDirectoriesFilterTypeDef](./type_defs.md#describeworkspacedirectoriesfiltertypedef)
- [DescribeWorkspaceImagePermissionsRequestRequestTypeDef](./type_defs.md#describeworkspaceimagepermissionsrequestrequesttypedef)
- [ImagePermissionTypeDef](./type_defs.md#imagepermissiontypedef)
- [DescribeWorkspaceImagesRequestRequestTypeDef](./type_defs.md#describeworkspaceimagesrequestrequesttypedef)
- [DescribeWorkspaceSnapshotsRequestRequestTypeDef](./type_defs.md#describeworkspacesnapshotsrequestrequesttypedef)
- [SnapshotTypeDef](./type_defs.md#snapshottypedef)
- [DescribeWorkspacesConnectionStatusRequestRequestTypeDef](./type_defs.md#describeworkspacesconnectionstatusrequestrequesttypedef)
- [WorkspaceConnectionStatusTypeDef](./type_defs.md#workspaceconnectionstatustypedef)
- [DescribeWorkspacesPoolSessionsRequestRequestTypeDef](./type_defs.md#describeworkspacespoolsessionsrequestrequesttypedef)
- [DescribeWorkspacesPoolsFilterTypeDef](./type_defs.md#describeworkspacespoolsfiltertypedef)
- [DescribeWorkspacesRequestRequestTypeDef](./type_defs.md#describeworkspacesrequestrequesttypedef)
- [DisassociateConnectionAliasRequestRequestTypeDef](./type_defs.md#disassociateconnectionaliasrequestrequesttypedef)
- [DisassociateIpGroupsRequestRequestTypeDef](./type_defs.md#disassociateipgroupsrequestrequesttypedef)
- [DisassociateWorkspaceApplicationRequestRequestTypeDef](./type_defs.md#disassociateworkspaceapplicationrequestrequesttypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef)
- [GetAccountLinkRequestRequestTypeDef](./type_defs.md#getaccountlinkrequestrequesttypedef)
- [IDCConfigTypeDef](./type_defs.md#idcconfigtypedef)
- [ListAccountLinksRequestRequestTypeDef](./type_defs.md#listaccountlinksrequestrequesttypedef)
- [ListAvailableManagementCidrRangesRequestRequestTypeDef](./type_defs.md#listavailablemanagementcidrrangesrequestrequesttypedef)
- [MicrosoftEntraConfigTypeDef](./type_defs.md#microsoftentraconfigtypedef)
- [MigrateWorkspaceRequestRequestTypeDef](./type_defs.md#migrateworkspacerequestrequesttypedef)
- [ModificationStateTypeDef](./type_defs.md#modificationstatetypedef)
- [ModifyAccountRequestRequestTypeDef](./type_defs.md#modifyaccountrequestrequesttypedef)
- [SamlPropertiesTypeDef](./type_defs.md#samlpropertiestypedef)
- [SelfservicePermissionsTypeDef](./type_defs.md#selfservicepermissionstypedef)
- [WorkspaceAccessPropertiesTypeDef](./type_defs.md#workspaceaccesspropertiestypedef)
- [WorkspaceCreationPropertiesTypeDef](./type_defs.md#workspacecreationpropertiestypedef)
- [WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef)
- [ModifyWorkspaceStateRequestRequestTypeDef](./type_defs.md#modifyworkspacestaterequestrequesttypedef)
- [NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef)
- [RebootRequestTypeDef](./type_defs.md#rebootrequesttypedef)
- [RebuildRequestTypeDef](./type_defs.md#rebuildrequesttypedef)
- [RejectAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#rejectaccountlinkinvitationrequestrequesttypedef)
- [RelatedWorkspacePropertiesTypeDef](./type_defs.md#relatedworkspacepropertiestypedef)
- [RestoreWorkspaceRequestRequestTypeDef](./type_defs.md#restoreworkspacerequestrequesttypedef)
- [RevokeIpRulesRequestRequestTypeDef](./type_defs.md#revokeiprulesrequestrequesttypedef)
- [StandbyWorkspacesPropertiesTypeDef](./type_defs.md#standbyworkspacespropertiestypedef)
- [StartRequestTypeDef](./type_defs.md#startrequesttypedef)
- [StartWorkspacesPoolRequestRequestTypeDef](./type_defs.md#startworkspacespoolrequestrequesttypedef)
- [StopRequestTypeDef](./type_defs.md#stoprequesttypedef)
- [StopWorkspacesPoolRequestRequestTypeDef](./type_defs.md#stopworkspacespoolrequestrequesttypedef)
- [StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef)
- [UserSettingTypeDef](./type_defs.md#usersettingtypedef)
- [TerminateRequestTypeDef](./type_defs.md#terminaterequesttypedef)
- [TerminateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#terminateworkspacespoolrequestrequesttypedef)
- [TerminateWorkspacesPoolSessionRequestRequestTypeDef](./type_defs.md#terminateworkspacespoolsessionrequestrequesttypedef)
- [UpdateConnectClientAddInRequestRequestTypeDef](./type_defs.md#updateconnectclientaddinrequestrequesttypedef)
- [UpdateResultTypeDef](./type_defs.md#updateresulttypedef)
- [UpdateWorkspaceBundleRequestRequestTypeDef](./type_defs.md#updateworkspacebundlerequestrequesttypedef)
- [UpdateWorkspaceImagePermissionRequestRequestTypeDef](./type_defs.md#updateworkspaceimagepermissionrequestrequesttypedef)
- [WorkspacePropertiesOutputTypeDef](./type_defs.md#workspacepropertiesoutputtypedef)
- [WorkspacesPoolErrorTypeDef](./type_defs.md#workspacespoolerrortypedef)
- [AcceptAccountLinkInvitationResultTypeDef](./type_defs.md#acceptaccountlinkinvitationresulttypedef)
- [AssociateConnectionAliasResultTypeDef](./type_defs.md#associateconnectionaliasresulttypedef)
- [CopyWorkspaceImageResultTypeDef](./type_defs.md#copyworkspaceimageresulttypedef)
- [CreateAccountLinkInvitationResultTypeDef](./type_defs.md#createaccountlinkinvitationresulttypedef)
- [CreateConnectClientAddInResultTypeDef](./type_defs.md#createconnectclientaddinresulttypedef)
- [CreateConnectionAliasResultTypeDef](./type_defs.md#createconnectionaliasresulttypedef)
- [CreateIpGroupResultTypeDef](./type_defs.md#createipgroupresulttypedef)
- [CreateUpdatedWorkspaceImageResultTypeDef](./type_defs.md#createupdatedworkspaceimageresulttypedef)
- [DeleteAccountLinkInvitationResultTypeDef](./type_defs.md#deleteaccountlinkinvitationresulttypedef)
- [DescribeAccountResultTypeDef](./type_defs.md#describeaccountresulttypedef)
- [GetAccountLinkResultTypeDef](./type_defs.md#getaccountlinkresulttypedef)
- [ImportWorkspaceImageResultTypeDef](./type_defs.md#importworkspaceimageresulttypedef)
- [ListAccountLinksResultTypeDef](./type_defs.md#listaccountlinksresulttypedef)
- [ListAvailableManagementCidrRangesResultTypeDef](./type_defs.md#listavailablemanagementcidrrangesresulttypedef)
- [MigrateWorkspaceResultTypeDef](./type_defs.md#migrateworkspaceresulttypedef)
- [RegisterWorkspaceDirectoryResultTypeDef](./type_defs.md#registerworkspacedirectoryresulttypedef)
- [RejectAccountLinkInvitationResultTypeDef](./type_defs.md#rejectaccountlinkinvitationresulttypedef)
- [DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef)
- [ApplicationResourceAssociationTypeDef](./type_defs.md#applicationresourceassociationtypedef)
- [BundleResourceAssociationTypeDef](./type_defs.md#bundleresourceassociationtypedef)
- [ImageResourceAssociationTypeDef](./type_defs.md#imageresourceassociationtypedef)
- [WorkspaceResourceAssociationTypeDef](./type_defs.md#workspaceresourceassociationtypedef)
- [AuthorizeIpRulesRequestRequestTypeDef](./type_defs.md#authorizeiprulesrequestrequesttypedef)
- [UpdateRulesOfIpGroupRequestRequestTypeDef](./type_defs.md#updaterulesofipgrouprequestrequesttypedef)
- [WorkspacesIpGroupTypeDef](./type_defs.md#workspacesipgrouptypedef)
- [DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef)
- [IosImportClientBrandingAttributesTypeDef](./type_defs.md#iosimportclientbrandingattributestypedef)
- [ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef](./type_defs.md#modifycertificatebasedauthpropertiesrequestrequesttypedef)
- [ClientPropertiesResultTypeDef](./type_defs.md#clientpropertiesresulttypedef)
- [ModifyClientPropertiesRequestRequestTypeDef](./type_defs.md#modifyclientpropertiesrequestrequesttypedef)
- [DescribeConnectClientAddInsResultTypeDef](./type_defs.md#describeconnectclientaddinsresulttypedef)
- [ConnectionAliasTypeDef](./type_defs.md#connectionaliastypedef)
- [DescribeConnectionAliasPermissionsResultTypeDef](./type_defs.md#describeconnectionaliaspermissionsresulttypedef)
- [UpdateConnectionAliasPermissionRequestRequestTypeDef](./type_defs.md#updateconnectionaliaspermissionrequestrequesttypedef)
- [CopyWorkspaceImageRequestRequestTypeDef](./type_defs.md#copyworkspaceimagerequestrequesttypedef)
- [CreateConnectionAliasRequestRequestTypeDef](./type_defs.md#createconnectionaliasrequestrequesttypedef)
- [CreateIpGroupRequestRequestTypeDef](./type_defs.md#createipgrouprequestrequesttypedef)
- [CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef)
- [CreateUpdatedWorkspaceImageRequestRequestTypeDef](./type_defs.md#createupdatedworkspaceimagerequestrequesttypedef)
- [CreateWorkspaceImageRequestRequestTypeDef](./type_defs.md#createworkspaceimagerequestrequesttypedef)
- [DescribeTagsResultTypeDef](./type_defs.md#describetagsresulttypedef)
- [ImportWorkspaceImageRequestRequestTypeDef](./type_defs.md#importworkspaceimagerequestrequesttypedef)
- [StandbyWorkspaceOutputTypeDef](./type_defs.md#standbyworkspaceoutputtypedef)
- [StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef)
- [CreateWorkspaceBundleRequestRequestTypeDef](./type_defs.md#createworkspacebundlerequestrequesttypedef)
- [WorkspaceBundleTypeDef](./type_defs.md#workspacebundletypedef)
- [CreateWorkspaceImageResultTypeDef](./type_defs.md#createworkspaceimageresulttypedef)
- [CreateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#createworkspacespoolrequestrequesttypedef)
- [UpdateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#updateworkspacespoolrequestrequesttypedef)
- [DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef](./type_defs.md#describeaccountmodificationsrequestdescribeaccountmodificationspaginatetypedef)
- [DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef](./type_defs.md#describeipgroupsrequestdescribeipgroupspaginatetypedef)
- [DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef](./type_defs.md#describeworkspacebundlesrequestdescribeworkspacebundlespaginatetypedef)
- [DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef](./type_defs.md#describeworkspaceimagesrequestdescribeworkspaceimagespaginatetypedef)
- [DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef](./type_defs.md#describeworkspacesconnectionstatusrequestdescribeworkspacesconnectionstatuspaginatetypedef)
- [DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef](./type_defs.md#describeworkspacesrequestdescribeworkspacespaginatetypedef)
- [ListAccountLinksRequestListAccountLinksPaginateTypeDef](./type_defs.md#listaccountlinksrequestlistaccountlinkspaginatetypedef)
- [ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef](./type_defs.md#listavailablemanagementcidrrangesrequestlistavailablemanagementcidrrangespaginatetypedef)
- [DescribeApplicationsResultTypeDef](./type_defs.md#describeapplicationsresulttypedef)
- [DescribeClientBrandingResultTypeDef](./type_defs.md#describeclientbrandingresulttypedef)
- [ImportClientBrandingResultTypeDef](./type_defs.md#importclientbrandingresulttypedef)
- [DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef](./type_defs.md#describeworkspacedirectoriesrequestdescribeworkspacedirectoriespaginatetypedef)
- [DescribeWorkspaceDirectoriesRequestRequestTypeDef](./type_defs.md#describeworkspacedirectoriesrequestrequesttypedef)
- [DescribeWorkspaceImagePermissionsResultTypeDef](./type_defs.md#describeworkspaceimagepermissionsresulttypedef)
- [DescribeWorkspaceSnapshotsResultTypeDef](./type_defs.md#describeworkspacesnapshotsresulttypedef)
- [DescribeWorkspacesConnectionStatusResultTypeDef](./type_defs.md#describeworkspacesconnectionstatusresulttypedef)
- [DescribeWorkspacesPoolsRequestRequestTypeDef](./type_defs.md#describeworkspacespoolsrequestrequesttypedef)
- [RebootWorkspacesResultTypeDef](./type_defs.md#rebootworkspacesresulttypedef)
- [RebuildWorkspacesResultTypeDef](./type_defs.md#rebuildworkspacesresulttypedef)
- [StartWorkspacesResultTypeDef](./type_defs.md#startworkspacesresulttypedef)
- [StopWorkspacesResultTypeDef](./type_defs.md#stopworkspacesresulttypedef)
- [TerminateWorkspacesResultTypeDef](./type_defs.md#terminateworkspacesresulttypedef)
- [RegisterWorkspaceDirectoryRequestRequestTypeDef](./type_defs.md#registerworkspacedirectoryrequestrequesttypedef)
- [ModifySamlPropertiesRequestRequestTypeDef](./type_defs.md#modifysamlpropertiesrequestrequesttypedef)
- [ModifySelfservicePermissionsRequestRequestTypeDef](./type_defs.md#modifyselfservicepermissionsrequestrequesttypedef)
- [ModifyWorkspaceAccessPropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspaceaccesspropertiesrequestrequesttypedef)
- [ModifyWorkspaceCreationPropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspacecreationpropertiesrequestrequesttypedef)
- [ModifyWorkspacePropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspacepropertiesrequestrequesttypedef)
- [WorkspacesPoolSessionTypeDef](./type_defs.md#workspacespoolsessiontypedef)
- [RebootWorkspacesRequestRequestTypeDef](./type_defs.md#rebootworkspacesrequestrequesttypedef)
- [RebuildWorkspacesRequestRequestTypeDef](./type_defs.md#rebuildworkspacesrequestrequesttypedef)
- [StartWorkspacesRequestRequestTypeDef](./type_defs.md#startworkspacesrequestrequesttypedef)
- [StopWorkspacesRequestRequestTypeDef](./type_defs.md#stopworkspacesrequestrequesttypedef)
- [StreamingPropertiesOutputTypeDef](./type_defs.md#streamingpropertiesoutputtypedef)
- [StreamingPropertiesTypeDef](./type_defs.md#streamingpropertiestypedef)
- [TerminateWorkspacesRequestRequestTypeDef](./type_defs.md#terminateworkspacesrequestrequesttypedef)
- [WorkspaceImageTypeDef](./type_defs.md#workspaceimagetypedef)
- [WorkspacePropertiesUnionTypeDef](./type_defs.md#workspacepropertiesuniontypedef)
- [WorkspaceRequestOutputTypeDef](./type_defs.md#workspacerequestoutputtypedef)
- [WorkspaceTypeDef](./type_defs.md#workspacetypedef)
- [WorkspacesPoolTypeDef](./type_defs.md#workspacespooltypedef)
- [DescribeApplicationAssociationsResultTypeDef](./type_defs.md#describeapplicationassociationsresulttypedef)
- [DescribeBundleAssociationsResultTypeDef](./type_defs.md#describebundleassociationsresulttypedef)
- [DescribeImageAssociationsResultTypeDef](./type_defs.md#describeimageassociationsresulttypedef)
- [AssociateWorkspaceApplicationResultTypeDef](./type_defs.md#associateworkspaceapplicationresulttypedef)
- [DescribeWorkspaceAssociationsResultTypeDef](./type_defs.md#describeworkspaceassociationsresulttypedef)
- [DisassociateWorkspaceApplicationResultTypeDef](./type_defs.md#disassociateworkspaceapplicationresulttypedef)
- [WorkSpaceApplicationDeploymentTypeDef](./type_defs.md#workspaceapplicationdeploymenttypedef)
- [DescribeIpGroupsResultTypeDef](./type_defs.md#describeipgroupsresulttypedef)
- [ImportClientBrandingRequestRequestTypeDef](./type_defs.md#importclientbrandingrequestrequesttypedef)
- [DescribeClientPropertiesResultTypeDef](./type_defs.md#describeclientpropertiesresulttypedef)
- [DescribeConnectionAliasesResultTypeDef](./type_defs.md#describeconnectionaliasesresulttypedef)
- [FailedCreateStandbyWorkspacesRequestTypeDef](./type_defs.md#failedcreatestandbyworkspacesrequesttypedef)
- [StandbyWorkspaceUnionTypeDef](./type_defs.md#standbyworkspaceuniontypedef)
- [CreateWorkspaceBundleResultTypeDef](./type_defs.md#createworkspacebundleresulttypedef)
- [DescribeWorkspaceBundlesResultTypeDef](./type_defs.md#describeworkspacebundlesresulttypedef)
- [DescribeWorkspacesPoolSessionsResultTypeDef](./type_defs.md#describeworkspacespoolsessionsresulttypedef)
- [WorkspaceDirectoryTypeDef](./type_defs.md#workspacedirectorytypedef)
- [ModifyStreamingPropertiesRequestRequestTypeDef](./type_defs.md#modifystreamingpropertiesrequestrequesttypedef)
- [DescribeWorkspaceImagesResultTypeDef](./type_defs.md#describeworkspaceimagesresulttypedef)
- [WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef)
- [FailedCreateWorkspaceRequestTypeDef](./type_defs.md#failedcreateworkspacerequesttypedef)
- [DescribeWorkspacesResultTypeDef](./type_defs.md#describeworkspacesresulttypedef)
- [CreateWorkspacesPoolResultTypeDef](./type_defs.md#createworkspacespoolresulttypedef)
- [DescribeWorkspacesPoolsResultTypeDef](./type_defs.md#describeworkspacespoolsresulttypedef)
- [UpdateWorkspacesPoolResultTypeDef](./type_defs.md#updateworkspacespoolresulttypedef)
- [DeployWorkspaceApplicationsResultTypeDef](./type_defs.md#deployworkspaceapplicationsresulttypedef)
- [CreateStandbyWorkspacesResultTypeDef](./type_defs.md#createstandbyworkspacesresulttypedef)
- [CreateStandbyWorkspacesRequestRequestTypeDef](./type_defs.md#createstandbyworkspacesrequestrequesttypedef)
- [DescribeWorkspaceDirectoriesResultTypeDef](./type_defs.md#describeworkspacedirectoriesresulttypedef)
- [WorkspaceRequestUnionTypeDef](./type_defs.md#workspacerequestuniontypedef)
- [CreateWorkspacesResultTypeDef](./type_defs.md#createworkspacesresulttypedef)
- [CreateWorkspacesRequestRequestTypeDef](./type_defs.md#createworkspacesrequestrequesttypedef)

