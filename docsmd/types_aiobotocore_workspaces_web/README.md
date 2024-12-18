# WorkSpacesWeb module

> [Index](../README.md) > WorkSpacesWeb


!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#workspacesweb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkSpacesWeb` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkSpacesWeb` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workspaces-web]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workspaces-web]'

# standalone installation
python -m pip install types-aiobotocore-workspaces-web
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workspaces-web
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkSpacesWebClient

Type annotations and code completion for  `#!python session.create_client("workspaces-web")` as [WorkSpacesWebClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client)

```python
# WorkSpacesWebClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient


session = get_session()
async with session.create_client("workspaces-web") as client:
    client: WorkSpacesWebClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("workspaces-web").get_paginator("...")`.

```python
# ListDataProtectionSettingsPaginator usage example

from types_aiobotocore_workspaces_web.paginator import ListDataProtectionSettingsPaginator

def get_list_data_protection_settings_paginator() -> ListDataProtectionSettingsPaginator:
    return client.get_paginator("list_data_protection_settings"))
```

- [ListDataProtectionSettingsPaginator](./paginators.md#listdataprotectionsettingspaginator)
- [ListSessionsPaginator](./paginators.md#listsessionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthenticationTypeType usage example

from types_aiobotocore_workspaces_web.literals import AuthenticationTypeType

def get_value() -> AuthenticationTypeType:
    return "IAM_Identity_Center"
```

- [AuthenticationTypeType](./literals.md#authenticationtypetype)
- [BrowserTypeType](./literals.md#browsertypetype)
- [EnabledTypeType](./literals.md#enabledtypetype)
- [IdentityProviderTypeType](./literals.md#identityprovidertypetype)
- [InstanceTypeType](./literals.md#instancetypetype)
- [ListDataProtectionSettingsPaginatorName](./literals.md#listdataprotectionsettingspaginatorname)
- [ListSessionsPaginatorName](./literals.md#listsessionspaginatorname)
- [PortalStatusType](./literals.md#portalstatustype)
- [RedactionPlaceHolderTypeType](./literals.md#redactionplaceholdertypetype)
- [RendererTypeType](./literals.md#renderertypetype)
- [SessionSortByType](./literals.md#sessionsortbytype)
- [SessionStatusType](./literals.md#sessionstatustype)
- [WorkSpacesWebServiceName](./literals.md#workspaceswebservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#associatebrowsersettingsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociateDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#associatedataprotectionsettingsrequestrequesttypedef)
- [AssociateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#associateipaccesssettingsrequestrequesttypedef)
- [AssociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#associatenetworksettingsrequestrequesttypedef)
- [AssociateTrustStoreRequestRequestTypeDef](./type_defs.md#associatetruststorerequestrequesttypedef)
- [AssociateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#associateuseraccessloggingsettingsrequestrequesttypedef)
- [AssociateUserSettingsRequestRequestTypeDef](./type_defs.md#associateusersettingsrequestrequesttypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BrowserSettingsSummaryTypeDef](./type_defs.md#browsersettingssummarytypedef)
- [BrowserSettingsTypeDef](./type_defs.md#browsersettingstypedef)
- [CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef)
- [CertificateTypeDef](./type_defs.md#certificatetypedef)
- [CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [IpRuleTypeDef](./type_defs.md#ipruletypedef)
- [CustomPatternTypeDef](./type_defs.md#custompatterntypedef)
- [DataProtectionSettingsSummaryTypeDef](./type_defs.md#dataprotectionsettingssummarytypedef)
- [DeleteBrowserSettingsRequestRequestTypeDef](./type_defs.md#deletebrowsersettingsrequestrequesttypedef)
- [DeleteDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#deletedataprotectionsettingsrequestrequesttypedef)
- [DeleteIdentityProviderRequestRequestTypeDef](./type_defs.md#deleteidentityproviderrequestrequesttypedef)
- [DeleteIpAccessSettingsRequestRequestTypeDef](./type_defs.md#deleteipaccesssettingsrequestrequesttypedef)
- [DeleteNetworkSettingsRequestRequestTypeDef](./type_defs.md#deletenetworksettingsrequestrequesttypedef)
- [DeletePortalRequestRequestTypeDef](./type_defs.md#deleteportalrequestrequesttypedef)
- [DeleteTrustStoreRequestRequestTypeDef](./type_defs.md#deletetruststorerequestrequesttypedef)
- [DeleteUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#deleteuseraccessloggingsettingsrequestrequesttypedef)
- [DeleteUserSettingsRequestRequestTypeDef](./type_defs.md#deleteusersettingsrequestrequesttypedef)
- [DisassociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#disassociatebrowsersettingsrequestrequesttypedef)
- [DisassociateDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#disassociatedataprotectionsettingsrequestrequesttypedef)
- [DisassociateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#disassociateipaccesssettingsrequestrequesttypedef)
- [DisassociateNetworkSettingsRequestRequestTypeDef](./type_defs.md#disassociatenetworksettingsrequestrequesttypedef)
- [DisassociateTrustStoreRequestRequestTypeDef](./type_defs.md#disassociatetruststorerequestrequesttypedef)
- [DisassociateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#disassociateuseraccessloggingsettingsrequestrequesttypedef)
- [DisassociateUserSettingsRequestRequestTypeDef](./type_defs.md#disassociateusersettingsrequestrequesttypedef)
- [ExpireSessionRequestRequestTypeDef](./type_defs.md#expiresessionrequestrequesttypedef)
- [GetBrowserSettingsRequestRequestTypeDef](./type_defs.md#getbrowsersettingsrequestrequesttypedef)
- [GetDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#getdataprotectionsettingsrequestrequesttypedef)
- [GetIdentityProviderRequestRequestTypeDef](./type_defs.md#getidentityproviderrequestrequesttypedef)
- [IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef)
- [GetIpAccessSettingsRequestRequestTypeDef](./type_defs.md#getipaccesssettingsrequestrequesttypedef)
- [GetNetworkSettingsRequestRequestTypeDef](./type_defs.md#getnetworksettingsrequestrequesttypedef)
- [NetworkSettingsTypeDef](./type_defs.md#networksettingstypedef)
- [GetPortalRequestRequestTypeDef](./type_defs.md#getportalrequestrequesttypedef)
- [PortalTypeDef](./type_defs.md#portaltypedef)
- [GetPortalServiceProviderMetadataRequestRequestTypeDef](./type_defs.md#getportalserviceprovidermetadatarequestrequesttypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [SessionTypeDef](./type_defs.md#sessiontypedef)
- [GetTrustStoreCertificateRequestRequestTypeDef](./type_defs.md#gettruststorecertificaterequestrequesttypedef)
- [GetTrustStoreRequestRequestTypeDef](./type_defs.md#gettruststorerequestrequesttypedef)
- [TrustStoreTypeDef](./type_defs.md#truststoretypedef)
- [GetUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#getuseraccessloggingsettingsrequestrequesttypedef)
- [UserAccessLoggingSettingsTypeDef](./type_defs.md#useraccessloggingsettingstypedef)
- [GetUserSettingsRequestRequestTypeDef](./type_defs.md#getusersettingsrequestrequesttypedef)
- [IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef)
- [RedactionPlaceHolderTypeDef](./type_defs.md#redactionplaceholdertypedef)
- [IpAccessSettingsSummaryTypeDef](./type_defs.md#ipaccesssettingssummarytypedef)
- [ListBrowserSettingsRequestRequestTypeDef](./type_defs.md#listbrowsersettingsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#listdataprotectionsettingsrequestrequesttypedef)
- [ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef)
- [ListIpAccessSettingsRequestRequestTypeDef](./type_defs.md#listipaccesssettingsrequestrequesttypedef)
- [ListNetworkSettingsRequestRequestTypeDef](./type_defs.md#listnetworksettingsrequestrequesttypedef)
- [NetworkSettingsSummaryTypeDef](./type_defs.md#networksettingssummarytypedef)
- [ListPortalsRequestRequestTypeDef](./type_defs.md#listportalsrequestrequesttypedef)
- [PortalSummaryTypeDef](./type_defs.md#portalsummarytypedef)
- [ListSessionsRequestRequestTypeDef](./type_defs.md#listsessionsrequestrequesttypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTrustStoreCertificatesRequestRequestTypeDef](./type_defs.md#listtruststorecertificatesrequestrequesttypedef)
- [ListTrustStoresRequestRequestTypeDef](./type_defs.md#listtruststoresrequestrequesttypedef)
- [TrustStoreSummaryTypeDef](./type_defs.md#truststoresummarytypedef)
- [ListUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#listuseraccessloggingsettingsrequestrequesttypedef)
- [UserAccessLoggingSettingsSummaryTypeDef](./type_defs.md#useraccessloggingsettingssummarytypedef)
- [ListUserSettingsRequestRequestTypeDef](./type_defs.md#listusersettingsrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateBrowserSettingsRequestRequestTypeDef](./type_defs.md#updatebrowsersettingsrequestrequesttypedef)
- [UpdateIdentityProviderRequestRequestTypeDef](./type_defs.md#updateidentityproviderrequestrequesttypedef)
- [UpdateNetworkSettingsRequestRequestTypeDef](./type_defs.md#updatenetworksettingsrequestrequesttypedef)
- [UpdatePortalRequestRequestTypeDef](./type_defs.md#updateportalrequestrequesttypedef)
- [UpdateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#updateuseraccessloggingsettingsrequestrequesttypedef)
- [AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef)
- [AssociateDataProtectionSettingsResponseTypeDef](./type_defs.md#associatedataprotectionsettingsresponsetypedef)
- [AssociateIpAccessSettingsResponseTypeDef](./type_defs.md#associateipaccesssettingsresponsetypedef)
- [AssociateNetworkSettingsResponseTypeDef](./type_defs.md#associatenetworksettingsresponsetypedef)
- [AssociateTrustStoreResponseTypeDef](./type_defs.md#associatetruststoreresponsetypedef)
- [AssociateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#associateuseraccessloggingsettingsresponsetypedef)
- [AssociateUserSettingsResponseTypeDef](./type_defs.md#associateusersettingsresponsetypedef)
- [CreateBrowserSettingsResponseTypeDef](./type_defs.md#createbrowsersettingsresponsetypedef)
- [CreateDataProtectionSettingsResponseTypeDef](./type_defs.md#createdataprotectionsettingsresponsetypedef)
- [CreateIdentityProviderResponseTypeDef](./type_defs.md#createidentityproviderresponsetypedef)
- [CreateIpAccessSettingsResponseTypeDef](./type_defs.md#createipaccesssettingsresponsetypedef)
- [CreateNetworkSettingsResponseTypeDef](./type_defs.md#createnetworksettingsresponsetypedef)
- [CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef)
- [CreateTrustStoreResponseTypeDef](./type_defs.md#createtruststoreresponsetypedef)
- [CreateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#createuseraccessloggingsettingsresponsetypedef)
- [CreateUserSettingsResponseTypeDef](./type_defs.md#createusersettingsresponsetypedef)
- [GetPortalServiceProviderMetadataResponseTypeDef](./type_defs.md#getportalserviceprovidermetadataresponsetypedef)
- [UpdateTrustStoreResponseTypeDef](./type_defs.md#updatetruststoreresponsetypedef)
- [UpdateTrustStoreRequestRequestTypeDef](./type_defs.md#updatetruststorerequestrequesttypedef)
- [ListBrowserSettingsResponseTypeDef](./type_defs.md#listbrowsersettingsresponsetypedef)
- [GetBrowserSettingsResponseTypeDef](./type_defs.md#getbrowsersettingsresponsetypedef)
- [UpdateBrowserSettingsResponseTypeDef](./type_defs.md#updatebrowsersettingsresponsetypedef)
- [ListTrustStoreCertificatesResponseTypeDef](./type_defs.md#listtruststorecertificatesresponsetypedef)
- [GetTrustStoreCertificateResponseTypeDef](./type_defs.md#gettruststorecertificateresponsetypedef)
- [CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef)
- [CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef)
- [CreateBrowserSettingsRequestRequestTypeDef](./type_defs.md#createbrowsersettingsrequestrequesttypedef)
- [CreateIdentityProviderRequestRequestTypeDef](./type_defs.md#createidentityproviderrequestrequesttypedef)
- [CreateNetworkSettingsRequestRequestTypeDef](./type_defs.md#createnetworksettingsrequestrequesttypedef)
- [CreatePortalRequestRequestTypeDef](./type_defs.md#createportalrequestrequesttypedef)
- [CreateTrustStoreRequestRequestTypeDef](./type_defs.md#createtruststorerequestrequesttypedef)
- [CreateUserAccessLoggingSettingsRequestRequestTypeDef](./type_defs.md#createuseraccessloggingsettingsrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#createipaccesssettingsrequestrequesttypedef)
- [IpAccessSettingsTypeDef](./type_defs.md#ipaccesssettingstypedef)
- [UpdateIpAccessSettingsRequestRequestTypeDef](./type_defs.md#updateipaccesssettingsrequestrequesttypedef)
- [ListDataProtectionSettingsResponseTypeDef](./type_defs.md#listdataprotectionsettingsresponsetypedef)
- [GetIdentityProviderResponseTypeDef](./type_defs.md#getidentityproviderresponsetypedef)
- [UpdateIdentityProviderResponseTypeDef](./type_defs.md#updateidentityproviderresponsetypedef)
- [GetNetworkSettingsResponseTypeDef](./type_defs.md#getnetworksettingsresponsetypedef)
- [UpdateNetworkSettingsResponseTypeDef](./type_defs.md#updatenetworksettingsresponsetypedef)
- [GetPortalResponseTypeDef](./type_defs.md#getportalresponsetypedef)
- [UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [GetTrustStoreResponseTypeDef](./type_defs.md#gettruststoreresponsetypedef)
- [GetUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#getuseraccessloggingsettingsresponsetypedef)
- [UpdateUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#updateuseraccessloggingsettingsresponsetypedef)
- [ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef)
- [InlineRedactionPatternOutputTypeDef](./type_defs.md#inlineredactionpatternoutputtypedef)
- [InlineRedactionPatternTypeDef](./type_defs.md#inlineredactionpatterntypedef)
- [ListIpAccessSettingsResponseTypeDef](./type_defs.md#listipaccesssettingsresponsetypedef)
- [ListDataProtectionSettingsRequestListDataProtectionSettingsPaginateTypeDef](./type_defs.md#listdataprotectionsettingsrequestlistdataprotectionsettingspaginatetypedef)
- [ListSessionsRequestListSessionsPaginateTypeDef](./type_defs.md#listsessionsrequestlistsessionspaginatetypedef)
- [ListNetworkSettingsResponseTypeDef](./type_defs.md#listnetworksettingsresponsetypedef)
- [ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef)
- [ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef)
- [ListTrustStoresResponseTypeDef](./type_defs.md#listtruststoresresponsetypedef)
- [ListUserAccessLoggingSettingsResponseTypeDef](./type_defs.md#listuseraccessloggingsettingsresponsetypedef)
- [UserSettingsSummaryTypeDef](./type_defs.md#usersettingssummarytypedef)
- [UserSettingsTypeDef](./type_defs.md#usersettingstypedef)
- [CreateUserSettingsRequestRequestTypeDef](./type_defs.md#createusersettingsrequestrequesttypedef)
- [UpdateUserSettingsRequestRequestTypeDef](./type_defs.md#updateusersettingsrequestrequesttypedef)
- [GetIpAccessSettingsResponseTypeDef](./type_defs.md#getipaccesssettingsresponsetypedef)
- [UpdateIpAccessSettingsResponseTypeDef](./type_defs.md#updateipaccesssettingsresponsetypedef)
- [InlineRedactionConfigurationOutputTypeDef](./type_defs.md#inlineredactionconfigurationoutputtypedef)
- [InlineRedactionPatternUnionTypeDef](./type_defs.md#inlineredactionpatternuniontypedef)
- [ListUserSettingsResponseTypeDef](./type_defs.md#listusersettingsresponsetypedef)
- [GetUserSettingsResponseTypeDef](./type_defs.md#getusersettingsresponsetypedef)
- [UpdateUserSettingsResponseTypeDef](./type_defs.md#updateusersettingsresponsetypedef)
- [DataProtectionSettingsTypeDef](./type_defs.md#dataprotectionsettingstypedef)
- [InlineRedactionConfigurationTypeDef](./type_defs.md#inlineredactionconfigurationtypedef)
- [GetDataProtectionSettingsResponseTypeDef](./type_defs.md#getdataprotectionsettingsresponsetypedef)
- [UpdateDataProtectionSettingsResponseTypeDef](./type_defs.md#updatedataprotectionsettingsresponsetypedef)
- [CreateDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#createdataprotectionsettingsrequestrequesttypedef)
- [UpdateDataProtectionSettingsRequestRequestTypeDef](./type_defs.md#updatedataprotectionsettingsrequestrequesttypedef)

