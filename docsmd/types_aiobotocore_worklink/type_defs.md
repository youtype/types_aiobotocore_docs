# Type definitions

> [Index](../README.md) > [WorkLink](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkLink](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
    type annotations stubs module [types-aiobotocore-worklink](https://pypi.org/project/types-aiobotocore-worklink/).



## AssociateDomainRequestRequestTypeDef

```python
# AssociateDomainRequestRequestTypeDef definition

class AssociateDomainRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
    AcmCertificateArn: str,
    DisplayName: NotRequired[str],
```

## AssociateWebsiteAuthorizationProviderRequestRequestTypeDef

```python
# AssociateWebsiteAuthorizationProviderRequestRequestTypeDef definition

class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    AuthorizationProviderType: AuthorizationProviderTypeType,  # (1)
    DomainName: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizationProviderTypeType](./literals.md#authorizationprovidertypetype) 
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

## AssociateWebsiteCertificateAuthorityRequestRequestTypeDef

```python
# AssociateWebsiteCertificateAuthorityRequestRequestTypeDef definition

class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    Certificate: str,
    DisplayName: NotRequired[str],
```

## CreateFleetRequestRequestTypeDef

```python
# CreateFleetRequestRequestTypeDef definition

class CreateFleetRequestRequestTypeDef(TypedDict):
    FleetName: str,
    DisplayName: NotRequired[str],
    OptimizeForEndUserLocation: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteFleetRequestRequestTypeDef

```python
# DeleteFleetRequestRequestTypeDef definition

class DeleteFleetRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeAuditStreamConfigurationRequestRequestTypeDef

```python
# DescribeAuditStreamConfigurationRequestRequestTypeDef definition

class DescribeAuditStreamConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeCompanyNetworkConfigurationRequestRequestTypeDef

```python
# DescribeCompanyNetworkConfigurationRequestRequestTypeDef definition

class DescribeCompanyNetworkConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeDevicePolicyConfigurationRequestRequestTypeDef

```python
# DescribeDevicePolicyConfigurationRequestRequestTypeDef definition

class DescribeDevicePolicyConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeDeviceRequestRequestTypeDef

```python
# DescribeDeviceRequestRequestTypeDef definition

class DescribeDeviceRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DeviceId: str,
```

## DescribeDomainRequestRequestTypeDef

```python
# DescribeDomainRequestRequestTypeDef definition

class DescribeDomainRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
```

## DescribeFleetMetadataRequestRequestTypeDef

```python
# DescribeFleetMetadataRequestRequestTypeDef definition

class DescribeFleetMetadataRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeIdentityProviderConfigurationRequestRequestTypeDef

```python
# DescribeIdentityProviderConfigurationRequestRequestTypeDef definition

class DescribeIdentityProviderConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
```

## DescribeWebsiteCertificateAuthorityRequestRequestTypeDef

```python
# DescribeWebsiteCertificateAuthorityRequestRequestTypeDef definition

class DescribeWebsiteCertificateAuthorityRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    WebsiteCaId: str,
```

## DeviceSummaryTypeDef

```python
# DeviceSummaryTypeDef definition

class DeviceSummaryTypeDef(TypedDict):
    DeviceId: NotRequired[str],
    DeviceStatus: NotRequired[DeviceStatusType],  # (1)
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
## DisassociateDomainRequestRequestTypeDef

```python
# DisassociateDomainRequestRequestTypeDef definition

class DisassociateDomainRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
```

## DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef

```python
# DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef definition

class DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    AuthorizationProviderId: str,
```

## DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef

```python
# DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef definition

class DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    WebsiteCaId: str,
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    DomainName: str,
    CreatedTime: datetime,
    DomainStatus: DomainStatusType,  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## FleetSummaryTypeDef

```python
# FleetSummaryTypeDef definition

class FleetSummaryTypeDef(TypedDict):
    FleetArn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    FleetName: NotRequired[str],
    DisplayName: NotRequired[str],
    CompanyCode: NotRequired[str],
    FleetStatus: NotRequired[FleetStatusType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFleetsRequestRequestTypeDef

```python
# ListFleetsRequestRequestTypeDef definition

class ListFleetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListWebsiteAuthorizationProvidersRequestRequestTypeDef

```python
# ListWebsiteAuthorizationProvidersRequestRequestTypeDef definition

class ListWebsiteAuthorizationProvidersRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## WebsiteAuthorizationProviderSummaryTypeDef

```python
# WebsiteAuthorizationProviderSummaryTypeDef definition

class WebsiteAuthorizationProviderSummaryTypeDef(TypedDict):
    AuthorizationProviderType: AuthorizationProviderTypeType,  # (1)
    AuthorizationProviderId: NotRequired[str],
    DomainName: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AuthorizationProviderTypeType](./literals.md#authorizationprovidertypetype) 
## ListWebsiteCertificateAuthoritiesRequestRequestTypeDef

```python
# ListWebsiteCertificateAuthoritiesRequestRequestTypeDef definition

class ListWebsiteCertificateAuthoritiesRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## WebsiteCaSummaryTypeDef

```python
# WebsiteCaSummaryTypeDef definition

class WebsiteCaSummaryTypeDef(TypedDict):
    WebsiteCaId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    DisplayName: NotRequired[str],
```

## RestoreDomainAccessRequestRequestTypeDef

```python
# RestoreDomainAccessRequestRequestTypeDef definition

class RestoreDomainAccessRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
```

## RevokeDomainAccessRequestRequestTypeDef

```python
# RevokeDomainAccessRequestRequestTypeDef definition

class RevokeDomainAccessRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
```

## SignOutUserRequestRequestTypeDef

```python
# SignOutUserRequestRequestTypeDef definition

class SignOutUserRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    Username: str,
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

## UpdateAuditStreamConfigurationRequestRequestTypeDef

```python
# UpdateAuditStreamConfigurationRequestRequestTypeDef definition

class UpdateAuditStreamConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    AuditStreamArn: NotRequired[str],
```

## UpdateCompanyNetworkConfigurationRequestRequestTypeDef

```python
# UpdateCompanyNetworkConfigurationRequestRequestTypeDef definition

class UpdateCompanyNetworkConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    VpcId: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
```

## UpdateDevicePolicyConfigurationRequestRequestTypeDef

```python
# UpdateDevicePolicyConfigurationRequestRequestTypeDef definition

class UpdateDevicePolicyConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DeviceCaCertificate: NotRequired[str],
```

## UpdateDomainMetadataRequestRequestTypeDef

```python
# UpdateDomainMetadataRequestRequestTypeDef definition

class UpdateDomainMetadataRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DomainName: str,
    DisplayName: NotRequired[str],
```

## UpdateFleetMetadataRequestRequestTypeDef

```python
# UpdateFleetMetadataRequestRequestTypeDef definition

class UpdateFleetMetadataRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    DisplayName: NotRequired[str],
    OptimizeForEndUserLocation: NotRequired[bool],
```

## UpdateIdentityProviderConfigurationRequestRequestTypeDef

```python
# UpdateIdentityProviderConfigurationRequestRequestTypeDef definition

class UpdateIdentityProviderConfigurationRequestRequestTypeDef(TypedDict):
    FleetArn: str,
    IdentityProviderType: IdentityProviderTypeType,  # (1)
    IdentityProviderSamlMetadata: NotRequired[str],
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
## AssociateWebsiteAuthorizationProviderResponseTypeDef

```python
# AssociateWebsiteAuthorizationProviderResponseTypeDef definition

class AssociateWebsiteAuthorizationProviderResponseTypeDef(TypedDict):
    AuthorizationProviderId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateWebsiteCertificateAuthorityResponseTypeDef

```python
# AssociateWebsiteCertificateAuthorityResponseTypeDef definition

class AssociateWebsiteCertificateAuthorityResponseTypeDef(TypedDict):
    WebsiteCaId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResponseTypeDef

```python
# CreateFleetResponseTypeDef definition

class CreateFleetResponseTypeDef(TypedDict):
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAuditStreamConfigurationResponseTypeDef

```python
# DescribeAuditStreamConfigurationResponseTypeDef definition

class DescribeAuditStreamConfigurationResponseTypeDef(TypedDict):
    AuditStreamArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCompanyNetworkConfigurationResponseTypeDef

```python
# DescribeCompanyNetworkConfigurationResponseTypeDef definition

class DescribeCompanyNetworkConfigurationResponseTypeDef(TypedDict):
    VpcId: str,
    SubnetIds: List[str],
    SecurityGroupIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDevicePolicyConfigurationResponseTypeDef

```python
# DescribeDevicePolicyConfigurationResponseTypeDef definition

class DescribeDevicePolicyConfigurationResponseTypeDef(TypedDict):
    DeviceCaCertificate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeviceResponseTypeDef

```python
# DescribeDeviceResponseTypeDef definition

class DescribeDeviceResponseTypeDef(TypedDict):
    Status: DeviceStatusType,  # (1)
    Model: str,
    Manufacturer: str,
    OperatingSystem: str,
    OperatingSystemVersion: str,
    PatchLevel: str,
    FirstAccessedTime: datetime,
    LastAccessedTime: datetime,
    Username: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainResponseTypeDef

```python
# DescribeDomainResponseTypeDef definition

class DescribeDomainResponseTypeDef(TypedDict):
    DomainName: str,
    DisplayName: str,
    CreatedTime: datetime,
    DomainStatus: DomainStatusType,  # (1)
    AcmCertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetMetadataResponseTypeDef

```python
# DescribeFleetMetadataResponseTypeDef definition

class DescribeFleetMetadataResponseTypeDef(TypedDict):
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    FleetName: str,
    DisplayName: str,
    OptimizeForEndUserLocation: bool,
    CompanyCode: str,
    FleetStatus: FleetStatusType,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIdentityProviderConfigurationResponseTypeDef

```python
# DescribeIdentityProviderConfigurationResponseTypeDef definition

class DescribeIdentityProviderConfigurationResponseTypeDef(TypedDict):
    IdentityProviderType: IdentityProviderTypeType,  # (1)
    ServiceProviderSamlMetadata: str,
    IdentityProviderSamlMetadata: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWebsiteCertificateAuthorityResponseTypeDef

```python
# DescribeWebsiteCertificateAuthorityResponseTypeDef definition

class DescribeWebsiteCertificateAuthorityResponseTypeDef(TypedDict):
    Certificate: str,
    CreatedTime: datetime,
    DisplayName: str,
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
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    Devices: List[DeviceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    Domains: List[DomainSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsResponseTypeDef

```python
# ListFleetsResponseTypeDef definition

class ListFleetsResponseTypeDef(TypedDict):
    FleetSummaryList: List[FleetSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetSummaryTypeDef](./type_defs.md#fleetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebsiteAuthorizationProvidersResponseTypeDef

```python
# ListWebsiteAuthorizationProvidersResponseTypeDef definition

class ListWebsiteAuthorizationProvidersResponseTypeDef(TypedDict):
    WebsiteAuthorizationProviders: List[WebsiteAuthorizationProviderSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebsiteAuthorizationProviderSummaryTypeDef](./type_defs.md#websiteauthorizationprovidersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebsiteCertificateAuthoritiesResponseTypeDef

```python
# ListWebsiteCertificateAuthoritiesResponseTypeDef definition

class ListWebsiteCertificateAuthoritiesResponseTypeDef(TypedDict):
    WebsiteCertificateAuthorities: List[WebsiteCaSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebsiteCaSummaryTypeDef](./type_defs.md#websitecasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
