# Type definitions

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## ActiveDirectoryIdentityProviderUnionTypeDef

```python
# ActiveDirectoryIdentityProviderUnionTypeDef definition

ActiveDirectoryIdentityProviderUnionTypeDef = Union[
    ActiveDirectoryIdentityProviderTypeDef,  # (1)
    ActiveDirectoryIdentityProviderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef) 
2. See [:material-code-braces: ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef) 



## DomainNetworkSettingsOutputTypeDef

```python
# DomainNetworkSettingsOutputTypeDef definition

class DomainNetworkSettingsOutputTypeDef(TypedDict):
    Subnets: List[str],
```

## DomainNetworkSettingsTypeDef

```python
# DomainNetworkSettingsTypeDef definition

class DomainNetworkSettingsTypeDef(TypedDict):
    Subnets: Sequence[str],
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

## SecretsManagerCredentialsProviderTypeDef

```python
# SecretsManagerCredentialsProviderTypeDef definition

class SecretsManagerCredentialsProviderTypeDef(TypedDict):
    SecretId: NotRequired[str],
```

## DeleteLicenseServerEndpointRequestRequestTypeDef

```python
# DeleteLicenseServerEndpointRequestRequestTypeDef definition

class DeleteLicenseServerEndpointRequestRequestTypeDef(TypedDict):
    LicenseServerEndpointArn: str,
    ServerType: ServerTypeType,  # (1)
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Attribute: NotRequired[str],
    Operation: NotRequired[str],
    Value: NotRequired[str],
```

## SettingsOutputTypeDef

```python
# SettingsOutputTypeDef definition

class SettingsOutputTypeDef(TypedDict):
    SecurityGroupId: str,
    Subnets: List[str],
```

## InstanceSummaryTypeDef

```python
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
# ServerEndpointTypeDef definition

class ServerEndpointTypeDef(TypedDict):
    Endpoint: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## SettingsTypeDef

```python
# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
    SecurityGroupId: str,
    Subnets: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateSettingsTypeDef

```python
# UpdateSettingsTypeDef definition

class UpdateSettingsTypeDef(TypedDict):
    AddSubnets: Sequence[str],
    RemoveSubnets: Sequence[str],
    SecurityGroupId: NotRequired[str],
```

## CreateLicenseServerEndpointResponseTypeDef

```python
# CreateLicenseServerEndpointResponseTypeDef definition

class CreateLicenseServerEndpointResponseTypeDef(TypedDict):
    IdentityProviderArn: str,
    LicenseServerEndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CredentialsProviderTypeDef

```python
# CredentialsProviderTypeDef definition

class CredentialsProviderTypeDef(TypedDict):
    SecretsManagerCredentialsProvider: NotRequired[SecretsManagerCredentialsProviderTypeDef],  # (1)
```

1. See [:material-code-braces: SecretsManagerCredentialsProviderTypeDef](./type_defs.md#secretsmanagercredentialsprovidertypedef) 
## ListIdentityProvidersRequestRequestTypeDef

```python
# ListIdentityProvidersRequestRequestTypeDef definition

class ListIdentityProvidersRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicenseServerEndpointsRequestRequestTypeDef

```python
# ListLicenseServerEndpointsRequestRequestTypeDef definition

class ListLicenseServerEndpointsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListInstancesResponseTypeDef

```python
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
# ListIdentityProvidersRequestPaginateTypeDef definition

class ListIdentityProvidersRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseServerEndpointsRequestPaginateTypeDef

```python
# ListLicenseServerEndpointsRequestPaginateTypeDef definition

class ListLicenseServerEndpointsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ActiveDirectorySettingsOutputTypeDef

```python
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
# RdsSalSettingsTypeDef definition

class RdsSalSettingsTypeDef(TypedDict):
    RdsSalCredentialsProvider: CredentialsProviderTypeDef,  # (1)
```

1. See [:material-code-braces: CredentialsProviderTypeDef](./type_defs.md#credentialsprovidertypedef) 
## DeleteLicenseServerEndpointResponseTypeDef

```python
# DeleteLicenseServerEndpointResponseTypeDef definition

