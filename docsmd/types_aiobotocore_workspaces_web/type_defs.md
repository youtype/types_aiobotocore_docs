# Type definitions

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#workspacesweb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_workspaces_web.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ToolbarConfigurationUnionTypeDef

```python
# ToolbarConfigurationUnionTypeDef Union usage example

from types_aiobotocore_workspaces_web.type_defs import ToolbarConfigurationUnionTypeDef


def get_value() -> ToolbarConfigurationUnionTypeDef:
    return ...


# ToolbarConfigurationUnionTypeDef definition

ToolbarConfigurationUnionTypeDef = Union[
    ToolbarConfigurationTypeDef,  # (1)
    ToolbarConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolbarConfigurationTypeDef](./type_defs.md#toolbarconfigurationtypedef) 
2. See [:material-code-braces: ToolbarConfigurationOutputTypeDef](./type_defs.md#toolbarconfigurationoutputtypedef) 

## CookieSynchronizationConfigurationUnionTypeDef

```python
# CookieSynchronizationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_workspaces_web.type_defs import CookieSynchronizationConfigurationUnionTypeDef


def get_value() -> CookieSynchronizationConfigurationUnionTypeDef:
    return ...


# CookieSynchronizationConfigurationUnionTypeDef definition

CookieSynchronizationConfigurationUnionTypeDef = Union[
    CookieSynchronizationConfigurationTypeDef,  # (1)
    CookieSynchronizationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef) 
