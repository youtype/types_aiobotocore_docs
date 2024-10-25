# Type definitions

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## AssociateBrowserSettingsRequestRequestTypeDef

```python
# AssociateBrowserSettingsRequestRequestTypeDef definition

class AssociateBrowserSettingsRequestRequestTypeDef(TypedDict):
    browserSettingsArn: str,
    portalArn: str,
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

## AssociateIpAccessSettingsRequestRequestTypeDef

```python
# AssociateIpAccessSettingsRequestRequestTypeDef definition

class AssociateIpAccessSettingsRequestRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    portalArn: str,
```

## AssociateNetworkSettingsRequestRequestTypeDef

```python
# AssociateNetworkSettingsRequestRequestTypeDef definition

class AssociateNetworkSettingsRequestRequestTypeDef(TypedDict):
    networkSettingsArn: str,
    portalArn: str,
```

## AssociateTrustStoreRequestRequestTypeDef

```python
# AssociateTrustStoreRequestRequestTypeDef definition

class AssociateTrustStoreRequestRequestTypeDef(TypedDict):
    portalArn: str,
    trustStoreArn: str,
```

## AssociateUserAccessLoggingSettingsRequestRequestTypeDef

```python
# AssociateUserAccessLoggingSettingsRequestRequestTypeDef definition

class AssociateUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
    userAccessLoggingSettingsArn: str,
```

## AssociateUserSettingsRequestRequestTypeDef

```python
# AssociateUserSettingsRequestRequestTypeDef definition

class AssociateUserSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
    userSettingsArn: str,
```

## BrowserSettingsSummaryTypeDef

```python
# BrowserSettingsSummaryTypeDef definition

class BrowserSettingsSummaryTypeDef(TypedDict):
    browserSettingsArn: str,
```

## BrowserSettingsTypeDef

```python
# BrowserSettingsTypeDef definition

class BrowserSettingsTypeDef(TypedDict):
    browserSettingsArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    associatedPortalArns: NotRequired[List[str]],
    browserPolicy: NotRequired[str],
    customerManagedKey: NotRequired[str],
```

## CertificateSummaryTypeDef

```python
# CertificateSummaryTypeDef definition

class CertificateSummaryTypeDef(TypedDict):
    issuer: NotRequired[str],
    notValidAfter: NotRequired[datetime],
    notValidBefore: NotRequired[datetime],
    subject: NotRequired[str],
    thumbprint: NotRequired[str],
```

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    body: NotRequired[bytes],
    issuer: NotRequired[str],
    notValidAfter: NotRequired[datetime],
    notValidBefore: NotRequired[datetime],
    subject: NotRequired[str],
    thumbprint: NotRequired[str],
```

## CookieSpecificationTypeDef

```python
# CookieSpecificationTypeDef definition

class CookieSpecificationTypeDef(TypedDict):
    domain: str,
    name: NotRequired[str],
    path: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## IpRuleTypeDef

```python
# IpRuleTypeDef definition

class IpRuleTypeDef(TypedDict):
    ipRange: str,
    description: NotRequired[str],
```

## DeleteBrowserSettingsRequestRequestTypeDef

```python
# DeleteBrowserSettingsRequestRequestTypeDef definition

class DeleteBrowserSettingsRequestRequestTypeDef(TypedDict):
    browserSettingsArn: str,
```

## DeleteIdentityProviderRequestRequestTypeDef

```python
# DeleteIdentityProviderRequestRequestTypeDef definition

class DeleteIdentityProviderRequestRequestTypeDef(TypedDict):
    identityProviderArn: str,
```

## DeleteIpAccessSettingsRequestRequestTypeDef

```python
# DeleteIpAccessSettingsRequestRequestTypeDef definition

class DeleteIpAccessSettingsRequestRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
```

## DeleteNetworkSettingsRequestRequestTypeDef

```python
# DeleteNetworkSettingsRequestRequestTypeDef definition

class DeleteNetworkSettingsRequestRequestTypeDef(TypedDict):
    networkSettingsArn: str,