class DeleteLicenseServerEndpointResponseTypeDef(TypedDict):
    LicenseServerEndpoint: LicenseServerEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LicenseServerEndpointTypeDef](./type_defs.md#licenseserverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseServerEndpointsResponseTypeDef

```python
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
# ServerSettingsTypeDef definition

class ServerSettingsTypeDef(TypedDict):
    RdsSalSettings: NotRequired[RdsSalSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: RdsSalSettingsTypeDef](./type_defs.md#rdssalsettingstypedef) 
## IdentityProviderOutputTypeDef

```python
# IdentityProviderOutputTypeDef definition

class IdentityProviderOutputTypeDef(TypedDict):
    ActiveDirectoryIdentityProvider: NotRequired[ActiveDirectoryIdentityProviderOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef) 
## LicenseServerSettingsTypeDef

```python
# LicenseServerSettingsTypeDef definition

class LicenseServerSettingsTypeDef(TypedDict):
    ServerSettings: ServerSettingsTypeDef,  # (1)
    ServerType: ServerTypeType,  # (2)
```

1. See [:material-code-braces: ServerSettingsTypeDef](./type_defs.md#serversettingstypedef) 
2. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
## IdentityProviderSummaryTypeDef

```python
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
## IdentityProviderTypeDef

```python
# IdentityProviderTypeDef definition

class IdentityProviderTypeDef(TypedDict):
    ActiveDirectoryIdentityProvider: NotRequired[ActiveDirectoryIdentityProviderUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef) [:material-code-braces: ActiveDirectoryIdentityProviderOutputTypeDef](./type_defs.md#activedirectoryidentityprovideroutputtypedef) 
## CreateLicenseServerEndpointRequestRequestTypeDef

```python
# CreateLicenseServerEndpointRequestRequestTypeDef definition

class CreateLicenseServerEndpointRequestRequestTypeDef(TypedDict):
    IdentityProviderArn: str,
    LicenseServerSettings: LicenseServerSettingsTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LicenseServerSettingsTypeDef](./type_defs.md#licenseserversettingstypedef) 
## DeregisterIdentityProviderResponseTypeDef

```python
# DeregisterIdentityProviderResponseTypeDef definition

class DeregisterIdentityProviderResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityProvidersResponseTypeDef

```python
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
# RegisterIdentityProviderResponseTypeDef definition

class RegisterIdentityProviderResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdentityProviderSettingsResponseTypeDef

```python
# UpdateIdentityProviderSettingsResponseTypeDef definition

class UpdateIdentityProviderSettingsResponseTypeDef(TypedDict):
    IdentityProviderSummary: IdentityProviderSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderSummaryTypeDef](./type_defs.md#identityprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserResponseTypeDef

```python
# AssociateUserResponseTypeDef definition

class AssociateUserResponseTypeDef(TypedDict):
    InstanceUserSummary: InstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateUserResponseTypeDef

```python
# DisassociateUserResponseTypeDef definition

class DisassociateUserResponseTypeDef(TypedDict):
    InstanceUserSummary: InstanceUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserAssociationsResponseTypeDef

```python
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
# StartProductSubscriptionResponseTypeDef definition

class StartProductSubscriptionResponseTypeDef(TypedDict):
    ProductUserSummary: ProductUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopProductSubscriptionResponseTypeDef

```python
# StopProductSubscriptionResponseTypeDef definition

class StopProductSubscriptionResponseTypeDef(TypedDict):
    ProductUserSummary: ProductUserSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductUserSummaryTypeDef](./type_defs.md#productusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateUserRequestRequestTypeDef

```python
# AssociateUserRequestRequestTypeDef definition

class AssociateUserRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Username: str,
    Domain: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## DeregisterIdentityProviderRequestRequestTypeDef

```python
# DeregisterIdentityProviderRequestRequestTypeDef definition

class DeregisterIdentityProviderRequestRequestTypeDef(TypedDict):
    IdentityProvider: NotRequired[IdentityProviderTypeDef],  # (1)
    IdentityProviderArn: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## DisassociateUserRequestRequestTypeDef

```python
# DisassociateUserRequestRequestTypeDef definition

class DisassociateUserRequestRequestTypeDef(TypedDict):
    Domain: NotRequired[str],
    IdentityProvider: NotRequired[IdentityProviderTypeDef],  # (1)
    InstanceId: NotRequired[str],
    InstanceUserArn: NotRequired[str],
    Username: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## ListProductSubscriptionsRequestPaginateTypeDef

```python
# ListProductSubscriptionsRequestPaginateTypeDef definition

class ListProductSubscriptionsRequestPaginateTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    Product: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProductSubscriptionsRequestRequestTypeDef

```python
# ListProductSubscriptionsRequestRequestTypeDef definition

class ListProductSubscriptionsRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListUserAssociationsRequestPaginateTypeDef

```python
# ListUserAssociationsRequestPaginateTypeDef definition

class ListUserAssociationsRequestPaginateTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserAssociationsRequestRequestTypeDef

```python
# ListUserAssociationsRequestRequestTypeDef definition

class ListUserAssociationsRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## RegisterIdentityProviderRequestRequestTypeDef

```python
# RegisterIdentityProviderRequestRequestTypeDef definition

class RegisterIdentityProviderRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Settings: NotRequired[SettingsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
## StartProductSubscriptionRequestRequestTypeDef

```python
# StartProductSubscriptionRequestRequestTypeDef definition

class StartProductSubscriptionRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Username: str,
    Domain: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## StopProductSubscriptionRequestRequestTypeDef

```python
# StopProductSubscriptionRequestRequestTypeDef definition

class StopProductSubscriptionRequestRequestTypeDef(TypedDict):
    Domain: NotRequired[str],
    IdentityProvider: NotRequired[IdentityProviderTypeDef],  # (1)
    Product: NotRequired[str],
    ProductUserArn: NotRequired[str],
    Username: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## UpdateIdentityProviderSettingsRequestRequestTypeDef

```python
# UpdateIdentityProviderSettingsRequestRequestTypeDef definition

class UpdateIdentityProviderSettingsRequestRequestTypeDef(TypedDict):
    UpdateSettings: UpdateSettingsTypeDef,  # (1)
    IdentityProvider: NotRequired[IdentityProviderTypeDef],  # (2)
    IdentityProviderArn: NotRequired[str],
    Product: NotRequired[str],
```

1. See [:material-code-braces: UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef) 
2. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
