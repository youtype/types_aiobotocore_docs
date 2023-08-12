# Type definitions

> [Index](../README.md) > [LicenseManagerLinuxSubscriptions](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).



## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Operator: NotRequired[OperatorType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## LinuxSubscriptionsDiscoverySettingsTypeDef

```python
# LinuxSubscriptionsDiscoverySettingsTypeDef definition

class LinuxSubscriptionsDiscoverySettingsTypeDef(TypedDict):
    OrganizationIntegration: OrganizationIntegrationType,  # (1)
    SourceRegions: List[str],
```

1. See [:material-code-brackets: OrganizationIntegrationType](./literals.md#organizationintegrationtype) 
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

## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    AccountID: NotRequired[str],
    AmiId: NotRequired[str],
    InstanceID: NotRequired[str],
    InstanceType: NotRequired[str],
    LastUpdatedTime: NotRequired[str],
    ProductCode: NotRequired[List[str]],
    Region: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionName: NotRequired[str],
    UsageOperation: NotRequired[str],
```

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
## GetServiceSettingsResponseTypeDef

```python
# GetServiceSettingsResponseTypeDef definition

class GetServiceSettingsResponseTypeDef(TypedDict):
    HomeRegions: List[str],
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,  # (2)
    Status: StatusType,  # (3)
    StatusMessage: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingstypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceSettingsResponseTypeDef

```python
# UpdateServiceSettingsResponseTypeDef definition

class UpdateServiceSettingsResponseTypeDef(TypedDict):
    HomeRegions: List[str],
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,  # (2)
    Status: StatusType,  # (3)
    StatusMessage: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingstypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLinuxSubscriptionInstancesResponseTypeDef

```python
# ListLinuxSubscriptionInstancesResponseTypeDef definition

class ListLinuxSubscriptionInstancesResponseTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ListLinuxSubscriptionsResponseTypeDef

```python
# ListLinuxSubscriptionsResponseTypeDef definition

class ListLinuxSubscriptionsResponseTypeDef(TypedDict):
    NextToken: str,
    Subscriptions: List[SubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