```

## DeletePortalRequestRequestTypeDef

```python
# DeletePortalRequestRequestTypeDef definition

class DeletePortalRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DeleteTrustStoreRequestRequestTypeDef

```python
# DeleteTrustStoreRequestRequestTypeDef definition

class DeleteTrustStoreRequestRequestTypeDef(TypedDict):
    trustStoreArn: str,
```

## DeleteUserAccessLoggingSettingsRequestRequestTypeDef

```python
# DeleteUserAccessLoggingSettingsRequestRequestTypeDef definition

class DeleteUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
```

## DeleteUserSettingsRequestRequestTypeDef

```python
# DeleteUserSettingsRequestRequestTypeDef definition

class DeleteUserSettingsRequestRequestTypeDef(TypedDict):
    userSettingsArn: str,
```

## DisassociateBrowserSettingsRequestRequestTypeDef

```python
# DisassociateBrowserSettingsRequestRequestTypeDef definition

class DisassociateBrowserSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateIpAccessSettingsRequestRequestTypeDef

```python
# DisassociateIpAccessSettingsRequestRequestTypeDef definition

class DisassociateIpAccessSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateNetworkSettingsRequestRequestTypeDef

```python
# DisassociateNetworkSettingsRequestRequestTypeDef definition

class DisassociateNetworkSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateTrustStoreRequestRequestTypeDef

```python
# DisassociateTrustStoreRequestRequestTypeDef definition

class DisassociateTrustStoreRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateUserAccessLoggingSettingsRequestRequestTypeDef

```python
# DisassociateUserAccessLoggingSettingsRequestRequestTypeDef definition

class DisassociateUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateUserSettingsRequestRequestTypeDef

```python
# DisassociateUserSettingsRequestRequestTypeDef definition

class DisassociateUserSettingsRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## ExpireSessionRequestRequestTypeDef

```python
# ExpireSessionRequestRequestTypeDef definition

class ExpireSessionRequestRequestTypeDef(TypedDict):
    portalId: str,
    sessionId: str,
```

## GetBrowserSettingsRequestRequestTypeDef

```python
# GetBrowserSettingsRequestRequestTypeDef definition

class GetBrowserSettingsRequestRequestTypeDef(TypedDict):
    browserSettingsArn: str,
```

## GetIdentityProviderRequestRequestTypeDef

```python
# GetIdentityProviderRequestRequestTypeDef definition

class GetIdentityProviderRequestRequestTypeDef(TypedDict):
    identityProviderArn: str,
```

## IdentityProviderTypeDef

```python
# IdentityProviderTypeDef definition

class IdentityProviderTypeDef(TypedDict):
    identityProviderArn: str,
    identityProviderDetails: NotRequired[Dict[str, str]],
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## GetIpAccessSettingsRequestRequestTypeDef

```python
# GetIpAccessSettingsRequestRequestTypeDef definition

class GetIpAccessSettingsRequestRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
```

## GetNetworkSettingsRequestRequestTypeDef

```python
# GetNetworkSettingsRequestRequestTypeDef definition

class GetNetworkSettingsRequestRequestTypeDef(TypedDict):
    networkSettingsArn: str,
```

## NetworkSettingsTypeDef

```python
# NetworkSettingsTypeDef definition

class NetworkSettingsTypeDef(TypedDict):
    networkSettingsArn: str,
    associatedPortalArns: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
    subnetIds: NotRequired[List[str]],
    vpcId: NotRequired[str],
```

## GetPortalRequestRequestTypeDef

```python
# GetPortalRequestRequestTypeDef definition

class GetPortalRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## PortalTypeDef

