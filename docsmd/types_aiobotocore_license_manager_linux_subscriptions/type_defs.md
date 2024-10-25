# Type definitions

> [Index](../README.md) > [LicenseManagerLinuxSubscriptions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).



## DeregisterSubscriptionProviderRequestRequestTypeDef

```python
# DeregisterSubscriptionProviderRequestRequestTypeDef definition

class DeregisterSubscriptionProviderRequestRequestTypeDef(TypedDict):
    SubscriptionProviderArn: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Operator: NotRequired[OperatorType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## GetRegisteredSubscriptionProviderRequestRequestTypeDef

```python
# GetRegisteredSubscriptionProviderRequestRequestTypeDef definition

class GetRegisteredSubscriptionProviderRequestRequestTypeDef(TypedDict):
    SubscriptionProviderArn: str,
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

## LinuxSubscriptionsDiscoverySettingsOutputTypeDef

```python
# LinuxSubscriptionsDiscoverySettingsOutputTypeDef definition

class LinuxSubscriptionsDiscoverySettingsOutputTypeDef(TypedDict):
    OrganizationIntegration: OrganizationIntegrationType,  # (1)
    SourceRegions: List[str],
```

1. See [:material-code-brackets: OrganizationIntegrationType](./literals.md#organizationintegrationtype) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    AccountID: NotRequired[str],
    AmiId: NotRequired[str],
    DualSubscription: NotRequired[str],
    InstanceID: NotRequired[str],
    InstanceType: NotRequired[str],
    LastUpdatedTime: NotRequired[str],
    OsVersion: NotRequired[str],
    ProductCode: NotRequired[List[str]],
    Region: NotRequired[str],
    RegisteredWithSubscriptionProvider: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionName: NotRequired[str],
    SubscriptionProviderCreateTime: NotRequired[str],
    SubscriptionProviderUpdateTime: NotRequired[str],
    UsageOperation: NotRequired[str],
```

## LinuxSubscriptionsDiscoverySettingsTypeDef

```python
# LinuxSubscriptionsDiscoverySettingsTypeDef definition

class LinuxSubscriptionsDiscoverySettingsTypeDef(TypedDict):
    OrganizationIntegration: OrganizationIntegrationType,  # (1)
    SourceRegions: Sequence[str],
```

1. See [:material-code-brackets: OrganizationIntegrationType](./literals.md#organizationintegrationtype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    InstanceCount: NotRequired[int],
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## ListRegisteredSubscriptionProvidersRequestRequestTypeDef

```python
# ListRegisteredSubscriptionProvidersRequestRequestTypeDef definition

class ListRegisteredSubscriptionProvidersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SubscriptionProviderSources: NotRequired[Sequence[SubscriptionProviderSourceType]],  # (1)
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
## RegisteredSubscriptionProviderTypeDef

```python
# RegisteredSubscriptionProviderTypeDef definition

class RegisteredSubscriptionProviderTypeDef(TypedDict):
    LastSuccessfulDataRetrievalTime: NotRequired[str],
    SecretArn: NotRequired[str],
    SubscriptionProviderArn: NotRequired[str],
    SubscriptionProviderSource: NotRequired[SubscriptionProviderSourceType],  # (1)
    SubscriptionProviderStatus: NotRequired[SubscriptionProviderStatusType],  # (2)
    SubscriptionProviderStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
2. See [:material-code-brackets: SubscriptionProviderStatusType](./literals.md#subscriptionproviderstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterSubscriptionProviderRequestRequestTypeDef

```python
# RegisterSubscriptionProviderRequestRequestTypeDef definition

class RegisterSubscriptionProviderRequestRequestTypeDef(TypedDict):
    SecretArn: str,
    SubscriptionProviderSource: SubscriptionProviderSourceType,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## ListLinuxSubscriptionInstancesRequestRequestTypeDef

```python
# ListLinuxSubscriptionInstancesRequestRequestTypeDef definition

class ListLinuxSubscriptionInstancesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLinuxSubscriptionsRequestRequestTypeDef

```python
# ListLinuxSubscriptionsRequestRequestTypeDef definition

class ListLinuxSubscriptionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetRegisteredSubscriptionProviderResponseTypeDef

```python
# GetRegisteredSubscriptionProviderResponseTypeDef definition

class GetRegisteredSubscriptionProviderResponseTypeDef(TypedDict):
    LastSuccessfulDataRetrievalTime: str,
    SecretArn: str,
    SubscriptionProviderArn: str,
    SubscriptionProviderSource: SubscriptionProviderSourceType,  # (1)
    SubscriptionProviderStatus: SubscriptionProviderStatusType,  # (2)
    SubscriptionProviderStatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
2. See [:material-code-brackets: SubscriptionProviderStatusType](./literals.md#subscriptionproviderstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterSubscriptionProviderResponseTypeDef

```python
# RegisterSubscriptionProviderResponseTypeDef definition

class RegisterSubscriptionProviderResponseTypeDef(TypedDict):
    SubscriptionProviderArn: str,
    SubscriptionProviderSource: SubscriptionProviderSourceType,  # (1)
    SubscriptionProviderStatus: SubscriptionProviderStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
2. See [:material-code-brackets: SubscriptionProviderStatusType](./literals.md#subscriptionproviderstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceSettingsResponseTypeDef

```python
# GetServiceSettingsResponseTypeDef definition

class GetServiceSettingsResponseTypeDef(TypedDict):
    HomeRegions: List[str],
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsOutputTypeDef,  # (2)
    Status: StatusType,  # (3)
    StatusMessage: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsOutputTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingsoutputtypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceSettingsResponseTypeDef

```python
# UpdateServiceSettingsResponseTypeDef definition

class UpdateServiceSettingsResponseTypeDef(TypedDict):
    HomeRegions: List[str],
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsOutputTypeDef,  # (2)
    Status: StatusType,  # (3)
    StatusMessage: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsOutputTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingsoutputtypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLinuxSubscriptionInstancesResponseTypeDef

```python
# ListLinuxSubscriptionInstancesResponseTypeDef definition

class ListLinuxSubscriptionInstancesResponseTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceSettingsRequestRequestTypeDef

```python
# UpdateServiceSettingsRequestRequestTypeDef definition

class UpdateServiceSettingsRequestRequestTypeDef(TypedDict):
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,  # (2)
    AllowUpdate: NotRequired[bool],
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingstypedef) 
## ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef

```python
# ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef definition

class ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef

```python
# ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef definition

class ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRegisteredSubscriptionProvidersRequestListRegisteredSubscriptionProvidersPaginateTypeDef

```python
# ListRegisteredSubscriptionProvidersRequestListRegisteredSubscriptionProvidersPaginateTypeDef definition

class ListRegisteredSubscriptionProvidersRequestListRegisteredSubscriptionProvidersPaginateTypeDef(TypedDict):
    SubscriptionProviderSources: NotRequired[Sequence[SubscriptionProviderSourceType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SubscriptionProviderSourceType](./literals.md#subscriptionprovidersourcetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLinuxSubscriptionsResponseTypeDef

```python
# ListLinuxSubscriptionsResponseTypeDef definition

class ListLinuxSubscriptionsResponseTypeDef(TypedDict):
    Subscriptions: List[SubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegisteredSubscriptionProvidersResponseTypeDef

```python
# ListRegisteredSubscriptionProvidersResponseTypeDef definition

class ListRegisteredSubscriptionProvidersResponseTypeDef(TypedDict):
    RegisteredSubscriptionProviders: List[RegisteredSubscriptionProviderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegisteredSubscriptionProviderTypeDef](./type_defs.md#registeredsubscriptionprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
