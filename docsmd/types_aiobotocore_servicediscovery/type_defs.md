# Type definitions

> [Index](../README.md) > [ServiceDiscovery](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ServiceDiscovery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#servicediscovery)
    type annotations stubs module [types-aiobotocore-servicediscovery](https://pypi.org/project/types-aiobotocore-servicediscovery/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## HealthCheckConfigTypeDef

```python
# HealthCheckConfigTypeDef definition

class HealthCheckConfigTypeDef(TypedDict):
    Type: HealthCheckTypeType,  # (1)
    ResourcePath: NotRequired[str],
    FailureThreshold: NotRequired[int],
```

1. See [:material-code-brackets: HealthCheckTypeType](./literals.md#healthchecktypetype) 
## HealthCheckCustomConfigTypeDef

```python
# HealthCheckCustomConfigTypeDef definition

class HealthCheckCustomConfigTypeDef(TypedDict):
    FailureThreshold: NotRequired[int],
```

## DeleteNamespaceRequestRequestTypeDef

```python
# DeleteNamespaceRequestRequestTypeDef definition

class DeleteNamespaceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteServiceAttributesRequestRequestTypeDef

```python
# DeleteServiceAttributesRequestRequestTypeDef definition

class DeleteServiceAttributesRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    Attributes: Sequence[str],
```

## DeleteServiceRequestRequestTypeDef

```python
# DeleteServiceRequestRequestTypeDef definition

class DeleteServiceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeregisterInstanceRequestRequestTypeDef

```python
# DeregisterInstanceRequestRequestTypeDef definition

class DeregisterInstanceRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    InstanceId: str,
```

## DiscoverInstancesRequestRequestTypeDef

```python
# DiscoverInstancesRequestRequestTypeDef definition

class DiscoverInstancesRequestRequestTypeDef(TypedDict):
    NamespaceName: str,
    ServiceName: str,
    MaxResults: NotRequired[int],
    QueryParameters: NotRequired[Mapping[str, str]],
    OptionalParameters: NotRequired[Mapping[str, str]],
    HealthStatus: NotRequired[HealthStatusFilterType],  # (1)
```

1. See [:material-code-brackets: HealthStatusFilterType](./literals.md#healthstatusfiltertype) 
## HttpInstanceSummaryTypeDef

```python
# HttpInstanceSummaryTypeDef definition

class HttpInstanceSummaryTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    NamespaceName: NotRequired[str],
    ServiceName: NotRequired[str],
    HealthStatus: NotRequired[HealthStatusType],  # (1)
    Attributes: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
## DiscoverInstancesRevisionRequestRequestTypeDef

```python
# DiscoverInstancesRevisionRequestRequestTypeDef definition

class DiscoverInstancesRevisionRequestRequestTypeDef(TypedDict):
    NamespaceName: str,
    ServiceName: str,
```

## DnsRecordTypeDef

```python
# DnsRecordTypeDef definition

class DnsRecordTypeDef(TypedDict):
    Type: RecordTypeType,  # (1)
    TTL: int,
```

1. See [:material-code-brackets: RecordTypeType](./literals.md#recordtypetype) 
## SOATypeDef

```python
# SOATypeDef definition

class SOATypeDef(TypedDict):
    TTL: int,
```

## GetInstanceRequestRequestTypeDef

```python
# GetInstanceRequestRequestTypeDef definition

class GetInstanceRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    InstanceId: str,
```

## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: str,
    CreatorRequestId: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## GetInstancesHealthStatusRequestRequestTypeDef

```python
# GetInstancesHealthStatusRequestRequestTypeDef definition

class GetInstancesHealthStatusRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    Instances: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetNamespaceRequestRequestTypeDef

```python
# GetNamespaceRequestRequestTypeDef definition

class GetNamespaceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetOperationRequestRequestTypeDef

```python
# GetOperationRequestRequestTypeDef definition

class GetOperationRequestRequestTypeDef(TypedDict):
    OperationId: str,
```

## OperationTypeDef

```python
# OperationTypeDef definition

class OperationTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[OperationTypeType],  # (1)
    Status: NotRequired[OperationStatusType],  # (2)
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[str],
    CreateDate: NotRequired[datetime],
    UpdateDate: NotRequired[datetime],
    Targets: NotRequired[Dict[OperationTargetTypeType, str]],  # (3)
```

1. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
2. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
3. See [:material-code-brackets: OperationTargetTypeType](./literals.md#operationtargettypetype) 
## GetServiceAttributesRequestRequestTypeDef

```python
# GetServiceAttributesRequestRequestTypeDef definition

class GetServiceAttributesRequestRequestTypeDef(TypedDict):
    ServiceId: str,
```

## ServiceAttributesTypeDef

```python
# ServiceAttributesTypeDef definition

class ServiceAttributesTypeDef(TypedDict):
    ServiceArn: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## GetServiceRequestRequestTypeDef

```python
# GetServiceRequestRequestTypeDef definition

class GetServiceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## HttpNamespaceChangeTypeDef

```python
# HttpNamespaceChangeTypeDef definition

class HttpNamespaceChangeTypeDef(TypedDict):
    Description: str,
```

## HttpPropertiesTypeDef

```python
# HttpPropertiesTypeDef definition

class HttpPropertiesTypeDef(TypedDict):
    HttpName: NotRequired[str],
```

## InstanceSummaryTypeDef

```python
# InstanceSummaryTypeDef definition

class InstanceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## NamespaceFilterTypeDef

```python
# NamespaceFilterTypeDef definition

class NamespaceFilterTypeDef(TypedDict):
    Name: NamespaceFilterNameType,  # (1)
    Values: Sequence[str],
    Condition: NotRequired[FilterConditionType],  # (2)
```

1. See [:material-code-brackets: NamespaceFilterNameType](./literals.md#namespacefilternametype) 
2. See [:material-code-brackets: FilterConditionType](./literals.md#filterconditiontype) 
## OperationFilterTypeDef

```python
# OperationFilterTypeDef definition

class OperationFilterTypeDef(TypedDict):
    Name: OperationFilterNameType,  # (1)
    Values: Sequence[str],
    Condition: NotRequired[FilterConditionType],  # (2)
```

1. See [:material-code-brackets: OperationFilterNameType](./literals.md#operationfilternametype) 
2. See [:material-code-brackets: FilterConditionType](./literals.md#filterconditiontype) 
## OperationSummaryTypeDef

```python
# OperationSummaryTypeDef definition

class OperationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Status: NotRequired[OperationStatusType],  # (1)
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
## ServiceFilterTypeDef

```python
# ServiceFilterTypeDef definition

class ServiceFilterTypeDef(TypedDict):
    Name: ServiceFilterNameType,  # (1)
    Values: Sequence[str],
    Condition: NotRequired[FilterConditionType],  # (2)
```

1. See [:material-code-brackets: ServiceFilterNameType](./literals.md#servicefilternametype) 
2. See [:material-code-brackets: FilterConditionType](./literals.md#filterconditiontype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## SOAChangeTypeDef

```python
# SOAChangeTypeDef definition

class SOAChangeTypeDef(TypedDict):
    TTL: int,
```

## RegisterInstanceRequestRequestTypeDef

```python
# RegisterInstanceRequestRequestTypeDef definition

class RegisterInstanceRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    InstanceId: str,
    Attributes: Mapping[str, str],
    CreatorRequestId: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateInstanceCustomHealthStatusRequestRequestTypeDef

```python
# UpdateInstanceCustomHealthStatusRequestRequestTypeDef definition

class UpdateInstanceCustomHealthStatusRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    InstanceId: str,
    Status: CustomHealthStatusType,  # (1)
```

1. See [:material-code-brackets: CustomHealthStatusType](./literals.md#customhealthstatustype) 
## UpdateServiceAttributesRequestRequestTypeDef

```python
# UpdateServiceAttributesRequestRequestTypeDef definition

class UpdateServiceAttributesRequestRequestTypeDef(TypedDict):
    ServiceId: str,
    Attributes: Mapping[str, str],
```

## CreateHttpNamespaceRequestRequestTypeDef

```python
# CreateHttpNamespaceRequestRequestTypeDef definition

class CreateHttpNamespaceRequestRequestTypeDef(TypedDict):
    Name: str,
    CreatorRequestId: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateHttpNamespaceResponseTypeDef

```python
# CreateHttpNamespaceResponseTypeDef definition

class CreateHttpNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrivateDnsNamespaceResponseTypeDef

```python
# CreatePrivateDnsNamespaceResponseTypeDef definition

class CreatePrivateDnsNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePublicDnsNamespaceResponseTypeDef

```python
# CreatePublicDnsNamespaceResponseTypeDef definition

class CreatePublicDnsNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNamespaceResponseTypeDef

```python
# DeleteNamespaceResponseTypeDef definition

class DeleteNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterInstanceResponseTypeDef

```python
# DeregisterInstanceResponseTypeDef definition

class DeregisterInstanceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DiscoverInstancesRevisionResponseTypeDef

```python
# DiscoverInstancesRevisionResponseTypeDef definition

class DiscoverInstancesRevisionResponseTypeDef(TypedDict):
    InstancesRevision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstancesHealthStatusResponseTypeDef

```python
# GetInstancesHealthStatusResponseTypeDef definition

class GetInstancesHealthStatusResponseTypeDef(TypedDict):
    Status: Dict[str, HealthStatusType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterInstanceResponseTypeDef

```python
# RegisterInstanceResponseTypeDef definition

class RegisterInstanceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHttpNamespaceResponseTypeDef

```python
# UpdateHttpNamespaceResponseTypeDef definition

class UpdateHttpNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePrivateDnsNamespaceResponseTypeDef

```python
# UpdatePrivateDnsNamespaceResponseTypeDef definition

class UpdatePrivateDnsNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePublicDnsNamespaceResponseTypeDef

```python
# UpdatePublicDnsNamespaceResponseTypeDef definition

class UpdatePublicDnsNamespaceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceResponseTypeDef

```python
# UpdateServiceResponseTypeDef definition

class UpdateServiceResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DiscoverInstancesResponseTypeDef

```python
# DiscoverInstancesResponseTypeDef definition

class DiscoverInstancesResponseTypeDef(TypedDict):
    Instances: List[HttpInstanceSummaryTypeDef],  # (1)
    InstancesRevision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpInstanceSummaryTypeDef](./type_defs.md#httpinstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DnsConfigChangeTypeDef

```python
# DnsConfigChangeTypeDef definition

class DnsConfigChangeTypeDef(TypedDict):
    DnsRecords: Sequence[DnsRecordTypeDef],  # (1)
```

1. See [:material-code-braces: DnsRecordTypeDef](./type_defs.md#dnsrecordtypedef) 
## DnsConfigOutputTypeDef

```python
# DnsConfigOutputTypeDef definition

class DnsConfigOutputTypeDef(TypedDict):
    DnsRecords: List[DnsRecordTypeDef],  # (2)
    NamespaceId: NotRequired[str],
    RoutingPolicy: NotRequired[RoutingPolicyType],  # (1)
```

1. See [:material-code-brackets: RoutingPolicyType](./literals.md#routingpolicytype) 
2. See [:material-code-braces: DnsRecordTypeDef](./type_defs.md#dnsrecordtypedef) 
## DnsConfigTypeDef

```python
# DnsConfigTypeDef definition

class DnsConfigTypeDef(TypedDict):
    DnsRecords: Sequence[DnsRecordTypeDef],  # (2)
    NamespaceId: NotRequired[str],
    RoutingPolicy: NotRequired[RoutingPolicyType],  # (1)
```

1. See [:material-code-brackets: RoutingPolicyType](./literals.md#routingpolicytype) 
2. See [:material-code-braces: DnsRecordTypeDef](./type_defs.md#dnsrecordtypedef) 
## DnsPropertiesTypeDef

```python
# DnsPropertiesTypeDef definition

class DnsPropertiesTypeDef(TypedDict):
    HostedZoneId: NotRequired[str],
    SOA: NotRequired[SOATypeDef],  # (1)
```

1. See [:material-code-braces: SOATypeDef](./type_defs.md#soatypedef) 
## PrivateDnsPropertiesMutableTypeDef

```python
# PrivateDnsPropertiesMutableTypeDef definition

class PrivateDnsPropertiesMutableTypeDef(TypedDict):
    SOA: SOATypeDef,  # (1)
```

1. See [:material-code-braces: SOATypeDef](./type_defs.md#soatypedef) 
## PublicDnsPropertiesMutableTypeDef

```python
# PublicDnsPropertiesMutableTypeDef definition

class PublicDnsPropertiesMutableTypeDef(TypedDict):
    SOA: SOATypeDef,  # (1)
```

1. See [:material-code-braces: SOATypeDef](./type_defs.md#soatypedef) 
## GetInstanceResponseTypeDef

```python
# GetInstanceResponseTypeDef definition

class GetInstanceResponseTypeDef(TypedDict):
    Instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOperationResponseTypeDef

```python
# GetOperationResponseTypeDef definition

class GetOperationResponseTypeDef(TypedDict):
    Operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceAttributesResponseTypeDef

```python
# GetServiceAttributesResponseTypeDef definition

class GetServiceAttributesResponseTypeDef(TypedDict):
    ServiceAttributes: ServiceAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceAttributesTypeDef](./type_defs.md#serviceattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHttpNamespaceRequestRequestTypeDef

```python
# UpdateHttpNamespaceRequestRequestTypeDef definition

class UpdateHttpNamespaceRequestRequestTypeDef(TypedDict):
    Id: str,
    Namespace: HttpNamespaceChangeTypeDef,  # (1)
    UpdaterRequestId: NotRequired[str],
```

1. See [:material-code-braces: HttpNamespaceChangeTypeDef](./type_defs.md#httpnamespacechangetypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    Instances: List[InstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstancesRequestPaginateTypeDef

```python
# ListInstancesRequestPaginateTypeDef definition

class ListInstancesRequestPaginateTypeDef(TypedDict):
    ServiceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesRequestPaginateTypeDef

```python
# ListNamespacesRequestPaginateTypeDef definition

class ListNamespacesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[NamespaceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: NamespaceFilterTypeDef](./type_defs.md#namespacefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesRequestRequestTypeDef

```python
# ListNamespacesRequestRequestTypeDef definition

class ListNamespacesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[NamespaceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: NamespaceFilterTypeDef](./type_defs.md#namespacefiltertypedef) 
## ListOperationsRequestPaginateTypeDef

```python
# ListOperationsRequestPaginateTypeDef definition

class ListOperationsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[OperationFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OperationFilterTypeDef](./type_defs.md#operationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOperationsRequestRequestTypeDef

```python
# ListOperationsRequestRequestTypeDef definition

class ListOperationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[OperationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: OperationFilterTypeDef](./type_defs.md#operationfiltertypedef) 
## ListOperationsResponseTypeDef

```python
# ListOperationsResponseTypeDef definition

class ListOperationsResponseTypeDef(TypedDict):
    Operations: List[OperationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OperationSummaryTypeDef](./type_defs.md#operationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesRequestPaginateTypeDef

```python
# ListServicesRequestPaginateTypeDef definition

class ListServicesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ServiceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceFilterTypeDef](./type_defs.md#servicefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestRequestTypeDef

```python
# ListServicesRequestRequestTypeDef definition

class ListServicesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[ServiceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ServiceFilterTypeDef](./type_defs.md#servicefiltertypedef) 
## PrivateDnsPropertiesMutableChangeTypeDef

```python
# PrivateDnsPropertiesMutableChangeTypeDef definition

class PrivateDnsPropertiesMutableChangeTypeDef(TypedDict):
    SOA: SOAChangeTypeDef,  # (1)
```

1. See [:material-code-braces: SOAChangeTypeDef](./type_defs.md#soachangetypedef) 
## PublicDnsPropertiesMutableChangeTypeDef

```python
# PublicDnsPropertiesMutableChangeTypeDef definition

class PublicDnsPropertiesMutableChangeTypeDef(TypedDict):
    SOA: SOAChangeTypeDef,  # (1)
```

1. See [:material-code-braces: SOAChangeTypeDef](./type_defs.md#soachangetypedef) 
## ServiceChangeTypeDef

```python
# ServiceChangeTypeDef definition

class ServiceChangeTypeDef(TypedDict):
    Description: NotRequired[str],
    DnsConfig: NotRequired[DnsConfigChangeTypeDef],  # (1)
    HealthCheckConfig: NotRequired[HealthCheckConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DnsConfigChangeTypeDef](./type_defs.md#dnsconfigchangetypedef) 
2. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ServiceTypeType],  # (1)
    Description: NotRequired[str],
    InstanceCount: NotRequired[int],
    DnsConfig: NotRequired[DnsConfigOutputTypeDef],  # (2)
    HealthCheckConfig: NotRequired[HealthCheckConfigTypeDef],  # (3)
    HealthCheckCustomConfig: NotRequired[HealthCheckCustomConfigTypeDef],  # (4)
    CreateDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: DnsConfigOutputTypeDef](./type_defs.md#dnsconfigoutputtypedef) 
3. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
4. See [:material-code-braces: HealthCheckCustomConfigTypeDef](./type_defs.md#healthcheckcustomconfigtypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    NamespaceId: NotRequired[str],
    Description: NotRequired[str],
    InstanceCount: NotRequired[int],
    DnsConfig: NotRequired[DnsConfigOutputTypeDef],  # (1)
    Type: NotRequired[ServiceTypeType],  # (2)
    HealthCheckConfig: NotRequired[HealthCheckConfigTypeDef],  # (3)
    HealthCheckCustomConfig: NotRequired[HealthCheckCustomConfigTypeDef],  # (4)
    CreateDate: NotRequired[datetime],
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-braces: DnsConfigOutputTypeDef](./type_defs.md#dnsconfigoutputtypedef) 
2. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
3. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
4. See [:material-code-braces: HealthCheckCustomConfigTypeDef](./type_defs.md#healthcheckcustomconfigtypedef) 
## CreateServiceRequestRequestTypeDef

```python
# CreateServiceRequestRequestTypeDef definition

class CreateServiceRequestRequestTypeDef(TypedDict):
    Name: str,
    NamespaceId: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    Description: NotRequired[str],
    DnsConfig: NotRequired[DnsConfigTypeDef],  # (1)
    HealthCheckConfig: NotRequired[HealthCheckConfigTypeDef],  # (2)
    HealthCheckCustomConfig: NotRequired[HealthCheckCustomConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    Type: NotRequired[ServiceTypeOptionType],  # (5)
```

1. See [:material-code-braces: DnsConfigTypeDef](./type_defs.md#dnsconfigtypedef) 
2. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
3. See [:material-code-braces: HealthCheckCustomConfigTypeDef](./type_defs.md#healthcheckcustomconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ServiceTypeOptionType](./literals.md#servicetypeoptiontype) 
## NamespacePropertiesTypeDef

```python
# NamespacePropertiesTypeDef definition

class NamespacePropertiesTypeDef(TypedDict):
    DnsProperties: NotRequired[DnsPropertiesTypeDef],  # (1)
    HttpProperties: NotRequired[HttpPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: DnsPropertiesTypeDef](./type_defs.md#dnspropertiestypedef) 
2. See [:material-code-braces: HttpPropertiesTypeDef](./type_defs.md#httppropertiestypedef) 
## PrivateDnsNamespacePropertiesTypeDef

```python
# PrivateDnsNamespacePropertiesTypeDef definition

class PrivateDnsNamespacePropertiesTypeDef(TypedDict):
    DnsProperties: PrivateDnsPropertiesMutableTypeDef,  # (1)
```

1. See [:material-code-braces: PrivateDnsPropertiesMutableTypeDef](./type_defs.md#privatednspropertiesmutabletypedef) 
## PublicDnsNamespacePropertiesTypeDef

```python
# PublicDnsNamespacePropertiesTypeDef definition

class PublicDnsNamespacePropertiesTypeDef(TypedDict):
    DnsProperties: PublicDnsPropertiesMutableTypeDef,  # (1)
```

1. See [:material-code-braces: PublicDnsPropertiesMutableTypeDef](./type_defs.md#publicdnspropertiesmutabletypedef) 
## PrivateDnsNamespacePropertiesChangeTypeDef

```python
# PrivateDnsNamespacePropertiesChangeTypeDef definition

class PrivateDnsNamespacePropertiesChangeTypeDef(TypedDict):
    DnsProperties: PrivateDnsPropertiesMutableChangeTypeDef,  # (1)
```

1. See [:material-code-braces: PrivateDnsPropertiesMutableChangeTypeDef](./type_defs.md#privatednspropertiesmutablechangetypedef) 
## PublicDnsNamespacePropertiesChangeTypeDef

```python
# PublicDnsNamespacePropertiesChangeTypeDef definition

class PublicDnsNamespacePropertiesChangeTypeDef(TypedDict):
    DnsProperties: PublicDnsPropertiesMutableChangeTypeDef,  # (1)
```

1. See [:material-code-braces: PublicDnsPropertiesMutableChangeTypeDef](./type_defs.md#publicdnspropertiesmutablechangetypedef) 
## UpdateServiceRequestRequestTypeDef

```python
# UpdateServiceRequestRequestTypeDef definition

class UpdateServiceRequestRequestTypeDef(TypedDict):
    Id: str,
    Service: ServiceChangeTypeDef,  # (1)
```

1. See [:material-code-braces: ServiceChangeTypeDef](./type_defs.md#servicechangetypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    Services: List[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceResponseTypeDef

```python
# CreateServiceResponseTypeDef definition

class CreateServiceResponseTypeDef(TypedDict):
    Service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceResponseTypeDef

```python
# GetServiceResponseTypeDef definition

class GetServiceResponseTypeDef(TypedDict):
    Service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NamespaceSummaryTypeDef

```python
# NamespaceSummaryTypeDef definition

class NamespaceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[NamespaceTypeType],  # (1)
    Description: NotRequired[str],
    ServiceCount: NotRequired[int],
    Properties: NotRequired[NamespacePropertiesTypeDef],  # (2)
    CreateDate: NotRequired[datetime],
```

1. See [:material-code-brackets: NamespaceTypeType](./literals.md#namespacetypetype) 
2. See [:material-code-braces: NamespacePropertiesTypeDef](./type_defs.md#namespacepropertiestypedef) 
## NamespaceTypeDef

```python
# NamespaceTypeDef definition

class NamespaceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[NamespaceTypeType],  # (1)
    Description: NotRequired[str],
    ServiceCount: NotRequired[int],
    Properties: NotRequired[NamespacePropertiesTypeDef],  # (2)
    CreateDate: NotRequired[datetime],
    CreatorRequestId: NotRequired[str],
```

1. See [:material-code-brackets: NamespaceTypeType](./literals.md#namespacetypetype) 
2. See [:material-code-braces: NamespacePropertiesTypeDef](./type_defs.md#namespacepropertiestypedef) 
## CreatePrivateDnsNamespaceRequestRequestTypeDef

```python
# CreatePrivateDnsNamespaceRequestRequestTypeDef definition

class CreatePrivateDnsNamespaceRequestRequestTypeDef(TypedDict):
    Name: str,
    Vpc: str,
    CreatorRequestId: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    Properties: NotRequired[PrivateDnsNamespacePropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PrivateDnsNamespacePropertiesTypeDef](./type_defs.md#privatednsnamespacepropertiestypedef) 
## CreatePublicDnsNamespaceRequestRequestTypeDef

```python
# CreatePublicDnsNamespaceRequestRequestTypeDef definition

class CreatePublicDnsNamespaceRequestRequestTypeDef(TypedDict):
    Name: str,
    CreatorRequestId: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    Properties: NotRequired[PublicDnsNamespacePropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PublicDnsNamespacePropertiesTypeDef](./type_defs.md#publicdnsnamespacepropertiestypedef) 
## PrivateDnsNamespaceChangeTypeDef

```python
# PrivateDnsNamespaceChangeTypeDef definition

class PrivateDnsNamespaceChangeTypeDef(TypedDict):
    Description: NotRequired[str],
    Properties: NotRequired[PrivateDnsNamespacePropertiesChangeTypeDef],  # (1)
```

1. See [:material-code-braces: PrivateDnsNamespacePropertiesChangeTypeDef](./type_defs.md#privatednsnamespacepropertieschangetypedef) 
## PublicDnsNamespaceChangeTypeDef

```python
# PublicDnsNamespaceChangeTypeDef definition

class PublicDnsNamespaceChangeTypeDef(TypedDict):
    Description: NotRequired[str],
    Properties: NotRequired[PublicDnsNamespacePropertiesChangeTypeDef],  # (1)
```

1. See [:material-code-braces: PublicDnsNamespacePropertiesChangeTypeDef](./type_defs.md#publicdnsnamespacepropertieschangetypedef) 
## ListNamespacesResponseTypeDef

```python
# ListNamespacesResponseTypeDef definition

class ListNamespacesResponseTypeDef(TypedDict):
    Namespaces: List[NamespaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NamespaceSummaryTypeDef](./type_defs.md#namespacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamespaceResponseTypeDef

```python
# GetNamespaceResponseTypeDef definition

class GetNamespaceResponseTypeDef(TypedDict):
    Namespace: NamespaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePrivateDnsNamespaceRequestRequestTypeDef

```python
# UpdatePrivateDnsNamespaceRequestRequestTypeDef definition

class UpdatePrivateDnsNamespaceRequestRequestTypeDef(TypedDict):
    Id: str,
    Namespace: PrivateDnsNamespaceChangeTypeDef,  # (1)
    UpdaterRequestId: NotRequired[str],
```

1. See [:material-code-braces: PrivateDnsNamespaceChangeTypeDef](./type_defs.md#privatednsnamespacechangetypedef) 
## UpdatePublicDnsNamespaceRequestRequestTypeDef

```python
# UpdatePublicDnsNamespaceRequestRequestTypeDef definition

class UpdatePublicDnsNamespaceRequestRequestTypeDef(TypedDict):
    Id: str,
    Namespace: PublicDnsNamespaceChangeTypeDef,  # (1)
    UpdaterRequestId: NotRequired[str],
```

1. See [:material-code-braces: PublicDnsNamespaceChangeTypeDef](./type_defs.md#publicdnsnamespacechangetypedef) 