```python
# PortalTypeDef definition

class PortalTypeDef(TypedDict):
    portalArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    browserSettingsArn: NotRequired[str],
    browserType: NotRequired[BrowserTypeType],  # (2)
    creationDate: NotRequired[datetime],
    customerManagedKey: NotRequired[str],
    displayName: NotRequired[str],
    instanceType: NotRequired[InstanceTypeType],  # (3)
    ipAccessSettingsArn: NotRequired[str],
    maxConcurrentSessions: NotRequired[int],
    networkSettingsArn: NotRequired[str],
    portalEndpoint: NotRequired[str],
    portalStatus: NotRequired[PortalStatusType],  # (4)
    rendererType: NotRequired[RendererTypeType],  # (5)
    statusReason: NotRequired[str],
    trustStoreArn: NotRequired[str],
    userAccessLoggingSettingsArn: NotRequired[str],
    userSettingsArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: BrowserTypeType](./literals.md#browsertypetype) 
3. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
4. See [:material-code-brackets: PortalStatusType](./literals.md#portalstatustype) 
5. See [:material-code-brackets: RendererTypeType](./literals.md#renderertypetype) 
## GetPortalServiceProviderMetadataRequestRequestTypeDef

```python
# GetPortalServiceProviderMetadataRequestRequestTypeDef definition

class GetPortalServiceProviderMetadataRequestRequestTypeDef(TypedDict):
    portalArn: str,
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    portalId: str,
    sessionId: str,
```

## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    clientIpAddresses: NotRequired[List[str]],
    endTime: NotRequired[datetime],
    portalArn: NotRequired[str],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    status: NotRequired[SessionStatusType],  # (1)
    username: NotRequired[str],
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
## GetTrustStoreCertificateRequestRequestTypeDef

```python
# GetTrustStoreCertificateRequestRequestTypeDef definition

class GetTrustStoreCertificateRequestRequestTypeDef(TypedDict):
    thumbprint: str,
    trustStoreArn: str,
```

## GetTrustStoreRequestRequestTypeDef

```python
# GetTrustStoreRequestRequestTypeDef definition

class GetTrustStoreRequestRequestTypeDef(TypedDict):
    trustStoreArn: str,
```

## TrustStoreTypeDef

```python
# TrustStoreTypeDef definition

class TrustStoreTypeDef(TypedDict):
    trustStoreArn: str,
    associatedPortalArns: NotRequired[List[str]],
```

## GetUserAccessLoggingSettingsRequestRequestTypeDef

```python
# GetUserAccessLoggingSettingsRequestRequestTypeDef definition

class GetUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
```

## UserAccessLoggingSettingsTypeDef

```python
# UserAccessLoggingSettingsTypeDef definition

class UserAccessLoggingSettingsTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    associatedPortalArns: NotRequired[List[str]],
    kinesisStreamArn: NotRequired[str],
```

## GetUserSettingsRequestRequestTypeDef

```python
# GetUserSettingsRequestRequestTypeDef definition

class GetUserSettingsRequestRequestTypeDef(TypedDict):
    userSettingsArn: str,
```

## IdentityProviderSummaryTypeDef

```python
# IdentityProviderSummaryTypeDef definition

class IdentityProviderSummaryTypeDef(TypedDict):
    identityProviderArn: str,
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## IpAccessSettingsSummaryTypeDef

```python
# IpAccessSettingsSummaryTypeDef definition

class IpAccessSettingsSummaryTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    creationDate: NotRequired[datetime],
    description: NotRequired[str],
    displayName: NotRequired[str],
```

## ListBrowserSettingsRequestRequestTypeDef

```python
# ListBrowserSettingsRequestRequestTypeDef definition

class ListBrowserSettingsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdentityProvidersRequestRequestTypeDef

```python
# ListIdentityProvidersRequestRequestTypeDef definition

class ListIdentityProvidersRequestRequestTypeDef(TypedDict):
    portalArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIpAccessSettingsRequestRequestTypeDef

```python
# ListIpAccessSettingsRequestRequestTypeDef definition

class ListIpAccessSettingsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListNetworkSettingsRequestRequestTypeDef

```python
# ListNetworkSettingsRequestRequestTypeDef definition

class ListNetworkSettingsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NetworkSettingsSummaryTypeDef

