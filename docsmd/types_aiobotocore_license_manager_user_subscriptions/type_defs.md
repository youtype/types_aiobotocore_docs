# Type definitions

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).



## ActiveDirectoryIdentityProviderTypeDef

```python
# ActiveDirectoryIdentityProviderTypeDef definition

class ActiveDirectoryIdentityProviderTypeDef(TypedDict):
    DirectoryId: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Attribute: NotRequired[str],
    Operation: NotRequired[str],
    Value: NotRequired[str],
```

## SettingsTypeDef

```python
# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIdentityProvidersRequestRequestTypeDef

```python
# ListIdentityProvidersRequestRequestTypeDef definition

class ListIdentityProvidersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## UpdateSettingsTypeDef

```python
# UpdateSettingsTypeDef definition

class UpdateSettingsTypeDef(TypedDict):
    AddSubnets: Sequence[str],
    RemoveSubnets: Sequence[str],
    SecurityGroupId: NotRequired[str],
```

## IdentityProviderTypeDef

```python
# IdentityProviderTypeDef definition

class IdentityProviderTypeDef(TypedDict):
    ActiveDirectoryIdentityProvider: NotRequired[ActiveDirectoryIdentityProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ActiveDirectoryIdentityProviderTypeDef](./type_defs.md#activedirectoryidentityprovidertypedef) 
## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef

```python
# ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef definition

class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestListInstancesPaginateTypeDef

```python
# ListInstancesRequestListInstancesPaginateTypeDef definition

class ListInstancesRequestListInstancesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## AssociateUserRequestRequestTypeDef

```python
# AssociateUserRequestRequestTypeDef definition

class AssociateUserRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Username: str,
    Domain: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## DeregisterIdentityProviderRequestRequestTypeDef

```python
# DeregisterIdentityProviderRequestRequestTypeDef definition

class DeregisterIdentityProviderRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## DisassociateUserRequestRequestTypeDef

```python
# DisassociateUserRequestRequestTypeDef definition

class DisassociateUserRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Username: str,
    Domain: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## IdentityProviderSummaryTypeDef

```python
# IdentityProviderSummaryTypeDef definition

class IdentityProviderSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Settings: SettingsTypeDef,  # (2)
    Status: str,
    FailureMessage: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
## InstanceUserSummaryTypeDef

```python
# InstanceUserSummaryTypeDef definition

class InstanceUserSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Status: str,
    Username: str,
    AssociationDate: NotRequired[str],
    DisassociationDate: NotRequired[str],
    Domain: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef

```python
# ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef definition

class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
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
    Product: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListUserAssociationsRequestListUserAssociationsPaginateTypeDef

```python
# ListUserAssociationsRequestListUserAssociationsPaginateTypeDef definition

class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(TypedDict):
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
## ProductUserSummaryTypeDef

```python
# ProductUserSummaryTypeDef definition

class ProductUserSummaryTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Status: str,
    Username: str,
    Domain: NotRequired[str],
    StatusMessage: NotRequired[str],
    SubscriptionEndDate: NotRequired[str],
    SubscriptionStartDate: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## RegisterIdentityProviderRequestRequestTypeDef

```python
# RegisterIdentityProviderRequestRequestTypeDef definition

class RegisterIdentityProviderRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Settings: NotRequired[SettingsTypeDef],  # (2)
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
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## StopProductSubscriptionRequestRequestTypeDef

```python
# StopProductSubscriptionRequestRequestTypeDef definition

class StopProductSubscriptionRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Username: str,
    Domain: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
## UpdateIdentityProviderSettingsRequestRequestTypeDef

```python
# UpdateIdentityProviderSettingsRequestRequestTypeDef definition

class UpdateIdentityProviderSettingsRequestRequestTypeDef(TypedDict):
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    UpdateSettings: UpdateSettingsTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef) 
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceUserSummaryTypeDef](./type_defs.md#instanceusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProductSubscriptionsResponseTypeDef

```python
# ListProductSubscriptionsResponseTypeDef definition

class ListProductSubscriptionsResponseTypeDef(TypedDict):
    NextToken: str,
    ProductUserSummaries: List[ProductUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