2. See [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 

## InlineRedactionConfigurationUnionTypeDef

```python
# InlineRedactionConfigurationUnionTypeDef Union usage example

from types_aiobotocore_workspaces_web.type_defs import InlineRedactionConfigurationUnionTypeDef


def get_value() -> InlineRedactionConfigurationUnionTypeDef:
    return ...


# InlineRedactionConfigurationUnionTypeDef definition

InlineRedactionConfigurationUnionTypeDef = Union[
    InlineRedactionConfigurationTypeDef,  # (1)
    InlineRedactionConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InlineRedactionConfigurationTypeDef](./type_defs.md#inlineredactionconfigurationtypedef) 
2. See [:material-code-braces: InlineRedactionConfigurationOutputTypeDef](./type_defs.md#inlineredactionconfigurationoutputtypedef) 



## AssociateBrowserSettingsRequestTypeDef

```python
# AssociateBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestTypeDef


def get_value() -> AssociateBrowserSettingsRequestTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# AssociateBrowserSettingsRequestTypeDef definition

class AssociateBrowserSettingsRequestTypeDef(TypedDict):
    browserSettingsArn: str,
    portalArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## AssociateDataProtectionSettingsRequestTypeDef

```python
# AssociateDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateDataProtectionSettingsRequestTypeDef


def get_value() -> AssociateDataProtectionSettingsRequestTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# AssociateDataProtectionSettingsRequestTypeDef definition

class AssociateDataProtectionSettingsRequestTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    portalArn: str,
```

## AssociateIpAccessSettingsRequestTypeDef

```python
# AssociateIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateIpAccessSettingsRequestTypeDef


def get_value() -> AssociateIpAccessSettingsRequestTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# AssociateIpAccessSettingsRequestTypeDef definition

class AssociateIpAccessSettingsRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    portalArn: str,
```

## AssociateNetworkSettingsRequestTypeDef

```python
# AssociateNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateNetworkSettingsRequestTypeDef


def get_value() -> AssociateNetworkSettingsRequestTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# AssociateNetworkSettingsRequestTypeDef definition

class AssociateNetworkSettingsRequestTypeDef(TypedDict):
    networkSettingsArn: str,
    portalArn: str,
```

## AssociateTrustStoreRequestTypeDef

```python
# AssociateTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateTrustStoreRequestTypeDef


def get_value() -> AssociateTrustStoreRequestTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateTrustStoreRequestTypeDef definition

class AssociateTrustStoreRequestTypeDef(TypedDict):
    portalArn: str,
    trustStoreArn: str,
```

## AssociateUserAccessLoggingSettingsRequestTypeDef

```python
# AssociateUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateUserAccessLoggingSettingsRequestTypeDef


def get_value() -> AssociateUserAccessLoggingSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateUserAccessLoggingSettingsRequestTypeDef definition

class AssociateUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    portalArn: str,
    userAccessLoggingSettingsArn: str,
```

## AssociateUserSettingsRequestTypeDef

```python
# AssociateUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateUserSettingsRequestTypeDef


def get_value() -> AssociateUserSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateUserSettingsRequestTypeDef definition

class AssociateUserSettingsRequestTypeDef(TypedDict):
    portalArn: str,
    userSettingsArn: str,
```

## BrowserSettingsSummaryTypeDef

```python
# BrowserSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import BrowserSettingsSummaryTypeDef


def get_value() -> BrowserSettingsSummaryTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# BrowserSettingsSummaryTypeDef definition

class BrowserSettingsSummaryTypeDef(TypedDict):
    browserSettingsArn: str,
```

## BrowserSettingsTypeDef

```python
# BrowserSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import BrowserSettingsTypeDef


def get_value() -> BrowserSettingsTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


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
# CertificateSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CertificateSummaryTypeDef


def get_value() -> CertificateSummaryTypeDef:
    return {
        "issuer": ...,
    }


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
# CertificateTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CertificateTypeDef


def get_value() -> CertificateTypeDef:
    return {
        "body": ...,
    }


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
# CookieSpecificationTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CookieSpecificationTypeDef


def get_value() -> CookieSpecificationTypeDef:
    return {
        "domain": ...,
    }


# CookieSpecificationTypeDef definition

class CookieSpecificationTypeDef(TypedDict):
    domain: str,
    name: NotRequired[str],
    path: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## IpRuleTypeDef

```python
# IpRuleTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import IpRuleTypeDef


def get_value() -> IpRuleTypeDef:
    return {
        "description": ...,
    }


# IpRuleTypeDef definition

class IpRuleTypeDef(TypedDict):
    ipRange: str,
    description: NotRequired[str],
```

## CustomPatternTypeDef

```python
# CustomPatternTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CustomPatternTypeDef


def get_value() -> CustomPatternTypeDef:
    return {
        "keywordRegex": ...,
    }


# CustomPatternTypeDef definition

class CustomPatternTypeDef(TypedDict):
    patternName: str,
    patternRegex: str,
    keywordRegex: NotRequired[str],
    patternDescription: NotRequired[str],
```

## DataProtectionSettingsSummaryTypeDef

```python
# DataProtectionSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DataProtectionSettingsSummaryTypeDef


def get_value() -> DataProtectionSettingsSummaryTypeDef:
    return {
        "creationDate": ...,
    }


# DataProtectionSettingsSummaryTypeDef definition

class DataProtectionSettingsSummaryTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    creationDate: NotRequired[datetime],
    description: NotRequired[str],
    displayName: NotRequired[str],
```

## DeleteBrowserSettingsRequestTypeDef

```python
# DeleteBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteBrowserSettingsRequestTypeDef


def get_value() -> DeleteBrowserSettingsRequestTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# DeleteBrowserSettingsRequestTypeDef definition

class DeleteBrowserSettingsRequestTypeDef(TypedDict):
    browserSettingsArn: str,
```

## DeleteDataProtectionSettingsRequestTypeDef

```python
# DeleteDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteDataProtectionSettingsRequestTypeDef


def get_value() -> DeleteDataProtectionSettingsRequestTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# DeleteDataProtectionSettingsRequestTypeDef definition

class DeleteDataProtectionSettingsRequestTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
```

## DeleteIdentityProviderRequestTypeDef

```python
# DeleteIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteIdentityProviderRequestTypeDef


def get_value() -> DeleteIdentityProviderRequestTypeDef:
    return {
        "identityProviderArn": ...,
    }


# DeleteIdentityProviderRequestTypeDef definition

class DeleteIdentityProviderRequestTypeDef(TypedDict):
    identityProviderArn: str,
```

## DeleteIpAccessSettingsRequestTypeDef

```python
# DeleteIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteIpAccessSettingsRequestTypeDef


def get_value() -> DeleteIpAccessSettingsRequestTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# DeleteIpAccessSettingsRequestTypeDef definition

class DeleteIpAccessSettingsRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
```

## DeleteNetworkSettingsRequestTypeDef

```python
# DeleteNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteNetworkSettingsRequestTypeDef


def get_value() -> DeleteNetworkSettingsRequestTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# DeleteNetworkSettingsRequestTypeDef definition

class DeleteNetworkSettingsRequestTypeDef(TypedDict):
    networkSettingsArn: str,
```

## DeletePortalRequestTypeDef

```python
# DeletePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeletePortalRequestTypeDef


def get_value() -> DeletePortalRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DeletePortalRequestTypeDef definition

class DeletePortalRequestTypeDef(TypedDict):
    portalArn: str,
```

## DeleteTrustStoreRequestTypeDef

```python
# DeleteTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteTrustStoreRequestTypeDef


def get_value() -> DeleteTrustStoreRequestTypeDef:
    return {
        "trustStoreArn": ...,
    }


# DeleteTrustStoreRequestTypeDef definition

class DeleteTrustStoreRequestTypeDef(TypedDict):
    trustStoreArn: str,
```

## DeleteUserAccessLoggingSettingsRequestTypeDef

```python
# DeleteUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteUserAccessLoggingSettingsRequestTypeDef


def get_value() -> DeleteUserAccessLoggingSettingsRequestTypeDef:
    return {
        "userAccessLoggingSettingsArn": ...,
    }


# DeleteUserAccessLoggingSettingsRequestTypeDef definition

class DeleteUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
```

## DeleteUserSettingsRequestTypeDef

```python
# DeleteUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DeleteUserSettingsRequestTypeDef


def get_value() -> DeleteUserSettingsRequestTypeDef:
    return {
        "userSettingsArn": ...,
    }


# DeleteUserSettingsRequestTypeDef definition

class DeleteUserSettingsRequestTypeDef(TypedDict):
    userSettingsArn: str,
```

## DisassociateBrowserSettingsRequestTypeDef

```python
# DisassociateBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateBrowserSettingsRequestTypeDef


def get_value() -> DisassociateBrowserSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateBrowserSettingsRequestTypeDef definition

class DisassociateBrowserSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateDataProtectionSettingsRequestTypeDef

```python
# DisassociateDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateDataProtectionSettingsRequestTypeDef


def get_value() -> DisassociateDataProtectionSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateDataProtectionSettingsRequestTypeDef definition

class DisassociateDataProtectionSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateIpAccessSettingsRequestTypeDef

```python
# DisassociateIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateIpAccessSettingsRequestTypeDef


def get_value() -> DisassociateIpAccessSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateIpAccessSettingsRequestTypeDef definition

class DisassociateIpAccessSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateNetworkSettingsRequestTypeDef

```python
# DisassociateNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateNetworkSettingsRequestTypeDef


def get_value() -> DisassociateNetworkSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateNetworkSettingsRequestTypeDef definition

class DisassociateNetworkSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateTrustStoreRequestTypeDef

```python
# DisassociateTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateTrustStoreRequestTypeDef


def get_value() -> DisassociateTrustStoreRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateTrustStoreRequestTypeDef definition

class DisassociateTrustStoreRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateUserAccessLoggingSettingsRequestTypeDef

```python
# DisassociateUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateUserAccessLoggingSettingsRequestTypeDef


def get_value() -> DisassociateUserAccessLoggingSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateUserAccessLoggingSettingsRequestTypeDef definition

class DisassociateUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## DisassociateUserSettingsRequestTypeDef

```python
# DisassociateUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DisassociateUserSettingsRequestTypeDef


def get_value() -> DisassociateUserSettingsRequestTypeDef:
    return {
        "portalArn": ...,
    }


# DisassociateUserSettingsRequestTypeDef definition

class DisassociateUserSettingsRequestTypeDef(TypedDict):
    portalArn: str,
```

## ExpireSessionRequestTypeDef

```python
# ExpireSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ExpireSessionRequestTypeDef


def get_value() -> ExpireSessionRequestTypeDef:
    return {
        "portalId": ...,
    }


# ExpireSessionRequestTypeDef definition

class ExpireSessionRequestTypeDef(TypedDict):
    portalId: str,
    sessionId: str,
```

## GetBrowserSettingsRequestTypeDef

```python
# GetBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetBrowserSettingsRequestTypeDef


def get_value() -> GetBrowserSettingsRequestTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# GetBrowserSettingsRequestTypeDef definition

class GetBrowserSettingsRequestTypeDef(TypedDict):
    browserSettingsArn: str,
```

## GetDataProtectionSettingsRequestTypeDef

```python
# GetDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetDataProtectionSettingsRequestTypeDef


def get_value() -> GetDataProtectionSettingsRequestTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# GetDataProtectionSettingsRequestTypeDef definition

class GetDataProtectionSettingsRequestTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
```

## GetIdentityProviderRequestTypeDef

```python
# GetIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetIdentityProviderRequestTypeDef


def get_value() -> GetIdentityProviderRequestTypeDef:
    return {
        "identityProviderArn": ...,
    }


# GetIdentityProviderRequestTypeDef definition

class GetIdentityProviderRequestTypeDef(TypedDict):
    identityProviderArn: str,
```

## IdentityProviderTypeDef

```python
# IdentityProviderTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import IdentityProviderTypeDef


def get_value() -> IdentityProviderTypeDef:
    return {
        "identityProviderArn": ...,
    }


# IdentityProviderTypeDef definition

class IdentityProviderTypeDef(TypedDict):
    identityProviderArn: str,
    identityProviderDetails: NotRequired[Dict[str, str]],
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## GetIpAccessSettingsRequestTypeDef

```python
# GetIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetIpAccessSettingsRequestTypeDef


def get_value() -> GetIpAccessSettingsRequestTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# GetIpAccessSettingsRequestTypeDef definition

class GetIpAccessSettingsRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
```

## GetNetworkSettingsRequestTypeDef

```python
# GetNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetNetworkSettingsRequestTypeDef


def get_value() -> GetNetworkSettingsRequestTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# GetNetworkSettingsRequestTypeDef definition

class GetNetworkSettingsRequestTypeDef(TypedDict):
    networkSettingsArn: str,
```

## NetworkSettingsTypeDef

```python
# NetworkSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import NetworkSettingsTypeDef


def get_value() -> NetworkSettingsTypeDef:
    return {
        "associatedPortalArns": ...,
    }


# NetworkSettingsTypeDef definition

class NetworkSettingsTypeDef(TypedDict):
    networkSettingsArn: str,
    associatedPortalArns: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
    subnetIds: NotRequired[List[str]],
    vpcId: NotRequired[str],
```

## GetPortalRequestTypeDef

```python
# GetPortalRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetPortalRequestTypeDef


def get_value() -> GetPortalRequestTypeDef:
    return {
        "portalArn": ...,
    }


# GetPortalRequestTypeDef definition

class GetPortalRequestTypeDef(TypedDict):
    portalArn: str,
```

## PortalTypeDef

```python
# PortalTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import PortalTypeDef


def get_value() -> PortalTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


# PortalTypeDef definition

class PortalTypeDef(TypedDict):
    portalArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    browserSettingsArn: NotRequired[str],
    browserType: NotRequired[BrowserTypeType],  # (2)
    creationDate: NotRequired[datetime],
    customerManagedKey: NotRequired[str],
    dataProtectionSettingsArn: NotRequired[str],
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
## GetPortalServiceProviderMetadataRequestTypeDef

```python
# GetPortalServiceProviderMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetPortalServiceProviderMetadataRequestTypeDef


def get_value() -> GetPortalServiceProviderMetadataRequestTypeDef:
    return {
        "portalArn": ...,
    }


# GetPortalServiceProviderMetadataRequestTypeDef definition

class GetPortalServiceProviderMetadataRequestTypeDef(TypedDict):
    portalArn: str,
```

## GetSessionRequestTypeDef

```python
# GetSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetSessionRequestTypeDef


def get_value() -> GetSessionRequestTypeDef:
    return {
        "portalId": ...,
    }


# GetSessionRequestTypeDef definition

class GetSessionRequestTypeDef(TypedDict):
    portalId: str,
    sessionId: str,
```

## SessionTypeDef

```python
# SessionTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import SessionTypeDef


def get_value() -> SessionTypeDef:
    return {
        "clientIpAddresses": ...,
    }


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
## GetTrustStoreCertificateRequestTypeDef

```python
# GetTrustStoreCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetTrustStoreCertificateRequestTypeDef


def get_value() -> GetTrustStoreCertificateRequestTypeDef:
    return {
        "thumbprint": ...,
    }


# GetTrustStoreCertificateRequestTypeDef definition

class GetTrustStoreCertificateRequestTypeDef(TypedDict):
    thumbprint: str,
    trustStoreArn: str,
```

## GetTrustStoreRequestTypeDef

```python
# GetTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetTrustStoreRequestTypeDef


def get_value() -> GetTrustStoreRequestTypeDef:
    return {
        "trustStoreArn": ...,
    }


# GetTrustStoreRequestTypeDef definition

class GetTrustStoreRequestTypeDef(TypedDict):
    trustStoreArn: str,
```

## TrustStoreTypeDef

```python
# TrustStoreTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import TrustStoreTypeDef


def get_value() -> TrustStoreTypeDef:
    return {
        "associatedPortalArns": ...,
    }


# TrustStoreTypeDef definition

class TrustStoreTypeDef(TypedDict):
    trustStoreArn: str,
    associatedPortalArns: NotRequired[List[str]],
```

## GetUserAccessLoggingSettingsRequestTypeDef

```python
# GetUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetUserAccessLoggingSettingsRequestTypeDef


def get_value() -> GetUserAccessLoggingSettingsRequestTypeDef:
    return {
        "userAccessLoggingSettingsArn": ...,
    }


# GetUserAccessLoggingSettingsRequestTypeDef definition

class GetUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
```

## UserAccessLoggingSettingsTypeDef

```python
# UserAccessLoggingSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UserAccessLoggingSettingsTypeDef


def get_value() -> UserAccessLoggingSettingsTypeDef:
    return {
        "associatedPortalArns": ...,
    }


# UserAccessLoggingSettingsTypeDef definition

class UserAccessLoggingSettingsTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    associatedPortalArns: NotRequired[List[str]],
    kinesisStreamArn: NotRequired[str],
```

## GetUserSettingsRequestTypeDef

```python
# GetUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetUserSettingsRequestTypeDef


def get_value() -> GetUserSettingsRequestTypeDef:
    return {
        "userSettingsArn": ...,
    }


# GetUserSettingsRequestTypeDef definition

class GetUserSettingsRequestTypeDef(TypedDict):
    userSettingsArn: str,
```

## IdentityProviderSummaryTypeDef

```python
# IdentityProviderSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import IdentityProviderSummaryTypeDef


def get_value() -> IdentityProviderSummaryTypeDef:
    return {
        "identityProviderArn": ...,
    }


# IdentityProviderSummaryTypeDef definition

class IdentityProviderSummaryTypeDef(TypedDict):
    identityProviderArn: str,
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## RedactionPlaceHolderTypeDef

```python
# RedactionPlaceHolderTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import RedactionPlaceHolderTypeDef


def get_value() -> RedactionPlaceHolderTypeDef:
    return {
        "redactionPlaceHolderText": ...,
    }


# RedactionPlaceHolderTypeDef definition

class RedactionPlaceHolderTypeDef(TypedDict):
    redactionPlaceHolderType: RedactionPlaceHolderTypeType,  # (1)
    redactionPlaceHolderText: NotRequired[str],
```

1. See [:material-code-brackets: RedactionPlaceHolderTypeType](./literals.md#redactionplaceholdertypetype) 
## IpAccessSettingsSummaryTypeDef

```python
# IpAccessSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import IpAccessSettingsSummaryTypeDef


def get_value() -> IpAccessSettingsSummaryTypeDef:
    return {
        "creationDate": ...,
    }


# IpAccessSettingsSummaryTypeDef definition

class IpAccessSettingsSummaryTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    creationDate: NotRequired[datetime],
    description: NotRequired[str],
    displayName: NotRequired[str],
```

## ListBrowserSettingsRequestTypeDef

```python
# ListBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListBrowserSettingsRequestTypeDef


def get_value() -> ListBrowserSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListBrowserSettingsRequestTypeDef definition

class ListBrowserSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDataProtectionSettingsRequestTypeDef

```python
# ListDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListDataProtectionSettingsRequestTypeDef


def get_value() -> ListDataProtectionSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListDataProtectionSettingsRequestTypeDef definition

class ListDataProtectionSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdentityProvidersRequestTypeDef

```python
# ListIdentityProvidersRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListIdentityProvidersRequestTypeDef


def get_value() -> ListIdentityProvidersRequestTypeDef:
    return {
        "portalArn": ...,
    }


# ListIdentityProvidersRequestTypeDef definition

class ListIdentityProvidersRequestTypeDef(TypedDict):
    portalArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIpAccessSettingsRequestTypeDef

```python
# ListIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListIpAccessSettingsRequestTypeDef


def get_value() -> ListIpAccessSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListIpAccessSettingsRequestTypeDef definition

class ListIpAccessSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListNetworkSettingsRequestTypeDef

```python
# ListNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListNetworkSettingsRequestTypeDef


def get_value() -> ListNetworkSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListNetworkSettingsRequestTypeDef definition

class ListNetworkSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NetworkSettingsSummaryTypeDef

```python
# NetworkSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import NetworkSettingsSummaryTypeDef


def get_value() -> NetworkSettingsSummaryTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# NetworkSettingsSummaryTypeDef definition

class NetworkSettingsSummaryTypeDef(TypedDict):
    networkSettingsArn: str,
    vpcId: NotRequired[str],
```

## ListPortalsRequestTypeDef

```python
# ListPortalsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListPortalsRequestTypeDef


def get_value() -> ListPortalsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListPortalsRequestTypeDef definition

class ListPortalsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PortalSummaryTypeDef

```python
# PortalSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import PortalSummaryTypeDef


def get_value() -> PortalSummaryTypeDef:
    return {
        "authenticationType": ...,
    }


# PortalSummaryTypeDef definition

class PortalSummaryTypeDef(TypedDict):
    portalArn: str,
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    browserSettingsArn: NotRequired[str],
    browserType: NotRequired[BrowserTypeType],  # (2)
    creationDate: NotRequired[datetime],
    dataProtectionSettingsArn: NotRequired[str],
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
## ListSessionsRequestTypeDef

```python
# ListSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListSessionsRequestTypeDef


def get_value() -> ListSessionsRequestTypeDef:
    return {
        "portalId": ...,
    }


# ListSessionsRequestTypeDef definition

class ListSessionsRequestTypeDef(TypedDict):
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
# SessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import SessionSummaryTypeDef


def get_value() -> SessionSummaryTypeDef:
    return {
        "endTime": ...,
    }


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
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTrustStoreCertificatesRequestTypeDef

```python
# ListTrustStoreCertificatesRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTrustStoreCertificatesRequestTypeDef


def get_value() -> ListTrustStoreCertificatesRequestTypeDef:
    return {
        "trustStoreArn": ...,
    }


# ListTrustStoreCertificatesRequestTypeDef definition

class ListTrustStoreCertificatesRequestTypeDef(TypedDict):
    trustStoreArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTrustStoresRequestTypeDef

```python
# ListTrustStoresRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTrustStoresRequestTypeDef


def get_value() -> ListTrustStoresRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListTrustStoresRequestTypeDef definition

class ListTrustStoresRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TrustStoreSummaryTypeDef

```python
# TrustStoreSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import TrustStoreSummaryTypeDef


def get_value() -> TrustStoreSummaryTypeDef:
    return {
        "trustStoreArn": ...,
    }


# TrustStoreSummaryTypeDef definition

class TrustStoreSummaryTypeDef(TypedDict):
    trustStoreArn: NotRequired[str],
```

## ListUserAccessLoggingSettingsRequestTypeDef

```python
# ListUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListUserAccessLoggingSettingsRequestTypeDef


def get_value() -> ListUserAccessLoggingSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListUserAccessLoggingSettingsRequestTypeDef definition

class ListUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## UserAccessLoggingSettingsSummaryTypeDef

```python
# UserAccessLoggingSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UserAccessLoggingSettingsSummaryTypeDef


def get_value() -> UserAccessLoggingSettingsSummaryTypeDef:
    return {
        "kinesisStreamArn": ...,
    }


# UserAccessLoggingSettingsSummaryTypeDef definition

class UserAccessLoggingSettingsSummaryTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    kinesisStreamArn: NotRequired[str],
```

## ListUserSettingsRequestTypeDef

```python
# ListUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListUserSettingsRequestTypeDef


def get_value() -> ListUserSettingsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListUserSettingsRequestTypeDef definition

class ListUserSettingsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ToolbarConfigurationOutputTypeDef

```python
# ToolbarConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ToolbarConfigurationOutputTypeDef


def get_value() -> ToolbarConfigurationOutputTypeDef:
    return {
        "hiddenToolbarItems": ...,
    }


# ToolbarConfigurationOutputTypeDef definition

class ToolbarConfigurationOutputTypeDef(TypedDict):
    hiddenToolbarItems: NotRequired[List[ToolbarItemType]],  # (1)
    maxDisplayResolution: NotRequired[MaxDisplayResolutionType],  # (2)
    toolbarType: NotRequired[ToolbarTypeType],  # (3)
    visualMode: NotRequired[VisualModeType],  # (4)
```

1. See [:material-code-brackets: ToolbarItemType](./literals.md#toolbaritemtype) 
2. See [:material-code-brackets: MaxDisplayResolutionType](./literals.md#maxdisplayresolutiontype) 
3. See [:material-code-brackets: ToolbarTypeType](./literals.md#toolbartypetype) 
4. See [:material-code-brackets: VisualModeType](./literals.md#visualmodetype) 
## ToolbarConfigurationTypeDef

```python
# ToolbarConfigurationTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ToolbarConfigurationTypeDef


def get_value() -> ToolbarConfigurationTypeDef:
    return {
        "hiddenToolbarItems": ...,
    }


# ToolbarConfigurationTypeDef definition

class ToolbarConfigurationTypeDef(TypedDict):
    hiddenToolbarItems: NotRequired[Sequence[ToolbarItemType]],  # (1)
    maxDisplayResolution: NotRequired[MaxDisplayResolutionType],  # (2)
    toolbarType: NotRequired[ToolbarTypeType],  # (3)
    visualMode: NotRequired[VisualModeType],  # (4)
```

1. See [:material-code-brackets: ToolbarItemType](./literals.md#toolbaritemtype) 
2. See [:material-code-brackets: MaxDisplayResolutionType](./literals.md#maxdisplayresolutiontype) 
3. See [:material-code-brackets: ToolbarTypeType](./literals.md#toolbartypetype) 
4. See [:material-code-brackets: VisualModeType](./literals.md#visualmodetype) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateBrowserSettingsRequestTypeDef

```python
# UpdateBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateBrowserSettingsRequestTypeDef


def get_value() -> UpdateBrowserSettingsRequestTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# UpdateBrowserSettingsRequestTypeDef definition

class UpdateBrowserSettingsRequestTypeDef(TypedDict):
    browserSettingsArn: str,
    browserPolicy: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateIdentityProviderRequestTypeDef

```python
# UpdateIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateIdentityProviderRequestTypeDef


def get_value() -> UpdateIdentityProviderRequestTypeDef:
    return {
        "identityProviderArn": ...,
    }


# UpdateIdentityProviderRequestTypeDef definition

class UpdateIdentityProviderRequestTypeDef(TypedDict):
    identityProviderArn: str,
    clientToken: NotRequired[str],
    identityProviderDetails: NotRequired[Mapping[str, str]],
    identityProviderName: NotRequired[str],
    identityProviderType: NotRequired[IdentityProviderTypeType],  # (1)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## UpdateNetworkSettingsRequestTypeDef

```python
# UpdateNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateNetworkSettingsRequestTypeDef


def get_value() -> UpdateNetworkSettingsRequestTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# UpdateNetworkSettingsRequestTypeDef definition

class UpdateNetworkSettingsRequestTypeDef(TypedDict):
    networkSettingsArn: str,
    clientToken: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
    vpcId: NotRequired[str],
```

## UpdatePortalRequestTypeDef

```python
# UpdatePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdatePortalRequestTypeDef


def get_value() -> UpdatePortalRequestTypeDef:
    return {
        "portalArn": ...,
    }


# UpdatePortalRequestTypeDef definition

class UpdatePortalRequestTypeDef(TypedDict):
    portalArn: str,
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    displayName: NotRequired[str],
    instanceType: NotRequired[InstanceTypeType],  # (2)
    maxConcurrentSessions: NotRequired[int],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## UpdateUserAccessLoggingSettingsRequestTypeDef

```python
# UpdateUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateUserAccessLoggingSettingsRequestTypeDef


def get_value() -> UpdateUserAccessLoggingSettingsRequestTypeDef:
    return {
        "userAccessLoggingSettingsArn": ...,
    }


# UpdateUserAccessLoggingSettingsRequestTypeDef definition

class UpdateUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    clientToken: NotRequired[str],
    kinesisStreamArn: NotRequired[str],
```

## AssociateBrowserSettingsResponseTypeDef

```python
# AssociateBrowserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsResponseTypeDef


def get_value() -> AssociateBrowserSettingsResponseTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# AssociateBrowserSettingsResponseTypeDef definition

class AssociateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateDataProtectionSettingsResponseTypeDef

```python
# AssociateDataProtectionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateDataProtectionSettingsResponseTypeDef


def get_value() -> AssociateDataProtectionSettingsResponseTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# AssociateDataProtectionSettingsResponseTypeDef definition

class AssociateDataProtectionSettingsResponseTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIpAccessSettingsResponseTypeDef

```python
# AssociateIpAccessSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateIpAccessSettingsResponseTypeDef


def get_value() -> AssociateIpAccessSettingsResponseTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# AssociateIpAccessSettingsResponseTypeDef definition

class AssociateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateNetworkSettingsResponseTypeDef

```python
# AssociateNetworkSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateNetworkSettingsResponseTypeDef


def get_value() -> AssociateNetworkSettingsResponseTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# AssociateNetworkSettingsResponseTypeDef definition

class AssociateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettingsArn: str,
    portalArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateTrustStoreResponseTypeDef

```python
# AssociateTrustStoreResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateTrustStoreResponseTypeDef


def get_value() -> AssociateTrustStoreResponseTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateTrustStoreResponseTypeDef definition

class AssociateTrustStoreResponseTypeDef(TypedDict):
    portalArn: str,
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserAccessLoggingSettingsResponseTypeDef

```python
# AssociateUserAccessLoggingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateUserAccessLoggingSettingsResponseTypeDef


def get_value() -> AssociateUserAccessLoggingSettingsResponseTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateUserAccessLoggingSettingsResponseTypeDef definition

class AssociateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    portalArn: str,
    userAccessLoggingSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserSettingsResponseTypeDef

```python
# AssociateUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import AssociateUserSettingsResponseTypeDef


def get_value() -> AssociateUserSettingsResponseTypeDef:
    return {
        "portalArn": ...,
    }


# AssociateUserSettingsResponseTypeDef definition

class AssociateUserSettingsResponseTypeDef(TypedDict):
    portalArn: str,
    userSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBrowserSettingsResponseTypeDef

```python
# CreateBrowserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateBrowserSettingsResponseTypeDef


def get_value() -> CreateBrowserSettingsResponseTypeDef:
    return {
        "browserSettingsArn": ...,
    }


# CreateBrowserSettingsResponseTypeDef definition

class CreateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataProtectionSettingsResponseTypeDef

```python
# CreateDataProtectionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateDataProtectionSettingsResponseTypeDef


def get_value() -> CreateDataProtectionSettingsResponseTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# CreateDataProtectionSettingsResponseTypeDef definition

class CreateDataProtectionSettingsResponseTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdentityProviderResponseTypeDef

```python
# CreateIdentityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateIdentityProviderResponseTypeDef


def get_value() -> CreateIdentityProviderResponseTypeDef:
    return {
        "identityProviderArn": ...,
    }


# CreateIdentityProviderResponseTypeDef definition

class CreateIdentityProviderResponseTypeDef(TypedDict):
    identityProviderArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIpAccessSettingsResponseTypeDef

```python
# CreateIpAccessSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateIpAccessSettingsResponseTypeDef


def get_value() -> CreateIpAccessSettingsResponseTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# CreateIpAccessSettingsResponseTypeDef definition

class CreateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkSettingsResponseTypeDef

```python
# CreateNetworkSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateNetworkSettingsResponseTypeDef


def get_value() -> CreateNetworkSettingsResponseTypeDef:
    return {
        "networkSettingsArn": ...,
    }


# CreateNetworkSettingsResponseTypeDef definition

class CreateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortalResponseTypeDef

```python
# CreatePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreatePortalResponseTypeDef


def get_value() -> CreatePortalResponseTypeDef:
    return {
        "portalArn": ...,
    }


# CreatePortalResponseTypeDef definition

class CreatePortalResponseTypeDef(TypedDict):
    portalArn: str,
    portalEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrustStoreResponseTypeDef

```python
# CreateTrustStoreResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateTrustStoreResponseTypeDef


def get_value() -> CreateTrustStoreResponseTypeDef:
    return {
        "trustStoreArn": ...,
    }


# CreateTrustStoreResponseTypeDef definition

class CreateTrustStoreResponseTypeDef(TypedDict):
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserAccessLoggingSettingsResponseTypeDef

```python
# CreateUserAccessLoggingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateUserAccessLoggingSettingsResponseTypeDef


def get_value() -> CreateUserAccessLoggingSettingsResponseTypeDef:
    return {
        "userAccessLoggingSettingsArn": ...,
    }


# CreateUserAccessLoggingSettingsResponseTypeDef definition

class CreateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserSettingsResponseTypeDef

```python
# CreateUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateUserSettingsResponseTypeDef


def get_value() -> CreateUserSettingsResponseTypeDef:
    return {
        "userSettingsArn": ...,
    }


# CreateUserSettingsResponseTypeDef definition

class CreateUserSettingsResponseTypeDef(TypedDict):
    userSettingsArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPortalServiceProviderMetadataResponseTypeDef

```python
# GetPortalServiceProviderMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetPortalServiceProviderMetadataResponseTypeDef


def get_value() -> GetPortalServiceProviderMetadataResponseTypeDef:
    return {
        "portalArn": ...,
    }


# GetPortalServiceProviderMetadataResponseTypeDef definition

class GetPortalServiceProviderMetadataResponseTypeDef(TypedDict):
    portalArn: str,
    serviceProviderSamlMetadata: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrustStoreResponseTypeDef

```python
# UpdateTrustStoreResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateTrustStoreResponseTypeDef


def get_value() -> UpdateTrustStoreResponseTypeDef:
    return {
        "trustStoreArn": ...,
    }


# UpdateTrustStoreResponseTypeDef definition

class UpdateTrustStoreResponseTypeDef(TypedDict):
    trustStoreArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrustStoreRequestTypeDef

```python
# UpdateTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateTrustStoreRequestTypeDef


def get_value() -> UpdateTrustStoreRequestTypeDef:
    return {
        "trustStoreArn": ...,
    }


# UpdateTrustStoreRequestTypeDef definition

class UpdateTrustStoreRequestTypeDef(TypedDict):
    trustStoreArn: str,
    certificatesToAdd: NotRequired[Sequence[BlobTypeDef]],
    certificatesToDelete: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

## ListBrowserSettingsResponseTypeDef

```python
# ListBrowserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListBrowserSettingsResponseTypeDef


def get_value() -> ListBrowserSettingsResponseTypeDef:
    return {
        "browserSettings": ...,
    }


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
# GetBrowserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetBrowserSettingsResponseTypeDef


def get_value() -> GetBrowserSettingsResponseTypeDef:
    return {
        "browserSettings": ...,
    }


# GetBrowserSettingsResponseTypeDef definition

class GetBrowserSettingsResponseTypeDef(TypedDict):
    browserSettings: BrowserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSettingsTypeDef](./type_defs.md#browsersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrowserSettingsResponseTypeDef

```python
# UpdateBrowserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateBrowserSettingsResponseTypeDef


def get_value() -> UpdateBrowserSettingsResponseTypeDef:
    return {
        "browserSettings": ...,
    }


# UpdateBrowserSettingsResponseTypeDef definition

class UpdateBrowserSettingsResponseTypeDef(TypedDict):
    browserSettings: BrowserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrowserSettingsTypeDef](./type_defs.md#browsersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrustStoreCertificatesResponseTypeDef

```python
# ListTrustStoreCertificatesResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTrustStoreCertificatesResponseTypeDef


def get_value() -> ListTrustStoreCertificatesResponseTypeDef:
    return {
        "certificateList": ...,
    }


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
# GetTrustStoreCertificateResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetTrustStoreCertificateResponseTypeDef


def get_value() -> GetTrustStoreCertificateResponseTypeDef:
    return {
        "certificate": ...,
    }


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
# CookieSynchronizationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CookieSynchronizationConfigurationOutputTypeDef


def get_value() -> CookieSynchronizationConfigurationOutputTypeDef:
    return {
        "allowlist": ...,
    }


# CookieSynchronizationConfigurationOutputTypeDef definition

class CookieSynchronizationConfigurationOutputTypeDef(TypedDict):
    allowlist: List[CookieSpecificationTypeDef],  # (1)
    blocklist: NotRequired[List[CookieSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
2. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
## CookieSynchronizationConfigurationTypeDef

```python
# CookieSynchronizationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CookieSynchronizationConfigurationTypeDef


def get_value() -> CookieSynchronizationConfigurationTypeDef:
    return {
        "allowlist": ...,
    }


# CookieSynchronizationConfigurationTypeDef definition

class CookieSynchronizationConfigurationTypeDef(TypedDict):
    allowlist: Sequence[CookieSpecificationTypeDef],  # (1)
    blocklist: NotRequired[Sequence[CookieSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
2. See [:material-code-braces: CookieSpecificationTypeDef](./type_defs.md#cookiespecificationtypedef) 
## CreateBrowserSettingsRequestTypeDef

```python
# CreateBrowserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateBrowserSettingsRequestTypeDef


def get_value() -> CreateBrowserSettingsRequestTypeDef:
    return {
        "browserPolicy": ...,
    }


# CreateBrowserSettingsRequestTypeDef definition

class CreateBrowserSettingsRequestTypeDef(TypedDict):
    browserPolicy: str,
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    customerManagedKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIdentityProviderRequestTypeDef

```python
# CreateIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateIdentityProviderRequestTypeDef


def get_value() -> CreateIdentityProviderRequestTypeDef:
    return {
        "identityProviderDetails": ...,
    }


# CreateIdentityProviderRequestTypeDef definition

class CreateIdentityProviderRequestTypeDef(TypedDict):
    identityProviderDetails: Mapping[str, str],
    identityProviderName: str,
    identityProviderType: IdentityProviderTypeType,  # (1)
    portalArn: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNetworkSettingsRequestTypeDef

```python
# CreateNetworkSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateNetworkSettingsRequestTypeDef


def get_value() -> CreateNetworkSettingsRequestTypeDef:
    return {
        "securityGroupIds": ...,
    }


# CreateNetworkSettingsRequestTypeDef definition

class CreateNetworkSettingsRequestTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
    vpcId: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePortalRequestTypeDef

```python
# CreatePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreatePortalRequestTypeDef


def get_value() -> CreatePortalRequestTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


# CreatePortalRequestTypeDef definition

class CreatePortalRequestTypeDef(TypedDict):
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
## CreateTrustStoreRequestTypeDef

```python
# CreateTrustStoreRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateTrustStoreRequestTypeDef


def get_value() -> CreateTrustStoreRequestTypeDef:
    return {
        "certificateList": ...,
    }


# CreateTrustStoreRequestTypeDef definition

class CreateTrustStoreRequestTypeDef(TypedDict):
    certificateList: Sequence[BlobTypeDef],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserAccessLoggingSettingsRequestTypeDef

```python
# CreateUserAccessLoggingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateUserAccessLoggingSettingsRequestTypeDef


def get_value() -> CreateUserAccessLoggingSettingsRequestTypeDef:
    return {
        "kinesisStreamArn": ...,
    }


# CreateUserAccessLoggingSettingsRequestTypeDef definition

class CreateUserAccessLoggingSettingsRequestTypeDef(TypedDict):
    kinesisStreamArn: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIpAccessSettingsRequestTypeDef

```python
# CreateIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateIpAccessSettingsRequestTypeDef


def get_value() -> CreateIpAccessSettingsRequestTypeDef:
    return {
        "ipRules": ...,
    }


# CreateIpAccessSettingsRequestTypeDef definition

class CreateIpAccessSettingsRequestTypeDef(TypedDict):
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
# IpAccessSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import IpAccessSettingsTypeDef


def get_value() -> IpAccessSettingsTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


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
## UpdateIpAccessSettingsRequestTypeDef

```python
# UpdateIpAccessSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateIpAccessSettingsRequestTypeDef


def get_value() -> UpdateIpAccessSettingsRequestTypeDef:
    return {
        "ipAccessSettingsArn": ...,
    }


# UpdateIpAccessSettingsRequestTypeDef definition

class UpdateIpAccessSettingsRequestTypeDef(TypedDict):
    ipAccessSettingsArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    ipRules: NotRequired[Sequence[IpRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: IpRuleTypeDef](./type_defs.md#ipruletypedef) 
## ListDataProtectionSettingsResponseTypeDef

```python
# ListDataProtectionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListDataProtectionSettingsResponseTypeDef


def get_value() -> ListDataProtectionSettingsResponseTypeDef:
    return {
        "dataProtectionSettings": ...,
    }


# ListDataProtectionSettingsResponseTypeDef definition

class ListDataProtectionSettingsResponseTypeDef(TypedDict):
    dataProtectionSettings: List[DataProtectionSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataProtectionSettingsSummaryTypeDef](./type_defs.md#dataprotectionsettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdentityProviderResponseTypeDef

```python
# GetIdentityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetIdentityProviderResponseTypeDef


def get_value() -> GetIdentityProviderResponseTypeDef:
    return {
        "identityProvider": ...,
    }


# GetIdentityProviderResponseTypeDef definition

class GetIdentityProviderResponseTypeDef(TypedDict):
    identityProvider: IdentityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentityProviderResponseTypeDef

```python
# UpdateIdentityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateIdentityProviderResponseTypeDef


def get_value() -> UpdateIdentityProviderResponseTypeDef:
    return {
        "identityProvider": ...,
    }


# UpdateIdentityProviderResponseTypeDef definition

class UpdateIdentityProviderResponseTypeDef(TypedDict):
    identityProvider: IdentityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNetworkSettingsResponseTypeDef

```python
# GetNetworkSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetNetworkSettingsResponseTypeDef


def get_value() -> GetNetworkSettingsResponseTypeDef:
    return {
        "networkSettings": ...,
    }


# GetNetworkSettingsResponseTypeDef definition

class GetNetworkSettingsResponseTypeDef(TypedDict):
    networkSettings: NetworkSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSettingsTypeDef](./type_defs.md#networksettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNetworkSettingsResponseTypeDef

```python
# UpdateNetworkSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateNetworkSettingsResponseTypeDef


def get_value() -> UpdateNetworkSettingsResponseTypeDef:
    return {
        "networkSettings": ...,
    }


# UpdateNetworkSettingsResponseTypeDef definition

class UpdateNetworkSettingsResponseTypeDef(TypedDict):
    networkSettings: NetworkSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NetworkSettingsTypeDef](./type_defs.md#networksettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPortalResponseTypeDef

```python
# GetPortalResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetPortalResponseTypeDef


def get_value() -> GetPortalResponseTypeDef:
    return {
        "portal": ...,
    }


# GetPortalResponseTypeDef definition

class GetPortalResponseTypeDef(TypedDict):
    portal: PortalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalTypeDef](./type_defs.md#portaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortalResponseTypeDef

```python
# UpdatePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdatePortalResponseTypeDef


def get_value() -> UpdatePortalResponseTypeDef:
    return {
        "portal": ...,
    }


# UpdatePortalResponseTypeDef definition

class UpdatePortalResponseTypeDef(TypedDict):
    portal: PortalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalTypeDef](./type_defs.md#portaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetSessionResponseTypeDef


def get_value() -> GetSessionResponseTypeDef:
    return {
        "session": ...,
    }


# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrustStoreResponseTypeDef

```python
# GetTrustStoreResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetTrustStoreResponseTypeDef


def get_value() -> GetTrustStoreResponseTypeDef:
    return {
        "trustStore": ...,
    }


# GetTrustStoreResponseTypeDef definition

class GetTrustStoreResponseTypeDef(TypedDict):
    trustStore: TrustStoreTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustStoreTypeDef](./type_defs.md#truststoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserAccessLoggingSettingsResponseTypeDef

```python
# GetUserAccessLoggingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetUserAccessLoggingSettingsResponseTypeDef


def get_value() -> GetUserAccessLoggingSettingsResponseTypeDef:
    return {
        "userAccessLoggingSettings": ...,
    }


# GetUserAccessLoggingSettingsResponseTypeDef definition

class GetUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettings: UserAccessLoggingSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessLoggingSettingsTypeDef](./type_defs.md#useraccessloggingsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserAccessLoggingSettingsResponseTypeDef

```python
# UpdateUserAccessLoggingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateUserAccessLoggingSettingsResponseTypeDef


def get_value() -> UpdateUserAccessLoggingSettingsResponseTypeDef:
    return {
        "userAccessLoggingSettings": ...,
    }


# UpdateUserAccessLoggingSettingsResponseTypeDef definition

class UpdateUserAccessLoggingSettingsResponseTypeDef(TypedDict):
    userAccessLoggingSettings: UserAccessLoggingSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessLoggingSettingsTypeDef](./type_defs.md#useraccessloggingsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityProvidersResponseTypeDef

```python
# ListIdentityProvidersResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListIdentityProvidersResponseTypeDef


def get_value() -> ListIdentityProvidersResponseTypeDef:
    return {
        "identityProviders": ...,
    }


# ListIdentityProvidersResponseTypeDef definition

class ListIdentityProvidersResponseTypeDef(TypedDict):
    identityProviders: List[IdentityProviderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InlineRedactionPatternOutputTypeDef

```python
# InlineRedactionPatternOutputTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import InlineRedactionPatternOutputTypeDef


def get_value() -> InlineRedactionPatternOutputTypeDef:
    return {
        "builtInPatternId": ...,
    }


# InlineRedactionPatternOutputTypeDef definition

class InlineRedactionPatternOutputTypeDef(TypedDict):
    redactionPlaceHolder: RedactionPlaceHolderTypeDef,  # (2)
    builtInPatternId: NotRequired[str],
    confidenceLevel: NotRequired[int],
    customPattern: NotRequired[CustomPatternTypeDef],  # (1)
    enforcedUrls: NotRequired[List[str]],
    exemptUrls: NotRequired[List[str]],
```

1. See [:material-code-braces: CustomPatternTypeDef](./type_defs.md#custompatterntypedef) 
2. See [:material-code-braces: RedactionPlaceHolderTypeDef](./type_defs.md#redactionplaceholdertypedef) 
## InlineRedactionPatternTypeDef

```python
# InlineRedactionPatternTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import InlineRedactionPatternTypeDef


def get_value() -> InlineRedactionPatternTypeDef:
    return {
        "builtInPatternId": ...,
    }


# InlineRedactionPatternTypeDef definition

class InlineRedactionPatternTypeDef(TypedDict):
    redactionPlaceHolder: RedactionPlaceHolderTypeDef,  # (2)
    builtInPatternId: NotRequired[str],
    confidenceLevel: NotRequired[int],
    customPattern: NotRequired[CustomPatternTypeDef],  # (1)
    enforcedUrls: NotRequired[Sequence[str]],
    exemptUrls: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CustomPatternTypeDef](./type_defs.md#custompatterntypedef) 
2. See [:material-code-braces: RedactionPlaceHolderTypeDef](./type_defs.md#redactionplaceholdertypedef) 
## ListIpAccessSettingsResponseTypeDef

```python
# ListIpAccessSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListIpAccessSettingsResponseTypeDef


def get_value() -> ListIpAccessSettingsResponseTypeDef:
    return {
        "ipAccessSettings": ...,
    }


# ListIpAccessSettingsResponseTypeDef definition

class ListIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: List[IpAccessSettingsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IpAccessSettingsSummaryTypeDef](./type_defs.md#ipaccesssettingssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataProtectionSettingsRequestPaginateTypeDef

```python
# ListDataProtectionSettingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListDataProtectionSettingsRequestPaginateTypeDef


def get_value() -> ListDataProtectionSettingsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDataProtectionSettingsRequestPaginateTypeDef definition

class ListDataProtectionSettingsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsRequestPaginateTypeDef

```python
# ListSessionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListSessionsRequestPaginateTypeDef


def get_value() -> ListSessionsRequestPaginateTypeDef:
    return {
        "portalId": ...,
    }


# ListSessionsRequestPaginateTypeDef definition

class ListSessionsRequestPaginateTypeDef(TypedDict):
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
## ListNetworkSettingsResponseTypeDef

```python
# ListNetworkSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListNetworkSettingsResponseTypeDef


def get_value() -> ListNetworkSettingsResponseTypeDef:
    return {
        "networkSettings": ...,
    }


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
# ListPortalsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListPortalsResponseTypeDef


def get_value() -> ListPortalsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListPortalsResponseTypeDef definition

class ListPortalsResponseTypeDef(TypedDict):
    portals: List[PortalSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PortalSummaryTypeDef](./type_defs.md#portalsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListSessionsResponseTypeDef


def get_value() -> ListSessionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListTrustStoresResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListTrustStoresResponseTypeDef


def get_value() -> ListTrustStoresResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListUserAccessLoggingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListUserAccessLoggingSettingsResponseTypeDef


def get_value() -> ListUserAccessLoggingSettingsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# UserSettingsSummaryTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UserSettingsSummaryTypeDef


def get_value() -> UserSettingsSummaryTypeDef:
    return {
        "cookieSynchronizationConfiguration": ...,
    }


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
    toolbarConfiguration: NotRequired[ToolbarConfigurationOutputTypeDef],  # (7)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-braces: ToolbarConfigurationOutputTypeDef](./type_defs.md#toolbarconfigurationoutputtypedef) 
8. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## UserSettingsTypeDef

```python
# UserSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UserSettingsTypeDef


def get_value() -> UserSettingsTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


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
    toolbarConfiguration: NotRequired[ToolbarConfigurationOutputTypeDef],  # (7)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-braces: ToolbarConfigurationOutputTypeDef](./type_defs.md#toolbarconfigurationoutputtypedef) 
8. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## GetIpAccessSettingsResponseTypeDef

```python
# GetIpAccessSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetIpAccessSettingsResponseTypeDef


def get_value() -> GetIpAccessSettingsResponseTypeDef:
    return {
        "ipAccessSettings": ...,
    }


# GetIpAccessSettingsResponseTypeDef definition

class GetIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: IpAccessSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IpAccessSettingsTypeDef](./type_defs.md#ipaccesssettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIpAccessSettingsResponseTypeDef

```python
# UpdateIpAccessSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateIpAccessSettingsResponseTypeDef


def get_value() -> UpdateIpAccessSettingsResponseTypeDef:
    return {
        "ipAccessSettings": ...,
    }


# UpdateIpAccessSettingsResponseTypeDef definition

class UpdateIpAccessSettingsResponseTypeDef(TypedDict):
    ipAccessSettings: IpAccessSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IpAccessSettingsTypeDef](./type_defs.md#ipaccesssettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InlineRedactionConfigurationOutputTypeDef

```python
# InlineRedactionConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import InlineRedactionConfigurationOutputTypeDef


def get_value() -> InlineRedactionConfigurationOutputTypeDef:
    return {
        "globalConfidenceLevel": ...,
    }


# InlineRedactionConfigurationOutputTypeDef definition

class InlineRedactionConfigurationOutputTypeDef(TypedDict):
    inlineRedactionPatterns: List[InlineRedactionPatternOutputTypeDef],  # (1)
    globalConfidenceLevel: NotRequired[int],
    globalEnforcedUrls: NotRequired[List[str]],
    globalExemptUrls: NotRequired[List[str]],
```

1. See [:material-code-braces: InlineRedactionPatternOutputTypeDef](./type_defs.md#inlineredactionpatternoutputtypedef) 
## InlineRedactionConfigurationTypeDef

```python
# InlineRedactionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import InlineRedactionConfigurationTypeDef


def get_value() -> InlineRedactionConfigurationTypeDef:
    return {
        "globalConfidenceLevel": ...,
    }


# InlineRedactionConfigurationTypeDef definition

class InlineRedactionConfigurationTypeDef(TypedDict):
    inlineRedactionPatterns: Sequence[InlineRedactionPatternTypeDef],  # (1)
    globalConfidenceLevel: NotRequired[int],
    globalEnforcedUrls: NotRequired[Sequence[str]],
    globalExemptUrls: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: InlineRedactionPatternTypeDef](./type_defs.md#inlineredactionpatterntypedef) 
## ListUserSettingsResponseTypeDef

```python
# ListUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import ListUserSettingsResponseTypeDef


def get_value() -> ListUserSettingsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetUserSettingsResponseTypeDef


def get_value() -> GetUserSettingsResponseTypeDef:
    return {
        "userSettings": ...,
    }


# GetUserSettingsResponseTypeDef definition

class GetUserSettingsResponseTypeDef(TypedDict):
    userSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserSettingsResponseTypeDef

```python
# UpdateUserSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateUserSettingsResponseTypeDef


def get_value() -> UpdateUserSettingsResponseTypeDef:
    return {
        "userSettings": ...,
    }


# UpdateUserSettingsResponseTypeDef definition

class UpdateUserSettingsResponseTypeDef(TypedDict):
    userSettings: UserSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserSettingsRequestTypeDef

```python
# CreateUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateUserSettingsRequestTypeDef


def get_value() -> CreateUserSettingsRequestTypeDef:
    return {
        "copyAllowed": ...,
    }


# CreateUserSettingsRequestTypeDef definition

class CreateUserSettingsRequestTypeDef(TypedDict):
    copyAllowed: EnabledTypeType,  # (1)
    downloadAllowed: EnabledTypeType,  # (1)
    pasteAllowed: EnabledTypeType,  # (1)
    printAllowed: EnabledTypeType,  # (1)
    uploadAllowed: EnabledTypeType,  # (1)
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationUnionTypeDef],  # (6)
    customerManagedKey: NotRequired[str],
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (1)
    disconnectTimeoutInMinutes: NotRequired[int],
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    toolbarConfiguration: NotRequired[ToolbarConfigurationUnionTypeDef],  # (9)
```

1. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-braces: CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef) [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
7. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: ToolbarConfigurationTypeDef](./type_defs.md#toolbarconfigurationtypedef) [:material-code-braces: ToolbarConfigurationOutputTypeDef](./type_defs.md#toolbarconfigurationoutputtypedef) 
## UpdateUserSettingsRequestTypeDef

```python
# UpdateUserSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateUserSettingsRequestTypeDef


def get_value() -> UpdateUserSettingsRequestTypeDef:
    return {
        "userSettingsArn": ...,
    }


# UpdateUserSettingsRequestTypeDef definition

class UpdateUserSettingsRequestTypeDef(TypedDict):
    userSettingsArn: str,
    clientToken: NotRequired[str],
    cookieSynchronizationConfiguration: NotRequired[CookieSynchronizationConfigurationUnionTypeDef],  # (1)
    copyAllowed: NotRequired[EnabledTypeType],  # (2)
    deepLinkAllowed: NotRequired[EnabledTypeType],  # (2)
    disconnectTimeoutInMinutes: NotRequired[int],
    downloadAllowed: NotRequired[EnabledTypeType],  # (2)
    idleDisconnectTimeoutInMinutes: NotRequired[int],
    pasteAllowed: NotRequired[EnabledTypeType],  # (2)
    printAllowed: NotRequired[EnabledTypeType],  # (2)
    toolbarConfiguration: NotRequired[ToolbarConfigurationUnionTypeDef],  # (7)
    uploadAllowed: NotRequired[EnabledTypeType],  # (2)
```

1. See [:material-code-braces: CookieSynchronizationConfigurationTypeDef](./type_defs.md#cookiesynchronizationconfigurationtypedef) [:material-code-braces: CookieSynchronizationConfigurationOutputTypeDef](./type_defs.md#cookiesynchronizationconfigurationoutputtypedef) 
2. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
3. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
4. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
5. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
6. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
7. See [:material-code-braces: ToolbarConfigurationTypeDef](./type_defs.md#toolbarconfigurationtypedef) [:material-code-braces: ToolbarConfigurationOutputTypeDef](./type_defs.md#toolbarconfigurationoutputtypedef) 
8. See [:material-code-brackets: EnabledTypeType](./literals.md#enabledtypetype) 
## DataProtectionSettingsTypeDef

```python
# DataProtectionSettingsTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import DataProtectionSettingsTypeDef


def get_value() -> DataProtectionSettingsTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


# DataProtectionSettingsTypeDef definition

class DataProtectionSettingsTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    additionalEncryptionContext: NotRequired[Dict[str, str]],
    associatedPortalArns: NotRequired[List[str]],
    creationDate: NotRequired[datetime],
    customerManagedKey: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    inlineRedactionConfiguration: NotRequired[InlineRedactionConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InlineRedactionConfigurationOutputTypeDef](./type_defs.md#inlineredactionconfigurationoutputtypedef) 
## GetDataProtectionSettingsResponseTypeDef

```python
# GetDataProtectionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import GetDataProtectionSettingsResponseTypeDef


def get_value() -> GetDataProtectionSettingsResponseTypeDef:
    return {
        "dataProtectionSettings": ...,
    }


# GetDataProtectionSettingsResponseTypeDef definition

class GetDataProtectionSettingsResponseTypeDef(TypedDict):
    dataProtectionSettings: DataProtectionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProtectionSettingsTypeDef](./type_defs.md#dataprotectionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataProtectionSettingsResponseTypeDef

```python
# UpdateDataProtectionSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateDataProtectionSettingsResponseTypeDef


def get_value() -> UpdateDataProtectionSettingsResponseTypeDef:
    return {
        "dataProtectionSettings": ...,
    }


# UpdateDataProtectionSettingsResponseTypeDef definition

class UpdateDataProtectionSettingsResponseTypeDef(TypedDict):
    dataProtectionSettings: DataProtectionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataProtectionSettingsTypeDef](./type_defs.md#dataprotectionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataProtectionSettingsRequestTypeDef

```python
# CreateDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import CreateDataProtectionSettingsRequestTypeDef


def get_value() -> CreateDataProtectionSettingsRequestTypeDef:
    return {
        "additionalEncryptionContext": ...,
    }


# CreateDataProtectionSettingsRequestTypeDef definition

class CreateDataProtectionSettingsRequestTypeDef(TypedDict):
    additionalEncryptionContext: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    customerManagedKey: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    inlineRedactionConfiguration: NotRequired[InlineRedactionConfigurationUnionTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: InlineRedactionConfigurationTypeDef](./type_defs.md#inlineredactionconfigurationtypedef) [:material-code-braces: InlineRedactionConfigurationOutputTypeDef](./type_defs.md#inlineredactionconfigurationoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDataProtectionSettingsRequestTypeDef

```python
# UpdateDataProtectionSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_workspaces_web.type_defs import UpdateDataProtectionSettingsRequestTypeDef


def get_value() -> UpdateDataProtectionSettingsRequestTypeDef:
    return {
        "dataProtectionSettingsArn": ...,
    }


# UpdateDataProtectionSettingsRequestTypeDef definition

class UpdateDataProtectionSettingsRequestTypeDef(TypedDict):
    dataProtectionSettingsArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    inlineRedactionConfiguration: NotRequired[InlineRedactionConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InlineRedactionConfigurationTypeDef](./type_defs.md#inlineredactionconfigurationtypedef) [:material-code-braces: InlineRedactionConfigurationOutputTypeDef](./type_defs.md#inlineredactionconfigurationoutputtypedef) 
