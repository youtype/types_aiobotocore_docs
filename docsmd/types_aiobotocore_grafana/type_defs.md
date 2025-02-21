# Type definitions

> [Index](../README.md) > [ManagedGrafana](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## NetworkAccessConfigurationUnionTypeDef

```python
# NetworkAccessConfigurationUnionTypeDef Union usage example

from types_aiobotocore_grafana.type_defs import NetworkAccessConfigurationUnionTypeDef


def get_value() -> NetworkAccessConfigurationUnionTypeDef:
    return ...


# NetworkAccessConfigurationUnionTypeDef definition

NetworkAccessConfigurationUnionTypeDef = Union[
    NetworkAccessConfigurationTypeDef,  # (1)
    NetworkAccessConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
2. See [:material-code-braces: NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef) 

## VpcConfigurationUnionTypeDef

```python
# VpcConfigurationUnionTypeDef Union usage example

from types_aiobotocore_grafana.type_defs import VpcConfigurationUnionTypeDef


def get_value() -> VpcConfigurationUnionTypeDef:
    return ...


# VpcConfigurationUnionTypeDef definition

VpcConfigurationUnionTypeDef = Union[
    VpcConfigurationTypeDef,  # (1)
    VpcConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
2. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 

## UpdateInstructionUnionTypeDef

```python
# UpdateInstructionUnionTypeDef Union usage example

from types_aiobotocore_grafana.type_defs import UpdateInstructionUnionTypeDef


def get_value() -> UpdateInstructionUnionTypeDef:
    return ...


# UpdateInstructionUnionTypeDef definition

UpdateInstructionUnionTypeDef = Union[
    UpdateInstructionTypeDef,  # (1)
    UpdateInstructionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef) 
2. See [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 

## SamlConfigurationUnionTypeDef

```python
# SamlConfigurationUnionTypeDef Union usage example

from types_aiobotocore_grafana.type_defs import SamlConfigurationUnionTypeDef


def get_value() -> SamlConfigurationUnionTypeDef:
    return ...


# SamlConfigurationUnionTypeDef definition

SamlConfigurationUnionTypeDef = Union[
    SamlConfigurationTypeDef,  # (1)
    SamlConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) 
2. See [:material-code-braces: SamlConfigurationOutputTypeDef](./type_defs.md#samlconfigurationoutputtypedef) 



## AssertionAttributesTypeDef

```python
# AssertionAttributesTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AssertionAttributesTypeDef


def get_value() -> AssertionAttributesTypeDef:
    return {
        "email": ...,
    }


# AssertionAttributesTypeDef definition

class AssertionAttributesTypeDef(TypedDict):
    email: NotRequired[str],
    groups: NotRequired[str],
    login: NotRequired[str],
    name: NotRequired[str],
    org: NotRequired[str],
    role: NotRequired[str],
```

## AssociateLicenseRequestTypeDef

```python
# AssociateLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AssociateLicenseRequestTypeDef


def get_value() -> AssociateLicenseRequestTypeDef:
    return {
        "licenseType": ...,
    }


# AssociateLicenseRequestTypeDef definition

class AssociateLicenseRequestTypeDef(TypedDict):
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
    grafanaToken: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ResponseMetadataTypeDef


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

## AwsSsoAuthenticationTypeDef

```python
# AwsSsoAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AwsSsoAuthenticationTypeDef


def get_value() -> AwsSsoAuthenticationTypeDef:
    return {
        "ssoClientId": ...,
    }


# AwsSsoAuthenticationTypeDef definition

class AwsSsoAuthenticationTypeDef(TypedDict):
    ssoClientId: NotRequired[str],
```

## AuthenticationSummaryTypeDef

```python
# AuthenticationSummaryTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AuthenticationSummaryTypeDef


def get_value() -> AuthenticationSummaryTypeDef:
    return {
        "providers": ...,
    }


# AuthenticationSummaryTypeDef definition

class AuthenticationSummaryTypeDef(TypedDict):
    providers: List[AuthenticationProviderTypesType],  # (1)
    samlConfigurationStatus: NotRequired[SamlConfigurationStatusType],  # (2)
```

1. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
2. See [:material-code-brackets: SamlConfigurationStatusType](./literals.md#samlconfigurationstatustype) 
## CreateWorkspaceApiKeyRequestTypeDef

```python
# CreateWorkspaceApiKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceApiKeyRequestTypeDef


def get_value() -> CreateWorkspaceApiKeyRequestTypeDef:
    return {
        "keyName": ...,
    }


# CreateWorkspaceApiKeyRequestTypeDef definition

class CreateWorkspaceApiKeyRequestTypeDef(TypedDict):
    keyName: str,
    keyRole: str,
    secondsToLive: int,
    workspaceId: str,
```

## CreateWorkspaceServiceAccountRequestTypeDef

```python
# CreateWorkspaceServiceAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceServiceAccountRequestTypeDef


def get_value() -> CreateWorkspaceServiceAccountRequestTypeDef:
    return {
        "grafanaRole": ...,
    }


# CreateWorkspaceServiceAccountRequestTypeDef definition

class CreateWorkspaceServiceAccountRequestTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    name: str,
    workspaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## CreateWorkspaceServiceAccountTokenRequestTypeDef

```python
# CreateWorkspaceServiceAccountTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceServiceAccountTokenRequestTypeDef


def get_value() -> CreateWorkspaceServiceAccountTokenRequestTypeDef:
    return {
        "name": ...,
    }


# CreateWorkspaceServiceAccountTokenRequestTypeDef definition

class CreateWorkspaceServiceAccountTokenRequestTypeDef(TypedDict):
    name: str,
    secondsToLive: int,
    serviceAccountId: str,
    workspaceId: str,
```

## ServiceAccountTokenSummaryWithKeyTypeDef

```python
# ServiceAccountTokenSummaryWithKeyTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ServiceAccountTokenSummaryWithKeyTypeDef


def get_value() -> ServiceAccountTokenSummaryWithKeyTypeDef:
    return {
        "id": ...,
    }


# ServiceAccountTokenSummaryWithKeyTypeDef definition

class ServiceAccountTokenSummaryWithKeyTypeDef(TypedDict):
    id: str,
    key: str,
    name: str,
```

## DeleteWorkspaceApiKeyRequestTypeDef

```python
# DeleteWorkspaceApiKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceApiKeyRequestTypeDef


def get_value() -> DeleteWorkspaceApiKeyRequestTypeDef:
    return {
        "keyName": ...,
    }


# DeleteWorkspaceApiKeyRequestTypeDef definition

class DeleteWorkspaceApiKeyRequestTypeDef(TypedDict):
    keyName: str,
    workspaceId: str,
```

## DeleteWorkspaceRequestTypeDef

```python
# DeleteWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceRequestTypeDef


def get_value() -> DeleteWorkspaceRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DeleteWorkspaceRequestTypeDef definition

class DeleteWorkspaceRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DeleteWorkspaceServiceAccountRequestTypeDef

```python
# DeleteWorkspaceServiceAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceServiceAccountRequestTypeDef


def get_value() -> DeleteWorkspaceServiceAccountRequestTypeDef:
    return {
        "serviceAccountId": ...,
    }


# DeleteWorkspaceServiceAccountRequestTypeDef definition

class DeleteWorkspaceServiceAccountRequestTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
```

## DeleteWorkspaceServiceAccountTokenRequestTypeDef

```python
# DeleteWorkspaceServiceAccountTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceServiceAccountTokenRequestTypeDef


def get_value() -> DeleteWorkspaceServiceAccountTokenRequestTypeDef:
    return {
        "serviceAccountId": ...,
    }


# DeleteWorkspaceServiceAccountTokenRequestTypeDef definition

class DeleteWorkspaceServiceAccountTokenRequestTypeDef(TypedDict):
    serviceAccountId: str,
    tokenId: str,
    workspaceId: str,
```

## DescribeWorkspaceAuthenticationRequestTypeDef

```python
# DescribeWorkspaceAuthenticationRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceAuthenticationRequestTypeDef


def get_value() -> DescribeWorkspaceAuthenticationRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceAuthenticationRequestTypeDef definition

class DescribeWorkspaceAuthenticationRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeWorkspaceConfigurationRequestTypeDef

```python
# DescribeWorkspaceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceConfigurationRequestTypeDef


def get_value() -> DescribeWorkspaceConfigurationRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceConfigurationRequestTypeDef definition

class DescribeWorkspaceConfigurationRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeWorkspaceRequestTypeDef

```python
# DescribeWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceRequestTypeDef


def get_value() -> DescribeWorkspaceRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceRequestTypeDef definition

class DescribeWorkspaceRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DisassociateLicenseRequestTypeDef

```python
# DisassociateLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DisassociateLicenseRequestTypeDef


def get_value() -> DisassociateLicenseRequestTypeDef:
    return {
        "licenseType": ...,
    }


# DisassociateLicenseRequestTypeDef definition

class DisassociateLicenseRequestTypeDef(TypedDict):
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## IdpMetadataTypeDef

```python
# IdpMetadataTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import IdpMetadataTypeDef


def get_value() -> IdpMetadataTypeDef:
    return {
        "url": ...,
    }


# IdpMetadataTypeDef definition

class IdpMetadataTypeDef(TypedDict):
    url: NotRequired[str],
    xml: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import PaginatorConfigTypeDef


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

## ListPermissionsRequestTypeDef

```python
# ListPermissionsRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListPermissionsRequestTypeDef


def get_value() -> ListPermissionsRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# ListPermissionsRequestTypeDef definition

class ListPermissionsRequestTypeDef(TypedDict):
    workspaceId: str,
    groupId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    userId: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListVersionsRequestTypeDef

```python
# ListVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListVersionsRequestTypeDef


def get_value() -> ListVersionsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListVersionsRequestTypeDef definition

class ListVersionsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    workspaceId: NotRequired[str],
```

## ListWorkspaceServiceAccountTokensRequestTypeDef

```python
# ListWorkspaceServiceAccountTokensRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountTokensRequestTypeDef


def get_value() -> ListWorkspaceServiceAccountTokensRequestTypeDef:
    return {
        "serviceAccountId": ...,
    }


# ListWorkspaceServiceAccountTokensRequestTypeDef definition

class ListWorkspaceServiceAccountTokensRequestTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceAccountTokenSummaryTypeDef

```python
# ServiceAccountTokenSummaryTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ServiceAccountTokenSummaryTypeDef


def get_value() -> ServiceAccountTokenSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# ServiceAccountTokenSummaryTypeDef definition

class ServiceAccountTokenSummaryTypeDef(TypedDict):
    createdAt: datetime,
    expiresAt: datetime,
    id: str,
    name: str,
    lastUsedAt: NotRequired[datetime],
```

## ListWorkspaceServiceAccountsRequestTypeDef

```python
# ListWorkspaceServiceAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountsRequestTypeDef


def get_value() -> ListWorkspaceServiceAccountsRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# ListWorkspaceServiceAccountsRequestTypeDef definition

class ListWorkspaceServiceAccountsRequestTypeDef(TypedDict):
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceAccountSummaryTypeDef

```python
# ServiceAccountSummaryTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ServiceAccountSummaryTypeDef


def get_value() -> ServiceAccountSummaryTypeDef:
    return {
        "grafanaRole": ...,
    }


# ServiceAccountSummaryTypeDef definition

class ServiceAccountSummaryTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    id: str,
    isDisabled: str,
    name: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## ListWorkspacesRequestTypeDef

```python
# ListWorkspacesRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspacesRequestTypeDef


def get_value() -> ListWorkspacesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListWorkspacesRequestTypeDef definition

class ListWorkspacesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NetworkAccessConfigurationOutputTypeDef

```python
# NetworkAccessConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import NetworkAccessConfigurationOutputTypeDef


def get_value() -> NetworkAccessConfigurationOutputTypeDef:
    return {
        "prefixListIds": ...,
    }


# NetworkAccessConfigurationOutputTypeDef definition

class NetworkAccessConfigurationOutputTypeDef(TypedDict):
    prefixListIds: List[str],
    vpceIds: List[str],
```

## NetworkAccessConfigurationTypeDef

```python
# NetworkAccessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import NetworkAccessConfigurationTypeDef


def get_value() -> NetworkAccessConfigurationTypeDef:
    return {
        "prefixListIds": ...,
    }


# NetworkAccessConfigurationTypeDef definition

class NetworkAccessConfigurationTypeDef(TypedDict):
    prefixListIds: Sequence[str],
    vpceIds: Sequence[str],
```

## UserTypeDef

```python
# UserTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UserTypeDef


def get_value() -> UserTypeDef:
    return {
        "id": ...,
    }


# UserTypeDef definition

class UserTypeDef(TypedDict):
    id: str,
    type: UserTypeType,  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## RoleValuesOutputTypeDef

```python
# RoleValuesOutputTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import RoleValuesOutputTypeDef


def get_value() -> RoleValuesOutputTypeDef:
    return {
        "admin": ...,
    }


# RoleValuesOutputTypeDef definition

class RoleValuesOutputTypeDef(TypedDict):
    admin: NotRequired[List[str]],
    editor: NotRequired[List[str]],
```

## RoleValuesTypeDef

```python
# RoleValuesTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import RoleValuesTypeDef


def get_value() -> RoleValuesTypeDef:
    return {
        "admin": ...,
    }


# RoleValuesTypeDef definition

class RoleValuesTypeDef(TypedDict):
    admin: NotRequired[Sequence[str]],
    editor: NotRequired[Sequence[str]],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateWorkspaceConfigurationRequestTypeDef

```python
# UpdateWorkspaceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateWorkspaceConfigurationRequestTypeDef


def get_value() -> UpdateWorkspaceConfigurationRequestTypeDef:
    return {
        "configuration": ...,
    }


# UpdateWorkspaceConfigurationRequestTypeDef definition

class UpdateWorkspaceConfigurationRequestTypeDef(TypedDict):
    configuration: str,
    workspaceId: str,
    grafanaVersion: NotRequired[str],
```

## VpcConfigurationOutputTypeDef

```python
# VpcConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import VpcConfigurationOutputTypeDef


def get_value() -> VpcConfigurationOutputTypeDef:
    return {
        "securityGroupIds": ...,
    }


# VpcConfigurationOutputTypeDef definition

class VpcConfigurationOutputTypeDef(TypedDict):
    securityGroupIds: List[str],
    subnetIds: List[str],
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import VpcConfigurationTypeDef


def get_value() -> VpcConfigurationTypeDef:
    return {
        "securityGroupIds": ...,
    }


# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
```

## CreateWorkspaceApiKeyResponseTypeDef

```python
# CreateWorkspaceApiKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceApiKeyResponseTypeDef


def get_value() -> CreateWorkspaceApiKeyResponseTypeDef:
    return {
        "key": ...,
    }


# CreateWorkspaceApiKeyResponseTypeDef definition

class CreateWorkspaceApiKeyResponseTypeDef(TypedDict):
    key: str,
    keyName: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceServiceAccountResponseTypeDef

```python
# CreateWorkspaceServiceAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceServiceAccountResponseTypeDef


def get_value() -> CreateWorkspaceServiceAccountResponseTypeDef:
    return {
        "grafanaRole": ...,
    }


# CreateWorkspaceServiceAccountResponseTypeDef definition

class CreateWorkspaceServiceAccountResponseTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    id: str,
    name: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceApiKeyResponseTypeDef

```python
# DeleteWorkspaceApiKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceApiKeyResponseTypeDef


def get_value() -> DeleteWorkspaceApiKeyResponseTypeDef:
    return {
        "keyName": ...,
    }


# DeleteWorkspaceApiKeyResponseTypeDef definition

class DeleteWorkspaceApiKeyResponseTypeDef(TypedDict):
    keyName: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceServiceAccountResponseTypeDef

```python
# DeleteWorkspaceServiceAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceServiceAccountResponseTypeDef


def get_value() -> DeleteWorkspaceServiceAccountResponseTypeDef:
    return {
        "serviceAccountId": ...,
    }


# DeleteWorkspaceServiceAccountResponseTypeDef definition

class DeleteWorkspaceServiceAccountResponseTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceServiceAccountTokenResponseTypeDef

```python
# DeleteWorkspaceServiceAccountTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceServiceAccountTokenResponseTypeDef


def get_value() -> DeleteWorkspaceServiceAccountTokenResponseTypeDef:
    return {
        "serviceAccountId": ...,
    }


# DeleteWorkspaceServiceAccountTokenResponseTypeDef definition

class DeleteWorkspaceServiceAccountTokenResponseTypeDef(TypedDict):
    serviceAccountId: str,
    tokenId: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceConfigurationResponseTypeDef

```python
# DescribeWorkspaceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceConfigurationResponseTypeDef


def get_value() -> DescribeWorkspaceConfigurationResponseTypeDef:
    return {
        "configuration": ...,
    }


# DescribeWorkspaceConfigurationResponseTypeDef definition

class DescribeWorkspaceConfigurationResponseTypeDef(TypedDict):
    configuration: str,
    grafanaVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVersionsResponseTypeDef

```python
# ListVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListVersionsResponseTypeDef


def get_value() -> ListVersionsResponseTypeDef:
    return {
        "grafanaVersions": ...,
    }


# ListVersionsResponseTypeDef definition

class ListVersionsResponseTypeDef(TypedDict):
    grafanaVersions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceSummaryTypeDef

```python
# WorkspaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import WorkspaceSummaryTypeDef


def get_value() -> WorkspaceSummaryTypeDef:
    return {
        "authentication": ...,
    }


# WorkspaceSummaryTypeDef definition

class WorkspaceSummaryTypeDef(TypedDict):
    authentication: AuthenticationSummaryTypeDef,  # (1)
    created: datetime,
    endpoint: str,
    grafanaVersion: str,
    id: str,
    modified: datetime,
    status: WorkspaceStatusType,  # (4)
    description: NotRequired[str],
    grafanaToken: NotRequired[str],
    licenseType: NotRequired[LicenseTypeType],  # (2)
    name: NotRequired[str],
    notificationDestinations: NotRequired[List[NotificationDestinationTypeType]],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AuthenticationSummaryTypeDef](./type_defs.md#authenticationsummarytypedef) 
2. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
3. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
4. See [:material-code-brackets: WorkspaceStatusType](./literals.md#workspacestatustype) 
## CreateWorkspaceServiceAccountTokenResponseTypeDef

```python
# CreateWorkspaceServiceAccountTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceServiceAccountTokenResponseTypeDef


def get_value() -> CreateWorkspaceServiceAccountTokenResponseTypeDef:
    return {
        "serviceAccountId": ...,
    }


# CreateWorkspaceServiceAccountTokenResponseTypeDef definition

class CreateWorkspaceServiceAccountTokenResponseTypeDef(TypedDict):
    serviceAccountId: str,
    serviceAccountToken: ServiceAccountTokenSummaryWithKeyTypeDef,  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceAccountTokenSummaryWithKeyTypeDef](./type_defs.md#serviceaccounttokensummarywithkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsRequestPaginateTypeDef

```python
# ListPermissionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListPermissionsRequestPaginateTypeDef


def get_value() -> ListPermissionsRequestPaginateTypeDef:
    return {
        "workspaceId": ...,
    }


# ListPermissionsRequestPaginateTypeDef definition

class ListPermissionsRequestPaginateTypeDef(TypedDict):
    workspaceId: str,
    groupId: NotRequired[str],
    userId: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVersionsRequestPaginateTypeDef

```python
# ListVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListVersionsRequestPaginateTypeDef


def get_value() -> ListVersionsRequestPaginateTypeDef:
    return {
        "workspaceId": ...,
    }


# ListVersionsRequestPaginateTypeDef definition

class ListVersionsRequestPaginateTypeDef(TypedDict):
    workspaceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountTokensRequestPaginateTypeDef

```python
# ListWorkspaceServiceAccountTokensRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountTokensRequestPaginateTypeDef


def get_value() -> ListWorkspaceServiceAccountTokensRequestPaginateTypeDef:
    return {
        "serviceAccountId": ...,
    }


# ListWorkspaceServiceAccountTokensRequestPaginateTypeDef definition

class ListWorkspaceServiceAccountTokensRequestPaginateTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountsRequestPaginateTypeDef

```python
# ListWorkspaceServiceAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountsRequestPaginateTypeDef


def get_value() -> ListWorkspaceServiceAccountsRequestPaginateTypeDef:
    return {
        "workspaceId": ...,
    }


# ListWorkspaceServiceAccountsRequestPaginateTypeDef definition

class ListWorkspaceServiceAccountsRequestPaginateTypeDef(TypedDict):
    workspaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspacesRequestPaginateTypeDef

```python
# ListWorkspacesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspacesRequestPaginateTypeDef


def get_value() -> ListWorkspacesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListWorkspacesRequestPaginateTypeDef definition

class ListWorkspacesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountTokensResponseTypeDef

```python
# ListWorkspaceServiceAccountTokensResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountTokensResponseTypeDef


def get_value() -> ListWorkspaceServiceAccountTokensResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListWorkspaceServiceAccountTokensResponseTypeDef definition

class ListWorkspaceServiceAccountTokensResponseTypeDef(TypedDict):
    serviceAccountId: str,
    serviceAccountTokens: List[ServiceAccountTokenSummaryTypeDef],  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceAccountTokenSummaryTypeDef](./type_defs.md#serviceaccounttokensummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkspaceServiceAccountsResponseTypeDef

```python
# ListWorkspaceServiceAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspaceServiceAccountsResponseTypeDef


def get_value() -> ListWorkspaceServiceAccountsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListWorkspaceServiceAccountsResponseTypeDef definition

class ListWorkspaceServiceAccountsResponseTypeDef(TypedDict):
    serviceAccounts: List[ServiceAccountSummaryTypeDef],  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceAccountSummaryTypeDef](./type_defs.md#serviceaccountsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PermissionEntryTypeDef

```python
# PermissionEntryTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import PermissionEntryTypeDef


def get_value() -> PermissionEntryTypeDef:
    return {
        "role": ...,
    }


# PermissionEntryTypeDef definition

class PermissionEntryTypeDef(TypedDict):
    role: RoleType,  # (1)
    user: UserTypeDef,  # (2)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## UpdateInstructionOutputTypeDef

```python
# UpdateInstructionOutputTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateInstructionOutputTypeDef


def get_value() -> UpdateInstructionOutputTypeDef:
    return {
        "action": ...,
    }


# UpdateInstructionOutputTypeDef definition

class UpdateInstructionOutputTypeDef(TypedDict):
    action: UpdateActionType,  # (1)
    role: RoleType,  # (2)
    users: List[UserTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateActionType](./literals.md#updateactiontype) 
2. See [:material-code-brackets: RoleType](./literals.md#roletype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## UpdateInstructionTypeDef

```python
# UpdateInstructionTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateInstructionTypeDef


def get_value() -> UpdateInstructionTypeDef:
    return {
        "action": ...,
    }


# UpdateInstructionTypeDef definition

class UpdateInstructionTypeDef(TypedDict):
    action: UpdateActionType,  # (1)
    role: RoleType,  # (2)
    users: Sequence[UserTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateActionType](./literals.md#updateactiontype) 
2. See [:material-code-brackets: RoleType](./literals.md#roletype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## SamlConfigurationOutputTypeDef

```python
# SamlConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import SamlConfigurationOutputTypeDef


def get_value() -> SamlConfigurationOutputTypeDef:
    return {
        "allowedOrganizations": ...,
    }


# SamlConfigurationOutputTypeDef definition

class SamlConfigurationOutputTypeDef(TypedDict):
    idpMetadata: IdpMetadataTypeDef,  # (2)
    allowedOrganizations: NotRequired[List[str]],
    assertionAttributes: NotRequired[AssertionAttributesTypeDef],  # (1)
    loginValidityDuration: NotRequired[int],
    roleValues: NotRequired[RoleValuesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AssertionAttributesTypeDef](./type_defs.md#assertionattributestypedef) 
2. See [:material-code-braces: IdpMetadataTypeDef](./type_defs.md#idpmetadatatypedef) 
3. See [:material-code-braces: RoleValuesOutputTypeDef](./type_defs.md#rolevaluesoutputtypedef) 
## SamlConfigurationTypeDef

```python
# SamlConfigurationTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import SamlConfigurationTypeDef


def get_value() -> SamlConfigurationTypeDef:
    return {
        "allowedOrganizations": ...,
    }


# SamlConfigurationTypeDef definition

class SamlConfigurationTypeDef(TypedDict):
    idpMetadata: IdpMetadataTypeDef,  # (2)
    allowedOrganizations: NotRequired[Sequence[str]],
    assertionAttributes: NotRequired[AssertionAttributesTypeDef],  # (1)
    loginValidityDuration: NotRequired[int],
    roleValues: NotRequired[RoleValuesTypeDef],  # (3)
```

1. See [:material-code-braces: AssertionAttributesTypeDef](./type_defs.md#assertionattributestypedef) 
2. See [:material-code-braces: IdpMetadataTypeDef](./type_defs.md#idpmetadatatypedef) 
3. See [:material-code-braces: RoleValuesTypeDef](./type_defs.md#rolevaluestypedef) 
## WorkspaceDescriptionTypeDef

```python
# WorkspaceDescriptionTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import WorkspaceDescriptionTypeDef


def get_value() -> WorkspaceDescriptionTypeDef:
    return {
        "accountAccessType": ...,
    }


# WorkspaceDescriptionTypeDef definition

class WorkspaceDescriptionTypeDef(TypedDict):
    authentication: AuthenticationSummaryTypeDef,  # (2)
    created: datetime,
    dataSources: List[DataSourceTypeType],  # (3)
    endpoint: str,
    grafanaVersion: str,
    id: str,
    modified: datetime,
    status: WorkspaceStatusType,  # (8)
    accountAccessType: NotRequired[AccountAccessTypeType],  # (1)
    description: NotRequired[str],
    freeTrialConsumed: NotRequired[bool],
    freeTrialExpiration: NotRequired[datetime],
    grafanaToken: NotRequired[str],
    licenseExpiration: NotRequired[datetime],
    licenseType: NotRequired[LicenseTypeType],  # (4)
    name: NotRequired[str],
    networkAccessControl: NotRequired[NetworkAccessConfigurationOutputTypeDef],  # (5)
    notificationDestinations: NotRequired[List[NotificationDestinationTypeType]],  # (6)
    organizationRoleName: NotRequired[str],
    organizationalUnits: NotRequired[List[str]],
    permissionType: NotRequired[PermissionTypeType],  # (7)
    stackSetName: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    vpcConfiguration: NotRequired[VpcConfigurationOutputTypeDef],  # (9)
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-braces: AuthenticationSummaryTypeDef](./type_defs.md#authenticationsummarytypedef) 
3. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
4. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
5. See [:material-code-braces: NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef) 
6. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
7. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
8. See [:material-code-brackets: WorkspaceStatusType](./literals.md#workspacestatustype) 
9. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
## ListWorkspacesResponseTypeDef

```python
# ListWorkspacesResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListWorkspacesResponseTypeDef


def get_value() -> ListWorkspacesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListWorkspacesResponseTypeDef definition

class ListWorkspacesResponseTypeDef(TypedDict):
    workspaces: List[WorkspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsResponseTypeDef

```python
# ListPermissionsResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import ListPermissionsResponseTypeDef


def get_value() -> ListPermissionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListPermissionsResponseTypeDef definition

class ListPermissionsResponseTypeDef(TypedDict):
    permissions: List[PermissionEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionEntryTypeDef](./type_defs.md#permissionentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateErrorTypeDef

```python
# UpdateErrorTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateErrorTypeDef


def get_value() -> UpdateErrorTypeDef:
    return {
        "causedBy": ...,
    }


# UpdateErrorTypeDef definition

class UpdateErrorTypeDef(TypedDict):
    causedBy: UpdateInstructionOutputTypeDef,  # (1)
    code: int,
    message: str,
```

1. See [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 
## SamlAuthenticationTypeDef

```python
# SamlAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import SamlAuthenticationTypeDef


def get_value() -> SamlAuthenticationTypeDef:
    return {
        "configuration": ...,
    }


# SamlAuthenticationTypeDef definition

class SamlAuthenticationTypeDef(TypedDict):
    status: SamlConfigurationStatusType,  # (2)
    configuration: NotRequired[SamlConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SamlConfigurationOutputTypeDef](./type_defs.md#samlconfigurationoutputtypedef) 
2. See [:material-code-brackets: SamlConfigurationStatusType](./literals.md#samlconfigurationstatustype) 
## AssociateLicenseResponseTypeDef

```python
# AssociateLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AssociateLicenseResponseTypeDef


def get_value() -> AssociateLicenseResponseTypeDef:
    return {
        "workspace": ...,
    }


# AssociateLicenseResponseTypeDef definition

class AssociateLicenseResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceResponseTypeDef

```python
# CreateWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceResponseTypeDef


def get_value() -> CreateWorkspaceResponseTypeDef:
    return {
        "workspace": ...,
    }


# CreateWorkspaceResponseTypeDef definition

class CreateWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceResponseTypeDef

```python
# DeleteWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DeleteWorkspaceResponseTypeDef


def get_value() -> DeleteWorkspaceResponseTypeDef:
    return {
        "workspace": ...,
    }


# DeleteWorkspaceResponseTypeDef definition

class DeleteWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceResponseTypeDef

```python
# DescribeWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceResponseTypeDef


def get_value() -> DescribeWorkspaceResponseTypeDef:
    return {
        "workspace": ...,
    }


# DescribeWorkspaceResponseTypeDef definition

class DescribeWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateLicenseResponseTypeDef

```python
# DisassociateLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DisassociateLicenseResponseTypeDef


def get_value() -> DisassociateLicenseResponseTypeDef:
    return {
        "workspace": ...,
    }


# DisassociateLicenseResponseTypeDef definition

class DisassociateLicenseResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspaceResponseTypeDef

```python
# UpdateWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateWorkspaceResponseTypeDef


def get_value() -> UpdateWorkspaceResponseTypeDef:
    return {
        "workspace": ...,
    }


# UpdateWorkspaceResponseTypeDef definition

class UpdateWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceRequestTypeDef

```python
# CreateWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import CreateWorkspaceRequestTypeDef


def get_value() -> CreateWorkspaceRequestTypeDef:
    return {
        "accountAccessType": ...,
    }


# CreateWorkspaceRequestTypeDef definition

class CreateWorkspaceRequestTypeDef(TypedDict):
    accountAccessType: AccountAccessTypeType,  # (1)
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (2)
    permissionType: PermissionTypeType,  # (3)
    clientToken: NotRequired[str],
    configuration: NotRequired[str],
    grafanaVersion: NotRequired[str],
    networkAccessControl: NotRequired[NetworkAccessConfigurationUnionTypeDef],  # (4)
    organizationRoleName: NotRequired[str],
    stackSetName: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    vpcConfiguration: NotRequired[VpcConfigurationUnionTypeDef],  # (5)
    workspaceDataSources: NotRequired[Sequence[DataSourceTypeType]],  # (6)
    workspaceDescription: NotRequired[str],
    workspaceName: NotRequired[str],
    workspaceNotificationDestinations: NotRequired[Sequence[NotificationDestinationTypeType]],  # (7)
    workspaceOrganizationalUnits: NotRequired[Sequence[str]],
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) [:material-code-braces: NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef) 
5. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
6. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
7. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
## UpdateWorkspaceRequestTypeDef

```python
# UpdateWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateWorkspaceRequestTypeDef


def get_value() -> UpdateWorkspaceRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# UpdateWorkspaceRequestTypeDef definition

class UpdateWorkspaceRequestTypeDef(TypedDict):
    workspaceId: str,
    accountAccessType: NotRequired[AccountAccessTypeType],  # (1)
    networkAccessControl: NotRequired[NetworkAccessConfigurationUnionTypeDef],  # (2)
    organizationRoleName: NotRequired[str],
    permissionType: NotRequired[PermissionTypeType],  # (3)
    removeNetworkAccessConfiguration: NotRequired[bool],
    removeVpcConfiguration: NotRequired[bool],
    stackSetName: NotRequired[str],
    vpcConfiguration: NotRequired[VpcConfigurationUnionTypeDef],  # (4)
    workspaceDataSources: NotRequired[Sequence[DataSourceTypeType]],  # (5)
    workspaceDescription: NotRequired[str],
    workspaceName: NotRequired[str],
    workspaceNotificationDestinations: NotRequired[Sequence[NotificationDestinationTypeType]],  # (6)
    workspaceOrganizationalUnits: NotRequired[Sequence[str]],
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) [:material-code-braces: NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
6. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
## UpdatePermissionsResponseTypeDef

```python
# UpdatePermissionsResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdatePermissionsResponseTypeDef


def get_value() -> UpdatePermissionsResponseTypeDef:
    return {
        "errors": ...,
    }


# UpdatePermissionsResponseTypeDef definition

class UpdatePermissionsResponseTypeDef(TypedDict):
    errors: List[UpdateErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateErrorTypeDef](./type_defs.md#updateerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePermissionsRequestTypeDef

```python
# UpdatePermissionsRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdatePermissionsRequestTypeDef


def get_value() -> UpdatePermissionsRequestTypeDef:
    return {
        "updateInstructionBatch": ...,
    }


# UpdatePermissionsRequestTypeDef definition

class UpdatePermissionsRequestTypeDef(TypedDict):
    updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef],  # (1)
    workspaceId: str,
```

1. See [:material-code-braces: UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef) [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 
## AuthenticationDescriptionTypeDef

```python
# AuthenticationDescriptionTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import AuthenticationDescriptionTypeDef


def get_value() -> AuthenticationDescriptionTypeDef:
    return {
        "awsSso": ...,
    }


# AuthenticationDescriptionTypeDef definition

class AuthenticationDescriptionTypeDef(TypedDict):
    providers: List[AuthenticationProviderTypesType],  # (2)
    awsSso: NotRequired[AwsSsoAuthenticationTypeDef],  # (1)
    saml: NotRequired[SamlAuthenticationTypeDef],  # (3)
```

1. See [:material-code-braces: AwsSsoAuthenticationTypeDef](./type_defs.md#awsssoauthenticationtypedef) 
2. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
3. See [:material-code-braces: SamlAuthenticationTypeDef](./type_defs.md#samlauthenticationtypedef) 
## UpdateWorkspaceAuthenticationRequestTypeDef

```python
# UpdateWorkspaceAuthenticationRequestTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateWorkspaceAuthenticationRequestTypeDef


def get_value() -> UpdateWorkspaceAuthenticationRequestTypeDef:
    return {
        "authenticationProviders": ...,
    }


# UpdateWorkspaceAuthenticationRequestTypeDef definition

class UpdateWorkspaceAuthenticationRequestTypeDef(TypedDict):
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (1)
    workspaceId: str,
    samlConfiguration: NotRequired[SamlConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
2. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) [:material-code-braces: SamlConfigurationOutputTypeDef](./type_defs.md#samlconfigurationoutputtypedef) 
## DescribeWorkspaceAuthenticationResponseTypeDef

```python
# DescribeWorkspaceAuthenticationResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import DescribeWorkspaceAuthenticationResponseTypeDef


def get_value() -> DescribeWorkspaceAuthenticationResponseTypeDef:
    return {
        "authentication": ...,
    }


# DescribeWorkspaceAuthenticationResponseTypeDef definition

class DescribeWorkspaceAuthenticationResponseTypeDef(TypedDict):
    authentication: AuthenticationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationDescriptionTypeDef](./type_defs.md#authenticationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspaceAuthenticationResponseTypeDef

```python
# UpdateWorkspaceAuthenticationResponseTypeDef TypedDict usage example

from types_aiobotocore_grafana.type_defs import UpdateWorkspaceAuthenticationResponseTypeDef


def get_value() -> UpdateWorkspaceAuthenticationResponseTypeDef:
    return {
        "authentication": ...,
    }


# UpdateWorkspaceAuthenticationResponseTypeDef definition

class UpdateWorkspaceAuthenticationResponseTypeDef(TypedDict):
    authentication: AuthenticationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationDescriptionTypeDef](./type_defs.md#authenticationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