```python
# NetworkSettingsSummaryTypeDef definition

class NetworkSettingsSummaryTypeDef(TypedDict):
    networkSettingsArn: str,
    vpcId: NotRequired[str],
```

## ListPortalsRequestRequestTypeDef

```python
# ListPortalsRequestRequestTypeDef definition

class ListPortalsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PortalSummaryTypeDef

```python
# PortalSummaryTypeDef definition

class PortalSummaryTypeDef(TypedDict):
    portalArn: str,
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    browserSettingsArn: NotRequired[str],
    browserType: NotRequired[BrowserTypeType],  # (2)
    creationDate: NotRequired[datetime],
    displayName: NotRequired[str],
    instanceType: NotRequired[InstanceTypeType],  # (3)
    ipAccessSettingsArn: NotRequired[str],
    maxConcurrentSessions: NotRequired[int],
    networkSettingsArn: NotRequired[str],
    portalEndpoint: NotRequired[str],
    portalStatus: NotRequired[PortalStatusType],  # (4)
    rendererType: NotRequired[RendererTypeType],  # (5)
    trustStoreArn: NotRequired[str],
    userAccessLoggingSettingsArn: NotRequired[str],
    userSettingsArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: BrowserTypeType](./literals.md#browsertypetype) 
3. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
4. See [:material-code-brackets: PortalStatusType](./literals.md#portalstatustype) 
5. See [:material-code-brackets: RendererTypeType](./literals.md#renderertypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSessionsRequestRequestTypeDef

```python
# ListSessionsRequestRequestTypeDef definition

class ListSessionsRequestRequestTypeDef(TypedDict):
    portalId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sessionId: NotRequired[str],
    sortBy: NotRequired[SessionSortByType],  # (1)
    status: NotRequired[SessionStatusType],  # (2)
    username: NotRequired[str],
```

1. See [:material-code-brackets: SessionSortByType](./literals.md#sessionsortbytype) 
2. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
## SessionSummaryTypeDef

```python
# SessionSummaryTypeDef definition

class SessionSummaryTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    portalArn: NotRequired[str],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
    status: NotRequired[SessionStatusType],  # (1)
    username: NotRequired[str],
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTrustStoreCertificatesRequestRequestTypeDef

```python
# ListTrustStoreCertificatesRequestRequestTypeDef definition

class ListTrustStoreCertificatesRequestRequestTypeDef(TypedDict):
    trustStoreArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTrustStoresRequestRequestTypeDef

```python
# ListTrustStoresRequestRequestTypeDef definition

class ListTrustStoresRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TrustStoreSummaryTypeDef

```python
# TrustStoreSummaryTypeDef definition

class TrustStoreSummaryTypeDef(TypedDict):
    trustStoreArn: NotRequired[str],
```

## ListUserAccessLoggingSettingsRequestRequestTypeDef

```python
# ListUserAccessLoggingSettingsRequestRequestTypeDef definition

class ListUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## UserAccessLoggingSettingsSummaryTypeDef

```python
# UserAccessLoggingSettingsSummaryTypeDef definition

class UserAccessLoggingSettingsSummaryTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    kinesisStreamArn: NotRequired[str],
```

## ListUserSettingsRequestRequestTypeDef

```python
# ListUserSettingsRequestRequestTypeDef definition

class ListUserSettingsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateBrowserSettingsRequestRequestTypeDef

```python
# UpdateBrowserSettingsRequestRequestTypeDef definition

class UpdateBrowserSettingsRequestRequestTypeDef(TypedDict):
    browserSettingsArn: str,
    browserPolicy: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateIdentityProviderRequestRequestTypeDef

```python
# UpdateIdentityProviderRequestRequestTypeDef definition

class UpdateIdentityProviderRequestRequestTypeDef(TypedDict):
    identityProviderArn: str,
    clientToken: NotRequired[str],
    identityProviderDetails: NotRequired[Mapping[str, str]],
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## UpdateNetworkSettingsRequestRequestTypeDef

```python
# UpdateNetworkSettingsRequestRequestTypeDef definition

class UpdateNetworkSettingsRequestRequestTypeDef(TypedDict):
    networkSettingsArn: str,
    clientToken: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
    vpcId: NotRequired[str],
```

## UpdatePortalRequestRequestTypeDef

```python
# UpdatePortalRequestRequestTypeDef definition

class UpdatePortalRequestRequestTypeDef(TypedDict):
    portalArn: str,
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    displayName: NotRequired[str],
    instanceType: NotRequired[InstanceTypeType],  # (2)
    maxConcurrentSessions: NotRequired[int],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## UpdateUserAccessLoggingSettingsRequestRequestTypeDef

```python
# UpdateUserAccessLoggingSettingsRequestRequestTypeDef definition

class UpdateUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    clientToken: NotRequired[str],
    kinesisStreamArn: NotRequired[str],
```

## AssociateBrowserSettingsResponseTypeDef

```python
# AssociateBrowserSettingsResponseTypeDef definition

class AssociateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIpAccessSettingsResponseTypeDef

```python
# AssociateIpAccessSettingsResponseTypeDef definition

class AssociateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateNetworkSettingsResponseTypeDef

```python
# AssociateNetworkSettingsResponseTypeDef definition

class AssociateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateTrustStoreResponseTypeDef

```python
# AssociateTrustStoreResponseTypeDef definition

class AssociateTrustStoreResponseTypeDef(TypedDict):
    portalArn: str,
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserAccessLoggingSettingsResponseTypeDef

```python
# AssociateUserAccessLoggingSettingsResponseTypeDef definition

class AssociateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    portalArn: str,
    userAccessLoggingSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserSettingsResponseTypeDef

```python
# AssociateUserSettingsResponseTypeDef definition

class AssociateUserSettingsResponseTypeDef(TypedDict):
    portalArn: str,
    userSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBrowserSettingsResponseTypeDef

```python
# CreateBrowserSettingsResponseTypeDef definition

class CreateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdentityProviderResponseTypeDef

```python
# CreateIdentityProviderResponseTypeDef definition

class CreateIdentityProviderResponseTypeDef(TypedDict):
    identityProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIpAccessSettingsResponseTypeDef

```python
# CreateIpAccessSettingsResponseTypeDef definition

class CreateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSettingsResponseTypeDef

```python
# CreateNetworkSettingsResponseTypeDef definition

class CreateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortalResponseTypeDef

```python
# CreatePortalResponseTypeDef definition

class CreatePortalResponseTypeDef(TypedDict):
    portalArn: str,
    portalEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrustStoreResponseTypeDef

```python
# CreateTrustStoreResponseTypeDef definition

class CreateTrustStoreResponseTypeDef(TypedDict):
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserAccessLoggingSettingsResponseTypeDef

```python
# CreateUserAccessLoggingSettingsResponseTypeDef definition

class CreateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserSettingsResponseTypeDef

```python
# CreateUserSettingsResponseTypeDef definition

class CreateUserSettingsResponseTypeDef(TypedDict):
    userSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPortalServiceProviderMetadataResponseTypeDef

```python
# GetPortalServiceProviderMetadataResponseTypeDef definition

class GetPortalServiceProviderMetadataResponseTypeDef(TypedDict):
    portalArn: str,
    serviceProviderSamlMetadata: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrustStoreResponseTypeDef

```python
# UpdateTrustStoreResponseTypeDef definition

class UpdateTrustStoreResponseTypeDef(TypedDict):
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrustStoreRequestRequestTypeDef

```python
# UpdateTrustStoreRequestRequestTypeDef definition

class UpdateTrustStoreRequestRequestTypeDef(TypedDict):
    trustStoreArn: str,
    certificatesToAdd: NotRequired[Sequence[BlobTypeDef]],
    certificatesToDelete: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

## ListBrowserSettingsResponseTypeDef

```python
# ListBrowserSettingsResponseTypeDef definition

class ListBrowserSettingsResponseTypeDef(TypedDict):
    browserSettings: List[BrowserSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BrowserSettingsSummaryTypeDef](./type_defs.md#browsersettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBrowserSettingsResponseTypeDef

```python
# GetBrowserSettingsResponseTypeDef definition

class GetBrowserSettingsResponseTypeDef(TypedDict):
    browserSettings: BrowserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSettingsTypeDef](./type_defs.md#browsersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrowserSettingsResponseTypeDef

```python
# UpdateBrowserSettingsResponseTypeDef definition

class UpdateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettings: BrowserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSettingsTypeDef](./type_defs.md#browsersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrustStoreCertificatesResponseTypeDef

```python
# ListTrustStoreCertificatesResponseTypeDef definition

class ListTrustStoreCertificatesResponseTypeDef(TypedDict):
    certificateList: List[CertificateSummaryTypeDef],  # (1)
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrustStoreCertificateResponseTypeDef

```python
# GetTrustStoreCertificateResponseTypeDef definition

class GetTrustStoreCertificateResponseTypeDef(TypedDict):
    certificate: CertificateTypeDef,  # (1)
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CookieSynchronizationConfigurationOutputTypeDef

```python
# CookieSynchronizationConfigurationOutputTypeDef definition

class CookieSynchronizationConfigurationOutputTypeDef(TypedDict):
    allowlist: List[CookieSpecificationTypeDef],  # (1)
    blocklist: NotRequired[List[CookieSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
2. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
## CookieSynchronizationConfigurationTypeDef

```python
# CookieSynchronizationConfigurationTypeDef definition

class CookieSynchronizationConfigurationTypeDef(TypedDict):
    allowlist: Sequence[CookieSpecificationTypeDef],  # (1)
    blocklist: NotRequired[Sequence[CookieSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
2. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
## CreateBrowserSettingsRequestRequestTypeDef

```python
# CreateBrowserSettingsRequestRequestTypeDef definition

class CreateBrowserSettingsRequestRequestTypeDef(TypedDict):
    browserPolicy: str,
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    customerManagedKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIdentityProviderRequestRequestTypeDef

```python
# CreateIdentityProviderRequestRequestTypeDef definition

class CreateIdentityProviderRequestRequestTypeDef(TypedDict):
    identityProviderDetails: Mapping[str, str],
    identityProviderName: str,
    identityProviderType: IdentityProviderTypeType,  # (1)
    portalArn: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNetworkSettingsRequestRequestTypeDef

```python
# CreateNetworkSettingsRequestRequestTypeDef definition

class CreateNetworkSettingsRequestRequestTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
    vpcId: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePortalRequestRequestTypeDef

```python
# CreatePortalRequestRequestTypeDef definition

class CreatePortalRequestRequestTypeDef(TypedDict):
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    clientToken: NotRequired[str],
    customerManagedKey: NotRequired[str],
    displayName: NotRequired[str],
    instanceType: NotRequired[InstanceTypeType],  # (2)
    maxConcurrentSessions: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTrustStoreRequestRequestTypeDef

```python
# CreateTrustStoreRequestRequestTypeDef definition

class CreateTrustStoreRequestRequestTypeDef(TypedDict):
    certificateList: Sequence[BlobTypeDef],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserAccessLoggingSettingsRequestRequestTypeDef

```python
# CreateUserAccessLoggingSettingsRequestRequestTypeDef definition

class CreateUserAccessLoggingSettingsRequestRequestTypeDef(TypedDict):
    kinesisStreamArn: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIpAccessSettingsRequestRequestTypeDef

```python
# CreateIpAccessSettingsRequestRequestTypeDef definition

class CreateIpAccessSettingsRequestRequestTypeDef(TypedDict):
    ipRules: Sequence[IpRuleTypeDef],  # (1)
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    customerManagedKey: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## IpAccessSettingsTypeDef

```python
# IpAccessSettingsTypeDef definition

class IpAccessSettingsTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    associatedPortalArns: NotRequired[List[str]],
    creationDate: NotRequired[datetime],
    customerManagedKey: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    ipRules: NotRequired[List[IpRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
## UpdateIpAccessSettingsRequestRequestTypeDef

```python
# UpdateIpAccessSettingsRequestRequestTypeDef definition

class UpdateIpAccessSettingsRequestRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    ipRules: NotRequired[Sequence[IpRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
## GetIdentityProviderResponseTypeDef

```python
# GetIdentityProviderResponseTypeDef definition

class GetIdentityProviderResponseTypeDef(TypedDict):
    identityProvider: IdentityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentityProviderResponseTypeDef

```python
# UpdateIdentityProviderResponseTypeDef definition

class UpdateIdentityProviderResponseTypeDef(TypedDict):
    identityProvider: IdentityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkSettingsResponseTypeDef

```python
# GetNetworkSettingsResponseTypeDef definition

class GetNetworkSettingsResponseTypeDef(TypedDict):
    networkSettings: NetworkSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSettingsTypeDef](./type_defs.md#networksettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNetworkSettingsResponseTypeDef

```python
# UpdateNetworkSettingsResponseTypeDef definition

class UpdateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettings: NetworkSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSettingsTypeDef](./type_defs.md#networksettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPortalResponseTypeDef

```python
# GetPortalResponseTypeDef definition

class GetPortalResponseTypeDef(TypedDict):
    portal: PortalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalTypeDef](./type_defs.md#portaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortalResponseTypeDef

```python
# UpdatePortalResponseTypeDef definition

class UpdatePortalResponseTypeDef(TypedDict):
    portal: PortalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalTypeDef](./type_defs.md#portaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrustStoreResponseTypeDef

```python
# GetTrustStoreResponseTypeDef definition

class GetTrustStoreResponseTypeDef(TypedDict):
    trustStore: TrustStoreTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreTypeDef](./type_defs.md#truststoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserAccessLoggingSettingsResponseTypeDef

```python
# GetUserAccessLoggingSettingsResponseTypeDef definition

class GetUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettings: UserAccessLoggingSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessLoggingSettingsTypeDef](./type_defs.md#useraccessloggingsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserAccessLoggingSettingsResponseTypeDef

```python
# UpdateUserAccessLoggingSettingsResponseTypeDef definition

class UpdateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettings: UserAccessLoggingSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessLoggingSettingsTypeDef](./type_defs.md#useraccessloggingsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityProvidersResponseTypeDef

```python
# ListIdentityProvidersResponseTypeDef definition

class ListIdentityProvidersResponseTypeDef(TypedDict):
    identityProviders: List[IdentityProviderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIpAccessSettingsResponseTypeDef

```python
# ListIpAccessSettingsResponseTypeDef definition

class ListIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: List[IpAccessSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IpAccessSettingsSummaryTypeDef](./type_defs.md#ipaccesssettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworkSettingsResponseTypeDef

```python
# ListNetworkSettingsResponseTypeDef definition

class ListNetworkSettingsResponseTypeDef(TypedDict):
    networkSettings: List[NetworkSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkSettingsSummaryTypeDef](./type_defs.md#networksettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPortalsResponseTypeDef

```python
# ListPortalsResponseTypeDef definition

class ListPortalsResponseTypeDef(TypedDict):
    portals: List[PortalSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PortalSummaryTypeDef](./type_defs.md#portalsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsRequestListSessionsPaginateTypeDef

```python
# ListSessionsRequestListSessionsPaginateTypeDef definition

class ListSessionsRequestListSessionsPaginateTypeDef(TypedDict):
    portalId: str,
    sessionId: NotRequired[str],
    sortBy: NotRequired[SessionSortByType],  # (1)
    status: NotRequired[SessionStatusType],  # (2)
    username: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SessionSortByType](./literals.md#sessionsortbytype) 
2. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef definition

class ListSessionsResponseTypeDef(TypedDict):
    sessions: List[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrustStoresResponseTypeDef

```python
# ListTrustStoresResponseTypeDef definition

class ListTrustStoresResponseTypeDef(TypedDict):
    trustStores: List[TrustStoreSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TrustStoreSummaryTypeDef](./type_defs.md#truststoresummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserAccessLoggingSettingsResponseTypeDef

```python
# ListUserAccessLoggingSettingsResponseTypeDef definition

class ListUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettings: List[UserAccessLoggingSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserAccessLoggingSettingsSummaryTypeDef](./type_defs.md#useraccessloggingsettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserSettingsSummaryTypeDef

```python
# UserSettingsSummaryTypeDef definition

class UserSettingsSummaryTypeDef(TypedDict):
    userSettingsArn: str,
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationOutputTypeDef],  # (1)
    copyAllowed: NotRequired[EnabledTypeType],  # (2)
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (2)
    disconnectTimeoutInMinutes: NotRequired[int],
    downloadAllowed: NotRequired[EnabledTypeType],  # (2)
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    pasteAllowed: NotRequired[EnabledTypeType],  # (2)
    printAllowed: NotRequired[EnabledTypeType],  # (2)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## UserSettingsTypeDef

```python
# UserSettingsTypeDef definition

class UserSettingsTypeDef(TypedDict):
    userSettingsArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    associatedPortalArns: NotRequired[List[str]],
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationOutputTypeDef],  # (1)
    copyAllowed: NotRequired[EnabledTypeType],  # (2)
    customerManagedKey: NotRequired[str],
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (2)
    disconnectTimeoutInMinutes: NotRequired[int],
    downloadAllowed: NotRequired[EnabledTypeType],  # (2)
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    pasteAllowed: NotRequired[EnabledTypeType],  # (2)
    printAllowed: NotRequired[EnabledTypeType],  # (2)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## CreateUserSettingsRequestRequestTypeDef

```python
# CreateUserSettingsRequestRequestTypeDef definition

class CreateUserSettingsRequestRequestTypeDef(TypedDict):
    copyAllowed: EnabledTypeType,  # (1)
    downloadAllowed: EnabledTypeType,  # (1)
    pasteAllowed: EnabledTypeType,  # (1)
    printAllowed: EnabledTypeType,  # (1)
    uploadAllowed: EnabledTypeType,  # (1)
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationTypeDef],  # (6)
    customerManagedKey: NotRequired[str],
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (1)
    disconnectTimeoutInMinutes: NotRequired[int],
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-braces: CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef) 
7. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateUserSettingsRequestRequestTypeDef

```python
# UpdateUserSettingsRequestRequestTypeDef definition

class UpdateUserSettingsRequestRequestTypeDef(TypedDict):
    userSettingsArn: str,
    clientToken: NotRequired[str],
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationTypeDef],  # (1)
    copyAllowed: NotRequired[EnabledTypeType],  # (2)
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (2)
    disconnectTimeoutInMinutes: NotRequired[int],
    downloadAllowed: NotRequired[EnabledTypeType],  # (2)
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    pasteAllowed: NotRequired[EnabledTypeType],  # (2)
    printAllowed: NotRequired[EnabledTypeType],  # (2)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## GetIpAccessSettingsResponseTypeDef

```python
# GetIpAccessSettingsResponseTypeDef definition

class GetIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: IpAccessSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IpAccessSettingsTypeDef](./type_defs.md#ipaccesssettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIpAccessSettingsResponseTypeDef

```python
# UpdateIpAccessSettingsResponseTypeDef definition

class UpdateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: IpAccessSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IpAccessSettingsTypeDef](./type_defs.md#ipaccesssettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserSettingsResponseTypeDef

```python
# ListUserSettingsResponseTypeDef definition

class ListUserSettingsResponseTypeDef(TypedDict):
    userSettings: List[UserSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserSettingsSummaryTypeDef](./type_defs.md#usersettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserSettingsResponseTypeDef

```python
# GetUserSettingsResponseTypeDef definition

class GetUserSettingsResponseTypeDef(TypedDict):
    userSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserSettingsResponseTypeDef

```python
# UpdateUserSettingsResponseTypeDef definition

class UpdateUserSettingsResponseTypeDef(TypedDict):
    userSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
