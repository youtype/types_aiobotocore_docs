# Type definitions

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## SettingsUnionTypeDef

```python
# SettingsUnionTypeDef Union usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import SettingsUnionTypeDef


def get_value() -> SettingsUnionTypeDef:
    return ...


# SettingsUnionTypeDef definition

SettingsUnionTypeDef = Union[
    SettingsTypeDef,  # (1)
    SettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
2. See [:material-code-braces: SettingsOutputTypeDef](./type_defs.md#settingsoutputtypedef) 

## IdentityProviderUnionTypeDef

```python
# IdentityProviderUnionTypeDef Union usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import IdentityProviderUnionTypeDef


def get_value() -> IdentityProviderUnionTypeDef:
    return ...


# IdentityProviderUnionTypeDef definition

IdentityProviderUnionTypeDef = Union[
    IdentityProviderTypeDef,  # (1)
    IdentityProviderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 



## DomainNetworkSettingsOutputTypeDef

```python
# DomainNetworkSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DomainNetworkSettingsOutputTypeDef


def get_value() -> DomainNetworkSettingsOutputTypeDef:
    return {
        "Subnets": ...,
    }


# DomainNetworkSettingsOutputTypeDef definition

class DomainNetworkSettingsOutputTypeDef(TypedDict):
    Subnets: List[str],
```

## DomainNetworkSettingsTypeDef

```python
# DomainNetworkSettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DomainNetworkSettingsTypeDef


def get_value() -> DomainNetworkSettingsTypeDef:
    return {
        "Subnets": ...,
    }


# DomainNetworkSettingsTypeDef definition

class DomainNetworkSettingsTypeDef(TypedDict):
    Subnets: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ResponseMetadataTypeDef


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

## SecretsManagerCredentialsProviderTypeDef

```python
# SecretsManagerCredentialsProviderTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import SecretsManagerCredentialsProviderTypeDef


def get_value() -> SecretsManagerCredentialsProviderTypeDef:
    return {
        "SecretId": ...,
    }


# SecretsManagerCredentialsProviderTypeDef definition

class SecretsManagerCredentialsProviderTypeDef(TypedDict):
    SecretId: NotRequired[str],
```

## DeleteLicenseServerEndpointRequestTypeDef

```python
# DeleteLicenseServerEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DeleteLicenseServerEndpointRequestTypeDef


def get_value() -> DeleteLicenseServerEndpointRequestTypeDef:
    return {
        "LicenseServerEndpointArn": ...,
    }


# DeleteLicenseServerEndpointRequestTypeDef definition

class DeleteLicenseServerEndpointRequestTypeDef(TypedDict):
    LicenseServerEndpointArn: str,
    ServerType: ServerTypeType,  # (1)
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "Attribute": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Attribute: NotRequired[str],
    Operation: NotRequired[str],
    Value: NotRequired[str],
```

## SettingsOutputTypeDef

```python
# SettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import SettingsOutputTypeDef


def get_value() -> SettingsOutputTypeDef:
    return {
        "SecurityGroupId": ...,
    }


# SettingsOutputTypeDef definition

class SettingsOutputTypeDef(TypedDict):
    SecurityGroupId: str,
    Subnets: List[str],
```

## InstanceSummaryTypeDef

```python
# InstanceSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import InstanceSummaryTypeDef


def get_value() -> InstanceSummaryTypeDef:
    return {
        "InstanceId": ...,
    }


# InstanceSummaryTypeDef definition

class InstanceSummaryTypeDef(TypedDict):
    InstanceId: str,
    Products: List[str],
    Status: str,
    LastStatusCheckDate: NotRequired[str],
    StatusMessage: NotRequired[str],
```

## LicenseServerTypeDef

```python
# LicenseServerTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import LicenseServerTypeDef


def get_value() -> LicenseServerTypeDef:
    return {
        "HealthStatus": ...,
    }


# LicenseServerTypeDef definition

class LicenseServerTypeDef(TypedDict):
    HealthStatus: NotRequired[LicenseServerHealthStatusType],  # (1)
    Ipv4Address: NotRequired[str],
    ProvisioningStatus: NotRequired[LicenseServerEndpointProvisioningStatusType],  # (2)
```

1. See [:material-code-brackets: LicenseServerHealthStatusType](./literals.md#licenseserverhealthstatustype) 
2. See [:material-code-brackets: LicenseServerEndpointProvisioningStatusType](./literals.md#licenseserverendpointprovisioningstatustype) 
## ServerEndpointTypeDef

```python
# ServerEndpointTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ServerEndpointTypeDef


def get_value() -> ServerEndpointTypeDef:
    return {
        "Endpoint": ...,
    }


# ServerEndpointTypeDef definition

class ServerEndpointTypeDef(TypedDict):
    Endpoint: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import PaginatorConfigTypeDef


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

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## SettingsTypeDef

```python
# SettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import SettingsTypeDef


def get_value() -> SettingsTypeDef:
    return {
        "SecurityGroupId": ...,
    }


# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
    SecurityGroupId: str,
    Subnets: Sequence[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateSettingsTypeDef

```python
# UpdateSettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import UpdateSettingsTypeDef


def get_value() -> UpdateSettingsTypeDef:
    return {
        "AddSubnets": ...,
    }


# UpdateSettingsTypeDef definition

class UpdateSettingsTypeDef(TypedDict):
    AddSubnets: Sequence[str],
    RemoveSubnets: Sequence[str],
    SecurityGroupId: NotRequired[str],
```

## CreateLicenseServerEndpointResponseTypeDef

```python
# CreateLicenseServerEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import CreateLicenseServerEndpointResponseTypeDef


def get_value() -> CreateLicenseServerEndpointResponseTypeDef:
    return {
        "IdentityProviderArn": ...,
    }


# CreateLicenseServerEndpointResponseTypeDef definition

class CreateLicenseServerEndpointResponseTypeDef(TypedDict):
    IdentityProviderArn: str,
    LicenseServerEndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CredentialsProviderTypeDef

```python
# CredentialsProviderTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import CredentialsProviderTypeDef


def get_value() -> CredentialsProviderTypeDef:
    return {
        "SecretsManagerCredentialsProvider": ...,
    }


# CredentialsProviderTypeDef definition

class CredentialsProviderTypeDef(TypedDict):
    SecretsManagerCredentialsProvider: NotRequired[SecretsManagerCredentialsProviderTypeDef],  # (1)
```

1. See [:material-code-braces: SecretsManagerCredentialsProviderTypeDef](./type_defs.md#secretsmanagercredentialsprovidertypedef) 
## ListIdentityProvidersRequestTypeDef

```python
# ListIdentityProvidersRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListIdentityProvidersRequestTypeDef


def get_value() -> ListIdentityProvidersRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListIdentityProvidersRequestTypeDef definition

class ListIdentityProvidersRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListInstancesRequestTypeDef

```python
# ListInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListInstancesRequestTypeDef


def get_value() -> ListInstancesRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListInstancesRequestTypeDef definition

class ListInstancesRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicenseServerEndpointsRequestTypeDef

```python
# ListLicenseServerEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListLicenseServerEndpointsRequestTypeDef


def get_value() -> ListLicenseServerEndpointsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListLicenseServerEndpointsRequestTypeDef definition

class ListLicenseServerEndpointsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListInstancesResponseTypeDef


def get_value() -> ListInstancesResponseTypeDef:
    return {
        "InstanceSummaries": ...,
    }


# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    InstanceSummaries: List[InstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LicenseServerEndpointTypeDef

```python
# LicenseServerEndpointTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import LicenseServerEndpointTypeDef


def get_value() -> LicenseServerEndpointTypeDef:
    return {
        "CreationTime": ...,
    }


# LicenseServerEndpointTypeDef definition

class LicenseServerEndpointTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    IdentityProviderArn: NotRequired[str],
    LicenseServerEndpointArn: NotRequired[str],
    LicenseServerEndpointId: NotRequired[str],
    LicenseServerEndpointProvisioningStatus: NotRequired[LicenseServerEndpointProvisioningStatusType],  # (1)
    LicenseServers: NotRequired[List[LicenseServerTypeDef]],  # (2)
    ServerEndpoint: NotRequired[ServerEndpointTypeDef],  # (3)
    ServerType: NotRequired[ServerTypeType],  # (4)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: LicenseServerEndpointProvisioningStatusType](./literals.md#licenseserverendpointprovisioningstatustype) 
2. See [:material-code-braces: LicenseServerTypeDef](./type_defs.md#licenseservertypedef) 
3. See [:material-code-braces: ServerEndpointTypeDef](./type_defs.md#serverendpointtypedef) 
4. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
## ListIdentityProvidersRequestPaginateTypeDef

```python
# ListIdentityProvidersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListIdentityProvidersRequestPaginateTypeDef


def get_value() -> ListIdentityProvidersRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListIdentityProvidersRequestPaginateTypeDef definition

class ListIdentityProvidersRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListInstancesRequestPaginateTypeDef


def get_value() -> ListInstancesRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseServerEndpointsRequestPaginateTypeDef

```python
# ListLicenseServerEndpointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListLicenseServerEndpointsRequestPaginateTypeDef


def get_value() -> ListLicenseServerEndpointsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListLicenseServerEndpointsRequestPaginateTypeDef definition

class ListLicenseServerEndpointsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ActiveDirectorySettingsOutputTypeDef

```python
# ActiveDirectorySettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectorySettingsOutputTypeDef


def get_value() -> ActiveDirectorySettingsOutputTypeDef:
    return {
        "DomainCredentialsProvider": ...,
    }


# ActiveDirectorySettingsOutputTypeDef definition

class ActiveDirectorySettingsOutputTypeDef(TypedDict):
    DomainCredentialsProvider: NotRequired[CredentialsProviderTypeDef],  # (1)
    DomainIpv4List: NotRequired[List[str]],
    DomainName: NotRequired[str],
    DomainNetworkSettings: NotRequired[DomainNetworkSettingsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef) 
2. See [:material-code-braces: DomainNetworkSettingsOutputTypeDef](./type_defs.md#domainnetworksettingsoutputtypedef) 
## ActiveDirectorySettingsTypeDef

```python
# ActiveDirectorySettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectorySettingsTypeDef


def get_value() -> ActiveDirectorySettingsTypeDef:
    return {
        "DomainCredentialsProvider": ...,
    }


# ActiveDirectorySettingsTypeDef definition

class ActiveDirectorySettingsTypeDef(TypedDict):
    DomainCredentialsProvider: NotRequired[CredentialsProviderTypeDef],  # (1)
    DomainIpv4List: NotRequired[Sequence[str]],
    DomainName: NotRequired[str],
    DomainNetworkSettings: NotRequired[DomainNetworkSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef) 
2. See [:material-code-braces: DomainNetworkSettingsTypeDef](./type_defs.md#domainnetworksettingstypedef) 
## RdsSalSettingsTypeDef

```python
# RdsSalSettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import RdsSalSettingsTypeDef


def get_value() -> RdsSalSettingsTypeDef:
    return {
        "RdsSalCredentialsProvider": ...,
    }


# RdsSalSettingsTypeDef definition

class RdsSalSettingsTypeDef(TypedDict):
    RdsSalCredentialsProvider: CredentialsProviderTypeDef,  # (1)
```

1. See [:material-code-braces: CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef) 
## DeleteLicenseServerEndpointResponseTypeDef

```python
# DeleteLicenseServerEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DeleteLicenseServerEndpointResponseTypeDef


def get_value() -> DeleteLicenseServerEndpointResponseTypeDef:
    return {
        "LicenseServerEndpoint": ...,
    }


# DeleteLicenseServerEndpointResponseTypeDef definition

class DeleteLicenseServerEndpointResponseTypeDef(TypedDict):
    LicenseServerEndpoint: LicenseServerEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LicenseServerEndpointTypeDef](./type_defs.md#licenseserverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseServerEndpointsResponseTypeDef

```python
# ListLicenseServerEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListLicenseServerEndpointsResponseTypeDef


def get_value() -> ListLicenseServerEndpointsResponseTypeDef:
    return {
        "LicenseServerEndpoints": ...,
    }


# ListLicenseServerEndpointsResponseTypeDef definition

class ListLicenseServerEndpointsResponseTypeDef(TypedDict):
    LicenseServerEndpoints: List[LicenseServerEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseServerEndpointTypeDef](./type_defs.md#licenseserverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActiveDirectoryIdentityProviderOutputTypeDef

```python
# ActiveDirectoryIdentityProviderOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderOutputTypeDef


def get_value() -> ActiveDirectoryIdentityProviderOutputTypeDef:
    return {
        "ActiveDirectorySettings": ...,
    }


# ActiveDirectoryIdentityProviderOutputTypeDef definition

class ActiveDirectoryIdentityProviderOutputTypeDef(TypedDict):
    ActiveDirectorySettings: NotRequired[ActiveDirectorySettingsOutputTypeDef],  # (1)
    ActiveDirectoryType: NotRequired[ActiveDirectoryTypeType],  # (2)
    DirectoryId: NotRequired[str],
```

1. See [:material-code-braces: ActiveDirectorySettingsOutputTypeDef](./type_defs.md#activedirectorysettingsoutputtypedef) 
2. See [:material-code-brackets: ActiveDirectoryTypeType](./literals.md#activedirectorytypetype) 
## ActiveDirectoryIdentityProviderTypeDef

```python
# ActiveDirectoryIdentityProviderTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef


def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
    return {
        "ActiveDirectorySettings": ...,
    }


# ActiveDirectoryIdentityProviderTypeDef definition

class ActiveDirectoryIdentityProviderTypeDef(TypedDict):
    ActiveDirectorySettings: NotRequired[ActiveDirectorySettingsTypeDef],  # (1)
    ActiveDirectoryType: NotRequired[ActiveDirectoryTypeType],  # (2)
    DirectoryId: NotRequired[str],
```

1. See [:material-code-braces: ActiveDirectorySettingsTypeDef](./type_defs.md#activedirectorysettingstypedef) 
2. See [:material-code-brackets: ActiveDirectoryTypeType](./literals.md#activedirectorytypetype) 
## ServerSettingsTypeDef

```python
# ServerSettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ServerSettingsTypeDef


def get_value() -> ServerSettingsTypeDef:
    return {
        "RdsSalSettings": ...,
    }


# ServerSettingsTypeDef definition

class ServerSettingsTypeDef(TypedDict):
    RdsSalSettings: NotRequired[RdsSalSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: RdsSalSettingsTypeDef](./type_defs.md#rdssalsettingstypedef) 
## IdentityProviderOutputTypeDef

```python
# IdentityProviderOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import IdentityProviderOutputTypeDef


def get_value() -> IdentityProviderOutputTypeDef:
    return {
        "ActiveDirectoryIdentityProvider": ...,
    }


# IdentityProviderOutputTypeDef definition

class IdentityProviderOutputTypeDef(TypedDict):
    ActiveDirectoryIdentityProvider: NotRequired[ActiveDirectoryIdentityProviderOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef) 
## IdentityProviderTypeDef

```python
# IdentityProviderTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import IdentityProviderTypeDef


def get_value() -> IdentityProviderTypeDef:
    return {
        "ActiveDirectoryIdentityProvider": ...,
    }


# IdentityProviderTypeDef definition

class IdentityProviderTypeDef(TypedDict):
    ActiveDirectoryIdentityProvider: NotRequired[ActiveDirectoryIdentityProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef) 
## LicenseServerSettingsTypeDef

```python
# LicenseServerSettingsTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import LicenseServerSettingsTypeDef


def get_value() -> LicenseServerSettingsTypeDef:
    return {
        "ServerSettings": ...,
    }


# LicenseServerSettingsTypeDef definition

class LicenseServerSettingsTypeDef(TypedDict):
    ServerSettings: ServerSettingsTypeDef,  # (1)
    ServerType: ServerTypeType,  # (2)
```

1. See [:material-code-braces: ServerSettingsTypeDef](./type_defs.md#serversettingstypedef) 
2. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
## IdentityProviderSummaryTypeDef

```python
# IdentityProviderSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import IdentityProviderSummaryTypeDef


def get_value() -> IdentityProviderSummaryTypeDef:
    return {
        "FailureMessage": ...,
    }


# IdentityProviderSummaryTypeDef definition

class IdentityProviderSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderOutputTypeDef,  # (1)
    Product: str,
    Settings: SettingsOutputTypeDef,  # (2)
    Status: str,
    FailureMessage: NotRequired[str],
    IdentityProviderArn: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: SettingsOutputTypeDef](./type_defs.md#settingsoutputtypedef) 
## InstanceUserSummaryTypeDef

```python
# InstanceUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import InstanceUserSummaryTypeDef


def get_value() -> InstanceUserSummaryTypeDef:
    return {
        "AssociationDate": ...,
    }


# InstanceUserSummaryTypeDef definition

class InstanceUserSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderOutputTypeDef,  # (1)
    InstanceId: str,
    Status: str,
    Username: str,
    AssociationDate: NotRequired[str],
    DisassociationDate: NotRequired[str],
    Domain: NotRequired[str],
    InstanceUserArn: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## ProductUserSummaryTypeDef

```python
# ProductUserSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ProductUserSummaryTypeDef


def get_value() -> ProductUserSummaryTypeDef:
    return {
        "Domain": ...,
    }


# ProductUserSummaryTypeDef definition

class ProductUserSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderOutputTypeDef,  # (1)
    Product: str,
    Status: str,
    Username: str,
    Domain: NotRequired[str],
    ProductUserArn: NotRequired[str],
    StatusMessage: NotRequired[str],
    SubscriptionEndDate: NotRequired[str],
    SubscriptionStartDate: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## CreateLicenseServerEndpointRequestTypeDef

```python
# CreateLicenseServerEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import CreateLicenseServerEndpointRequestTypeDef


def get_value() -> CreateLicenseServerEndpointRequestTypeDef:
    return {
        "IdentityProviderArn": ...,
    }


# CreateLicenseServerEndpointRequestTypeDef definition

class CreateLicenseServerEndpointRequestTypeDef(TypedDict):
    IdentityProviderArn: str,
    LicenseServerSettings: LicenseServerSettingsTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LicenseServerSettingsTypeDef](./type_defs.md#licenseserversettingstypedef) 
## DeregisterIdentityProviderResponseTypeDef

```python
# DeregisterIdentityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DeregisterIdentityProviderResponseTypeDef


def get_value() -> DeregisterIdentityProviderResponseTypeDef:
    return {
        "IdentityProviderSummary": ...,
    }


# DeregisterIdentityProviderResponseTypeDef definition

class DeregisterIdentityProviderResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityProvidersResponseTypeDef

```python
# ListIdentityProvidersResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListIdentityProvidersResponseTypeDef


def get_value() -> ListIdentityProvidersResponseTypeDef:
    return {
        "IdentityProviderSummaries": ...,
    }


# ListIdentityProvidersResponseTypeDef definition

class ListIdentityProvidersResponseTypeDef(TypedDict):
    IdentityProviderSummaries: List[IdentityProviderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterIdentityProviderResponseTypeDef

```python
# RegisterIdentityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import RegisterIdentityProviderResponseTypeDef


def get_value() -> RegisterIdentityProviderResponseTypeDef:
    return {
        "IdentityProviderSummary": ...,
    }


# RegisterIdentityProviderResponseTypeDef definition

class RegisterIdentityProviderResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentityProviderSettingsResponseTypeDef

```python
# UpdateIdentityProviderSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import UpdateIdentityProviderSettingsResponseTypeDef


def get_value() -> UpdateIdentityProviderSettingsResponseTypeDef:
    return {
        "IdentityProviderSummary": ...,
    }


# UpdateIdentityProviderSettingsResponseTypeDef definition

class UpdateIdentityProviderSettingsResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserResponseTypeDef

```python
# AssociateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserResponseTypeDef


def get_value() -> AssociateUserResponseTypeDef:
    return {
        "InstanceUserSummary": ...,
    }


# AssociateUserResponseTypeDef definition

class AssociateUserResponseTypeDef(TypedDict):
    InstanceUserSummary: InstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateUserResponseTypeDef

```python
# DisassociateUserResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DisassociateUserResponseTypeDef


def get_value() -> DisassociateUserResponseTypeDef:
    return {
        "InstanceUserSummary": ...,
    }


# DisassociateUserResponseTypeDef definition

class DisassociateUserResponseTypeDef(TypedDict):
    InstanceUserSummary: InstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserAssociationsResponseTypeDef

```python
# ListUserAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListUserAssociationsResponseTypeDef


def get_value() -> ListUserAssociationsResponseTypeDef:
    return {
        "InstanceUserSummaries": ...,
    }


# ListUserAssociationsResponseTypeDef definition

class ListUserAssociationsResponseTypeDef(TypedDict):
    InstanceUserSummaries: List[InstanceUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProductSubscriptionsResponseTypeDef

```python
# ListProductSubscriptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListProductSubscriptionsResponseTypeDef


def get_value() -> ListProductSubscriptionsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListProductSubscriptionsResponseTypeDef definition

class ListProductSubscriptionsResponseTypeDef(TypedDict):
    ProductUserSummaries: List[ProductUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProductSubscriptionResponseTypeDef

```python
# StartProductSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import StartProductSubscriptionResponseTypeDef


def get_value() -> StartProductSubscriptionResponseTypeDef:
    return {
        "ProductUserSummary": ...,
    }


# StartProductSubscriptionResponseTypeDef definition

class StartProductSubscriptionResponseTypeDef(TypedDict):
    ProductUserSummary: ProductUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopProductSubscriptionResponseTypeDef

```python
# StopProductSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import StopProductSubscriptionResponseTypeDef


def get_value() -> StopProductSubscriptionResponseTypeDef:
    return {
        "ProductUserSummary": ...,
    }


# StopProductSubscriptionResponseTypeDef definition

class StopProductSubscriptionResponseTypeDef(TypedDict):
    ProductUserSummary: ProductUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserRequestTypeDef

```python
# AssociateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserRequestTypeDef


def get_value() -> AssociateUserRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# AssociateUserRequestTypeDef definition

class AssociateUserRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    InstanceId: str,
    Username: str,
    Domain: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## DeregisterIdentityProviderRequestTypeDef

```python
# DeregisterIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DeregisterIdentityProviderRequestTypeDef


def get_value() -> DeregisterIdentityProviderRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# DeregisterIdentityProviderRequestTypeDef definition

class DeregisterIdentityProviderRequestTypeDef(TypedDict):
    IdentityProvider: NotRequired[IdentityProviderUnionTypeDef],  # (1)
    IdentityProviderArn: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## DisassociateUserRequestTypeDef

```python
# DisassociateUserRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import DisassociateUserRequestTypeDef


def get_value() -> DisassociateUserRequestTypeDef:
    return {
        "Domain": ...,
    }


# DisassociateUserRequestTypeDef definition

class DisassociateUserRequestTypeDef(TypedDict):
    Domain: NotRequired[str],
    IdentityProvider: NotRequired[IdentityProviderUnionTypeDef],  # (1)
    InstanceId: NotRequired[str],
    InstanceUserArn: NotRequired[str],
    Username: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## ListProductSubscriptionsRequestPaginateTypeDef

```python
# ListProductSubscriptionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListProductSubscriptionsRequestPaginateTypeDef


def get_value() -> ListProductSubscriptionsRequestPaginateTypeDef:
    return {
        "IdentityProvider": ...,
    }


# ListProductSubscriptionsRequestPaginateTypeDef definition

class ListProductSubscriptionsRequestPaginateTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    Product: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProductSubscriptionsRequestTypeDef

```python
# ListProductSubscriptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListProductSubscriptionsRequestTypeDef


def get_value() -> ListProductSubscriptionsRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# ListProductSubscriptionsRequestTypeDef definition

class ListProductSubscriptionsRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListUserAssociationsRequestPaginateTypeDef

```python
# ListUserAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListUserAssociationsRequestPaginateTypeDef


def get_value() -> ListUserAssociationsRequestPaginateTypeDef:
    return {
        "IdentityProvider": ...,
    }


# ListUserAssociationsRequestPaginateTypeDef definition

class ListUserAssociationsRequestPaginateTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    InstanceId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserAssociationsRequestTypeDef

```python
# ListUserAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListUserAssociationsRequestTypeDef


def get_value() -> ListUserAssociationsRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# ListUserAssociationsRequestTypeDef definition

class ListUserAssociationsRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    InstanceId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## RegisterIdentityProviderRequestTypeDef

```python
# RegisterIdentityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import RegisterIdentityProviderRequestTypeDef


def get_value() -> RegisterIdentityProviderRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# RegisterIdentityProviderRequestTypeDef definition

class RegisterIdentityProviderRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    Product: str,
    Settings: NotRequired[SettingsUnionTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) [:material-code-braces: SettingsOutputTypeDef](./type_defs.md#settingsoutputtypedef) 
## StartProductSubscriptionRequestTypeDef

```python
# StartProductSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import StartProductSubscriptionRequestTypeDef


def get_value() -> StartProductSubscriptionRequestTypeDef:
    return {
        "IdentityProvider": ...,
    }


# StartProductSubscriptionRequestTypeDef definition

class StartProductSubscriptionRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderUnionTypeDef,  # (1)
    Product: str,
    Username: str,
    Domain: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## StopProductSubscriptionRequestTypeDef

```python
# StopProductSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import StopProductSubscriptionRequestTypeDef


def get_value() -> StopProductSubscriptionRequestTypeDef:
    return {
        "Domain": ...,
    }


# StopProductSubscriptionRequestTypeDef definition

class StopProductSubscriptionRequestTypeDef(TypedDict):
    Domain: NotRequired[str],
    IdentityProvider: NotRequired[IdentityProviderUnionTypeDef],  # (1)
    Product: NotRequired[str],
    ProductUserArn: NotRequired[str],
    Username: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
## UpdateIdentityProviderSettingsRequestTypeDef

```python
# UpdateIdentityProviderSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager_user_subscriptions.type_defs import UpdateIdentityProviderSettingsRequestTypeDef


def get_value() -> UpdateIdentityProviderSettingsRequestTypeDef:
    return {
        "UpdateSettings": ...,
    }


# UpdateIdentityProviderSettingsRequestTypeDef definition

class UpdateIdentityProviderSettingsRequestTypeDef(TypedDict):
    UpdateSettings: UpdateSettingsTypeDef,  # (1)
    IdentityProvider: NotRequired[IdentityProviderUnionTypeDef],  # (2)
    IdentityProviderArn: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef) 
2. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) [:material-code-braces: IdentityProviderOutputTypeDef](./type_defs.md#identityprovideroutputtypedef) 
